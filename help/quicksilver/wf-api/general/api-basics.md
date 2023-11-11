---
content-type: api
navigation-topic: general-api
title: API-Grundlagen
description: API-Grundlagen
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '4475'
ht-degree: 0%

---


# API-Grundlagen

Ziel der Adobe Workfront-API ist es, die Erstellung von Integrationen mit Workfront zu vereinfachen, indem eine REST-fähige Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind und den Ansatz der Workfront-API beschrieben.

Eine Kenntnis des Workfront-Schemas hilft Ihnen dabei, die Datenbankbeziehungen zu verstehen, die zum Abrufen von Daten aus Workfront für Integrationszwecke genutzt werden können.

## Einschränkungen und Richtlinien

Um eine konsistente On-Demand-Systemleistung von Workfront sicherzustellen, ist jeder Kunde auf 10 gleichzeitige API-Threads beschränkt. Die Sandbox-Umgebung hat dieselbe Grenze, sodass Kunden und Partner API-Aufrufe genau testen können, bevor Code für die Produktion freigegeben wird.

Für Produktions-, Vorschau- und Testumgebungen haben Endbenutzeranforderungen eine maximale URI-Länge von 8892 Byte, da sie über das Workfront CDN (Akamai) weitergeleitet werden. Diese Beschränkung gilt nur für URIs, die über das CDN weitergeleitet werden.

>[!NOTE]
>
>Diese Beschränkung gilt nicht für Sandbox-Umgebungen, da Sandbox-Umgebungen nicht über das CDN weitergeleitet werden.

### Haftungsausschluss

Jede Verwendung der API sollte in der Workfront Beta-Umgebung getestet werden, bevor sie in der Produktionsumgebung ausgeführt wird. Wenn ein Kunde die API für einen Prozess verwendet, der nach vernünftigem Ermessen für Workfront mit der On-Demand-Software belastend ist (d. h., der Prozess verursacht wesentliche negative Auswirkungen auf die Leistung der Software für andere Kunden), behält sich Workfront das Recht vor, vom Kunden die Beendigung dieses Prozesses zu verlangen. Wenn der Kunde nicht einhält und das Problem weiterhin besteht, behält sich Workfront das Recht vor, den Prozess zu beenden.

## REST-Grundlagen

In diesem Abschnitt erhalten Sie eine allgemeine Einführung in die Interaktion mit der Workfront REST-API für die folgenden REST-Grundsätze:

### Objekt-URI

Jedes Objekt im System erhält einen eindeutigen URI, der aus dem Objekttyp und der ID besteht. Die folgenden Beispiele zeigen URIs, die drei eindeutige Objekte beschreiben:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Beim Objekttyp wird nicht zwischen Groß- und Kleinschreibung unterschieden. Hierbei kann es sich entweder um den abgekürzten ObjCode (z. B. proj) oder den alternativen Objektnamen (project) handeln.

Eine Liste der gültigen ObjCodes finden Sie unter  [API-Explorer](../../wf-api/general/api-explorer.md).

### Vorgänge

Objekte werden bearbeitet, indem eine HTTP-Anfrage an ihren eindeutigen URI gesendet wird. Der auszuführende Vorgang wird durch die HTTP-Methode angegeben.

Die standardmäßigen HTTP-Methoden entsprechen den folgenden Vorgängen:

* **GET** - Ruft ein Objekt nach ID ab, sucht mithilfe einer Abfrage nach allen Objekten, führt Berichte aus oder führt benannte Abfragen aus
* **POST** - Fügt ein neues Objekt ein
* **PUT** - Bearbeiten eines vorhandenen Objekts
* **DELETE** - Löscht ein Objekt

Um Client-Mängel oder Beschränkungen der Protokolllänge zu umgehen, kann der Methodenparameter verwendet werden, um das HTTP-Verhalten zu überschreiben. Beispielsweise kann ein GET-Vorgang durch Posten des folgenden URI implementiert werden:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Antwort

Jede Anfrage erhält eine Antwort im JSON-Format. Die Antwort verfügt entweder über ein Datenattribut, wenn die Anfrage erfolgreich war, oder über ein Fehlerattribut, wenn ein Problem aufgetreten ist. Beispielsweise die Anfrage

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

gibt eine JSON-Antwort zurück, die der folgenden ähnelt:


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Bei der Ausführung einer GET-Anfrage über die Adressleiste Ihres Browsers ist es nicht erforderlich, die sessionID als Teil der Anfrage einzubeziehen.

