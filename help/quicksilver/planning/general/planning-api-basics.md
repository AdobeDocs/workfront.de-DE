---
title: Grundlagen zur Adobe Workfront-Planungs-API
description: Das Ziel der Adobe Workfront Planning-API besteht darin, die Erstellung von Integrationen mit Planning zu vereinfachen, indem eine REST-ful-Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind, und der von der Planungs-API verfolgte Ansatz beschrieben.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: fdbe3945f59306fc26424d7e88b799d9dcaea4da
workflow-type: tm+mt
source-wordcount: '2206'
ht-degree: 4%

---


# Grundlagen zur Adobe Workfront-Planung-API

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

Das Ziel der Adobe Workfront Planning-API besteht darin, die Erstellung von Integrationen mit Planning zu vereinfachen, indem eine RESTful-Architektur eingeführt wird, die über HTTP ausgeführt wird. In diesem Dokument wird davon ausgegangen, dass Sie mit REST- und JSON-Antworten vertraut sind.

Eine vollständige Endpunktreferenz, Anfrage-/Antwortschemata und versionsspezifische Details finden Sie in der Entwicklerdokumentation zur [Workfront Planning API](https://developer.adobe.com/wf-planning).

## Authentifizierung

Die Workfront Planning-API verwendet OAuth 2.0 zur Authentifizierung. Anmeldedaten werden über die Adobe Developer Console eingerichtet.

Je nach Integrationstyp werden die folgenden beiden Flüsse unterstützt:

* **Server-zu-Server-Authentifizierung (JWT)**: Für automatisierte Integrationen und Backend-Services ohne Benutzerinteraktion. Verwendet die OAuth Server-zu-Server-Anmeldedaten (Client-Anmeldedaten erteilen - Ihre Anwendung authentifiziert sich direkt mithilfe ihrer Client-ID und ihres Geheimnisses, um ein Zugriffstoken zu erhalten, ohne dass ein Benutzer-Login oder Einverständnisschritt erforderlich ist).

  Weitere Informationen finden Sie unter [Server-zu-Server-](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/).

* **Benutzerauthentifizierung (Autorisierungs-Code-Fluss)** für Integrationen, die im Namen eines bestimmten Benutzers handeln. Verwendet die Anmeldeinformationen für die OAuth-Web-App oder die Einzelseiten-App (Autorisierungs-Code erteilen - der Benutzer meldet sich an und willigt ein, woraufhin Ihre Anwendung einen Autorisierungs-Code erhält und gegen ein Zugriffs-Token eintauscht).

  Weitere Informationen finden Sie unter [Benutzerauthentifizierung](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/).

Erstellen Sie zunächst ein Projekt in der Adobe Developer Console und fügen Sie die Workfront Planning-API hinzu, um Ihre Anmeldeinformationen abzurufen.

Um Anmeldeinformationen einzurichten, erstellen Sie ein OAuth2-Programm in Workfront.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

>[!NOTE]
>
>Der `/login`-Endpunkt und die API-Schlüsselauthentifizierung werden für Workfront Planning nicht unterstützt. Verwenden Sie keine `sessionID` oder `apiKey` Parameter.


## API-Versionierung

Die Planning-API wird über den URL-Pfad versioniert.

Die folgenden Versionen werden derzeit unterstützt:

| Version | Veröffentlichungsdatum |
|-----------|----------------|
| Version 1 | Juli 2024 |
| Version 2 | Mai 2026 |

<!--

(*****************add deprecation date column above, when we have one*****************)

-->


Weitere Informationen zu den derzeit unterstützten Versionen finden Sie im Artikel [Entwicklerdokumentation für die Workfront Planning API](https://developer.adobe.com/wf-planning).

Es wird empfohlen, eine Version in allen Integrationen explizit festzulegen:

```
https://{customer-domain}/maestro/api/v2/...
```

Wenn eine neue Hauptversion veröffentlicht wird, ist die vorherige Version weiterhin verfügbar, bis ein Verfallsdatum mitgeteilt wird.

Folgen Sie den Workfront-Versionshinweisen , um über API-Änderungen auf dem Laufenden zu bleiben.


## URL-Struktur und -Vorgänge

Objekte werden durch Senden einer HTTP-Anfrage an den eindeutigen URI bearbeitet. Der Vorgang wird durch die HTTP-Methode angegeben.

| Methode | Vorgang |
|----------|----------------------------------------------------------------------|
| GET | Abrufen eines einzelnen Objekts nach ID oder Suche/Listenobjekte |
| POST | Neues Objekt erstellen |
| PUT | Vorhandenes Objekt ersetzen (vollständige Aktualisierung) |
| PATCH | Vorhandenes Objekt teilweise aktualisieren (nur die angegebenen Felder werden geändert) |
| LÖSCHEN | Löschen eines Objekts |

>[!NOTE]
>
>**Version1 Hinweis:** `PATCH` wird in Version 1 nicht unterstützt. `PUT` für alle Aktualisierungen verwenden.


Vollständige Endpunktpfade und Anfrage-/Antwortbeispiele finden Sie in der **API-Referenz** unter [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## HTTP-Status-Codes

Die Planning-API gibt Standard-HTTP-Status-Codes zurück:

| Code | Bedeutung |
|------------------------|-------------------------------------------------|
| 200 OK | Erfolgreicher GET-, PUT- oder PATCH-Test |
| 201 Erstellt | Erfolgreicher POST (Ressource erstellt) |
| 204 Kein Inhalt | Erfolgreiche DELETE |
| 207 Multi-Status | Massenvorgang mit gemischten Ergebnissen abgeschlossen, wobei einige Elemente erfolgreich waren und einige fehlgeschlagen sind. Details finden Sie in den Antworten auf einzelne Elemente. |
| 400 Fehlerhafte Anfrage | Ungültige Anfrage — Details finden Sie in der Fehlerantwort |
| 401 Nicht autorisiert | Fehlendes oder ungültiges Authentifizierungstoken |
| 403 Verboten | Authentifiziert, aber unzureichende Berechtigungen |
| 404 nicht gefunden | Ressource existiert nicht |
| 409 Konflikt | Bei einem Schreibkonflikt wurde die Ressource durch eine andere Anfrage geändert. Versuchen Sie es erneut mit der neuesten Version. |
| 429 zu viele Anfragen | Ratenlimit überschritten |

>[!NOTE]
>
>**Hinweis Version 1:** Version 1 gibt `200 OK` für alle erfolgreichen Vorgänge zurück, einschließlich POST und DELETE.


## Umgang mit Fehlern

Die Planning-API gibt Fehler in einem konsistenten Format zurück. Jede Fehlerantwort enthält eine für Menschen lesbare Nachricht, einen maschinenlesbaren Fehlercode und eine Anfrage-ID für die Support-Eskalation.

Beispielfehlerantwort:

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}
```

Verwenden Sie `errorCode` (nicht `status`), um die programmgesteuerte Fehlerbehandlung zu steuern. Er bietet die spezifischste Klassifizierung des Fehlers.

>[!NOTE]
>
>**Hinweis zu Version 1:** Fehlerantworten der Version 1 verwenden ein numerisches `type` (z. B. `40001`) anstelle eines `errorCode` und schließen Details in ein `report`-Objekt anstelle eines `detail`-Felds der obersten Ebene ein.

## Datensätze filtern

Verwenden Sie den `filter`-Parameter in Datensatzsuchanfragen, um nur Datensätze zurückzugeben, die bestimmten Kriterien entsprechen. Bei POST-Anfragen ist `filter` eine JSON-Eigenschaft im Anfragetext. Bei GET-Anfragen ist `filter` ein Abfrageparameter, der eine JSON-codierte Filtergruppe enthält. Filter verwenden eine typisierte zusammengesetzte Struktur mit expliziten logischen Operatoren.

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}
```

Filter können mit `AND`/`OR`-Operatoren verschachtelt werden, um zusammengesetzte Bedingungen zu erstellen:

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}
```

>[!NOTE]
>
>**Version 1 Hinweis:** Version 1 verwendet nicht typisierte Operatoren im Mongo-Stil in einem `filters`. Operatoren erhalten das Präfix `$` (z. B. `$and`, `$or`, `$is`, `$contains`, `$isBetween`). Paginierungsparameter (`offset`, `limit`) und `recordTypeId` werden im Anfragetext und nicht als URL-Pfad und Abfrageparameter übergeben.


## Feldtypen und Suchmodifikatoren

Sie können Modifikatoren und Filter mit Feldern verwenden, um zu steuern, welche Daten in den Ergebnissen zurückgegeben werden.

Beispiele finden Sie in der Entwicklerdokumentation zur [Workfront Planning API](https://developer.adobe.com/wf-planning/).

### Verwenden von Suchmodifikatoren

Workfront Planning unterstützt die folgenden Suchmodifikatoren:


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>Modifikator</th>
      <th>Beispiel</th>
      <th>Beschreibung</th>
      <th>Mögliche Werte</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTAINS</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„CONTAINS“,„value“:„product“}</td><td>Gibt Datensätze zurück, deren Feldwert den Filter enthält</td><td class="possible">„Neue Produkteinführung“</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„DOES_NOT_CONTAIN“,„value“:„product“}</td><td>Gibt Datensätze zurück, bei denen der Feldwert den Filter nicht enthält</td><td class="possible">„Neue Einführung“</td></tr>
    <tr><td class="modifier">IST</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS“,„value“:„New Product Launch“}</td><td>Gibt Datensätze zurück, deren Feldwert genau mit dem Filter übereinstimmt</td><td class="possible">„Neue Produkteinführung“</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_NOT“,„value“:„product“}</td><td>Gibt Datensätze zurück, deren Feldwert nicht genau mit dem Filter übereinstimmt</td><td class="possible">„Neue Produkteinführung“</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_EMPTY“}</td><td>Gibt Datensätze zurück, deren Feldwert leer ist</td><td class="possible">"" oder „null“</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_NOT_EMPTY“}</td><td>Gibt Datensätze zurück, deren Feldwert nicht leer ist</td><td class="possible">„Neue Produkteinführung“</td></tr>
    <tr><td class="modifier">GRÖSSER_ALS</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„GREATER_THAN“,„value“:„10“}</td><td>Gibt Datensätze zurück, deren Feldwert größer als der Filter ist</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GRÖSSER_ALS_ODER_GLEICH</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„GREATER_THAN_OR_EQUAL“,„value“:„10“}</td><td>Gibt Datensätze zurück, deren Feldwert größer oder gleich dem Filter ist.</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„LESS_THAN“,„value“:„10“}</td><td>Gibt Datensätze zurück, deren Feldwert kleiner als der Filter ist</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„LESS_THAN_OR_EQUAL“,„value“:„10“}</td><td>Gibt Datensätze zurück, deren Feldwert kleiner oder gleich dem Filter ist.</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_BETWEEN“,„value“:[„2024-01-01“,„2024-12-31“]}</td><td>Gibt Datensätze zurück, deren Feldwert zwischen den beiden Filterwerten liegt.</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_NOT_BETWEEN“,„value“:[„2024-01-01“,„2024-12-31“]}</td><td>Gibt Datensätze zurück, deren Feldwert nicht zwischen den beiden Filterwerten liegt</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_AFTER“,„value“:„2024-01-01“}</td><td>Gibt Datensätze zurück, deren Datumsfeldwert nach dem Filter liegt.</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_BEFORE“,„value“:„2024-12-31“}</td><td>Gibt Datensätze zurück, deren Datumsfeldwert vor dem Filter liegt.</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_ANY_OF“,„value“:[„Active“,„Planned“]}</td><td>Gibt Datensätze zurück, deren Feldwert mit einem Wert in der Filterliste übereinstimmt</td><td class="possible">[„Aktiv“,„Geplant“,„Abgeschlossen“]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_NONE_OF“,„value“:[„Active“,„Planned“]}</td><td>Gibt Datensätze zurück, deren Feldwert keinem der Werte in der Filterliste entspricht</td><td class="possible">[„Aktiv“,„Geplant“]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„HAS_ANY_OF“,„value“:[„Tag1“,„Tag2“]}</td><td>Gibt Datensätze zurück, deren mehrwertiges Feld einen der Filterwerte enthält</td><td class="possible">[„Tag1“,„Tag2“]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„HAS_ALL_OF“,„value“:[„Tag1“,„Tag2“]}</td><td>Gibt Datensätze zurück, deren mehrwertiges Feld alle Filterwerte enthält</td><td class="possible">[„Tag1“,„Tag2“]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„IS_EXACTLY“,„value“:[„Tag1“]}</td><td>Gibt Datensätze zurück, deren mehrwertiges Feld genau die Filterwerte und keine weiteren enthält</td><td class="possible">[„Tag1“]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{„fieldId“:“&lt;id&gt;",„condition“:„HAS_NONE_OF“,„value“:[„Tag1“]}</td><td>Gibt Datensätze zurück, deren mehrwertiges Feld keinen der Filterwerte enthält</td><td class="possible">[„Tag1“]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>Version 1 Hinweis: V1-Modifikatornamen verwenden `$-prefixed camelCase` (z. B. `$contains`, `$isNot`, `$isEmpty`, `$greaterThan`, `$greaterThanOrEqual`, `$lessThan`, `$lessThanOrEqual`, `$isBetween`, `$isNotBetween`, `$isAnyOf`, `$hasAllOf`). Das Verhalten der einzelnen Modifikatoren ist identisch.


## Unterstützte Filterbedingungen nach Feldtyp

| Feldtyp | Unterstützte Bedingungen |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| Text, Langtext | ENTHÄLT, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| Zahl, Prozentsatz, Währung | IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY |
| Datum | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| Einzelauswahl | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| Mehrfachauswahl, Benutzer | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| Boolescher Wert | IST |
| Formel | ENTHÄLT, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| created-by | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF |
| Aktualisiert von | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| created-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN |
| updated-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| Verweis | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| Lookup | Hängt vom verknüpften Feldtyp ab |

>[!NOTE]
>
>**Version 1 Hinweis:** Version 1 verwendet `$`-vorangestellte Operatornamen (z. B. `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). Der Satz unterstützter Bedingungen pro Feldtyp ist identisch.

