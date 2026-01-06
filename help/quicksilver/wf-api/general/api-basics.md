---
content-type: api
navigation-topic: general-api
title: API-Grundlagen
description: API-Grundlagen
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 319c45bc6617269f358af1e7b5f6132a8694710b
workflow-type: tm+mt
source-wordcount: '4396'
ht-degree: 0%

---


# API-Grundlagen

Ziel der Adobe Workfront-API ist es, die Erstellung von Integrationen mit Workfront zu vereinfachen, indem eine REST-fähige Architektur eingeführt wird, die über HTTP ausgeführt werden kann. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Workfront-API verfolgte Ansatz beschrieben.

Wenn Sie mit dem Workfront-Schema vertraut sind, können Sie die Datenbankbeziehungen verstehen, die Sie verwenden können, um Daten aus Workfront für Integrationszwecke abzurufen.

## Beschränkungen und Richtlinien

Um eine konsistente On-Demand-Systemleistung von Workfront sicherzustellen, beschränkt die Workfront-API gleichzeitige API-Threads. Diese Schutzmaßnahme verhindert Systemprobleme, die durch missbräuchliche API-Aufrufe verursacht werden. Die Sandbox-Umgebung verfügt über dieselbe maximale Anzahl gleichzeitiger API-Threads, sodass Kundinnen und Kunden sowie Partner API-Aufrufe genau testen können, bevor Code für die Produktion freigegeben wird.

Für Produktions-, Vorschau- und Testlaufwerk-Umgebungen haben Endbenutzeranfragen eine maximale URI-Länge von 8892 Byte, da sie über das Workfront CDN (Akamai) weitergeleitet werden. Diese Beschränkung gilt nur für URIs, die über das CDN weitergeleitet werden.

### Haftungsausschluss

Jede Verwendung der API sollte in der Beta-Umgebung von Workfront getestet werden, bevor sie in der Produktionsumgebung ausgeführt wird. Wenn ein Kunde die -API für einen Prozess verwendet, von dem Workfront vernünftigerweise annimmt, dass er die On-Demand-Software belastet (d. h. der Prozess hat für andere Kunden wesentliche negative Auswirkungen auf die Leistung der Software), behält sich Workfront das Recht vor, den Kunden aufzufordern, diesen Prozess einzustellen. Wenn der Kunde die Vorgaben nicht erfüllt und das Problem weiterhin besteht, behält sich Workfront das Recht vor, den Vorgang zu beenden.

## Workfront-API-URL

