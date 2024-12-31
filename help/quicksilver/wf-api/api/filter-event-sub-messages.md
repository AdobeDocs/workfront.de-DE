---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Nachrichten zu Ereignisabonnements filtern
description: Nachrichten zu Ereignisabonnements filtern
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1767'
ht-degree: 0%

---

# Nachrichten zu Ereignisabonnements filtern

Sie können zwischengeschaltete Verarbeitungskomponenten erstellen, mit denen Sie nur die Ereignisabonnementnachrichten filtern und verarbeiten können, die Ihr Unternehmen benötigt.

Informationen zu Ereignisabonnements finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## Filtern von Ereignisnachrichten

Dieser Abschnitt enthält Code-Snippets zur Filterung, die Sie implementieren können, um die Belastung von Ereignisabonnementnachrichten zu verringern.  Um die Unterschiede in der Syntax verschiedener Sprachen zu veranschaulichen, veranschaulichen diese Snippets denselben Satz von Filtern, die in den folgenden Sprachen geschrieben sind:

Beispiele für Filter finden Sie unter [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples). Dort können Sie die Unterschiede in der Syntax für die einzelnen Sprachen und die Interaktionsmöglichkeiten mit AWS SDK sehen. Diese Beispiele werden als AWS-Lambdas geschrieben, was eine gängige Methode für die Verwendung von Filterungs- und Verarbeitungskomponenten für Intermediäre ist.

Die folgenden Codeausschnitte sind nahezu bereitstellungsbereit und können als Ausgangspunkt verwendet werden, um Sie beim Schreiben Ihrer eigenen, komplexeren Filter und Verarbeitungskomponenten zu unterstützen.

### Java

Das folgende Beispiel in Java zeigt, wie Sie Projekt-Payloads basierend auf der Gruppen-ID des Projekts filtern, wie es in [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java) getan wird

1. Legen Sie die gesuchte Gruppen-ID fest und erstellen Sie sie als statische Konstante.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   In diesem Beispiel verwendet die handleRequest-Methode, bei der es sich um einen AWS Lambda-Standardmethodennamen handelt, als ersten Parameter einen Zuordnungstyp, d. h. den Inhalt der Ereignisabonnementnachricht.\
   Der zweite erforderliche Parameter ist der Kontext der aktuellen Lambda-Proxy-Anfrage.\
   Das Context-Objekt wird verwendet, um einen Lambda-Logger abzurufen, mit dem eine Meldung in die CloudWatchLogs geschrieben wird.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Rufen Sie beim Aufrufen der handleRequest-Methode das Attribut „newState“ der Ereignisabonnementnachricht ab, das den aktualisierten Status der Ressource darstellt.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Weitere Informationen zum newState-Format finden Sie unter [Format ausgehender Nachrichten für Ereignisabonnements](../../wf-api/api/message-format-event-subs.md).

3. Nachdem Sie die Zuordnung „newState“ aus der Nachricht analysiert haben, stellen Sie sicher, dass die Gruppen-ID des -Objekts mit der in Schritt 1 identifizierten Gruppen-ID übereinstimmt.

4. (Bedingt) Wenn die IDs **nicht** übereinstimmen, die Nachricht ablegen, sodass eine leere Antwort zurückgegeben wird.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >Die Rückgabe einer leeren, erfolgreichen Antwort ist von entscheidender Bedeutung. Alles außer einer Antwort auf 200 Ebenen wird als fehlgeschlagener Versand betrachtet.

