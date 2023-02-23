---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtern von Ereignis-Abonnementnachrichten
description: Filtern von Ereignis-Abonnementnachrichten
author: John
feature: Workfront API
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# Filtern von Ereignis-Abonnementnachrichten

Sie können intermediäre Verarbeitungskomponenten erstellen, die Ihnen dabei helfen, nur die für Ihr Unternehmen benötigten Ereignisabonnementnachrichten zu filtern und zu verarbeiten.

Weitere Informationen zu Ereignisanmeldungen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## Filtern von Ereignismeldungen

Dieser Abschnitt enthält Code-Snippets zum Filtern, die Sie implementieren können, um das Laden von Ereignis-Abonnementnachrichten zu verringern.  Um die Unterschiede in der Syntax verschiedener Sprachen zu veranschaulichen, veranschaulichen diese Snippets denselben Satz von Filtern, die in den folgenden Sprachen geschrieben wurden:

Sie können Beispiele für die Filterung unter [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples), wo Sie die Unterschiede in der Syntax für jede Sprache und die Möglichkeiten der Interaktion mit dem AWS SDK sehen können. Diese Beispiele werden als AWS Lambdas geschrieben, eine gängige Methode zur Verwendung von intermediären Filter- und Verarbeitungskomponenten.

Die folgenden Code-Snippets sind nahezu einsatzbereit und können als Ausgangspunkt verwendet werden, um Ihnen beim Schreiben Ihrer eigenen, komplexeren Filter und Verarbeitungskomponenten zu helfen.

### Java