Informationen über die URL, die Sie zum Aufrufen der Workfront-API verwenden werden, finden Sie unter [Domain-Format für Adobe Workfront-API-Aufrufe](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## REST-Grundlagen

In diesem Abschnitt finden Sie eine allgemeine Einführung in die Interaktion mit der Workfront REST-API für die folgenden REST-Prinzipien:

### Objekt-URI

Jedem Objekt im System wird ein eindeutiger URI zugewiesen, der aus dem Objekttyp und der ID besteht. Die folgenden Beispiele zeigen URIs, die drei eindeutige Objekte beschreiben:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Bei dem Objekttyp wird nicht zwischen Groß- und Kleinschreibung unterschieden und es kann sich entweder um den abgekürzten ObjCode (z. B. proj) oder den alternativen Objektnamen (project) handeln.

Eine Liste der Objekte, gültigen ObjCodes und Objektfelder finden Sie unter  [API-Explorer](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Im Kontext der Workfront-API ist ein benutzerdefiniertes Formular ein `Category` und ein benutzerdefiniertes Feld ein `Parameter`.

### Vorgänge

Objekte werden durch Senden einer HTTP-Anfrage an den eindeutigen URI bearbeitet. Der auszuführende Vorgang wird durch die HTTP-Methode angegeben.

Die standardmäßigen HTTP-Methoden entsprechen den folgenden Vorgängen:

* **GET** - Ruft ein Objekt nach ID ab, sucht nach allen Objekten anhand einer Abfrage, führt Berichte aus oder führt benannte Abfragen aus
* **POST** - Fügt ein neues Objekt ein.
* **PUT** - bearbeitet ein vorhandenes Objekt
* **DELETE** - Löscht ein Objekt

Um Client-Mängel oder Protokolllängenbeschränkungen zu umgehen, kann der Methodenparameter verwendet werden, um das HTTP-Verhalten zu überschreiben. Beispielsweise kann ein GET-Vorgang implementiert werden, indem der folgende URI gepostet wird:
<pre>GET /attask/api/v15.0/project?id=4c78…54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78…54d0?method=get</pre>

### Antwort

Jede Anfrage erhält eine Antwort im JSON-Format. Die Antwort enthält entweder ein Datenattribut, wenn die Anfrage erfolgreich war, oder ein Fehlerattribut, wenn ein Problem aufgetreten ist. Beispiel: die Anfrage

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

gibt eine JSON-Antwort ähnlich der folgenden zurück:


<pre>{<br>    „data“: [<br>        {<br>            „percentComplete“: 0,<br>            „status“: „CUR“,<br>            „Priorität“: 2,<br>            „name“: „Brand New Project“,<br>            „ID“: „4c7c08b20000002de5ca1ebc19edf2d5“ <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Beim Ausführen einer GET-Anfrage über die Adressleiste Ihres Browsers ist es nicht erforderlich, die Sitzungs-ID als Teil der Anfrage einzuschließen.

Besondere Sicherheit wurde für PUT-, POST- und DELETE-Anfragen hinzugefügt. Jede Anfrage, die zum Schreiben in oder Löschen aus der Datenbank führt, kann nur ausgeführt werden, wenn **sessionID=abc123** im URI enthalten ist. Die folgenden Beispiele zeigen, wie dies bei einer DELETE-Anfrage aussehen würde:
<pre>GET /attask/api/v15.0/project?id=4c78…54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78…54d0?method=delete&amp;sessionID=abc123</pre>

### Authentifizierung

Die API authentifiziert jede Anfrage, um sicherzustellen, dass der Client Zugriff zum Anzeigen oder Ändern eines angeforderten Objekts hat.

Die Authentifizierung erfolgt durch Übergabe einer Sitzungs-ID, die mithilfe einer der folgenden Methoden erteilt werden kann:

#### Authentifizierung beim Anforderungsheader

Die bevorzugte Authentifizierungsmethode besteht darin, einen Anfrage-Header mit dem Namen SessionID zu übergeben, der das Sitzungs-Token enthält. Dies hat den Vorteil, dass es vor [Cross-Site Request Forgery (CSRF)-Angriffen ](https://en.wikipedia.org/wiki/Cross-site_request_forgery) ist und den URI zu Caching-Zwecken nicht beeinträchtigt.

Im Folgenden finden Sie ein Beispiel für einen Anfrage-Header:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Cookie-basierte Authentifizierung

Die API verwendet dieselbe Cookie-basierte Authentifizierung wie die Web-Benutzeroberfläche im System. Wenn sich ein Client über die Web-Benutzeroberfläche bei Workfront anmeldet, verwenden alle AJAX-Aufrufe innerhalb desselben Browsers dieselbe Authentifizierung.

>[!NOTE]
>
>Zum Schutz vor möglichen CSRF-Angriffen (Cross Site Request Forgery) ist diese Authentifizierungsmethode nur für schreibgeschützte Vorgänge verfügbar.

## Anmeldung

>[!IMPORTANT]
>
>Workfront empfiehlt nicht mehr die Verwendung des `/login`-Endpunkts oder der API-Schlüssel. Verwenden Sie stattdessen eine der folgenden Authentifizierungsmethoden:
>
>* Server-Authentifizierung mit JWT
>* Benutzerauthentifizierung mit OAuth2
>
>Anweisungen zum Einrichten dieser Authentifizierungsmethoden finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Anweisungen zur Verwendung der Serverauthentifizierung in Workfront finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md)
>
>Anweisungen zur Verwendung der Benutzerauthentifizierung in Workfront finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungs-Code-Flusses](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
>Das in diesem Abschnitt beschriebene Verfahren gilt nur für Organisationen, die noch keine Einführung in die Adobe Business Platform erhalten haben. Die Anmeldung bei Workfront über die Workfront-API ist nicht verfügbar, wenn Ihr Unternehmen die Adobe Business-Plattform verwendet hat.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen die Adobe Business Platform verwendet, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Mit einem gültigen Benutzernamen und Kennwort können Sie die folgende Anfrage verwenden, um eine Sitzungs-ID abzurufen:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Damit wird ein Cookie gesetzt, um zukünftige Anfragen zu authentifizieren und eine JSON-Antwort mit der neu erstellten Sitzungs-ID, der Benutzer-ID des angemeldeten Benutzers und anderen Sitzungsattributen zurückzugeben.

>[!NOTE]
>
>Wenn Sie über einen benannten API-Benutzer verfügen, der auch Administrator ist, empfiehlt Workfront dringend, einen API-Schlüssel für die Anmeldung zu verwenden.

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

Sie können dieses Ergebnis dann verwenden, um jeden API-Aufruf zu authentifizieren, indem Sie „apiKey“ als Abfrageparameter mit diesem Wert anstelle einer Sitzungs-ID oder eines Benutzernamens und Kennworts hinzufügen. Dies ist aus Sicherheitssicht von Vorteil.

Die folgende Anfrage ist ein Beispiel für das Abrufen von Daten aus einem Projekt mithilfe des -API-Schlüssels:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidierung eines API-Schlüssels**

Wenn der apiKey-Wert kompromittiert wurde, können Sie „clearApiKey“ ausführen, wodurch der aktuelle API-Schlüssel ungültig wird, wie im folgenden Beispiel gezeigt:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Nach dem Löschen können Sie getApiKey erneut ausführen, um einen neuen API-Schlüssel zu generieren.

### Abmelden

Wenn eine Sitzung abgeschlossen ist, können Sie die folgende Anfrage verwenden, um den Benutzer abzumelden und so jeden weiteren Zugriff mit der Sitzungs-ID zu verhindern.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

Die Sitzungs-ID, die abgemeldet werden soll, kann entweder als Cookie, Anfragekopfzeile oder Anfrageparameter angegeben werden.

So melden Sie einen Benutzer ab:

1. Navigieren Sie zu Ihrem Anmeldebildschirm, melden Sie sich jedoch nicht an.
1. Ändern Sie die URL in /attask/api/v15.0/project/search.\
   Beachten Sie, dass die Seite nicht gefunden wurde.
1. Ersetzen Sie das Wort *Suche* durch Anmelden?username=admin&amp;password=user und ersetzen Sie *admin* und *user durch Ihren Benutzernamen und Ihr Kennwort\
   *Diese Sitzung wird im Browser als Cookie gespeichert und muss nicht bei jeder nachfolgenden GET-Anfrage neu angegeben werden.

1. Ändern Sie die URL zurück in **/attask/api/v15.0/project/search**.
1. Beachten Sie die bereitgestellte Antwort.

Bei PUT-, POST- und DELETE-Anfragen muss nach der Anmeldung immer die Sitzungs-ID angegeben werden.

## GET-Verhalten

Verwenden Sie die HTTP-GET-Methode zum Abrufen eines oder mehrerer Objekte und zum Ausführen von Berichten.

### Objekte werden abgerufen

Sie können die Suche nach Objekten mithilfe von Modifikatoren und Filtern verbessern.

#### Abrufen eines -Objekts mithilfe der Objekt-ID

Wenn Sie die ID eines -Objekts kennen, können Sie das -Objekt durch Zugriff auf seinen eindeutigen URI abrufen. Beispiel: die Anfrage

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

Gibt eine Antwort ähnlich der folgenden zurück:

<pre>{<br>    „percentComplete“: 0,<br>    „status“: „CUR“,<br>    „Priorität“: 2,<br>    „name“: „Brand New Project“,<br>    „ID“: „4c7c08b20000002de5ca1ebc19edf2d5“ <br>}</pre>


Sie können mehrere Objekte in derselben Anfrage abrufen, indem Sie den Anforderungsparameter id angeben und eine kommagetrennte Liste von IDs angeben, wie im folgenden Beispiel gezeigt:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Beachten Sie, dass die Anfrage /attask/api/v15.0/project?id=… mit der `/attask/api/v15.0/project/...`-Anfrage übereinstimmt.

#### Abrufen eines -Objekts mithilfe des URI

Wenn Sie ein Objekt nach anderen Kriterien als der ID abrufen möchten, können Sie nach dem URI suchen.

Beispielsweise können Sie die folgende Anfrage verwenden, um eine Liste aller Projekte im System zurückzugeben:

```
GET /attask/api/v15.0/project/search
```

Sie können Filter mithilfe der Anfrageparameter als Name-Wert-Paare angeben. Das folgende Beispiel zeigt beispielsweise eine Anfrage, die alle aktuellen Projekte finden würde:

```
GET /attask/api/v15.0/project/search?status=CUR
```

Die folgende Anfrage findet alle Aufgaben, die noch nicht abgeschlossen sind und die einem Benutzer namens „John“ zugewiesen sind.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Verwenden von Suchmodifikatoren

In der folgenden Tabelle sind einige der Modifikatoren aufgeführt, die Sie mit der Workfront-API verwenden können.

| **Modifier** | **Beschreibung** | **Beispiel** |
| --- | --- | --- |
| Äq | Gibt Ergebnisse mit dem Status „Geschlossen“ zurück | <pre>…status=cls&amp;status_mod=eq…</pre> |
| NE | Gibt Ergebnisse zurück, die nicht den Status „Geschlossen“ haben | <pre>…status=cls&amp;status_mode=ne…</pre> |
| Gate | Gibt Ergebnisse zurück, deren Prozentwert der Fertigstellung größer oder gleich 50 ist | <pre>…percentComplete=50&amp;percentComplete_Mod=get…</pre> |
| LTE | Gibt Ergebnisse zurück, deren Prozentwert kleiner oder gleich 50 ist | <pre>…percentComplete=50&amp;percentComplete_Mod=lte…</pre> |
| isnull | gibt Ergebnisse zurück, bei denen die Beschreibung null ist | <pre>…description_mod=isNull…</pre> |
| nicht null | gibt Ergebnisse zurück, bei denen die Beschreibung nicht null ist | <pre>…description_mod=notNull…</pre> |
| enthält | Gibt Ergebnisse zurück, bei denen der Name &quot;Workfront&quot; enthält | <pre>…name=Workfront&amp;name_mod=enthält…</pre> |
| zwischen | Gibt Ergebnisse zurück, die innerhalb der letzten 7 Tage ein Eingabedatum aufweisen | <pre>…entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between…</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>Bei Suchanfragen wird zwischen Groß- und Kleinschreibung unterschieden. Wenn Sie einen Fehler erhalten, stellen Sie Folgendes sicher  **_Mod** und **_Range** haben die richtige Groß-/Kleinschreibung.

#### Verwenden von OR-Anweisungen

Sie können eine Suche verbessern, indem Sie einen Parameter hinzufügen, der „OR“ sowie eine Zahl enthält, um die Ebene eines Filters oder einer Reihe von Filtern anzugeben.

Eine OR-Anweisung gibt nur Datensätze im API-Aufruf zurück, die den Filterkriterien der OR-Anweisung entsprechen. Filter sind nicht auf allen OR-Anweisungsebenen impliziert.

Wenn Sie beispielsweise nach filtern möchten

* Aufgaben mit einem Namen, der „Planung“ ODER enthält
* Aufgaben in einem Portfolio mit dem Namen „FixedAssets“ UND jemandem mit einem Namen zugewiesen, der „Steve“ ODER enthält
* Aufgaben mit einer übergeordneten Aufgabe namens „Endgültige Aufgabe“

verwenden Sie dann den folgenden API-Aufruf mit seinen mehreren OR-Anweisungen:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_mod=eq
</pre>

#### Filterparameter verwenden

Ein potenzieller Fehler bei der Verwendung von URL-Parametern für Suchfilter besteht darin, dass Workfront bestimmte Parameter analysiert, bevor nach verschiedenen Authentifizierungsmethoden (z. B. Benutzername, Kennwort, API-Schlüssel, Cookie) gesucht wird. In diesem Fall werden die Parameter nicht als Filter im Aufruf verwendet. 

Um dieses Problem zu vermeiden, können Sie diese Werte in Filterparametern mit JSON-Formatierung platzieren. Wenn Sie beispielsweise nach dem Benutzernamen „testuser“ filtern möchten, anstatt zu verwenden 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>Übergeben Sie den URL-Parameter in einem Filter, wie im folgenden Beispiel gezeigt:
<pre>/attask/api/v15.0/user/search?filters={„username“:“testuser@workfront.com"}</pre>

#### Verwenden des Map-Anforderungsparameters

Standardmäßig sind die von einer Suche zurückgegebenen Daten ein JSON-Array. Je nach Anwendungsfall ist es möglicherweise effizienter, das Ergebnis als ein nach ID indiziertes JSON-Objekt abzurufen. Verwenden Sie dazu den Anforderungsparameter „map“. Beispiel: die Anfrage 
<pre>/attask/api/v15.0/task/search?map=true</pre>gibt eine Antwort zurück, die nach ID ähnlich der folgenden indiziert ist:
<pre>{<br>    „data“: {<br>        „4c9a97db0000000f13ee4446b9aead9b“: {<br>            „percentComplete“: 0,<br>            „status“: „NEW“,<br>            „name“: „first task“,<br>            „ID“: „4c9a97db0000000f13ee4446b9aead9b“,<br>            „taskNumber“: 1 <br>        },<br>        „4CA28BA600002024CD49E75BD43CF601“: {<br>            „percentComplete“: 0,<br>            „status“: „INP:A“,<br>            „Name“: „Zweite Aufgabe“,<br>            „ID“: „4ca28ba600002024cd49e75bd43cf601“,<br>            „taskNumber“: 2 <br>        } <br>    } <br>}</pre>

#### Verwenden des Anforderungsparameters Fields

Standardmäßig wird beim Abrufen eines -Objekts nur die am häufigsten verwendete Teilmenge von Feldern zurückgegeben.

Mit dem Anforderungsparameter fields können Sie angeben, dass eine kommagetrennte Liste bestimmter Felder zurückgegeben wird. Beispiel: die Anfrage
<pre>/attask/api/v15.0/task/search?fields=scheduledStartDate,priority</pre>Gibt eine Antwort ähnlich der folgenden zurück:
<pre>{<br>    „Priorität“: 2,<br>    „name“: „first task“,<br>    „ID“: „4c7c08fa0000002ff924e298ee148df4“,<br>    „scheduledStartDate“: „2010-08-30T09:00:00:000-0600“ <br>}</pre>

>[!NOTE]
>
>Bei diesen Feldnamen wird zwischen Groß- und Kleinschreibung unterschieden.

Eine Liste der möglichen Feldverweise finden Sie in der  [API-Explorer](../../wf-api/general/api-explorer.md)

#### Suchen nach verschachtelten Objekten

Sie können nach verschachtelten Objekten suchen. Standardmäßig werden verschachtelte Objekte nur mit dem Namen und der ID zurückgegeben. Verwenden Sie beispielsweise die folgende Anfrage, um alle Probleme mit ihren Besitzern zu klären:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Wenn weitere Informationen erforderlich sind, können Sie ein verschachteltes Feld mithilfe der Doppelpunktsyntax anfordern. Mit der folgenden Anfrage werden beispielsweise alle Probleme zusammen mit dem Namen, der ID, dem Titel und der Telefonnummer des Besitzers gesucht
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>und gibt Folgendes zurück: 
<pre>{<br>    „Name“: „Ein wichtiges Thema“,<br>    „ID“: „4c78285f00000908ea8cfd66e084939f“,<br>    „Inhaber“: {<br>        „title“: „Operations Specialist“,<br>        „phoneNumber“: „555-1234“,<br>        „name“: „admin user“,<br>        „ID“: „4c76ed7a0000054c172b2c2d9f7f81c3“ <br>    } <br>}</pre>

#### Abrufen verschachtelter Sammlungen

Sie können verschachtelte Sammlungen von Objekten abrufen. Um beispielsweise ein Projekt mit allen seinen Aufgaben abzurufen, verwenden Sie die folgende Anfrage:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>Die folgende Anfrage erhält Aufgabenzuweisungen:
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Suchen nach mehreren verschachtelten Feldern

Standardmäßig werden nur der Name und die ID jeder Aufgabe zurückgegeben. Es können jedoch zusätzliche verschachtelte Felder mit Doppelpunkt-Syntax angegeben werden. Um alle verfügbaren Felder für ein verknüpftes Objekt oder eine Auflistung anzuzeigen, hängen Sie einfach einen Doppelpunkt und ein Sternchen an die Objekt-/Sammlungsreferenz an.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### Benutzerdefinierte Daten werden abgerufen

Benutzerdefinierte Datenfelder können mit dem Präfix „DE:“ abgerufen werden. Um beispielsweise ein Projekt mit einem Parameter namens „CustomText“ anzufordern, verwenden Sie die folgende Anfrage:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>, die zurückgeben würde
<pre>{<br>    „Name“: „Benutzerdefiniertes Datenprojekt“,<br>    „ID“: „4c9a954f0000001afad0687d7b1b4e43“,<br>    „DE:CustomText“: „task b“ <br>}</pre>Sie können auch alle benutzerdefinierten Daten für ein Objekt abrufen, indem Sie das Feld „parameterValues“ abrufen. Beispiel: 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>gibt ähnliche Daten wie die folgenden zurück:
<pre>{<br>    „Name“: „Benutzerdefiniertes Datenprojekt“,<br>    „ID“: „4c9a954f0000001afad0687d7b1b4e43“,<br>    parameterValues: { <br>        „DE:CustomText“: „task b“, <br>        „DE:CustomNumber“: 1.4, <br>        „DE:CustomCheckBoxes“: [„first“, „second“, „third“] <br>    } <br>}</pre>

#### Verwenden benannter Abfragen

Einige Objekttypen verfügen über benannte Suchvorgänge, die häufig ausgeführt werden und verfügbar sind, indem der Name der Abfrage an das Ende des Objekttyp-URI angehängt wird. Beispielsweise ruft die folgende Anfrage die Arbeitselemente (Aufgaben und Probleme) ab, denen der Benutzer derzeit zugewiesen ist:
<pre>/attask/api/v15.0/work/myWork</pre>Benannte Abfragen unterstützen das Anfordern des -Feldparameters zum Abrufen zusätzlicher Felder. Einige benannte Abfragen akzeptieren auch zusätzliche Filter. Eine Liste der zulässigen Abfragen mit dem Namen eines Objekts finden Sie auf der Registerkarte Aktion für das Objekt in der  [API-Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### Verwenden `Count`

Sie können `count` verwenden, um die Anzahl der Ergebnisse zurückzugeben, die Ihrer Abfrage entsprechen. Dies kann nützlich sein, wenn Sie die Daten in den Ergebnissen nicht benötigen. Durch die Rückgabe der Zählung kann der Server die Anfrage schneller verarbeiten und Bandbreite sparen. Beispiel: die Anfrage
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>Gibt die Anzahl der Ergebnisse im folgenden Format zurück:
<pre>{<br>    „count“: 3 <br>}</pre>Die Rückgabe einer Anzahl ist eine viel kleinere Datenübertragung als die Rückgabe der vollständigen Objekte. Die Syntax ist identisch mit dem Suchbefehl.

### Bericht anfordern

Sie können eine Berichtsanfrage ausführen, bei der mit einer oder mehreren Gruppierungen nur die Zusammenfassung eines Felds gewünscht wird. Wie im folgenden Beispiel gezeigt, ist die Berichtssyntax mit der Syntax für die SOAP-API identisch:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>gibt das folgende Ergebnis zurück
<pre>{<br>    „Erstes Projekt“: { <br>        „sum_hours“: 15 <br>    }, <br>     „Zweites Projekt“: { <br>        „sum_hours“: 30 <br>    } <br>}</pre>Das Hinzufügen des Parameters $$ROLLUP=true ergibt eine Summe auf jeder Gruppierungsebene:
<pre>{<br>    „Erstes Projekt“: { <br>        „sum_hours“: 15 <br>    }, <br>    „Zweites Projekt“: { <br>        „sum_hours“: 30 <br>    }, <br>    "$$ROLLUP“: { <br>        „sum_hours“: 45 <br>    } <br>}</pre>

### Sortieren von Abfrageergebnissen in der API

Sie können Ihre Ergebnisse nach einem beliebigen Feld sortieren, wenn Sie Folgendes an Ihren API-Aufruf anhängen:

&amp;entryDate_Sort=asc

Wenn Sie beispielsweise nach dem geplanten Startdatum der Aufgabe sortieren möchten, entfernen Sie entryDate und ersetzen Sie es durch scheduledCompletionDate.

Dies funktioniert für die meisten Felder in Workfront.

### Überlegungen zu Abfragebeschränkungen

Bei der Abfrage eines Objekts sollte die Beziehung verwandter Objekte und Sucheinschränkungen besonders berücksichtigt werden. Wie in der folgenden Tabelle dargestellt, kann eine Abfrage für Projekte beispielsweise nicht mehr als 2.000 Projekte zurückgeben. Diese 2.000 Projekte werden als „primäre Objekte“ betrachtet. Wenn Sie für die Projekte das Feld Aufgaben abfragen, wird das Feld Aufgaben , das eine Sammlung ist, zum sekundären Objekt des primären Projektobjekts. Eine Abfrage für das Feld Aufgaben kann Tausende von Aufgaben in Projekten enthalten. Insgesamt darf die Gesamtanzahl der zurückgegebenen Objekte (Projekte und Aufgaben) 50.000 nicht überschreiten.

Um eine optimale Leistung zu gewährleisten, werden in der folgenden Tabelle die Einschränkungen bei Suchanfragen aufgeführt. 

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
   <td width="200">Standardanzahl der Ergebnisse</td> 
   <td>100</td> 
   <td> Wenn im Abfragefilter kein Limit angegeben ist (d. h. $$LIMIT), kann das Ergebnis nicht mehr als 100 primäre Objekte enthalten. <br>Anweisungen zum Überschreiben dieser Beschränkung finden <a href="#using-paginated-responses" class="MCXref xref"> unter „Verwenden </a> paginierten Antworten“. </td> 
  </tr> 
  <tr> 
   <td>Maximale Ergebnisanzahl</td> 
   <td>2.000</td> 
   <td>Der Abfragefilter (d. h. $$LIMIT) kann nicht mehr als 2.000 Ergebnisse zurückgeben. Weitere Informationen finden Sie unter „Paginierte Antworten“.</td> 
  </tr> 
  <tr> 
   <td>Max. Feldtiefe</td> 
   <td>4</td> 
   <td>Bei der Identifizierung der Felder, die angezeigt werden sollen, können Sie nicht mehr als vier Ebenen vom abgefragten Objekt entfernt sein.</td> 
  </tr> 
  <tr> 
   <td>Max. Objektanzahl</td> 
   <td>50.000</td> 
   <td>Der Ergebnissatz kann 50000 primäre und sekundäre Objekte nicht enthalten.</td> 
  </tr> 
  <tr> 
   <td>Max. Anzahl von Feldern</td> 
   <td nowrap>1.000.000</td> 
   <td>Wenn der Ergebnissatz weniger als 50000 Objekte umfasst, können die Ergebnisse maximal 1.000.000 Felder enthalten.</td> 
  </tr> 
  <tr> 
   <td>Max. Anzahl von Batch-Erstellungen/-Aktualisierungen</td> 
   <td>100</td> 
   <td>Das Limit für die Erstellung oder Aktualisierung von Batches ist maximal 100.</td> 
  </tr> 
 </tbody> 
</table>

### Verwenden paginierter Antworten {#using-paginated-responses}

Um die Standardabfragebeschränkung für die Anzahl der Ergebnisse zu überschreiben und 200 Ergebnisse zuzulassen, können Sie den `$$LIMIT=200`-Filter in Ihre Abfrage einbeziehen, wie im folgenden Beispiel gezeigt:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Um die Zuverlässigkeit und Leistung anderer Mandanten im System sicherzustellen, beträgt die maximal zulässige Ergebnisgrenze pro Abfrage 2.000 Objekte. Der Versuch, eine größere Grenze anzugeben, führt zu einer `IllegalArgumentException` Fehlermeldung. 

Daher empfehlen wir die Verwendung paginierter Antworten für große Datensätze. Um das erste Ergebnis anzugeben, das zurückgegeben werden soll, fügen Sie den `$$FIRST` hinzu. Beispielsweise gibt die folgende Anfrage die Ergebnisse 201-250 für eine Abfrage zurück:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Beachten Sie, dass im obigen Beispiel `$$FIRST=200` das 201. Ergebnis zurückgibt. `$$FIRST=0` würde das erste Ergebnis zurückgeben. Es kann hilfreich sein, sich den Wert $$FIRST als die Anzahl der Ergebnisse vorzustellen, die Sie überspringen möchten, bevor Sie Ergebnisse zurückgeben.

Um sicherzustellen, dass Ihre Ergebnisse ordnungsgemäß paginiert werden, verwenden Sie einen Sortierparameter. Dadurch können die Ergebnisse in derselben Reihenfolge zurückgegeben werden, sodass die Paginierung die Ergebnisse nicht wiederholt oder überspringt. Um beispielsweise anhand der Objekt-ID zu sortieren, verwenden Sie `ID_Sort=asc`.

### Erstellen einer Zugriffsregel

Sie können eine Zugriffsregel erstellen, um zu bestimmen, wer auf ein Objekt zugreifen kann. Im Folgenden finden Sie Beispiele für Zugriffsregeln, die Sie festlegen können:

Um ein Projekt so einzurichten, dass es nur für einen Benutzer mit der ID „abc123“ freigegeben wird, verwenden Sie die folgende Anfrage:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Alternativ können Sie nur für eine neue Person freigeben und die vorhandenen Berechtigungen intakt lassen:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Abrufen der vorhandenen Zugriffsregeln:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST-Verhalten

POST fügt ein neues Objekt ein. Die Syntax entspricht der von PUT, mit einigen Ausnahmen. Da das neue Objekt noch nicht vorhanden ist, verfügt es über keine ID. Aus diesem Grund enthält der URI die ID nicht.

### Erstellen eines Objekts

Im Folgenden finden Sie ein Beispiel für eine Anfrage zum Erstellen eines neuen Projekts:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>Die Antwort enthält das neu erstellte Projekt zusammen mit seiner neuen ID und allen anderen angegebenen Feldern.

### Kopieren eines Objekts

Einige Objekte unterstützen das Kopieren. Für diese Objekttypen ist es möglich, neue Objekte durch Posten mit einem copySourceID-Parameter zu erstellen. Beispielsweise kopiert die folgende Anfrage das angegebene Projekt und gibt ihm einen neuen Namen:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Hochladen von Dokumenten

Sie können Dokumente über die folgende API-URL hochladen:
<pre>POST /attask/api/v15.0/upload</pre>Die API erwartet, dass der Inhaltstyp mehrteilig/formulardaten ist. Der Parametername für die Datei muss uploadedFile sein. Der Server gibt die folgenden JSON-Daten zurück:
<pre>{<br>    „Griff“: „4C7C08FA0000002FF924E298EE148DF4“<br>}</pre>Sie können beim Erstellen eines Workfront-Dokuments den -Handle verwenden und an die folgende URL senden:
<pre>POST /attask/api/v15.0/document?updates={<br>    name: aFileName,<br>    handle: abc…123, (handle from the file upload)<br>    docObjCode: PROJ, (oder TASK, OPTASK usw.<br>    objID: abc…123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## PUT-Verhalten

PUT wird verwendet, um ein vorhandenes Objekt zu aktualisieren.

Die Antwort für eine PUT ist identisch mit einer GET. In beiden Fällen gibt der Server den neuen Status des -Objekts nach der Aktualisierung zurück. Alle Regeln, die zum Ändern einer Antwort auf eine GET-Anfrage verwendet werden, funktionieren auch mit PUT, z. B. die Angabe zusätzlicher zurückzugebender Felder, benutzerdefinierter Daten usw.

### Objekte bearbeiten

Aktualisierungen an Objekten werden immer nach ID unter Verwendung der eindeutigen URI des Objekts durchgeführt. Zu aktualisierende Felder werden als Anfrageparameter angegeben. Um beispielsweise den Namen eines Projekts zu ändern, können Sie eine Anfrage ähnlich der folgenden senden:
<pre>PUT /attask/api/v15.0/project/4c7…?name=Neuer Projektname <br>PUT /attask/api/v15.0/project?id=4c7…&amp;name=Neuer Projektname</pre>Da für die Aktualisierung eine ID erforderlich ist, schlägt dieser Vorgang (ohne Einfügen) fehl, wenn das Objekt nicht auf dem Server vorhanden ist.

### Angeben von JSON-Bearbeitungen

Wie im folgenden Beispiel gezeigt, können Sie den Anforderungsparameter „updates“ verwenden, um die zu aktualisierenden Felder mithilfe der JSON-Syntax anzugeben:
<pre>PUT /attask/api/v15.0/project/4c7…?Updates= <br>{<br>     Name: „New Project Name“, <br>     Status: „CUR“, <br>     … <br>}</pre>

### Verschachtelte Aktualisierungen vornehmen

Einige Objekte verfügen über private Sammlungen, die aktualisiert werden können. Im folgenden Beispiel wird beispielsweise veranschaulicht, wie die vorhandenen Zuweisungen für eine bestimmte Aufgabe überschrieben werden:
<pre>PUT /attask/api/v15.0/task/4c7…?Updates= <br>{<br>    Arbeitsaufträge: [ <br>        { <br>            assignedToID: „2222…54d0, <br>            assignmentPercent: 50,0 <br>        },{ <br>            roleID: „1111…54d0“<br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Aktualisierungen an der obersten Ebene sind zwar selten, aber Aktualisierungen an einer Sammlung oder einem verschachtelten Objekt ersetzen die vorhandene Sammlung vollständig. Um eine einzelne Zuweisung für eine Aufgabe zu bearbeiten, ohne die Objekte zu beeinflussen, verwenden Sie PUT für die Zuweisung und nicht für die Aufgabe.

Im folgenden Beispiel wird ein Projekt zu einer öffentlichen Helpdesk-Warteschlange. Beachten Sie, dass die vorhandenen Warteschlangeneigenschaften ersetzt werden.
<pre>PUT /attask/api/v15.0/project/4c7…?Updates= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### Verwenden des Aktionserforderungsparameters

Einige Objekte unterstützen zusätzlich zu einfachen Bearbeitungen weitere Aktionen, die ausgeführt werden können. Sie können diese Aktionen mit dem Aktionserforderungsparameter angeben. Mit der folgenden Anfrage wird beispielsweise die Zeitleiste für ein bestimmtes Projekt neu berechnet:
<pre>PUT /attask/api/v15.0/project/4c7…?action=calculateTimeline<br><br>or<br><br>PUT /attask/api/v15.0/project/4c7…/calculateTimeline </pre>

### Objekte werden verschoben

Im Folgenden wird die Syntax zum Verschieben einer Aufgabe von einem Projekt in ein anderes veranschaulicht:
<pre>PUT /attask/api/v15.0/task/4c7…/move?projectID=5d8…</pre>Ein Beispiel für jeden Aktionstyp wird hier bereitgestellt: (??)
<pre>PUT /attask/api/v15.0/project/1234/approve<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/approve<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Nur für die Aktion Verschieben müssen zusätzliche Attribute identifiziert werden, um das Projekt anzugeben, in das das Arbeitselement verschoben werden soll.

Im Folgenden finden Sie ein Beispiel für jeden Aktionstyp: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Freigeben von Objekten

Das folgende Beispiel zeigt die Syntax für die Freigabe eines Projekts für ein Team:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Beim Bearbeiten eines Objekts können Sie alle Zugriffsregeln für ein Objekt ersetzen, indem Sie eine PUT durchführen und Aktualisierungen ähnlich dem folgenden Beispiel senden:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>Das folgende Beispiel zeigt die Syntax zum Verschieben einer Aufgabe von einem Projekt in ein anderes:
<pre>PUT /attask/api/v15.0/task/4c7…/move?projectID=5d8…</pre>

## DELETE-Verhalten

DELETE entfernt ein Objekt. In jedem Fall kann der URI den Parameter force=true enthalten, damit der Server die angegebenen Daten und deren abhängigen Elemente entfernt. Im folgenden Beispiel wird eine Aufgabe gelöscht, indem die HTTP-DELETE-Methode für einen URI ausgeführt wird:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Massenaktualisierungen

Eine Massen-Aktualisierungsanweisung aktualisiert innerhalb eines einzigen API-Aufrufs mehrere Objekte gleichzeitig. Ein Massenerstellungs-API-Aufruf wird ähnlich wie ein normaler Aktualisierungsaufruf erstellt, wie in den folgenden Beispielen gezeigt:
<pre>PUT /attask/api/v15.0/proj?updates=[{„name“:„Test_Project_1“},{„name“:„Test_Project_2“}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>oder <pre>PUSH /attask/api/v15.0/proj?updates=[{„name“:„Test_Project_1“},{„name“:„Test_Project_2“}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>was zu einem ähnlichen Ergebnis wie dem folgenden führt:
<pre>Daten: [{<br>    ID: „53ff8d3d003b438b57a8a784df38f6b3“,<br>    Name: „test_project_1“,<br>    objCode: „PROJ“,<br>    percentComplete: 0,<br>    scheduledCompletionDate: „2014-08-28T11:00:00:000-0400“,<br>    geplantes Startdatum: „2014-08-28T11:00:00:000-0400“,<br>    Priorität: 0,<br>    projectionCompletionDate: „2014-08-28T16:12:00:000-0400“,<br>    Status: „CUR“<br>},<br>{<br>    Kennung: „53ff8d49003b43a2562aa34ea3b6b10“,<br>    Name: „test_project_2“,<br>    objCode: „PROJ“,<br>    percentComplete: 0usi,<br>    scheduledCompletionDate: „2014-08-28T11:00:00:000-0400“,<br>    geplantes Startdatum: „2014-08-28T11:00:00:000-0400“,<br>    Priorität: 0,<br>    projectionCompletionDate: „2014-08-28T16:12:00:000-0400“,<br>    Status: „CUR“<br>}]</pre>Sie können auch eine Massenaktualisierung ähnlich der folgenden durchführen:
<pre>PUT /attask/api/v15.0/proj?umethod=PUT&amp;updates=[{„ID“:„123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx“,„name“:„Test_Project_1_ Edit“},{„ID“:„123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>was zu einem ähnlichen Ergebnis wie dem folgenden führt:
<pre>Daten: [ {<br>     Kennung: „53ff8e15003b461d4560f7f65a440078“,<br>     Name: „test_project_1_edit“,<br>     objCode: „PROJ“,<br>     percentComplete: 0,<br>     scheduledCompletionDate: „2014-08-28T11:00:00:000-0400“,<br>     geplantes Startdatum: „2014-08-28T11:00:00:000-0400“,<br>     Priorität: 0,<br>     projectionCompletionDate: „2014-08-28T16:16:00:000-0400“,<br>     Status: „CUR“<br>},<br>{<br>    Kennung: „53ff8e19003b46238a58d303608de502“,<br>    Name: „test_project_2_edit“,<br>    objCode: „PROJ“,<br>    percentComplete: 0,<br>    scheduledCompletionDate: „2014-08-28T11:00:00:000-0400“,<br>    geplantes Startdatum: „2014-08-28T11:00:00:000-0400“,<br>    Priorität: 0,<br>    projectionCompletionDate: „2014-08-28T16:16:00:000-0400“,<br>    Status: „CUR“<br>}]</pre>Wenn Sie möchten, dass alle Vorgänge in derselben Transaktion stattfinden, fügen Sie „atomic=true“ zu Ihrem Batch-API-Aufruf als Abfrageparameter hinzu. Auf diese Weise werden alle Vorgänge zurückgesetzt, wenn einer der Vorgänge fehlschlägt.

>[!NOTE]
>
>Atomare Batch-Vorgänge können nur „Erfolg: wahr“ oder einen Fehler zurückgeben.