## Nach Personenfeldern filtern

Personenfeldfilter (`user`, `created-by`, `updated-by`, `approved-by`) akzeptieren sowohl Adobe IMS- als auch Workfront-Benutzer-IDs. Ein einfacher Zeichenfolgenwert wird als Adobe IMS-Benutzer-ID interpretiert.

Um den Kennungstyp zur Überprüfung der Workfront-Benutzer-ID festzulegen, müssen Sie explizit `id`- und `idType` übergeben. Unterstützte Werte für `idType` sind &quot;`WF`&quot; für Workfront-Benutzer-IDs und &quot;`IMS`&quot; für Adobe IMS-Benutzer-IDs.

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
> Hinweis zur Version 1: V1 unterstützt nur das Filtern nach der IMS-ID der Benutzer.

## Filtern externer Referenzfelder nach externer ID

Externe Referenzfelder verknüpfen Datensätze mit Objekten in anderen Adobe-Systemen (z. B. Workfront-Projekten oder AEM Assets). Intern weist Planning diesen Objekten Planungsdatensatz-IDs zu. Um diese Felder direkt nach ihrer ursprünglichen Objekt-ID zu filtern, fügen Sie `"matchExternalId": true` zu einer Filterbedingung hinzu.

Dieses Flag ist nur für Referenzfelder gültig, bei denen `referenceOptions.isExternal` `true` ist. Bei nicht externen Referenzfeldern wird es ignoriert. Wenn ein einzelner Zeichenfolgenwert nicht aufgelöst werden kann, schlägt die Anfrage mit `400 Bad Request` fehl. Wenn ein Listenwert angegeben wird, durchlaufen nicht aufgelöste Einträge unveränderte Elemente und stimmen einfach nicht überein.

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
>Hinweis zu Version 1: V1 unterstützt nicht das Filtern nach externen Objekt-IDs.