Besondere Sicherheit wurde für PUT-, POST- und DELETE-Anfragen hinzugefügt. Eine Anforderung, die Schreibvorgänge an die Datenbank ausführt oder diese löscht, kann nur ausgeführt werden, wenn die Variable **sessionID=abc123** ist im URI enthalten. Die folgenden Beispiele zeigen, wie dies nach einer DELETE-Anfrage suchen würde:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Authentifizierung

Die API authentifiziert jede Anfrage, um sicherzustellen, dass der Client Zugriff auf das Anzeigen oder Ändern eines angeforderten Objekts hat.

Die Authentifizierung erfolgt durch Übergabe einer Sitzungs-ID, die mit einer der folgenden Methoden angegeben werden kann:

#### Authentifizierung des Anforderungsheaders

Die bevorzugte Authentifizierungsmethode besteht darin, einen Anforderungsheader namens SessionID zu übergeben, der das Sitzungstoken enthält. Das hat den Vorteil, dass man vor [Cross-Site Request Forgery (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) greift zu und stört nicht den URI zum Zwischenspeichern.

Im Folgenden finden Sie ein Beispiel für eine Anfrage-Kopfzeile:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Authentifizierung von Anfrageparametern

Sie können sich authentifizieren, indem Sie einen Anforderungsparameter namens sessionID übergeben, wie im folgenden Beispiel gezeigt: 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Cookie-basierte Authentifizierung

Die API verwendet dieselbe Cookie-basierte Authentifizierung, die von der Web-Benutzeroberfläche für das System verwendet wird. Wenn sich ein Client über die Web-Benutzeroberfläche bei Workfront anmeldet, verwenden alle AJAX Aufrufe, die innerhalb desselben Browsers durchgeführt werden, dieselbe Authentifizierung.

>[!NOTE]
>
>Zum Schutz vor CSRF-Angriffen (Cross Site Request Forgery) ist diese Authentifizierungsmethode nur für schreibgeschützte Vorgänge verfügbar.

## Anmeldung

>[!IMPORTANT]
>
Workfront empfiehlt nicht mehr die Verwendung der `/login` -Endpunkt oder API-Schlüssel. Verwenden Sie stattdessen eine der folgenden Authentifizierungsmethoden:
>
* Serverauthentifizierung mit JWT
* Benutzerauthentifizierung mit OAuth2
>
Anweisungen zum Einrichten dieser Authentifizierungsmethoden finden Sie unter [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
Anweisungen zur Verwendung der Serverauthentifizierung in Workfront finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-jwt-flow.md)
>
Anweisungen zur Verwendung der Benutzerauthentifizierung in Workfront finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscode-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
Das in diesem Abschnitt beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Adobe Business Platform integriert wurden. Die Anmeldung bei Workfront über die Workfront-API ist nicht verfügbar, wenn Ihr Unternehmen in die Adobe Business Platform integriert wurde.
>
Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Business Platform integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Mit einem gültigen Benutzernamen und Kennwort können Sie die folgende Anfrage verwenden, um eine Sitzungs-ID zu erhalten:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Dadurch wird ein Cookie gesetzt, um zukünftige Anforderungen zu authentifizieren und eine JSON-Antwort mit der neu erstellten sessionID, der Benutzer-ID des angemeldeten Benutzers und anderen Sitzungsattributen zurückzugeben.

>[!NOTE]
>
Wenn Sie über einen bestimmten API-Benutzer verfügen, der auch Administrator ist, empfiehlt Workfront dringend, sich mit einem API-Schlüssel anzumelden.

**Generieren eines API-Schlüssels**

Sie können einen API-Schlüssel generieren, wenn Sie sich als dieser Benutzer beim System anmelden, wie im folgenden Beispiel gezeigt:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Abrufen eines zuvor generierten API-Schlüssels**

Sie können auch einen API-Schlüssel abrufen, der zuvor für einen bestimmten Benutzer generiert wurde, indem Sie getApiKey ausführen:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Anschließend können Sie dieses Ergebnis verwenden, um jeden API-Aufruf zu authentifizieren, indem Sie &quot;apiKey&quot;als Anforderungsparameter mit diesem Wert anstelle einer sessionID oder eines Benutzernamen und Kennworts hinzufügen. Aus sicherheitspolitischer Sicht ist dies von Vorteil.

Die folgende Anfrage ist ein Beispiel für das Abrufen von Daten aus einem Projekt mithilfe des apiKey:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidierung eines API-Schlüssels**

Wenn der apiKey -Wert kompromittiert wurde, können Sie &quot;clearApiKey&quot;ausführen, der den aktuellen API-Schlüssel ungültig macht, wie im folgenden Beispiel gezeigt:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Nach der Löschung können Sie getApiKey erneut ausführen, um einen neuen API-Schlüssel zu generieren.

### Abmelden

Wenn eine Sitzung abgeschlossen ist, können Sie die folgende Anfrage verwenden, um den Benutzer abzumelden, wodurch jeder weitere Zugriff mit der sessionID verhindert wird.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

Die abgemeldete sessionID kann entweder als Cookie, Anfragekopfzeile oder Anfrageparameter angegeben werden.

So melden Sie einen Benutzer ab:

1. Navigieren Sie zu Ihrem Anmeldebildschirm, melden Sie sich jedoch nicht an.
1. Ändern Sie die URL in /attask/api/v15.0/project/search.\
   Beachten Sie, dass die Seite nicht gefunden wird.
1. Ersetzen Sie das Wort *suchen* mit login?username=admin&amp;password=user, ersetzen Ihren Benutzernamen und Ihr Kennwort für *admin* und *user\
   *Diese Sitzung wird im Browser als Cookie gespeichert und muss nicht bei jeder nachfolgenden GET-Anfrage neu angegeben werden.

1. Ändern Sie die URL zurück zu **/attask/api/v15.0/project/search**.
1. Beachten Sie die Antwort.

Sie müssen bei der Ausführung von PUT-, POST- und DELETE-Anfragen immer die sessionID angeben, die nach der Anmeldung angegeben wurde.

## Verhalten der GET

Verwenden Sie die HTTP-GET-Methode, um ein Objekt oder mehrere Objekte abzurufen und Berichte auszuführen.

### Abrufen von Objekten

Sie können die Suche nach Objekten mithilfe von Modifikatoren und Filtern optimieren.

#### Abrufen eines Objekts mit der Objekt-ID

Wenn Sie die ID eines Objekts kennen, können Sie das Objekt abrufen, indem Sie auf seinen eindeutigen URI zugreifen. Beispielsweise die Anfrage

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

gibt eine Antwort ähnlich der folgenden zurück:

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


Sie können mehrere Objekte in derselben Anforderung abrufen, indem Sie den Parameter für die ID-Anforderung angeben und eine kommagetrennte Liste von IDs angeben, wie im folgenden Beispiel gezeigt:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Beachten Sie, dass die Anforderung /attask/api/v15.0/project?id=... mit der Anforderung übereinstimmt, dass `/attask/api/v15.0/project/...` -Anfrage.

#### Abrufen eines Objekts mit dem URI

Wenn Sie ein Objekt anhand anderer Kriterien als der ID abrufen möchten, können Sie nach dem URI suchen.

Beispielsweise können Sie die folgende Anfrage verwenden, um eine Liste aller Projekte im System zurückzugeben:

```
GET /attask/api/v15.0/project/search
```

Sie können Filter mithilfe der Anforderungsparameter als Name-Wert-Paare angeben. Im folgenden Beispiel sehen Sie eine Anfrage, die alle aktuellen Projekte finden würde:

```
GET /attask/api/v15.0/project/search?status=CUR
```

Die folgende Anfrage sucht alle Aufgaben, die noch nicht abgeschlossen sind und die einem Benutzer mit dem Namen John zugewiesen sind.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Verwenden von Suchmodifikatoren

In der folgenden Tabelle sind einige der Modifikatoren aufgeführt, die Sie mit der Workfront-API verwenden können.

| **Modifikator** | **Beschreibung** | **Beispiel** |
|---|---|---|
| eq | gibt Ergebnisse zurück, die sich im Status &quot;Geschlossen&quot;befinden | <pre>...status=cls&amp;status_Mod=eq..</pre> |
| ne | gibt Ergebnisse zurück, die sich nicht im Status &quot;Geschlossen&quot;befinden | <pre>...status=cls&amp;status_Mod=ne..</pre> |
| get | gibt Ergebnisse zurück, deren vollständige Prozent größer als oder gleich 50 ist | <pre>...percentComplete=50&amp;percentComplete_Mod=get..</pre> |
| lte | gibt Ergebnisse zurück, deren Prozentsatz vollständig kleiner als oder gleich 50 ist | <pre>...percentComplete=50&amp;percentComplete_Mod=lte..</pre> |
| isnull | gibt Ergebnisse zurück, bei denen die Beschreibung null ist | <pre>...description_Mod=isnull..</pre> |
| notnull | gibt Ergebnisse zurück, bei denen die Beschreibung nicht Null ist | <pre>...description_Mod=notnull..</pre> |
| enthält | gibt Ergebnisse zurück, bei denen der Name &quot;Workfront&quot;enthält. | <pre>...name=Workfront&amp;name_Mod=contains..</pre> |
| zwischen | gibt Ergebnisse zurück, die innerhalb der letzten 7 Tage ein Einstiegsdatum haben. | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
Bei Suchanfragen wird zwischen Groß- und Kleinschreibung unterschieden. Wenn Sie einen Fehler erhalten, stellen Sie sicher, dass  **_Mod** und **_Range** die richtige Groß-/Kleinschreibung aufweisen.

#### Verwenden von ODER-Anweisungen

Sie können die Suche verbessern, indem Sie einen Parameter hinzufügen, der &quot;OR&quot;enthält, sowie eine Zahl, die die Ebene eines Filters oder einer Reihe von Filtern angibt.

Eine OR-Anweisung gibt nur Datensätze im API-Aufruf zurück, die den Filterkriterien der OR-Anweisung entsprechen. Filter werden nicht über OR-Anweisungsebenen hinweg impliziert.

Wenn Sie beispielsweise nach

* Aufgaben mit einem Namen, der &quot;Planning&quot;OR enthält
* Aufgaben in einem Portfolio mit dem Namen &quot;FixedAssets&quot;UND zugewiesen an eine Person mit dem Namen &quot;Steve&quot;ODER
* Aufgaben mit einer übergeordneten Aufgabe namens &quot;Final Task&quot;

verwenden Sie dann den folgenden API-Aufruf mit mehreren ODER-Anweisungen:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:Portfolio:name=FixedAssets<br>&amp;OR:1:Portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Filterparameter verwenden

Ein potenzieller Fehler bei der Verwendung von URL-Parametern für Suchfilter besteht darin, dass Workfront bestimmte Parameter analysiert, bevor nach verschiedenen Authentifizierungsmethoden gesucht wird (z. B. Benutzername, Kennwort, apiKey, Cookie). In diesem Fall werden die Parameter nicht als Filter im Aufruf verwendet. 

Um dieses Problem zu vermeiden, können Sie diese Werte in Filterparametern mit JSON-Formatierung platzieren. Wenn Sie beispielsweise nach dem Benutzernamen-Testbenutzer filtern möchten, anstatt 
<pre>/attask/api/v15.0/user/search?Benutzername=testuser@workfront.com</pre>den URL-Parameter in einen Filter übergeben, wie im folgenden Beispiel gezeigt:
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Verwenden des Map Request-Parameters

Standardmäßig sind die von einer Suche zurückgegebenen Daten ein JSON-Array. Je nach Anwendungsfall kann es effizienter sein, das Ergebnis als JSON-Objekt nach ID zu indizieren. Dies kann mithilfe des map -Anforderungsparameters erfolgen. Beispielsweise die Anfrage 
<pre>/attask/api/v15.0/task/search?map=true</pre>gibt eine Antwort zurück, die nach ID indiziert ist, ähnlich der folgenden:
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "first task",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "second task",<br>            "ID": "4ca28ba60002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Verwenden des Feldanfrageparameters

Beim Abrufen eines Objekts werden standardmäßig nur die am häufigsten verwendeten Felder zurückgegeben.

Sie können den Feldanforderungsparameter verwenden, um eine kommagetrennte Liste bestimmter Felder anzugeben, die zurückgegeben werden. Beispielsweise die Anfrage
<pre>/attask/api/v15.0/task/search?fields=scheduledStartDate,priority</pre>gibt eine Antwort ähnlich der folgenden zurück:
<pre>{<br>    "priority": 2,<br>    "name": "first task",<br>    "ID": "4c7c08fa000002ff924e298ee148df4",<br>    "scheduledStartDate": "2010-08-30T09":00:00:000-060" <br>}</pre>

>[!NOTE]
>
Bei diesen Feldnamen wird zwischen Groß- und Kleinschreibung unterschieden.

Eine Liste möglicher Feldverweise finden Sie unter  [API-Explorer](../../wf-api/general/api-explorer.md)

#### Suchen nach verschachtelten Objekten

Sie können nach verschachtelten Objekten suchen. Standardmäßig werden verschachtelte Objekte nur mit dem Namen und der ID zurückgegeben. Um beispielsweise alle Probleme zusammen mit den Eigentümern abzurufen, verwenden Sie die folgende Anfrage:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Wenn weitere Informationen erforderlich sind, können Sie ein verschachteltes Feld mit Doppelpunkt-Syntax anfordern. Die folgende Anfrage sucht beispielsweise nach allen Problemen zusammen mit dem Namen, der ID, dem Titel und der Telefonnummer des Eigentümers.
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>und gibt Folgendes zurück: 
<pre>{<br>    "name": "ein wichtiges Problem",<br>    "ID": "4c78285f0000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "Operations Specialist",<br>        "phoneNumber": "555-1234",<br>        "name": "Admin User",<br>        "ID": "4c76ed7a000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Abrufen verschachtelter Sammlungen

Sie können verschachtelte Sammlungen von Objekten abrufen. Um beispielsweise ein Projekt mit allen seinen Aufgaben zu erhalten, verwenden Sie die folgende Anfrage:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>Die folgende Anfrage erhält Aufgabenzuweisungen:
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Suchen nach mehreren verschachtelten Feldern

Standardmäßig werden nur der Name und die ID jeder Aufgabe zurückgegeben, es können jedoch zusätzliche verschachtelte Felder mit Doppelsyntax angegeben werden. Um alle verfügbaren Felder für ein verwandtes Objekt oder eine Sammlung anzuzeigen, hängen Sie einfach einen Doppelpunkt und ein Sternchen an die Objekt-/Sammlungsreferenz an.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### Abrufen benutzerdefinierter Daten

Sie können benutzerdefinierte Datenfelder mit dem Präfix &quot;DE:&quot;abrufen. Um beispielsweise ein Projekt mit einem Parameter namens &quot;CustomText&quot;anzufordern, verwenden Sie die folgende Anfrage:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>die
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f000001afad0687d7b1b4e43",<br>    "DE:CustomText": "task b" <br>}</pre>Sie können auch alle benutzerdefinierten Daten für ein Objekt abrufen, indem Sie das Feld parameterValues anfordern. Beispiel, 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>gibt ähnliche Daten wie die folgenden zurück:
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### Verwenden von benannten Abfragen

Einige Objektarten haben spezifische Suchen, die häufig ausgeführt werden und verfügbar sind, indem der Name der Abfrage an das Ende des URI des Objekttyps angehängt wird. Beispielsweise ruft die folgende Anfrage die Arbeitselemente (Aufgaben und Probleme) ab, denen der Benutzer derzeit zugewiesen ist:
<pre>/attask/api/v15.0/work/myWork</pre>Named-Abfragen unterstützen das Anfordern des Feldparameters, um zusätzliche Felder abzurufen. Einige benannte Abfragen akzeptieren auch zusätzliche Filter. Eine Liste der zulässigen benannten Abfragen und Objekte finden Sie auf der Registerkarte Aktion für das Objekt im [API Explorer](../../wf-api/general/api-explorer.md).

#### Verwenden des Filters &quot;Zählung&quot;

Sie können die Anzahl der Ergebnisse angeben, die von einer bestimmten Suche zurückgegeben werden sollen. Dadurch kann der Server die Anforderung schneller verarbeiten und Bandbreite sparen. Beispielsweise die Anfrage
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>gibt die Anzahl der Ergebnisse im folgenden Format zurück:
<pre>{<br>    "count": 3 <br>}</pre>Das Ergebnis ist ein wesentlich kleinerer Download als wenn die vollständigen Objekte gesendet werden. Die Filtersyntax ist mit dem Suchbefehl identisch.

### Anfordern eines Berichts

Sie können eine Berichtsanforderung durchführen, bei der nur das Aggregat eines Felds mit einer oder mehreren Gruppierungen gewünscht wird. Wie im folgenden Beispiel gezeigt, entspricht die Berichtssyntax der SOAP-API:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>, das das folgende Ergebnis zurückgibt
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>     "Second Project": { <br>        "sum_hours": 30 <br>    } <br>}</pre>Durch Hinzufügen des Parameters $$ROLLUP=true wird auf jeder Gruppierungsebene ein Gesamtwert angegeben:
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>    "Second Project": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### Sortieren von Abfrageergebnissen in der API

Sie können Ihre Ergebnisse nach jedem Feld sortieren, wenn Sie Folgendes an Ihren API-Aufruf anhängen:

&amp;entryDate_Sort=asc

Wenn Sie beispielsweise nach Aufgabe Geplantes Startdatum sortieren möchten, entfernen Sie entryDate und ersetzen Sie es durch scheduledCompletionDate.

Dies funktioniert für die meisten Felder in Workfront.

### Abfragebeschränkungen berücksichtigen

Bei der Abfrage eines Objekts sollten die Beziehung verwandter Objekte und Suchbeschränkungen besonders berücksichtigt werden. Beispielsweise kann eine Abfrage nach Projekten, wie in der folgenden Tabelle dargestellt, maximal 2.000 Projekte zurückgeben. Diese 2.000 Projekte gelten als &quot;primäre Objekte&quot;. Wenn Sie in den Projekten das Feld Aufgaben abfragen, wird das Feld Aufgaben (eine Sammlung) zum sekundären Objekt des primären Objektprojekts. Eine Abfrage für das Feld Aufgaben kann Tausende von Aufgaben für Projekte enthalten. Insgesamt kann die kombinierte Anzahl der zurückgegebenen Objekte (Projekte und Aufgaben) 50.000 nicht überschreiten.

Um eine optimale Leistung zu gewährleisten, werden in der folgenden Tabelle die Einschränkungen für Suchanfragen aufgeführt. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Abfrageergebnis</th> 
   <th>Einschränkung</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Standardanzahl von Ergebnissen</td> 
   <td>100</td> 
   <td> Wenn im Abfragefilter keine Begrenzung angegeben ist (d. h. $$LIMIT), kann das Ergebnis maximal 100 primäre Objekte enthalten. <br>Siehe <a href="#using-paginated-responses" class="MCXref xref">Verwenden von paginierten Antworten</a> für Anweisungen zur Außerkraftsetzung dieser Beschränkung. </td> 
  </tr> 
  <tr> 
   <td>Max. Anzahl an Ergebnissen</td> 
   <td>2,000</td> 
   <td>Der Abfragefilter (d. h. $$LIMIT) kann maximal 2000 Ergebnisse zurückgeben. Weitere Informationen finden Sie unter "Seitenbezogene Antworten".</td> 
  </tr> 
  <tr> 
   <td>Max. Feldtiefe</td> 
   <td>4</td> 
   <td>Bei der Identifizierung der Felder, die angezeigt werden sollen, dürfen Sie das abgefragte Objekt nicht auf mehr als vier Ebenen entfernen.</td> 
  </tr> 
  <tr> 
   <td>Max. Anzahl von Objekten</td> 
   <td>50,000</td> 
   <td>Die Ergebnismenge darf nicht 50000 primäre und sekundäre Objekte enthalten.</td> 
  </tr> 
  <tr> 
   <td>Max. Anzahl Felder</td> 
   <td nowrap>1,000,000</td> 
   <td>Wenn die Ergebnismenge weniger als 50.000 Objekte beträgt, können Ihre Ergebnisse maximal 1.000.000 Felder umfassen.</td> 
  </tr> 
  <tr> 
   <td>Maximale Anzahl an Batch-Erstellungen/-Aktualisierungen</td> 
   <td>100</td> 
   <td>Die maximale Batch-Erstellungs- oder -Aktualisierungsgrenze beträgt 100.</td> 
  </tr> 
 </tbody> 
</table>

### Verwenden von paginierten Antworten {#using-paginated-responses}

Um die Begrenzung der Anzahl der Ergebnisse-Standardabfragen zu überschreiben und 200 Ergebnisse zuzulassen, können Sie die Variable `$$LIMIT=200` in Ihrer Abfrage zu filtern, wie im folgenden Beispiel gezeigt:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Um die Zuverlässigkeit und Leistung anderer Mandanten im System sicherzustellen, beträgt die maximal zulässige Ergebnisbegrenzung pro Abfrage 2000 Objekte. Wenn Sie versuchen, eine größere Begrenzung anzugeben, wird eine `IllegalArgumentException` Fehlermeldung. 

Daher empfehlen wir die Verwendung paginierter Antworten für große Datensätze. Um das erste zurückgegebene Ergebnis anzugeben, fügen Sie die `$$FIRST` Filter. Beispielsweise gibt die folgende Anfrage die Ergebnisse 201-250 für eine Abfrage zurück:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Beachten Sie, dass im obigen Beispiel `$$FIRST=200` gibt das 201. Ergebnis zurück. `$$FIRST=0` das erste Ergebnis zurückgeben. Es kann hilfreich sein, sich den $$FIRST -Wert als die Anzahl der Ergebnisse vorzustellen, die Sie überspringen möchten, bevor Ergebnisse zurückgegeben werden.

Verwenden Sie einen Sortierparameter, um sicherzustellen, dass Ihre Ergebnisse korrekt paginiert werden. Dadurch können die Ergebnisse in derselben Reihenfolge zurückgegeben werden, sodass die Paginierung die Ergebnisse nicht wiederholt oder überspringt. Verwenden Sie zum Beispiel zur Sortierung mit der Objekt-ID `ID_Sort=asc`.

### Erstellen einer Zugriffsregel

Sie können eine Zugriffsregel erstellen, um zu bestimmen, wer auf ein Objekt zugreifen kann. Im Folgenden finden Sie Beispiele für Zugriffsregeln, die Sie festlegen können:

Um ein Projekt so festzulegen, dass es nur für einen Benutzer mit der ID &quot;abc123&quot;freigegeben wird, verwenden Sie die folgende Anfrage:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Alternativ können Sie nur für eine neue Person freigeben und vorhandene Berechtigungen beibehalten:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>So rufen Sie die vorhandenen Zugriffsregeln ab:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Verhalten der POST

POST fügt ein neues Objekt ein. Die Syntax ist mit dem PUT identisch, allerdings mit einigen Ausnahmen. Da das neue Objekt noch nicht vorhanden ist, verfügt es über keine ID. Aus diesem Grund enthält der URI die ID nicht.

### Erstellen eines Objekts

Im Folgenden finden Sie ein Beispiel für eine Anforderung zum Erstellen eines neuen Projekts:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>Die Antwort enthält das neu erstellte Projekt sowie seine neue ID und alle anderen angegebenen Felder.

### Kopieren eines Objekts

Einige Objekte unterstützen das Kopieren. Für diese Objekttypen ist es möglich, neue Objekte zu erstellen, indem Sie mit einem copySourceID -Parameter posten. Beispielsweise kopiert die folgende Anfrage das angegebene Projekt und gibt ihm einen neuen Namen:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Hochladen von Dokumenten

Sie können Dokumente über die folgende API-URL hochladen:
<pre>POST /attask/api/v15.0/upload</pre>Die API erwartet, dass der Inhaltstyp mehrteilige Formulardaten ist. Der Parametername für die Datei muss uploadedFile sein. Der Server gibt die folgenden JSON-Daten zurück:
<pre>{<br>    "handle": "4c7c08fa000002ff924e298ee148df4"<br>}</pre>Sie können beim Erstellen eines Workfront-Dokuments das Handle verwenden und an die folgende URL posten:
<pre>POST /attask/api/v15.0/document?updates={<br>    name: aFileName,<br>    handle: abc...123, (handle vom Datei-Upload)<br>    docObjCode: PROJ, (oder TASK, OPTASK usw.)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## PUT-Verhalten

PUT wird verwendet, um ein vorhandenes Objekt zu aktualisieren.

Die Antwort für eine PUT ist identisch mit einer GET. In beiden Fällen gibt der Server den neuen Status des Objekts nach der Aktualisierung zurück. Alle Regeln, die zum Ändern einer Antwort auf eine GET-Anfrage verwendet werden, funktionieren auch mit PUT, z. B. die Angabe zusätzlicher zurückzugebender Felder, benutzerdefinierter Daten usw.

### Bearbeiten von Objekten

Aktualisierungen von Objekten erfolgen immer per ID unter Verwendung des eindeutigen URI des Objekts. Zu aktualisierende Felder werden als Anforderungsparameter angegeben. Um beispielsweise den Namen eines Projekts zu ändern, können Sie eine Anfrage ähnlich der folgenden senden:
<pre>PUT /attask/api/v15.0/project/4c7..?name=New Project Name <br>PUT /attask/api/v15.0/project?id=4c7..&amp;name=New Project Name</pre>Da für die Aktualisierung eine ID erforderlich ist, schlägt dieser Vorgang (ohne Einfügung) fehl, wenn das -Objekt auf dem Server nicht vorhanden ist.

### Angeben von JSON-Bearbeitungen

Wie im folgenden Beispiel gezeigt, können Sie den Parameter für Aktualisierungsanfragen verwenden, um die Felder anzugeben, die mit der JSON-Syntax aktualisiert werden sollen:
<pre>PUT /attask/api/v15.0/project/4c7..?updates= <br>{<br>     name: "New Project Name", <br>     Status: "CUR", <br>     ... <br>}</pre>

### Verschachtelte Aktualisierungen vornehmen

Einige Objekte verfügen über private Sammlungen, die aktualisiert werden können. Das folgende Beispiel zeigt beispielsweise, wie die vorhandenen Zuweisungen für eine bestimmte Aufgabe überschrieben werden:
<pre>PUT /attask/api/v15.0/task/4c7..?updates= <br>{<br>    Zuweisungen: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50.0 <br>        },{ <br>            roleID: "111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
Während Aktualisierungen auf der obersten Ebene gering sind, ersetzen Aktualisierungen an einer Sammlung oder einem verschachtelten Objekt die vorhandene Sammlung vollständig. Um eine einzelne Zuweisung einer Aufgabe zu bearbeiten, ohne die Objekte zu beeinträchtigen, verwenden Sie PUT für die Zuweisung und nicht für die Aufgabe.

Im folgenden Beispiel wird ein Projekt zur Warteschlange eines öffentlichen Helpdesk. Beachten Sie, dass die vorhandenen Warteschlangeneigenschaften ersetzt werden.
<pre>PUT /attask/api/v15.0/project/4c7..?updates= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### Verwenden des Aktionsanfrageparameters

Einige Objekte unterstützen zusätzliche Aktionen, die zusätzlich zu einfachen Bearbeitungen durchgeführt werden können. Sie können diese Aktionen mithilfe des Aktionserforderungsparameters angeben. Beispielsweise wird mit der folgenden Anfrage die Timeline für ein bestimmtes Projekt neu berechnet:
<pre>PUT /attask/api/v15.0/project/4c7..?action=calculateTimeline<br><br>oder<br><br>PUT /attask/api/v15.0/project/4c7../calculateTimeline </pre>

### Verschieben von Objekten

Im Folgenden wird die Syntax zum Verschieben einer Aufgabe von einem Projekt in ein anderes veranschaulicht:
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8...</pre>Ein Beispiel für jeden Aktionstyp finden Sie hier: (???)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Nur die Aktion Verschieben erfordert die Identifizierung zusätzlicher Attribute, um das Projekt anzugeben, in das das Arbeitselement verschoben werden soll.

Im Folgenden finden Sie ein Beispiel für jeden Aktionstyp: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}}</pre>

### Freigeben von Objekten

Das folgende Beispiel zeigt die Syntax für die Freigabe eines Projekts für ein Team:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Beim Bearbeiten eines Objekts können Sie alle Zugriffsregeln für ein Objekt ersetzen, indem Sie eine PUT durchführen und ähnliche Aktualisierungen wie im folgenden Beispiel senden:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',Aktion:'VIEW'}}</pre>Das folgende Beispiel zeigt die Syntax zum Verschieben einer Aufgabe von einem Projekt in ein anderes:
<pre>PUT /attask/api/v15.0/task/4c7../move?projectID=5d8...</pre>

## Verhalten von DELETEN

DELETE entfernt ein Objekt. In jedem Fall kann der URI den Parameter force=true enthalten, damit der Server die angegebenen Daten und die abhängigen Elemente entfernt. Im folgenden Beispiel wird eine Aufgabe gelöscht, indem die HTTP-DELETE-Methode für einen URI ausgeführt wird:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Massenaktualisierungen

Eine Massen-Update-Anweisung aktualisiert mehrere Objekte gleichzeitig in einem einzelnen API-Aufruf. Ein Bulk-create-API-Aufruf wird ähnlich wie ein normaler Update-Aufruf erstellt, wie in den folgenden Beispielen gezeigt:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>, was zu einer Rückgabe ähnlich der folgenden führt:
<pre>data: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    scheduledCompleteDate: "2014-08-28T11:00:00:000-0400"<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400"<br>    Priorität: 0,<br>    forecastCompletionDate: "2014-08-28T16:12:00:000-0400"<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    scheduledCompleteDate: "2014-08-28T11:00:00:000-0400"<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400"<br>    Priorität: 0,<br>    forecastCompletionDate: "2014-08-28T16:12:00:000-0400"<br>    status: "CUR"<br>}]</pre>Sie können auch eine Massenaktualisierung vornehmen, die in etwa wie folgt aussieht:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Bearbeiten"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx.","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>, was zu einer Rückgabe ähnlich der folgenden führt:
<pre>data: [ {<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     scheduledCompleteDate: "2014-08-28T11:00:00:000-0400"<br>     scheduledStartDate: "2014-08-28T11:00:00:000-0400"<br>     Priorität: 0,<br>     forecastCompletionDate: "2014-08-28T16:16:00:000-0400"<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    scheduledCompleteDate: "2014-08-28T11:00:00:000-0400"<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400"<br>    Priorität: 0,<br>    forecastCompletionDate: "2014-08-28T16:16:00:000-0400"<br>    status: "CUR"<br>}]</pre>Wenn Sie möchten, dass alle Vorgänge in derselben Transaktion stattfinden, fügen Sie "atomic=true"zu Ihrem Batch-API-Aufruf als Anforderungsparameter hinzu. Auf diese Weise wurden alle Vorgänge zurückgesetzt, wenn einer der Vorgänge fehlschlägt.

>[!NOTE]
>
Atomische Batch-Vorgänge können nur &quot;success: true&quot;oder einen Fehler zurückgeben.