Das folgende Beispiel in Java zeigt, wie Projektnutzlasten basierend auf der Gruppen-ID des Projekts gefiltert werden, wie in [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Richten Sie die gesuchte Gruppen-ID ein und erstellen Sie sie als statische Konstante.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   In diesem Beispiel nimmt die handleRequest -Methode, bei der es sich um einen AWS-Lambda-Standardmethodennamen handelt, als ersten Parameter einen Zuordnungstyp an, nämlich den Inhalt der Ereignisabonnementnachricht.\
   Der zweite Parameter, der verwendet wird, ist der Kontext der aktuellen Lambda-Proxy-Anfrage.\
   Das Context-Objekt wird zum Abrufen eines Lambda-Loggers verwendet, der zum Schreiben einer Nachricht in die CloudWatchLogs verwendet wird.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Rufen Sie nach Aufruf der handleRequest -Methode das Attribut &quot;newState&quot;der Ereignisabonnementnachricht ab, die den aktualisierten Status der Ressource darstellt.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Weitere Informationen zum newState-Format finden Sie unter [Ausgehendes Nachrichtenformat für Ereignisabonnements](../../wf-api/api/message-format-event-subs.md).

3. Stellen Sie nach dem Analysieren der &quot;newState&quot;-Zuordnung aus der Nachricht sicher, dass die Gruppen-ID des Objekts mit der in Schritt 1 identifizierten Gruppen-ID übereinstimmt.

4. (Bedingt) Wenn die IDs **nicht** übereinstimmen, legen Sie die Nachricht ab, sodass eine leere Antwort zurückgegeben wird.

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
   >Es ist entscheidend, eine leere, erfolgreiche Antwort zurückzugeben. Alles außer einer Antwort auf 200 Ebenen gilt als fehlgeschlagener Versand.

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

   Das AWS SDK wird verwendet, um ein weiteres Lambda aufzurufen, das für die Bereitstellung der gefilterten Nachricht an den gewünschten Endpunkt zuständig ist.

   Der Zweck der Absendung der Nachricht an ein anderes Lambda besteht darin, eine Zeitüberschreitung bei der Versandanfrage zu vermeiden, die vom Event Subscription Service stammt. Derzeit ist der zulässige Timeout für die Bereitstellung auf fünf Sekunden festgelegt. Wenn der Filter länger dauert, als von der Einstellung erlaubt, können Sie die Anforderung verarbeiten. Der Ereignisabonnementdienst reagiert jedoch mit einer Zeitüberschreitung und fällt in eine Wiederholungsschleife, bis er innerhalb der Zeitüberschreitungsdauer eine Antwort von 200 Ebenen erhält.

   Weitere Informationen zur Verwaltung des Nachrichtenversands finden Sie unter [Verbessern der Nachrichtenbereitstellung bei gleichzeitiger Unterstützung von Timeouts](#improving-message-delivery-while-accommodating-timeouts).

### Python

Der Hauptunterschied zwischen den Java- und Python-Beispielen besteht darin, dass im Java-Beispiel die Ereignisabonnementnachricht als erster Parameter empfangen wird und im Python-Beispiel der erste Parameter ein Lambda-Proxy-Ereignis ist, das die Ereignisabonnementnachricht zusammen mit Informationen zur AWS-Lambda-Proxy-Anfrage enthält.

Das folgende Beispiel in Python zeigt, wie Projektnutzlasten basierend auf der Gruppen-ID des Projekts gefiltert werden, wie in  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Richten Sie die gesuchte Gruppen-ID ein und erstellen Sie sie als statische Konstante.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   Der erste Parameter ist das Lambda-Proxy-&quot;Ereignis&quot;, das die Abonnementnachricht für das Ereignis und einige zusätzliche Informationen enthält, die analysiert werden müssen.\
   Der zweite Parameter ist der Kontext der aktuellen Lambda-Proxy-Anfrage.\
   In diesem Beispiel wird das Context-Objekt zum Abrufen eines Lambda-Loggers verwendet, der zum Schreiben einer Nachricht in die CloudWatchLogs verwendet wird.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analysieren Sie die Nachricht aus dem Ereignis.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Rufen Sie das Attribut &quot;newState&quot;der Ereignisabonnementnachricht ab.\
   Das Attribut newState stellt den aktualisierten Status der Ressource dar.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Weitere Informationen zum newState-Format finden Sie unter [Ausgehendes Nachrichtenformat für Ereignisabonnements](../../wf-api/api/message-format-event-subs.md).

1. Stellen Sie nach dem Analysieren der &quot;newState&quot;-Zuordnung aus der Nachricht sicher, dass die Gruppen-ID des Objekts mit der in Schritt 1 identifizierten Gruppen-ID übereinstimmt.

1. (Bedingt) Wenn die IDs nicht übereinstimmen, legen Sie die Nachricht ab, damit eine leere Antwort zurückgegeben wird.

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
   >Es ist entscheidend, eine leere, erfolgreiche Antwort zurückzugeben. Alles außer einer Antwort auf 200 Ebenen gilt als fehlgeschlagener Versand.

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

   Das AWS SDK wird verwendet, um ein weiteres Lambda aufzurufen, das für die Bereitstellung der gefilterten Nachricht an den gewünschten Endpunkt zuständig ist.

   Der Zweck der Absendung der Nachricht an ein anderes Lambda besteht darin, eine Zeitüberschreitung bei der Versandanfrage zu vermeiden, die vom Event Subscription Service stammt. Derzeit ist der Timeout für die Bereitstellung auf fünf Sekunden festgelegt. Wenn der Filter länger dauert, als von der Einstellung erlaubt, können Sie die Anforderung verarbeiten. Der Ereignisabonnementdienst reagiert jedoch mit einer Zeitüberschreitung und fällt in eine Wiederholungsschleife, bis er innerhalb der Zeitüberschreitungsdauer eine Antwort von 200 Ebenen erhält.


### Node.js

Das Node.js-Beispiel für die Filterung der Projektgruppen-ID liest ähnlich den Beispielen für Java und Python. Wie beim Python-Beispiel ist der erste Parameter ein Lambda-Proxy-Ereignis und der zweite Parameter der Lambda-Kontext.

Im folgenden Beispiel in Node.js wird gezeigt, wie Projektnutzlasten basierend auf der Gruppen-ID des Projekts gefiltert werden, wie dies in  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Richten Sie die gesuchte Gruppen-ID ein und erstellen Sie sie als statische Konstante.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   Der erste Parameter ist das Lambda-Proxy-&quot;Ereignis&quot;, das die Abonnementnachricht für das Ereignis und einige zusätzliche Informationen enthält, die analysiert werden müssen.\
   Der zweite Parameter ist der Kontext der aktuellen Lambda-Proxy-Anfrage.\
   In diesem Beispiel wird das Context-Objekt zum Abrufen eines Lambda-Loggers verwendet, der zum Schreiben einer Nachricht in die CloudWatchLogs verwendet wird.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Analysieren Sie die Nachricht aus dem Ereignis.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Rufen Sie die projectGroupID aus dem Attribut &quot;newState&quot;der Ereignisabonnementnachricht ab und gleichen Sie sie dann mit der Gruppen-ID der Gruppe ab, die Sie in Schritt 1 identifiziert haben.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Weitere Informationen zum newState-Format finden Sie unter [Ausgehendes Nachrichtenformat für Ereignisabonnements](../../wf-api/api/message-format-event-subs.md).

4. (Bedingt) Wenn die IDs nicht übereinstimmen, legen Sie die Nachricht ab, damit eine leere Antwort zurückgegeben wird.\
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
   >Es ist entscheidend, eine leere, erfolgreiche Antwort zurückzugeben. Alles außer einer Antwort auf 200 Ebenen gilt als fehlgeschlagener Versand.

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

   Das AWS SDK wird verwendet, um ein weiteres Lambda aufzurufen, das für die Bereitstellung der gefilterten Nachricht an den gewünschten Endpunkt zuständig ist.\
   Der Zweck der Absendung der Nachricht an ein anderes Lambda besteht darin, eine Zeitüberschreitung bei der Versandanfrage zu vermeiden, die vom Event Subscription Service stammt. Derzeit ist der Timeout für die Bereitstellung auf fünf Sekunden festgelegt. Wenn der Filter länger dauert, als von der Einstellung erlaubt, können Sie die Anforderung verarbeiten. Der Ereignisabonnementdienst reagiert jedoch mit einer Zeitüberschreitung und fällt in eine Wiederholungsschleife, bis er innerhalb der Zeitüberschreitungsdauer eine Antwort von 200 Ebenen erhält.\
   Weitere Informationen zur Verwaltung des Nachrichtenversands finden Sie unter [Verbessern der Nachrichtenbereitstellung bei gleichzeitiger Unterstützung von Timeouts](#improving-message-delivery-while-accommodating-timeouts).

## Verbessern der Nachrichtenbereitstellung bei gleichzeitiger Unterstützung von Timeouts

Der Ereignisabonnement-Dienst hat eine strikte Zeitüberschreitung von **fünf Sekunden** für alle Versandanfragen. Falls der Versand einer Nachricht die zulässige Zeit überschreitet, beginnt der Ereignisabonnement-Dienst einen Wiederholungszyklus für diese Nachricht.

Sie erstellen beispielsweise einen Projektgruppen-ID-Filter ähnlich einem der Beispiele unter [Filtern von Ereignismeldungen](#filtering-event-messages) und Sie fügen eine Datenbanksuche hinzu, um zu bestimmen, ob die Nachricht benötigt wird. Es ist möglich, dass die Datenbanksuche zusammen mit der für die erforderliche Verarbeitung und den Kaltstart des Lambda erforderlichen Zeit mehr als fünf Sekunden dauern kann, wodurch der Ereignisabonnementdienst den Nachrichtenversand erneut versucht.

Sie können einen erneuten Versuch verhindern, indem Sie die zeitaufwendigen Teile des Prozesses von der Logik trennen, die dafür verantwortlich ist, zu bestimmen, ob die Nachricht verarbeitet und bereitgestellt werden soll. Auf diese Weise können Sie die Nachricht akzeptieren und eine 200-Grad-Antwort an den Event Subscription-Dienst zurücksenden, während Sie die Nachricht asynchron weiter im Hintergrund verarbeiten oder filtern (siehe Schritt 5 unter [Java](#java) Beispiel).


Auch wenn Ihre Verarbeitung oder Filterung die Zeitüberschreitung von fünf Sekunden nicht überschreitet, ist es dennoch von Vorteil, den ersten Touchpoint der Nachrichtenfilterung oder -verarbeitung von den anderen Verarbeitungs- oder Versandschritten auf der Clientseite zu trennen. Auf diese Weise hat die Übergabe der Nachricht vom Event Subscription-Dienst an das Ziel nur geringe Zeit- und Leistungseinbußen für beide Parteien.

Weitere Informationen zum Wiederholungsmechanismus finden Sie unter [Wiederholungen von Ereignisabonnements](../../wf-api/api/event-sub-retries.md).

## Implementieren gehosteter Filter in Cloudless Architecture

Wenn Sie keine Cloud-Architektur für die Filterung von Ereignisabonnements nutzen können, können Sie die Beispiele unter [Filtern von Ereignismeldungen](#filtering-event-messages) als Roadmaps zur Implementierung Ihrer eigenen gehosteten Filter oder Verarbeitungskomponenten.

### Anpassen von Filterbeispielen für eigenständige Dienste

Bevor Sie die Filterbeispiele in einer Cloudless-Umgebung verwenden, gehen Sie wie folgt vor:

* Lassen Sie die Lambda-spezifischen Teile der Beispiele weg, z. B. den Parameter Kontext .

* Ändern Sie die Aufrufe anderer Lambdas in den Beispielen, um zusätzliche asynchrone HTTP-Anfragen an andere Filter oder Verarbeitungskomponenten zu senden, die Sie hosten.

* Wenn Sie auf die Beispiele Python und Node.js verweisen, ersetzen Sie den ersten Ereignisparameter durch den ersten Payload-Parameter, der im Java-Beispiel gezeigt wird. Siehe Schritt 1 unter [Java](#java).

* Stellen Sie die Filter oder Prozessoren mit einer webbasierten API bereit.

### Fehlende Meldungen zur Ereignisanmeldung verhindern

Gelegentlich sind in einer Cloud-Architektur Dienste, die für den Empfang von Ereignis-Abonnementnachrichten verantwortlich sind, möglicherweise nicht erreichbar. In einem solchen Fall können Nachrichten die Wiederholungsgrenze überschreiten und gehen verloren, ohne dass die Informationen in den Nachrichten abgerufen werden können.

Es wird empfohlen, beim Starten Ihres Dienstes eine Abfrage zu implementieren, um den neuesten Status aller Ressourcen anzuzeigen, die möglicherweise in den verpassten Nachrichten enthalten waren. Wie im folgenden Beispiel gezeigt, können Sie mithilfe der Filterkriterien nach Ressourcen suchen, die diesen Kriterien entsprechen, und dann ihren aktuellen Status verarbeiten.

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

Durch die Abfrage von Ressourcen stellen Sie sicher, dass Ihre Integrationssysteme über die aktuellste Version der Ressourcen verfügen.

### Implementieren der asynchronen Verarbeitung im Versand von Nachrichten

Alle Beispiele im [Filtern von Ereignismeldungen](#filtering-event-messages) übergibt die Verantwortung für den Versand gefilterter Nachrichten an ein anderes AWS Lambda. Dies geschieht, um zu vermeiden, dass die 5-Sekunden-Zeitüberschreitung in der Versandanfrage überschritten wird, die vom Event Subscription Service erzwungen wird, der die Anfrage ausgibt.

In einer Cloud-losen Architektur müssen Sie möglicherweise einen asynchronen Verarbeitungsmechanismus implementieren, ähnlich wie das AWS SDK asynchrone Aufrufe an andere AWS Lambdas ermöglicht. Die meisten modernen Programmiersprachen verfügen über Drittanbieter- oder Core-Bibliotheken, die die asynchrone Verarbeitung handhaben, sodass Sie den in unseren Beispielen implementierten asynchronen Verarbeitungsstil nutzen können.
