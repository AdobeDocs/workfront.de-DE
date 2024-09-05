---
content-type: api
navigation-topic: general-api
title: Ereignisabonnement-API
description: Ereignisabonnement-API
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: d92dc8581bef1f5fdbef7a853ac27ffc3fa7ddbe
workflow-type: tm+mt
source-wordcount: '2157'
ht-degree: 3%

---


# Ereignisabonnement-API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Wenn eine Aktion auf einem Adobe Workfront-Objekt erfolgt, das von Ereignisabonnements unterstützt wird, können Sie Workfront so konfigurieren, dass eine Antwort an den gewünschten Endpunkt gesendet wird. Das bedeutet, dass Anwendungen von Drittanbietern Aktualisierungen von Workfront-Interaktionen über die Workfront-API erhalten können, sobald sie auftreten. Im Allgemeinen erhalten Sie in weniger als 5 Sekunden nach der Protokollierung der Datenänderung Webhook-Benachrichtigungen. Kunden erhalten im Durchschnitt Webhook-Benachrichtigungen in weniger als einer Sekunde, nachdem die Datenänderung protokolliert wurde.  

Um Payloads von Ereignisanmeldungen über Ihre Firewall zu erhalten, müssen Sie die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzufügen:

**Für Kunden in Europa:**

* 52 30 133 50
* 52 208 159 124
* 54 220 93 204
* 52 17 130 201
* 34 254 76 122
* 34 252 250 191

**Für Kunden an anderen Standorten als Europa:**

* 54 244 142 219
* 44 241 82 96
* 52 36 154 34
* 34 211 224,9
* 54 218 48 56
* 52 39 217 230

Die folgenden Themen unterstützen die API für die Ereignisanmeldung:

## Von Ereignisanmeldungen unterstützte Objekte

Die folgenden Workfront-Objekte werden von Ereignisabonnements unterstützt.

* Zuweisung
* Firma
* Dashboard
* Dokument
* Ausgabe
* Feld
* Stunde
* Problem
* Notiz
* Portfolio
* Programm
* Projekt
* Datensatz
* Datensatztyp
* Bericht
* Aufgabe
* Vorlage
* Arbeitszeittabelle
* Benutzerin oder Benutzer
* Arbeitsbereich

Eine Liste der Felder, die von Ereignisabonnement-Objekten unterstützt werden, finden Sie unter [Ressourcenfelder für Ereignisabonnements](../../wf-api/api/event-sub-resource-fields.md).

## Ereignisabonnement-Authentifizierung

Um ein Ereignisabonnement zu erstellen, abzufragen oder zu löschen, benötigt Ihr Workfront-Benutzer Folgendes:

