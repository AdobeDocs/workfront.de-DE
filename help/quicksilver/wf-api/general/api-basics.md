---
content-type: api
navigation-topic: general-api
title: API-Grundlagen
description: API-Grundlagen
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: be11c7417023ce2f310fce3e0cf77724d101b89e
workflow-type: tm+mt
source-wordcount: '4461'
ht-degree: 96%

---


# API-Grundlagen

Das Ziel der Adobe Workfront-API ist die Vereinfachung der Erstellung von Integrationen mit Workfront, indem eine REST-ful-Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Workfront-API verfolgte Ansatz wird beschrieben.

Wenn Sie mit dem Workfront-Schema vertraut sind, ist es einfacher, die Datenbankbeziehungen zu verstehen, die Sie verwenden können, um Daten aus Workfront für Integrationszwecke abzurufen.

## Beschränkungen und Richtlinien

Um eine konsistente On-Demand-Systemleistung von Workfront sicherzustellen, beschränkt die Workfront-API gleichzeitige API-Threads. Diese Schutzmaßnahme verhindert Systemprobleme, die durch missbräuchliche API-Aufrufe verursacht werden. Die Sandbox-Umgebung verfügt über dieselbe maximale Anzahl gleichzeitiger API-Threads, sodass Kundinnen und Kunden sowie Partner API-Aufrufe genau testen können, bevor Code für die Produktion freigegeben wird.

Für Produktions-, Vorschau- und Testlaufwerk-Umgebungen haben Endbenutzeranfragen eine maximale URI-Länge von 8.892 Byte, da sie über das Workfront-CDN (Akamai) weitergeleitet werden. Diese Beschränkung gilt nur für URIs, die über das CDN weitergeleitet werden.

### Haftungsausschluss

Jede Verwendung der API sollte in der Beta-Umgebung von Workfront getestet werden, bevor sie in der Produktionsumgebung ausgeführt wird. Wenn ein Kunde bzw. eine Kundin die API für einen Prozess verwendet, von dem Workfront nach vernünftiger Einschätzung annimmt, dass er die On-Demand-Software belastet (d. h. der Prozess hat erhebliche negative Auswirkungen auf die Leistung der Software für andere Kundschaft), behält sich Workfront das Recht vor, die Person aufzufordern, diesen Prozess einzustellen. Wenn der Kunde bzw. die Kundin der Aufforderung nicht nachkommt und das Problem weiterhin besteht, behält sich Workfront das Recht vor, den Vorgang zu beenden.

## Workfront-API-URL