## Felder für externe Verbindungen

Planungs-Datensatztypen können externe Referenzfelder hosten, die Datensätze mit Objekten in anderen Adobe-Systemen verknüpfen, anstatt mit anderen Planungs-Datensatztypen.

Um ein externes Referenzfeld über die API zu erstellen, legen Sie `referenceOptions.recordTypeId` in einem neuen `REFERENCE` auf die ID des gewünschten externen Datensatztyps fest. Der Server leitet `referenceOptions.isExternal=true` und die Verbindungsmetadaten (`connectionName, objectName`) automatisch vom Zieldatensatztyp ab.

Zu den unterstützten externen Objekttypen gehören Workfront-Objekte (Projekte, Aufgaben, Programme, Portfolios, Unternehmen, Gruppen, Teams, Benutzer) und AEM Assets (Assets, Inhaltsfragmente).

>[!NOTE]
>
>Hinweis zu Version 1: V1 unterstützt nicht das Erstellen externer Verbindungsfelder.


## Sortieren

Sortieren Sie die Ergebnisse nach einem beliebigen Feld, indem Sie ein `sort`-Array in Ihre Anfrage aufnehmen:

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

Mehrere Sortierfelder werden der Reihe nach ausgewertet. Wenden Sie bei der Paginierung immer eine Sortierung an, um eine konsistente Sortierung über Seiten hinweg sicherzustellen.