5. Verarbeiten Sie die Nachricht.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   AWS SDK wird verwendet, um einen anderen Lambda-Ausdruck aufzurufen, der für den Versand der gefilterten Nachricht an unseren gewünschten Endpunkt verantwortlich ist.

   Durch die Weitergabe der Verantwortung für den Versand der Nachricht an einen anderen Lambda-Service wird ein Timeout der Versandanfrage durch den Ereignisabonnement-Service vermieden. Derzeit ist die zulässige Zeitüberschreitung für den Versand auf fünf Sekunden festgelegt. Wenn der Filter länger dauert als durch die Einstellung zulässig, können Sie die Anfrage verarbeiten, aber der Ereignisabonnement-Service wird mit einer Zeitüberschreitung beendet und fällt in eine Wiederholungsschleife, bis er innerhalb der Zeitüberschreitungsspanne eine Antwort von 200 Ebenen erhält.

   Weitere Informationen zum Verwalten des Nachrichtenversands finden Sie unter [Verbessern des Nachrichtenversands bei gleichzeitiger Berücksichtigung von Zeitüberschreitungen](#improving-message-delivery-while-accommodating-timeouts).

### Python

Der Hauptunterschied zwischen den Java- und Python-Beispielen besteht darin, dass im Java-Beispiel die Ereignisabonnementnachricht als erster Parameter empfangen wird und im Python-Beispiel ist der erste Parameter ein Lambda-Proxy-Ereignis , das die Ereignisabonnementnachricht zusammen mit Informationen zur AWS Lambda-Proxy-Anfrage enthält.

Das folgende Beispiel in Python zeigt, wie Sie Projekt-Payloads basierend auf der Gruppen-ID des Projekts filtern, wie in [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Legen Sie die gesuchte Gruppen-ID fest und erstellen Sie sie als statische Konstante.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   Der erste Parameter ist der Lambda-Proxy „event“, der die Ereignisabonnementnachricht und einige zusätzliche Informationen enthält, die ausgewertet werden müssen.\
   Der zweite Parameter ist der Kontext der aktuellen Lambda-Proxy-Anfrage.\
   In diesem Beispiel wird das Context-Objekt verwendet, um eine Lambda-Protokollierung abzurufen, die zum Schreiben einer Meldung in die CloudWatchLogs verwendet wird.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analysieren Sie die Nachricht aus dem Ereignis.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Rufen Sie das Attribut „newState“ der Ereignisabonnementnachricht ab.\
   Das newState-Attribut stellt den aktualisierten Status der Ressource dar.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Weitere Informationen zum newState-Format finden Sie unter [Format ausgehender Nachrichten für Ereignisabonnements](../../wf-api/api/message-format-event-subs.md).

1. Nachdem Sie die Zuordnung „newState“ aus der Nachricht analysiert haben, stellen Sie sicher, dass die Gruppen-ID des -Objekts mit der in Schritt 1 identifizierten Gruppen-ID übereinstimmt.

1. (Bedingt) Wenn die IDs nicht übereinstimmen, die Nachricht ablegen, sodass eine leere Antwort zurückgegeben wird.

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >Die Rückgabe einer leeren, erfolgreichen Antwort ist von entscheidender Bedeutung. Alles außer einer Antwort auf 200 Ebenen wird als fehlgeschlagener Versand betrachtet.

1. Verarbeiten Sie die Nachricht.

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   AWS SDK wird verwendet, um einen anderen Lambda-Ausdruck aufzurufen, der für den Versand der gefilterten Nachricht an unseren gewünschten Endpunkt verantwortlich ist.

   Durch die Weitergabe der Verantwortung für den Versand der Nachricht an einen anderen Lambda-Service wird ein Timeout der Versandanfrage durch den Ereignisabonnement-Service vermieden. Derzeit ist die maximale Wartezeit für den Versand auf fünf Sekunden festgelegt. Wenn der Filter länger dauert als durch die Einstellung zulässig, können Sie die Anfrage verarbeiten, aber der Ereignisabonnement-Service wird mit einer Zeitüberschreitung beendet und fällt in eine Wiederholungsschleife, bis er innerhalb der Zeitüberschreitungsspanne eine Antwort von 200 Ebenen erhält.


### Node.js

Das Node.js-Beispiel für die Filterung der Projektgruppen-ID liest sich ähnlich wie die Java- und Python-Beispiele. Wie beim Python-Beispiel ist der erste Parameter ein Lambda-Proxy-Ereignis und der zweite Parameter der Lambda-Kontext.

Das folgende Beispiel in Node.js zeigt, wie Projekt-Payloads basierend auf der Gruppen-ID des Projekts gefiltert werden, wie in [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Legen Sie die gesuchte Gruppen-ID fest und erstellen Sie sie als statische Konstante.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   Der erste Parameter ist der Lambda-Proxy „event“, der die Ereignisabonnementnachricht und einige zusätzliche Informationen enthält, die ausgewertet werden müssen.\
   Der zweite Parameter ist der Kontext der aktuellen Lambda-Proxy-Anfrage.\
   In diesem Beispiel wird das Context-Objekt verwendet, um eine Lambda-Protokollierung abzurufen, die zum Schreiben einer Meldung in die CloudWatchLogs verwendet wird.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Analysieren Sie die Nachricht aus dem Ereignis.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Rufen Sie die projectGroupID aus dem Attribut „newState“ der Ereignisabonnementnachricht ab und gleichen Sie sie dann mit der Gruppen-ID der Gruppe ab, die Sie in Schritt 1 identifiziert haben.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Weitere Informationen zum newState-Format finden Sie unter [Format ausgehender Nachrichten für Ereignisabonnements](../../wf-api/api/message-format-event-subs.md).

4. (Bedingt) Wenn die IDs nicht übereinstimmen, die Nachricht ablegen, sodass eine leere Antwort zurückgegeben wird.\
   Das folgende Beispiel zeigt übereinstimmende Gruppen-IDs:

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >Die Rückgabe einer leeren, erfolgreichen Antwort ist von entscheidender Bedeutung. Alles außer einer Antwort auf 200 Ebenen wird als fehlgeschlagener Versand betrachtet.

5. Verarbeiten Sie die Nachricht.

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   AWS SDK wird verwendet, um einen anderen Lambda-Ausdruck aufzurufen, der für den Versand der gefilterten Nachricht an unseren gewünschten Endpunkt verantwortlich ist.\
   Durch die Weitergabe der Verantwortung für den Versand der Nachricht an einen anderen Lambda-Service wird ein Timeout der Versandanfrage durch den Ereignisabonnement-Service vermieden. Derzeit ist die maximale Wartezeit für den Versand auf fünf Sekunden festgelegt. Wenn der Filter länger dauert als durch die Einstellung zulässig, können Sie die Anfrage verarbeiten, aber der Ereignisabonnement-Service wird mit einer Zeitüberschreitung beendet und fällt in eine Wiederholungsschleife, bis er innerhalb der Zeitüberschreitungsspanne eine Antwort von 200 Ebenen erhält.\
   Informationen zum Verwalten des Nachrichtenversands finden Sie unter [Verbessern des Nachrichtenversands bei gleichzeitiger Berücksichtigung von Zeitüberschreitungen](#improving-message-delivery-while-accommodating-timeouts).

## Verbesserung des Nachrichtenversands bei gleichzeitiger Berücksichtigung von Zeitüberschreitungen

Der Ereignisabonnement-Service hat eine strikte Zeitüberschreitung von **fünf Sekunden** für alle Versandanfragen. Wenn der Versand einer Nachricht die zulässige Zeit überschreitet, beginnt der Ereignisabonnement-Service einen Wiederholungszyklus für diese Nachricht.

Sie erstellen beispielsweise einen Projektgruppen-ID-Filter, der einem der Beispiele unter &quot;[ von Ereignisnachrichten“ ähnelt](#filtering-event-messages) und Sie schließen eine Datenbanksuche ein, um zu ermitteln, ob die Nachricht benötigt wird. Möglicherweise dauert die Datenbanksuche zusammen mit der Zeit, die für die erforderliche Verarbeitung und den Kaltstart des Lambda-Elements erforderlich ist, mehr als fünf Sekunden, sodass der Ereignisabonnement-Service den Versand der Nachricht wiederholt.

Sie können einen erneuten Versuch verhindern, indem Sie die zeitaufwendigen Teile des Prozesses von der Logik trennen, die für die Bestimmung verantwortlich ist, ob es sich bei der Nachricht um eine Nachricht handelt, die Sie verarbeiten und versenden möchten. Auf diese Weise können Sie die Nachricht akzeptieren und eine Antwort der Ebene 200 an den Ereignisabonnement-Service zurücksenden, während Sie die Nachricht asynchron im Hintergrund weiter verarbeiten oder filtern (siehe Beispiel [ Schritt 5 in ](#java)Java).


Auch wenn Ihre Verarbeitung oder Filterung die Fünf-Sekunden-Zeitüberschreitung nicht überschreitet, ist es dennoch vorteilhaft, den ersten Berührungspunkt der Nachrichtenfilterung oder -verarbeitung von den anderen Verarbeitungs- oder Versandschritten auf der Client-Seite zu trennen. Auf diese Weise hat die Übergabe der Nachricht vom Ereignisabonnement-Service an das Ziel nur minimale Zeit- und Leistungsauswirkungen für beide Parteien.

Weitere Informationen zum Wiederholungsmechanismus finden Sie unter [Wiederholungen von Ereignisabonnements](../../wf-api/api/event-sub-retries.md).

## Implementieren gehosteter Filter in der Cloud-losen Architektur

Wenn Sie keine Cloud-Architektur für die Filterung von Ereignisabonnements nutzen können, können Sie die Beispiele unter [Filtern von Ereignisnachrichten](#filtering-event-messages) als Roadmaps für die Implementierung Ihrer eigenen gehosteten Filter oder Verarbeitungskomponenten verwenden.

### Anpassen von Filterbeispielen für eigenständige Services

Bevor Sie die Filterbeispiele in einer Cloud-losen Umgebung verwenden, gehen Sie wie folgt vor:

* Lassen Sie die Lambda-spezifischen Teile der Beispiele aus, z. B. den Kontextparameter.

* Ändern Sie die Aufrufe anderer Lambdas in den Beispielen in zusätzliche asynchrone HTTP-Anfragen an andere Filter oder Verarbeitungskomponenten, die Sie hosten.

* Wenn Sie auf die Beispiele Python und Node.js verweisen, ersetzen Sie den ersten Ereignisparameter durch den ersten Payload-Parameter, der im Java-Beispiel gezeigt wird. Siehe Schritt 1 in [Java](#java).

* Stellen Sie die Filter oder Prozessoren mit einer Web-basierten API bereit.

### Verpasste Ereignisabonnementnachrichten verhindern

In einer Cloud-losen Architektur sind Services, die für den Empfang von Ereignisabonnementnachrichten verantwortlich sind, gelegentlich nicht erreichbar. In einem solchen Fall können Nachrichten das Limit für weitere Zustellversuche überschreiten und verloren gehen, ohne dass die Informationen innerhalb der Nachrichten abgerufen werden können.

Es wird empfohlen, beim Start des Dienstes eine Abfrage zu implementieren, in der der aktuelle Status aller Ressourcen abgefragt wird, die in den verpassten Nachrichten enthalten sein könnten. Wie im folgenden Beispiel gezeigt, können Sie die Filterkriterien verwenden, um nach Ressourcen zu suchen, die diesen Kriterien entsprechen, und dann ihren aktuellen Status verarbeiten.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

Indem Sie nach Ressourcen suchen, stellen Sie sicher, dass Ihre integrierten Systeme über die aktuelle Version der Ressourcen verfügen.

### Implementieren der asynchronen Verarbeitung beim Nachrichtenversand

Bei allen Beispielen im Abschnitt [Filtern von Ereignisnachrichten](#filtering-event-messages) wird die Verantwortung für den Versand gefilterter Nachrichten an ein anderes AWS Lambda übergeben. Dies geschieht, um eine Überschreitung des Fünf-Sekunden-Timeouts in der Versandanfrage zu vermeiden, das vom Ereignisabonnement-Service erzwungen wird, der die Anfrage ausstellt.

In einer Cloud-losen Architektur müssen Sie möglicherweise einen asynchronen Verarbeitungsmechanismus implementieren, der dem ähnelt, mit dem AWS SDK asynchrone Aufrufe an andere AWS-Lambdas ermöglicht. Die meisten modernen Programmiersprachen verfügen über Drittanbieter- oder Kernbibliotheken für die asynchrone Verarbeitung, sodass Sie die in unseren Beispielen implementierte asynchrone Verarbeitung nutzen können.