Informationen über die URL, die Sie zum Aufrufen der Workfront-API verwenden werden, finden Sie unter [Domain-Format für Adobe Workfront-API-Aufrufe](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## REST-Grundlagen

In diesem Abschnitt finden Sie eine allgemeine Einführung in die Interaktion mit der Workfront-REST-API für die folgenden REST-Grundsätze:

### Objekt-URI

Jedem Objekt im System wird ein eindeutiger URI zugewiesen, der aus dem Objekttyp und der ID besteht. Die folgenden Beispiele zeigen URIs, die drei eindeutige Objekte beschreiben:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Beim Objekttyp wird nicht zwischen Groß- und Kleinschreibung unterschieden und es kann sich entweder um den abgekürzten ObjCode (z. B. proj) oder den alternativen Objektnamen (project) handeln.

Eine Liste der Objekte, gültigen ObjCodes und Objektfelder finden Sie unter [API-Explorer](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Im Kontext der Workfront-API ist ein benutzerdefiniertes Formular ein `Category`-Objekt und ein benutzerdefiniertes Feld ein `Parameter`-Objekt.

### Vorgänge

Objekte werden durch Senden einer HTTP-Anfrage an den eindeutigen URI bearbeitet. Der auszuführende Vorgang wird durch die HTTP-Methode angegeben.

Die standardmäßigen HTTP-Methoden entsprechen den folgenden Vorgängen:

* **GET**: Ruft ein Objekt nach ID ab, sucht nach allen Objekten anhand einer Abfrage, führt Berichte aus oder führt benannte Abfragen aus
* **POST**: Fügt ein neues Objekt ein
* **PUT**: Bearbeitet ein vorhandenes Objekt
* **DELETE**: Löscht ein Objekt

Um Client-Mängel oder Protokoll-Längenbeschränkungen zu umgehen, kann der Methodenparameter verwendet werden, um das HTTP-Verhalten zu überschreiben. Beispielsweise kann ein GET-Vorgang implementiert werden, indem der folgende URI gepostet wird:
<pre>GET /attask/api/v15.0/project?id=4c78…54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78…54d0?method=get</pre>

### Antwort

Jede Anfrage erhält eine Antwort im JSON-Format. Die Antwort enthält entweder ein Datenattribut, wenn die Anfrage erfolgreich war, oder ein Fehlerattribut, wenn ein Problem aufgetreten ist. Beispielsweise gibt die Anfrage

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

gibt eine JSON-Antwort ähnlich der folgenden zurück:


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Beim Ausführen einer GET-Anfrage über die Adressleiste Ihres Browsers ist es nicht erforderlich, die Sitzungs-ID als Teil der Anfrage einzuschließen.

Besondere Sicherheit wurde für PUT-, POST- und DELETE-Anfragen hinzugefügt. Jede Anfrage, die zum Schreiben in oder Löschen aus der Datenbank führt, kann nur ausgeführt werden, wenn **sessionID=abc123** im URI enthalten ist. Die folgenden Beispiele zeigen, wie dies bei einer DELETE-Anfrage aussehen würde:
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Authentifizierung

Die API authentifiziert jede Anfrage, um sicherzustellen, dass der Client Zugriff zum Anzeigen oder Ändern eines angeforderten Objekts hat.

Die Authentifizierung erfolgt durch Übergabe einer Sitzungs-ID, die mithilfe einer der folgenden Methoden vergeben werden kann:

#### Anfrage-Header-Authentifizierung

Die bevorzugte Authentifizierungsmethode besteht darin, einen Anfrage-Header mit dem Namen SessionID zu übergeben, der das Sitzungs-Token enthält. Diese hat den Vorteil, dass sie sicher vor [Cross-Site Request Forgery (CSRF)-Angriffen](https://en.wikipedia.org/wiki/Cross-site_request_forgery) ist und den URI zu Caching-Zwecken nicht beeinträchtigt.

Im Folgenden finden Sie ein Beispiel für einen Anfrage-Header:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Cookie-basierte Authentifizierung

Die API verwendet dieselbe Cookie-basierte Authentifizierung wie die Web-Benutzeroberfläche im System. Wenn sich ein Client über die Web-Benutzeroberfläche bei Workfront anmeldet, nutzen alle AJAX-Aufrufe innerhalb desselben Browsers dieselbe Authentifizierung.

>[!NOTE]
>
>Zum Schutz vor möglichen CSRF-Angriffen (Cross Site Request Forgery) ist diese Authentifizierungsmethode nur für schreibgeschützte Vorgänge verfügbar.

## Anmeldung

>[!IMPORTANT]
>
>Workfront empfiehlt die Verwendung des `/login`-Endpunkts oder der API-Schlüssel nicht mehr. Verwenden Sie stattdessen eine der folgenden Authentifizierungsmethoden:
>
>* Server-Authentifizierung mit JWT
>* Benutzerauthentifizierung mit OAuth2
>
>Anweisungen zum Einrichten dieser Authentifizierungsmethoden finden Sie unter [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>
>Anweisungen zur Verwendung der Server-Authentifizierung in Workfront finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md)
>
>Anweisungen zur Verwendung der Benutzerauthentifizierung in Workfront finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihrer Organisation mithilfe des Autorisierungs-Code-Flusses](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
>
>Das in diesem Abschnitt beschriebene Verfahren galt nur für Organisationen, die noch nicht in die Adobe Business Platform integriert wurden. Da nun alle Organisationen in die Adobe Business-Plattform integriert wurden, ist **die Anmeldung bei Workfront über die Workfront-API nicht mehr verfügbar** .
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen die Adobe Business Platform verwendet, unterscheiden, finden Sie unter [Administrationsunterschiede zwischen Adobe Workfront und Adobe Business Platform](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Mit einem gültigen Benutzernamen und einem Kennwort können Sie die folgende Anfrage verwenden, um eine Sitzungs-ID abzurufen:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Damit wird ein Cookie gesetzt, um zukünftige Anfragen zu authentifizieren und eine JSON-Antwort mit der neu erstellten Sitzungs-ID, der Benutzer-ID des angemeldeten Benutzers bzw. der angemeldeten Benutzerin und anderen Sitzungsattributen zurückzugeben.

>[!NOTE]
>
>Wenn Sie über einen benannten API-Benutzer bzw. eine benannte API-Benutzerin verfügen, der bzw. die auch Admin ist, empfiehlt Workfront dringend, einen API-Schlüssel für die Anmeldung zu verwenden.

**Generieren eines API-Schlüssels**

Sie können einen API-Schlüssel generieren, wenn Sie sich als dieser Benutzer bzw. diese Benutzerin beim System anmelden, wie im folgenden Beispiel gezeigt:


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Abrufen eines zuvor generierten API-Schlüssels**

Sie können auch einen API-Schlüssel abrufen, der zuvor für einen bestimmten Benutzer bzw. eine bestimmte Benutzerin generiert wurde, indem Sie getApiKey ausführen:


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Dieses Ergebnis können Sie dann verwenden, um jeden API-Aufruf zu authentifizieren, indem Sie „apiKey“ als Anfrageparameter mit diesem Wert anstelle einer Sitzungs-ID oder eines Benutzernamens und eines Kennworts hinzufügen. Dies ist aus einer Sicherheitsperspektive von Vorteil.

Die folgende Anfrage ist ein Beispiel für das Abrufen von Daten aus einem Projekt mithilfe des API-Schlüssels:

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidierung eines API-Schlüssels**

Wenn der apiKey-Wert kompromittiert wurde, können Sie „clearApiKey“ ausführen. Dadurch wird der aktuelle API-Schlüssel ungültig, wie im folgenden Beispiel gezeigt:

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Nach dem Löschen können Sie getApiKey erneut ausführen, um einen neuen API-Schlüssel zu generieren.

### Abmelden

Wenn eine Sitzung abgeschlossen ist, können Sie die folgende Anfrage verwenden, um den Benutzer bzw. die Benutzerin abzumelden und so jeden weiteren Zugriff mit der Sitzungs-ID zu verhindern.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

Die Sitzungs-ID, die abgemeldet werden soll, kann entweder als Cookie, Anfrage-Header oder Anfrageparameter angegeben werden.

So melden Sie einen Benutzer bzw. eine Benutzerin ab:

1. Navigieren Sie zu Ihrem Anmeldebildschirm, melden Sie sich jedoch nicht an.
1. Ändern Sie die URL in „/attask/api/v15.0/project/search“.\
   Beachten Sie, dass die Seite nicht gefunden wurde.
1. Ersetzen Sie das Wort *search* durch „login?username=admin&amp;password=user“ und ersetzen Sie Ihren Benutzernamen und Ihr Kennwort durch *admin* und „*user“\
   *Diese Sitzung wird im Browser als Cookie gespeichert und muss nicht bei jeder nachfolgenden GET-Anfrage neu angegeben werden.

1. Ändern Sie die URL zurück in **/attask/api/v15.0/project/search**.
1. Beachten Sie die angegebene Antwort.

Bei PUT-, POST- und DELETE-Anfragen muss nach der Anmeldung immer die Sitzungs-ID angegeben werden.

## GET-Verhalten

Verwenden Sie die HTTP-GET-Methode zum Abrufen eines oder mehrerer Objekte und zum Ausführen von Berichten.

### Abrufen von Objekten

Sie können die Suche nach Objekten mithilfe von Modifikatoren und Filtern verbessern.

#### Abrufen eines Objekts mithilfe der Objekt-ID

Wenn Sie die ID eines Objekts kennen, können Sie das Objekt durch Zugriff auf seinen eindeutigen URI abrufen. Beispielsweise gibt die Anfrage

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

eine Antwort ähnlich der folgenden zurück:

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


Sie können mehrere Objekte in derselben Anfrage abrufen, indem Sie den Anfrageparameter „id“ und eine kommagetrennte Liste von IDs angeben, wie im folgenden Beispiel gezeigt:


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Beachten Sie, dass die Anfrage „/attask/api/v15.0/prBeaoject?id=...“ mit der Anfrage `/attask/api/v15.0/project/...` identisch ist.

#### Abrufen eines Objekts mithilfe des URI

Wenn Sie ein Objekt anhand anderer Kriterien als der ID abrufen möchten, können Sie nach dem URI suchen.

Beispielsweise können Sie die folgende Anfrage verwenden, um eine Liste aller Projekte im System zurückzugeben:

```
GET /attask/api/v15.0/project/search
```

Sie können Filter mithilfe der Anfrageparameter als Name-Wert-Paare angeben. Das folgende Beispiel zeigt eine Anfrage, die alle aktuellen Projekte findet:

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

| **Modifikator** | **Beschreibung** | **Beispiel** |
| --- | --- | --- |
| eq | Gibt Ergebnisse mit dem Status „Geschlossen“ zurück | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | Gibt Ergebnisse zurück, die nicht den Status „Geschlossen“ haben | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | Gibt Ergebnisse zurück, deren Prozentwert der Fertigstellung größer oder gleich 50 ist | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | Gibt Ergebnisse zurück, deren Prozentwert der Fertigstellung kleiner oder gleich 50 ist | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | Gibt Ergebnisse zurück, bei denen die Beschreibung null ist | <pre>...description_Mod=isnull...</pre> |
| notnull | Gibt Ergebnisse zurück, bei denen die Beschreibung nicht null ist | <pre>...description_Mod=notnull...</pre> |
| contains | Gibt Ergebnisse zurück, bei denen der Name „Workfront“ enthält | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| between | Gibt Ergebnisse mit einem Eingabedatum innerhalb der letzten 7 Tage zurück | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>Bei Suchanfragen wird zwischen Groß- und Kleinschreibung unterschieden. Wenn Sie eine Fehlermeldung erhalten, stellen Sie sicher, dass  **_Mod** und **_Range** die korrekte Groß-/Kleinschreibung aufweisen.

#### Verwenden von ODER-Anweisungen

Sie können eine Suche verbessern, indem Sie einen Parameter hinzufügen, der „OR“ sowie eine Zahl enthält, um die Ebene eines Filters oder einer Reihe von Filtern anzugeben.

Eine ODER-Anweisung gibt nur Einträge im API-Aufruf zurück, die den Filterkriterien der ODER-Anweisung entsprechen. Filter werden nicht bei allen ODER-Anweisungsebenen impliziert.

Wenn Sie beispielsweise nach Folgendem filtern möchten

* Aufgaben mit einem Namen, der „Planning“ enthält ODER
* Aufgaben in einem Portfolio mit dem Namen „FixedAssets“ UND jemandem mit einem Namen zugewiesen, der „Steve“ enthält ODER
* Aufgaben mit einer übergeordneten Aufgabe namens „Final Task“,

dann verwenden Sie den folgenden API-Aufruf mit seinen mehreren ODER-Anweisungen:
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Verwenden von Filterparametern

Ein potenzieller Fehler bei der Verwendung von URL-Parametern für Suchfilter besteht darin, dass Workfront bestimmte Parameter analysiert, bevor nach verschiedenen Authentifizierungsmethoden (z. B. Benutzername, Kennwort, API-Schlüssel, Cookie) gesucht wird. In diesem Fall werden die Parameter nicht als Filter im Aufruf verwendet. 

Um dieses Problem zu vermeiden, können Sie diese Werte in Filterparametern mit JSON-Formatierung einfügen. Wenn Sie beispielsweise nach dem Benutzernamen „testuser“ filtern möchten, gehen Sie wie folgt vor: Anstatt 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>zu verwenden, übergeben Sie den URL-Parameter in einem Filter, wie im folgenden Beispiel gezeigt:
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Verwenden des Anfrageparameters „map“

Standardmäßig handelt es sich bei den von einer Suche zurückgegebenen Daten um ein JSON-Array. Je nach Anwendungsfall ist es möglicherweise effizienter, das Ergebnis als ein nach ID indiziertes JSON-Objekt abzurufen. Verwenden Sie dazu den Anfrageparameter „map“. Beispielsweise gibt die Anfrage 
<pre>/attask/api/v15.0/task/search?map=true</pre>eine nach ID indizierte Antwort ähnlich der folgenden zurück:
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "first task",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "second task",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Verwenden des Anfrageparameters „fields“

Standardmäßig wird beim Abrufen eines Objekts nur die am häufigsten verwendete Teilmenge von Feldern zurückgegeben.

Mit dem Anfrageparameter „fields“ können Sie angeben, dass eine kommagetrennte Liste bestimmter Felder zurückgegeben wird. Beispielsweise gibt die Anfrage
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>eine Antwort ähnlich der folgenden zurück:
<pre>{<br>    "priority": 2,<br>    "name": "first task",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
>Bei diesen Feldnamen wird zwischen Groß- und Kleinschreibung unterschieden.

Eine Liste der möglichen Feldverweise finden Sie unter [API-Explorer](../../wf-api/general/api-explorer.md)

#### Suchen nach verschachtelten Objekten

Sie können nach verschachtelten Objekten suchen. Standardmäßig werden verschachtelte Objekte nur mit dem Namen und der ID zurückgegeben. Verwenden Sie beispielsweise die folgende Anfrage, um alle Probleme zusammen mit ihren Inhabenden abzurufen:
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Wenn weitere Informationen erforderlich sind, können Sie ein verschachteltes Feld mithilfe der Doppelpunkt-Syntax anfordern. Beispielsweise sucht die folgende Anfrage nach allen Problemen zusammen mit dem Namen, der ID, dem Titel und der Telefonnummer des Inhabers bzw. der Inhaberin
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>und gibt Folgendes zurück: 
<pre>{<br>    "name": "an important issue",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "Operations Specialist",<br>        "phoneNumber": "555-1234",<br>        "name": "Admin User",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Abrufen verschachtelter Sammlungen

Sie können verschachtelte Sammlungen von Objekten abrufen. Um beispielsweise ein Projekt mit allen seinen Aufgaben abzurufen, verwenden Sie die folgende Anfrage:
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>Die folgende Anfrage ruft Aufgabenzuweisungen ab:
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Suchen nach mehreren verschachtelten Feldern

Standardmäßig werden nur der Name und die ID jeder Aufgabe zurückgegeben. Es können jedoch zusätzliche verschachtelte Felder mit Doppelpunkt-Syntax angegeben werden. Um alle verfügbaren Felder für ein verknüpftes Objekt oder eine Sammlung anzuzeigen, hängen Sie einfach einen Doppelpunkt und ein Sternchen an die Objekt-/Sammlungsreferenz an.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### Abrufen benutzerdefinierter Daten

Benutzerdefinierte Datenfelder können mit dem Präfix „DE:“ abgerufen werden. Um beispielsweise ein Projekt mit einem Parameter namens „CustomText“ anzufordern, verwenden Sie die folgende Anfrage:
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>die Folgendes zurückgibt
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "task b" <br>}</pre>Sie können auch alle benutzerdefinierten Daten für ein Objekt abrufen, indem Sie das Feld „parameterValues“ anfordern. Beispiel: 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>gibt Daten ähnlich den folgenden zurück:
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### Verwenden benannter Abfragen

Einige Objekttypen verfügen über benannte Suchvorgänge, die häufig ausgeführt werden und verfügbar sind, indem der Name der Abfrage an das Ende des Objekttyp-URI angehängt wird. Beispielsweise ruft die folgende Anfrage die Arbeitselemente (Aufgaben und Probleme) ab, denen der Benutzer bzw. die Benutzerin derzeit zugewiesen ist:
<pre>/attask/api/v15.0/work/myWork</pre>Benannte Abfragen unterstützen das Anfordern des Parameters „fields“ zum Abrufen zusätzlicher Felder. Einige benannte Abfragen akzeptieren auch zusätzliche Filter. Eine Liste der zulässigen Abfragen mit dem Namen eines Objekts finden Sie auf der Registerkarte „Aktion“ für das Objekt im [API-Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### Verwenden von `Count`

Sie können `count` verwenden, um die Anzahl der Ergebnisse zurückzugeben, die Ihrer Abfrage entsprechen. Dies kann nützlich sein, wenn Sie die Daten in den Ergebnissen nicht benötigen. Wird nur die Anzahl zurückgegeben, kann der Server die Anfrage schneller verarbeiten und Bandbreite sparen. Beispielsweise gibt die Anfrage
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>gibt die Anzahl der Ergebnisse im folgenden Format zurück:
<pre>{<br>    "count": 3 <br>}</pre>Bei der Rückgabe einer Anzahl werden viel weniger Daten übertragen als bei der Rückgabe der vollständigen Objekte. Die Syntax ist identisch mit dem Suchbefehl.

### Anfordern eines Berichts

Sie können eine Berichtsanfrage ausführen, bei der nur das Aggregat eines bestimmten Feldes mit einer oder mehreren Gruppierungen gewünscht wird. Wie im folgenden Beispiel gezeigt, ist die Berichtssyntax mit der Syntax für die SOAP-API identisch:
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>gibt das folgende Ergebnis zurück
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>     "Second Project": { <br>        "sum_hours": 30 <br>    } <br>}</pre>Das Hinzufügen des Parameters „$$ROLLUP=true“ ergibt eine Summe auf jeder Gruppierungsebene:
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>    "Second Project": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### Sortieren von Abfrageergebnissen in der API

Sie können Ihre Ergebnisse nach einem beliebigen Feld sortieren, wenn Sie Folgendes an Ihren API-Aufruf anhängen:

&amp;entryDate_Sort=asc

Wenn Sie beispielsweise nach dem geplanten Startdatum der Aufgabe sortieren möchten, entfernen Sie „entryDate“ und ersetzen Sie es durch „scheduledCompletionDate“.

Dies funktioniert für die meisten Felder in Workfront.

### Überlegungen zu Abfragebeschränkungen

Bei der Abfrage eines Objekts sollten Überlegungen hinsichtlich der Beziehung zwischen Objekten und Suchbeschränkungen angestellt werden. Wie in der folgenden Tabelle dargestellt, kann eine Abfrage für Projekte beispielsweise nicht mehr als 2.000 Projekte zurückgeben. Diese 2.000 Projekte werden als „primäre Objekte“ betrachtet. Wenn Sie das Feld „Aufgaben“ für die Projekte abfragen, wird das Feld „Aufgaben“, das eine Sammlung ist, zum sekundären Objekt des primären Objekts „Projekt“. Eine Abfrage für das Feld „Aufgaben“ kann Tausende von Aufgaben in Projekten enthalten. Insgesamt darf die Gesamtanzahl der zurückgegebenen Objekte (Projekte und Aufgaben) 50.000 nicht überschreiten.

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
   <td> Wenn im Abfragefilter (d. h. $$LIMIT) kein Limit angegeben ist, kann das Ergebnis nicht mehr als 100 primäre Objekte enthalten. <br>Unter <a href="#using-paginated-responses" class="MCXref xref">Verwenden paginierter Antworten</a> finden Sie Anweisungen zum Überschreiben dieser Einschränkung. </td> 
  </tr> 
  <tr> 
   <td>Max. Anzahl der Ergebnisse</td> 
   <td>2.000</td> 
   <td>Der Abfragefilter (d. h. $$LIMIT) kann nicht mehr als 2.000 Ergebnisse zurückgeben. Weitere Informationen finden Sie unter „Paginierte Antworten“.</td> 
  </tr> 
  <tr> 
   <td>Max. Feldtiefe</td> 
   <td>4</td> 
   <td>Bei der Ermittlung der Felder, die Sie anzeigen möchten, dürfen Sie sich nicht mehr als vier Ebenen vom abgefragten Objekt entfernen.</td> 
  </tr> 
  <tr> 
   <td>Max. Objektanzahl</td> 
   <td>50.000</td> 
   <td>Der Ergebnissatz darf nicht mehr als 50.000 primäre und sekundäre Objekte enthalten.</td> 
  </tr> 
  <tr> 
   <td>Max. Anzahl der Felder</td> 
   <td nowrap>1.000.000</td> 
   <td>Wenn der Ergebnissatz weniger als 50.000 Objekte umfasst, können die Ergebnisse maximal 1.000.000 Felder enthalten.</td> 
  </tr> 
  <tr> 
   <td>Max. Anzahl der Batch-Erstellungen/-Updates</td> 
   <td>100</td> 
   <td>Das maximale Limit für die Erstellung oder Aktualisierung von Batches ist 100.</td> 
  </tr> 
 </tbody> 
</table>

### Verwenden paginierter Antworten {#using-paginated-responses}

Um die Abfragebeschränkung für die Standardanzahl der Ergebnisse zu überschreiben und 200 Ergebnisse zuzulassen, können Sie den Filter `$$LIMIT=200` in Ihre Abfrage einbeziehen, wie im folgenden Beispiel gezeigt:
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Um die Zuverlässigkeit und die Leistung anderer Mandanten im System sicherzustellen, beträgt die maximal zulässige Anzahl der Ergebnisse pro Abfrage 2.000 Objekte. Der Versuch, ein höheres Limit anzugeben, führt zu einer Fehlermeldung vom Typ `IllegalArgumentException`. 

Daher empfehlen wir die Verwendung paginierter Antworten für große Datensätze. Um das erste Ergebnis anzugeben, das zurückgegeben werden soll, fügen Sie den Filter `$$FIRST` hinzu. Beispielsweise gibt die folgende Anfrage die Ergebnisse 201–250 für eine Abfrage zurück:
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Beachten Sie, dass `$$FIRST=200` im obigen Beispiel das 201. Ergebnis zurückgibt. `$$FIRST=0` würde das erste Ergebnis zurückgeben. Es kann hilfreich sein, sich den Wert „$$FIRST“ als die Anzahl der Ergebnisse vorzustellen, die Sie überspringen möchten, bevor Ergebnisse zurückgegeben werden.

Um sicherzustellen, dass Ihre Ergebnisse ordnungsgemäß paginiert werden, verwenden Sie einen Sortierparameter. Dadurch können die Ergebnisse in derselben Reihenfolge zurückgegeben werden, sodass die Ergebnisse bei der Paginierung nicht wiederholt oder übersprungen werden. Um beispielsweise anhand der Objekt-ID zu sortieren, verwenden Sie `ID_Sort=asc`.

### Erstellen einer Zugriffsregel

Sie können eine Zugriffsregel erstellen, um zu bestimmen, wer auf ein Objekt zugreifen kann. Im Folgenden finden Sie Beispiele für Zugriffsregeln, die Sie festlegen können:

Um ein Projekt so einzurichten, dass es nur für einen Benutzer bzw. eine Benutzerin mit der ID „abc123“ freigegeben wird, verwenden Sie die folgende Anfrage:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Alternativ können Sie die Freigabe nur für eine Person durchführen und die bestehenden Berechtigungen beibehalten:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>So rufen Sie die vorhandenen Zugriffsregeln ab:
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Verhalten von POST

POST fügt ein neues Objekt ein. Die Syntax entspricht der von PUT, mit einigen Ausnahmen. Da das neue Objekt noch nicht vorhanden ist, hat es keine ID. Aus diesem Grund enthält der URI die ID nicht.

### Erstellen eines Objekts

Im Folgenden finden Sie ein Beispiel für eine Anfrage zum Erstellen eines neuen Projekts:
<pre>POST /attask/api/v15.0/project?name=New Project</pre>Die Antwort enthält das neu erstellte Projekt zusammen mit seiner neuen ID und allen anderen angegebenen Feldern.

### Kopieren eines Objekts

Einige Objekte unterstützen das Kopieren. Für diese Objekttypen ist es möglich, neue Objekte durch Posten mit dem Parameter „copySourceID“ zu erstellen. Beispielsweise wird das angegebene Projekt mit der folgenden Anfrage kopiert und ein neuer Name für das Projekt festgelegt:

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Hochladen von Dokumenten

Sie können Dokumente über die folgende API-URL hochladen:
<pre>POST /attask/api/v15.0/upload</pre>Die API erwartet, dass der Inhaltstyp „multipart/form-data“ ist. Der Parametername für die Datei muss „uploadedFile“ sein. Der Server gibt die folgenden JSON-Daten zurück:
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Beim Erstellen eines Workfront-Dokuments können Sie den Handle verwenden und in der folgenden URL posten:
<pre>POST /attask/api/v15.0/document?updates={<br>    name: aFileName,<br>    handle: abc...123, (handle from the file upload)<br>    docObjCode: PROJ, (or TASK, OPTASK, etc)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## Verhalten von PUT

PUT wird verwendet, um ein vorhandenes Objekt zu aktualisieren.

Die Antwort für eine PUT-Anfrage ist identisch mit der einer GET-Anfrage. In beiden Fällen gibt der Server den neuen Status des Objekts nach der Aktualisierung zurück. Alle Regeln, die zum Ändern einer Antwort auf eine GET-Anfrage verwendet werden, funktionieren auch mit PUT, z. B. die Angabe zusätzlicher zurückzugebender Felder, benutzerdefinierter Daten usw.

### Bearbeiten von Objekten

Aktualisierungen an Objekten werden immer nach ID unter Verwendung des eindeutigen URI des Objekts durchgeführt. Zu aktualisierende Felder werden als Anfrageparameter angegeben. Um beispielsweise den Namen eines Projekts zu ändern, können Sie eine Anfrage ähnlich der folgenden senden:
<pre>PUT /attask/api/v15.0/project/4c7..?name=New Project Name <br>PUT /attask/api/v15.0/project?id=4c7…&amp;name=New Project Name</pre>Da für die Aktualisierung eine ID erforderlich ist, schlägt dieser Vorgang (ohne Einfügen) fehl, wenn das Objekt auf dem Server nicht vorhanden ist.

### Angeben von JSON-Änderungen

Wie im folgenden Beispiel gezeigt, können Sie den Anfrageparameter „updates“ verwenden, um die zu aktualisierenden Felder mithilfe der JSON-Syntax anzugeben:
<pre>PUT /attask/api/v15.0/project/4c7..?updates= <br>{<br> name: „New Project Name“, <br> status: „CUR“, <br> … <br>}</pre>

### Durchführen verschachtelter Aktualisierungen

Einige Objekte verfügen über private Sammlungen, die aktualisiert werden können. Im folgenden Beispiel wird beispielsweise veranschaulicht, wie die vorhandenen Arbeitsaufträge für eine bestimmte Aufgabe überschrieben werden:
<pre>PUT /attask/api/v15.0/task/4c7..?updates= <br>{<br> Arbeitsaufträge: [ <br> { <br> assignedToID: „2222…54d0, <br> assignmentPercent: 50.0 <br> },{ <br> roleID: „1111…54d0“<br> } <br> ] <br>}</pre>

>[!NOTE]
>
>Aktualisierungen an der obersten Ebene sind zwar selten, aber Aktualisierungen an einer Sammlung oder einem verschachtelten Objekt ersetzen die vorhandene Sammlung vollständig. Um einen einzelnen Arbeitsauftrag für eine Aufgabe zu bearbeiten, ohne dass sich dies auf die Objekte auswirkt, verwenden Sie PUT für den Arbeitsauftrag und nicht für die Aufgabe.

Im folgenden Beispiel wird ein Projekt zu einer öffentlichen Helpdesk-Warteschlange. Beachten Sie, dass die vorhandenen Warteschlangeneigenschaften ersetzt werden.
<pre>PUT /attask/api/v15.0/project/4c7…?updates= <br>{ <br> queueDef: { <br> isPublic: 1 <br> } <br>}</pre>

### Verwenden des Anfrageparameters „action“

Einige Objekte unterstützen weitere Aktionen, die zusätzlich zu einfachen Änderungen durchgeführt werden können. Diese Aktionen können Sie mit dem Anfrageparameter „action“ angeben. Mit der folgenden Anfrage wird beispielsweise die Timeline für ein bestimmtes Projekt neu berechnet:
<pre>PUT /attask/api/v15.0/project/4c7..?action=calculateTimeline<br><br>or<br><br>PUT /attask/api/v15.0/project/4c7…/calculateTimeline </pre>

### Verschieben von Objekten

Im Folgenden wird die Syntax zum Verschieben einer Aufgabe von einem Projekt zu einem anderen veranschaulicht:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>Hier ist ein Beispiel für jeden Aktionstyp angegeben: (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Nur für die Aktion zum Verschieben („move“) müssen zusätzliche Attribute angegeben werden, um das Projekt näher zu bestimmen, zu dem das Arbeitselement verschoben werden soll.

Nachfolgend finden Sie ein Beispiel für jeden Aktionstyp: 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Freigeben von Objekten

Das folgende Beispiel zeigt die Syntax für die Freigabe eines Projekts für ein Team:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Beim Bearbeiten eines Objekts können Sie alle Zugriffsregeln für ein Objekt ersetzen, indem Sie eine PUT-Anweisung durchführen und Aktualisierungen ähnlich dem folgenden Beispiel senden:
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>Das folgende Beispiel zeigt die Syntax zum Verschieben einer Aufgabe von einem Projekt zu einem anderen:
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## Verhalten von DELETE

Mit DELETE wird ein Objekt entfernt. In jedem Fall kann der URI den Parameter „force=true“ enthalten, damit die angegebenen Daten und deren abhängige Elemente vom Server entfernt werden. Im folgenden Beispiel wird eine Aufgabe gelöscht, indem die HTTP-DELETE-Methode für einen URI ausgeführt wird:
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Massenaktualisierungen

Mit einer Massenaktualisierungs-Anweisung werden mehrere Objekte gleichzeitig innerhalb eines einzigen API-Aufrufs aktualisiert. Ein Massenerstellungs-API-Aufruf wird ähnlich wie ein normaler Aktualisierungsaufruf erstellt, wie in den folgenden Beispielen gezeigt:
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>oder <pre>PUSH /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>was zu einem Ergebnis ähnlich dem folgenden führt:
<pre>data: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>}]</pre>Sie können auch eine Massenaktualisierung ähnlich der folgenden durchführen:
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>was zu einem Ergebnis ähnlich dem folgenden führt:
<pre>data: [ {<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>     priority: 0,<br>     projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    status: "CUR"<br>}]</pre>Wenn Sie möchten, dass alle Vorgänge in derselben Transaktion stattfinden, fügen Sie „atomic=true“ zu Ihrem Batch-API-Aufruf als Anfrageparameter hinzu. Auf diese Weise werden alle Vorgänge zurückgesetzt, wenn einer der Vorgänge fehlschlägt.

>[!NOTE]
>
>Atomic-Batch-Vorgänge können nur „success: true“ oder einen Fehler zurückgeben.