Um Ergebnisse zu gruppieren, fügen Sie neben Sortieren ein Gruppen-Array ein:

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>Hinweis zu Version 1: V1 verwendet `sorting` (nicht `sort`), `groupingFieldIds` (Array von Feld-IDs, nicht `group` Objekte) und die jetzt nicht mehr unterstützte `rowOrderViewId`, um die Zeilenreihenfolge einer vorhandenen Ansicht anzuwenden. Keiner dieser V1-Parameter wird in der Version unterstützt

## Feldprojektion

Um zu begrenzen, welche Felder in einer Antwort zurückgegeben werden, verwenden Sie die `fieldIds` oder `fieldAliases` Abfrageparameter mit einer kommagetrennten Liste. Dies reduziert die Größe der Antwort-Payload und wird für Integrationen mit hohem Volumen oder Latenzabhängigkeit empfohlen.

>[!NOTE]
>
>**Version 1 Hinweis:** Version 1 verwendet `?attributes=` für die Projektion (z. B. `?attributes=data,createdBy`) anstelle von `?fieldIds=` oder `?fieldAliases=`.

## Paginierung

Die Planning-API unterstützt paginierte Antworten zum Verwalten großer Datensätze.

* **Cursor-basierte Paginierung** wird für Arbeitsbereiche, Datensatztypen, Felder und Ansichten verwendet. Übergeben Sie einen `cursor` aus der vorherigen Antwort, um die nächste Seite abzurufen. Cursor-basierte Antworten enthalten das Flag HasMore , das angibt, ob mehr Seiten vorhanden sind oder nicht.
* **Seitenbasierte Paginierung** wird für die Datensatzsuche verwendet. Verwenden Sie `page` und `size` als Abfrageparameter. Wenden Sie bei der Paginierung immer eine Sortierung an, um eine konsistente Sortierung über Seiten hinweg sicherzustellen. Beachten Sie, dass die Paginierung auf Null basiert. Um die Ergebnisse der zweiten Seite abzurufen, verwenden Sie &quot;`page=1`&quot; als Parameter.