* Für die Verwendung von Ereignisanmeldungen ist eine Zugriffsstufe von &quot;Systemadministrator&quot;erforderlich.
* Zur Verwendung der API für Ereignisabonnements ist eine Kopfzeile vom Typ `sessionID` erforderlich.

  Weitere Informationen finden Sie unter [Authentifizierung](api-basics.md#authentication) in den [API-Grundlagen](api-basics.md).

## Erstellen der Abonnement-Ressource

Die Abonnement-Ressource enthält die folgenden Felder.

* objId (optional)

   * **String** - Die ID des Objekts des angegebenen objCode, für das Ereignisse ausgelöst werden. Wenn dieses Feld nicht angegeben ist, erhält der Benutzer Ereignisse für alle Objekte des angegebenen Typs.

* objCode (erforderlich)

   * **String** - Der objCode des Objekts, für das Änderungen abonniert werden. Die möglichen Werte für &quot;objCode&quot;sind in der folgenden Tabelle aufgeführt.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>Objekt</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">Zuweisung</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Firma </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Dashboard</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Dokument</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Ausgabe</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Feld</p></td> 
        <td scope="col"><p>FELD</p></td> 
       </tr> 
      <tr> 
        <td scope="col"><p>Stunde</p></td> 
        <td scope="col">HOUR</td> 
       </tr> 
       <tr> 
        <td scope="col">Problem</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Notiz</td> 
        <td scope="col">NOTIZ</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portfolio</p></td> 
        <td scope="col"><p>PORT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Programm</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Projekt</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Datensatz</p></td> 
        <td scope="col"><p>AUFZEICHNUNG</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Datensatztyp</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Bericht</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Aufgabe</p></td> 
        <td scope="col"><p>AUFGABE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Vorlage</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Arbeitszeittabelle</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">Benutzerin oder Benutzer</td> 
        <td scope="col">BENUTZER</td> 
       </tr> 
       <tr> 
        <td scope="col">Arbeitsbereich</td> 
        <td scope="col">WORKSPACE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (erforderlich)

   * **String** - Ein Wert, der den Ereignistyp darstellt, für den das Objekt abonniert wird. Zu den verfügbaren Ereignistypen gehören:

      * ERSTELLEN
      * DELETE 
      * AKTUALISIEREN

* url (erforderlich)

   * **String** - Die URL des Endpunkts, an den Abonnementereignis-Payloads über HTTP gesendet werden.

* authToken (erforderlich)

   * **String** - Das OAuth2-Träger-Token, das zur Authentifizierung mit der im Feld &quot;URL&quot;angegebenen URL verwendet wird. 

## Erstellen von API-Anfragen für Ereignisabonnements

Nachdem Sie sichergestellt haben, dass der Benutzer Administratorzugriff hat und die Abonnement-Ressource gebildet wurde, können Sie Ereignisabonnements erstellen.

Verwenden Sie die folgende Syntax, um die URL zu erstellen.

**Anforderungs-URL:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Anforderungsheader:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Kopfzeilenwert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Inhaltstyp</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID-Wert</p> </td> 
  </tr> 
 </tbody> 
</table>

**Beispiel für Anfragetext:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| Antwortcode | Beschreibung |
|---|---|
| 201 (Erstellt) | Das Ereignisabonnement wurde erfolgreich erstellt. |
| 400 (Bad Request) | Das URL-Feld der Abonnement-Ressource wurde als ungültig erachtet. |
| 401 (Nicht autorisiert) | Die bereitgestellte sessionID war leer oder wurde als ungültig eingestuft. |
| 403 (Verboten) | Der Benutzer, der mit der bereitgestellten sessionID übereinstimmt, hat keinen Administratorzugriff. |

Wenn Sie eine Abonnement-Ressource als Text einer Anfrage übergeben (der Inhaltstyp lautet &quot;application/json&quot;), wird ein Ereignisabonnement für das angegebene Objekt erstellt. Der Antwortcode 201 (Erstellt) zeigt an, dass das Abonnement erstellt wurde. Ein anderer Antwort-Code als 201 bedeutet, dass das Abonnement **NOT** erstellt wurde.

>[!NOTE]
>
> Der Antwortheader &quot;Ort&quot;enthält den URI des neu erstellten Ereignisabonnements.

Beispiel für **Antwortheader:**

| Antwortheader | Beispiel |
|---|---|
| Content-Length | `→0` |
| Datum | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Speicherort | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Server | `→Apache-Coyote/1.1` |

## Abfrage von Ereignisanmeldungen

Verwenden Sie beim Abfragen von Workfronts HTTP die GET-Methode. Es gibt zwei Möglichkeiten, um nach Abonnements für Ereignisse zu suchen: Abfrage nach Anmelde-ID (siehe unten) oder Abfrage aller Ereignisabonnationen.

### Abonnements für alle Ereignisse abfragen

Sie können alle Abonnements für Ereignisse eines Kunden abfragen oder die Antwort mit den folgenden Optionen verwalten. Sie können auch die folgenden Optionen verwenden, um die Antwort zu verwalten:

* **page**: Abfrageparameteroption zur Angabe der Anzahl der zurückzugebenden Seiten. Der Standardwert ist 1.
* **limit**: Abfrageparameteroption zur Angabe der Anzahl der pro Seite zurückzugebenden Ergebnisse. Der Standardwert ist 100 mit einer maximalen Anzahl von 1000.

Die Anforderungssyntax für die Auflistung aller Ereignisanmeldungen für einen bestimmten Kunden lautet wie folgt:

**Anforderungs-URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Anforderungsheader:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Kopfzeilenwert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID-Wert</p> </td> 
  </tr> 
 </tbody> 
</table>

**Antwortcodes:**

| Antwortcode | Beschreibung |
|---|---|
| 200 (OK) | Die Anfrage wurde mit allen für den Kunden gefundenen Ereignisabonnements zurückgegeben, die mit der bereitgestellten sessionID übereinstimmen. |
| 401 (Nicht autorisiert) | Die bereitgestellte sessionID war leer. |
| 403 (Verboten) | Der Benutzer, der mit der bereitgestellten sessionID übereinstimmt, hat keinen Administratorzugriff. |


Beispiel für **Antwortheader:**

| Antwortheader | Beispiel |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Datum | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Server | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


**Beispiel für Antworttext:**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

Wo

* **page** und **limit** sind die in der Anforderung angegebenen Werte oder die Standardwerte, wenn keine Werte angegeben werden
* **page_count** ist die Gesamtanzahl der Seiten, die abgefragt werden können.
* **total_count** ist die Gesamtzahl der Anmeldungen, die mit der Abfrage übereinstimmen.

### Abfrage nach Ereignisabonnement-ID

Sie können nach Ereignisabonnements anhand der ID des Ereignisabonnements abfragen. Die Anforderungssyntax für die Auflistung von Ereignisanmeldungen lautet wie folgt:

**Anforderungs-URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Anforderungsheader:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Kopfzeilenwert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID-Wert</p> </td> 
  </tr> 
 </tbody> 
</table>

**Antwortcodes:**

| Antwortcode | Beschreibung |
|---|---|
| 200 (OK) | Die zurückgegebene Anfrage mit dem Ereignisabonnement, das mit der angegebenen Anmelde-ID übereinstimmt. |
| 401 (Nicht autorisiert) | Die bereitgestellte sessionID war leer. |
| 403 (Verboten) | Der Benutzer, der mit der bereitgestellten sessionID übereinstimmt, hat keinen Administratorzugriff. |


**Beispiel für Antworttext:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## Filter für Ereignisabschlüsse

Die Filterung der Ereignisabonnements kann verwendet werden, um sicherzustellen, dass Sie nur relevante Nachrichten erhalten. Das Erstellen von Filtern für Ihre Abonnements kann die Anzahl der Nachrichten, die Ihr Endpunkt verbrauchen muss, erheblich verringern.

Beispielsweise kann ein Abonnement für ein Ereignis **UPDATE - TASK** nur dann auf Trigger gesetzt werden, wenn der **newState** einer Ereignis-Payload den **taskStatus** als **current** definiert.

>[!IMPORTANT]
>
>Die folgenden Attribute gelten für die Filterung der Ereignisabonnements

* Wenn ein Filterfeld einen nicht leeren Wert hat, werden nur Nachrichten mit dem Wert **newState** gesendet, die die Filterschlüssel und -werte enthalten.
* Sie können nach benutzerdefinierten Daten filtern, die im **newState** AND/OR **oldState** des Objekts enthalten sind
* Filter werden nur danach ausgewertet, ob sie einem bestimmten Wert entsprechen oder nicht
* Wenn Ihre Filtersyntax falsch ist oder mit den im **newState** der Payload enthaltenen Daten nicht übereinstimmt, wird keine Validierungsmeldung zurückgegeben, um anzuzeigen, dass ein Fehler aufgetreten ist
* Filter können nicht mit einem Abonnement aktualisiert werden, das bereits existiert. Ein neues Abonnement muss mit neuen Filterparametern erstellt werden.
* Mehrere Filter können auf ein Abonnement angewendet werden. Das Abonnement wird nur bereitgestellt, wenn alle Filterbedingungen erfüllt sind.
* Das Anwenden mehrerer Filter auf ein Abonnement entspricht der Verwendung eines logischen **AND** -Operators.
* Auf ein einzelnes Objekt können mehrere Ereignisabonnements angewendet werden, sofern mindestens ein Parameter für das Abonnementfeld für Ereignisse zwischen den einzelnen Ereignisabonnements unterschiedlich ist.
* Wenn einem einzelnen Objekt mehrere Ereignisabonnements zugewiesen sind, können alle mit diesem Objekt verknüpften Ereignisabonnements an einen einzelnen Endpunkt zurückgegeben werden. Diese Vorgehensweise kann als äquivalenter Ersatz für den logischen Operator **OR** verwendet werden, der nicht mithilfe von Filterparametern festgelegt werden kann.
* Die folgenden Felder können nicht gefiltert werden:

   * DOCU.groups
   * RECORD.data
   * RECORD_TYPE.data
   * RECORD_TYPE.fields

### Verwenden von Vergleichsoperatoren

Sie können ein Vergleichsfeld zusammen mit dem Filterfeld angeben. Verwenden Sie in diesem Feld einen Vergleichsoperator zum , um nach Vergleichsergebnissen zu filtern. Sie können beispielsweise ein UPDATE - TASK-Abonnement erstellen, das nur dann eine Payload sendet, wenn der Aufgabenstatus NICHT gleich aktuell ist. Sie können die folgenden Vergleichsoperatoren verwenden:

#### eq: equal

Mit diesem Filter können Nachrichten durchkommen, wenn die eingetretene Änderung genau mit `fieldValue` im Filter übereinstimmt. Beim Wert `fieldValue` wird zwischen Groß- und Kleinschreibung unterschieden.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne: nicht gleich

Mit diesem Filter können Nachrichten durchkommen, wenn die eingetretene Änderung nicht mit `fieldValue` im Filter genau übereinstimmt. Beim Wert `fieldValue` wird zwischen Groß- und Kleinschreibung unterschieden.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt: größer als

Dieser Filter ermöglicht das Durchkommen von Nachrichten, wenn die Aktualisierung des angegebenen `fieldName` größer ist als der Wert für `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### get: greater than or equal to

Dieser Filter ermöglicht das Durchkommen von Nachrichten, wenn die Aktualisierung des angegebenen `fieldName` größer oder gleich dem Wert für `fieldValue` ist.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt: kleiner als

Dieser Filter ermöglicht das Durchkommen von Nachrichten, wenn die Aktualisierung am angegebenen `fieldName` kleiner als der Wert für `fieldValue` ist.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte: kleiner oder gleich

Dieser Filter ermöglicht das Durchkommen von Nachrichten, wenn die Aktualisierung am angegebenen `fieldName` kleiner oder gleich dem Wert für `fieldValue` ist.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### enthält

Dieser Filter ermöglicht das Durchkommen von Nachrichten, wenn die aufgetretene Änderung den Wert `fieldValue` im Filter enthält. Beim Wert `fieldValue` wird zwischen Groß- und Kleinschreibung unterschieden

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### ändern

Dieser Filter ermöglicht es nur, dass Nachrichten durchkommen, wenn das angegebene Feld (`fieldName`) einen anderen Wert im alten und neuen Status aufweist. Wenn Sie andere Felder als das angegebene (`fieldName`) aktualisieren, wird diese Änderung nicht zurückgegeben.

>[!NOTE]
>
>`fieldValue` im Filterarray unten hat keine Auswirkungen.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### state

Durch diesen Connector wird der Filter auf den neuen Status oder den alten Status des erstellten oder aktualisierten Objekts angewendet. Dies ist hilfreich, wenn Sie wissen möchten, wo eine Änderung von etwas zu einem anderen vorgenommen wurde.
`oldState` ist bei CREATE `eventTypes` nicht möglich.

>[!NOTE]
>
>Das unten stehende Abonnement mit dem angegebenen Filter gibt nur Nachrichten zurück, in denen der Name der Aufgabe `again` für die `oldState` enthält, was vor einer Aktualisierung der Aufgabe war.
>Ein Anwendungsfall dafür wäre es, die objCode-Nachrichten zu finden, die sich von einer Sache zur anderen geändert haben. Um beispielsweise alle Aufgaben herauszufinden, die von &quot;Research Some name&quot;zu &quot;Research TeamName Some name&quot;geändert wurden

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### Connector-Felder verwenden

Im Feld `filterConnector` der Abonnement-Payload können Sie festlegen, wie die Filter angewendet werden sollen. Die Standardeinstellung ist &quot;AND&quot;, wobei die Filter alle `true` sein müssen, damit die Abonnementnachricht übermittelt wird. Wenn &quot;OR&quot;angegeben ist, muss nur ein Filter übereinstimmen, damit die Abonnementnachricht übermittelt wird.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## Löschen von Ereignisanmeldungen

Verwenden Sie beim Löschen von Workfronts HTTP die DELETE-Methode. Die Anforderungssyntax zum Löschen eines einzelnen Ereignisabonnements nach Anmelde-ID lautet wie folgt:

**Anforderungs-URL:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Anforderungsheader:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Kopfzeilenwert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID-Wert </p> </td> 
  </tr> 
 </tbody> 
</table>

**Antwortcodes:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Antwortcode</p> </th> 
   <th> Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (kein Inhalt)</td> 
   <td>Der Server entfernte erfolgreich das Ereignisabonnement, das mit der bereitgestellten subscriptionID übereinstimmt.</td> 
  </tr> 
  <tr> 
   <td>401 (Nicht autorisiert)</td> 
   <td>Die bereitgestellte sessionID war leer.</td> 
  </tr> 
  <tr> 
   <td>403 (Verboten)</td> 
   <td>Der Benutzer, der mit der bereitgestellten sessionID übereinstimmt, hat keinen Administratorzugriff.</td> 
  </tr> 
  <tr> 
   <td>404 (Nicht gefunden)</td> 
   <td>Der Server konnte kein Ereignisabonnement finden, das mit der zum Löschen bereitgestellten subscriptionID übereinstimmt.</td> 
  </tr> 
 </tbody> 
</table>

Beispiel für **Antwortheader:**

| Antwortheader | Beispiel |
|---|---|
| Datum | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Server | `→Apache-Coyote/1.1` |


**Beispiel für Antworttext:** nicht verfügbar

## Beispiele für Ereignis-Payloads

Die Payload, die ein Benutzer erhält, variiert je nach Objekttyp. Es gibt jedoch ein konsistentes Format, für das diese variierenden Payloads bereitgestellt werden.

Beispielsweise bleiben die folgenden Eigenschaften für alle Ereignis-Payloads konsistent:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Die in den Eigenschaften enthaltenen Werte sind zwar formatkonsistent, unterscheiden sich aber von Objekt zu Objekttyp.

Beispiele für Payloads für ein UPDATE-Ereignis und ein CREATE-Ereignis finden Sie unten. Beachten Sie im UPDATE-Beispiel, dass die Objekte oldState und newState identisch sind, während im CREATE-Beispiel das Objekt oldState leer ist (nicht NULL).

Im Folgenden finden Sie ein Beispiel für eine Payload für ein UPDATE-Ereignis:

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

Im Folgenden finden Sie eine Beispiel-Payload für ein CREATE-Ereignis:

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Basis-64-Kodierung

Wenn ein Abonnement für ein Ereignis aufgrund eines Konflikts zwischen Sonderzeichen in Ihren Ereignis-Abonnements und Ihren Netzwerkeinstellungen abgelehnt wird, können Sie die Base64-Kodierung verwenden, um Ihre Ereignis-Abonnements zu übermitteln. Base64 ist ein Satz von Kodierungs-Schemata, die beliebige Daten in ein ASCII-Zeichenfolgenformat übersetzen können. Es ist wichtig zu beachten, dass Base64 keine Form der Sicherheitsverschlüsselung ist.

### Basis-64-Kodierungsfeld

Das Feld base64Encoding ist ein optionales Feld, das verwendet wird, um die Base64-Kodierung von Payloads für Ereignisabonnements zu aktivieren. Der Standardwert ist false und die möglichen Werte sind: true, false und &quot;&quot; (leer).

### Beispiel einer Anfrage mit dem Feld base64Encoding

Wenn eine Anfrage mit dem base64Encoding -Feld auf true gestellt wird, werden die Objekte **newState** und **oldState** in der Payload als Basis-Kodierungs-Zeichenfolgen mit 64 Kodierungen bereitgestellt. Wenn das Feld base64Encoding auf false gesetzt, leer gelassen oder nicht in der Anfrage enthalten ist, wird die zurückgegebene Payload nicht in base 64 kodiert.

Im Folgenden finden Sie ein Beispiel für eine Anfrage, die das Feld base64Encoding verwendet:

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Beispiele für Antwort-Payloads in der Basis-64-Kodierung

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Veraltete Methode zur Abfrage aller Ereignisanmeldungen

Der folgende API-Endpunkt wird nicht mehr unterstützt und sollte nicht für neue Implementierungen verwendet werden. Wir empfehlen auch, alte Implementierungen in die -Methode im Abschnitt **Abfragefenster für Ereignisabonnements** zu überführen, wie oben beschrieben.

Sie können alle Ereignisabonnements für einen Kunden abfragen, wie durch den Wert sessionID angegeben. Die Anforderungssyntax für die Auflistung aller Ereignisanmeldungen für einen bestimmten Kunden lautet die folgende URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Anforderungsheader:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header Name</p> </th> 
   <th> <p>Kopfzeilenwert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID-Wert </p> </td> 
  </tr> 
 </tbody> 
</table>

**Antwortcodes:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Antwortcode</p> </th> 
   <th> Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (kein Inhalt)</td> 
   <td>Die Anfrage gab erfolgreich alle für den Benutzer gefundenen Ereignis-Abonnements zurück.</td> 
  </tr> 
  <tr> 
   <td>401 (Nicht autorisiert)</td> 
   <td>Die bereitgestellte sessionID war leer.</td> 
  </tr> 
  <tr> 
   <td>403 (Verboten)</td> 
   <td>Der Benutzer, der mit der bereitgestellten sessionID übereinstimmt, hat keinen Administratorzugriff.</td> 
  </tr> 
 </tbody> 
</table>

 

### Beispiel für Antworttext

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