Verwenden Sie beispielsweise die folgende Anfrage, um die zweite Seite mit 500 Datensätzen aus einer Datensatzsuche abzurufen:

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

Alle paginierten Antworten enthalten einen strukturierten Umschlag, der angibt, ob weitere Ergebnisse verfügbar sind. Wenden Sie bei der Paginierung immer eine Sortierung an, um eine konsistente Sortierung über Seiten hinweg sicherzustellen.

>[!NOTE]
>
> **Version 1 Hinweis:** V1 verwendet `offset` und `limit` im Anfrageinhalt übergeben (standardmäßig 500, max. 2.000). Um die Datensätze 2001-4000 abzurufen, legen Sie im Anfragetext &quot;`offset`&quot; fest: &quot;`2000`&quot;, &quot;`limit`&quot;: &quot;`2000`&quot;. Die Antwort gibt ein flaches Datensatz-Array mit einem `totalCount` zurück.

## Massenvorgänge

Die Planning-API unterstützt das Massenerstellen, Aktualisieren, Patchen und Löschen von Datensätzen in einer einzigen Anfrage. Informationen zu Endpunktpfaden **Anfrageformaten und Datensatzbeschränkungen pro Vorgang finden Sie in** API-Referenz[&#128279;](https://developer.adobe.com/wf-planning) unter developer.adobe.com/wf-planning.

>[!NOTE]
>
>**Version 1 Hinweis:** Massenvorgänge sind in Version 1 nicht verfügbar.


## Berechtigungen

Berechtigungen für Entitäten werden über eine dedizierte Berechtigungs-API verwaltet, die von den Ressourcenendpunkten selbst getrennt ist. Auf diese Weise können Sie aktuelle Berechtigungen lesen, die Freigabeliste verwalten und Zugriffsanfragen unabhängig von Datenvorgängen verarbeiten. Weitere Informationen finden Sie im Abschnitt „API-Referenzen“ im Artikel [Workfront Planning API](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**Version 1 Hinweis:** Version 1 stellt keine API für öffentliche Berechtigungen bereit. Berechtigungsstufe wird direkt in Ressourcenantwort-DTOs eingebettet.

## Verwenden der Planning-API mit benutzerdefinierten Workfront-Formularen

Sie können die Planning-API über ein externes Suchfeld in einem benutzerdefinierten Workfront-Formular aufrufen, um Planungsdaten direkt in Workfront-Objekten einzublenden. Weitere Informationen finden Sie unter [Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Verwandte Ressourcen

Weitere Informationen zur API finden Sie in den folgenden Artikeln:

* [Workfront Planning API](https://developer.adobe.com/wf-planning) Entwicklerdokumentation und Referenz
* [Erste Schritte mit Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-overview.md)
* [Überblick über den Zugriff auf Adobe Workfront-Planung](/help/quicksilver/planning/access/access-overview.md)
* [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->