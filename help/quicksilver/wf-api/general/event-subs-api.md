---
content-type: api
navigation-topic: general-api
title: Ereignisabonnement-API
description: Ereignisabonnement-API
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ZIuaLr4-N-g2ciqjiOtzrTpjz0GFpxcpb-KqdXc-Th0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 3146
ht-degree: 95%

---

# Ereignisabonnement-API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Wenn eine Aktion für ein Adobe Workfront-Objekt stattfindet, das von Ereignisabonnements unterstützt wird, können Sie Workfront so konfigurieren, dass eine Antwort an Ihren gewünschten Endpunkt gesendet wird. Dies bedeutet, dass Drittanbieteranwendungen Aktualisierungen von Workfront-Interaktionen bald nach ihrem Auftreten über die Workfront-API erhalten können. Im Allgemeinen können Sie davon ausgehen, dass Sie Webhook-Benachrichtigungen in weniger als 5 Sekunden nach der protokollierten Datenänderung erhalten. Im Durchschnitt erhalten Kundinnen und Kunden Webhook-Benachrichtigungen in weniger als 1 Sekunde, nachdem die Datenänderung protokolliert wurde.

Da Ereignisabonnements Daten an einen anderen Service senden, werden sie über Befehle und nicht über die Workfront-Anwendung verwaltet.

Um Payloads für Ereignisabonnements über Ihre Firewall zu erhalten, müssen Sie die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzufügen:

**Für Kundinnen und Kunden in Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Für Kundinnen und Kunden an anderen Standorten außerhalb von Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

Die folgenden Themen unterstützen die Ereignisabonnement-API:

## Von Ereignisabonnements unterstützte Objekte

Die folgenden Workfront-Objekte werden von Ereignisabonnements unterstützt.

* Genehmigung
* Genehmigungsphase
* Teilnehmerin oder Teilnehmer der Genehmigungsphase
* Zuweisung
* Firma
* Dashboard
* Dokument
* Dokumentversion
* Ausgabe
* Feld
* Stunde
* Problem
* Notiz
* Portfolio
* Programm
* Projekt
* Korrekturabzug-Genehmigung
* Eintrag
* Eintragstyp
* Bericht
* Personalplan
* Parameterwert für den Personalplan
* Personalplanressource
* Ressourcenattributwert für den Personalplan
* Ressourcenattributwert für den Personalplan festgelegt
* Ressourcenparameterwert für den Personalplan
* Aufgabe
* Vorlage
* Arbeitszeittabelle
* Benutzerin oder Benutzer
* Arbeitsbereich

>[!NOTE]
>
>Eine Liste der Felder, die von Ereignisabonnementobjekten unterstützt werden, finden Sie unter [Ressourcenfelder für Ereignisabonnements](../../wf-api/api/event-sub-resource-fields.md).

## Authentifizierung von Ereignisabonnements

Um ein Ereignisabonnement zu erstellen, abzufragen oder zu löschen, benötigen Benutzenden in Workfront Folgendes:

* Für die Verwendung von Ereignisabonnements ist die Zugriffsebene „Systemadmin“ erforderlich.
* Für die Verwendung der Ereignisabonnement-API ist ein `sessionID`-Header erforderlich

  Weitere Informationen finden Sie unter [Authentifizierung](api-basics.md#authentication) in [API-Grundlagen](api-basics.md).

## Vermeiden einer Überlastung von Ereignisabonnements

Der Ereignisabonnementdienst wurde entwickelt, um für alle Benutzenden eine zuverlässige Bereitstellung von Ereignissen zu gewährleisten. Damit dies sichergestellt wird, wurden Schutzmaßnahmen eingeführt, um eine übermäßige Ereignisproduktion durch eine einzelne Person zu verhindern, die potenziell die Service-Qualität für alle Benutzenden beeinträchtigen könnte. Daher kann es bei Benutzenden, die innerhalb eines kurzen Zeitraums zu viele Ereignisse mit hoher Rate produzieren, zu Sandboxing und zu Verzögerungen bei der Ereignisbereitstellung kommen.

## Bilden der Abonnementressource

Die Abonnementressource enthält die folgenden Felder.

* objId (optional)

   * **String**: Die ID des Objekts des angegebenen objCode, für das Ereignisse ausgelöst werden. Wenn dieses Feld nicht angegeben ist, erhält der Benutzer bzw. die Benutzerin Ereignisse für alle Objekte des angegebenen Typs.

* objCode (erforderlich)

   * **String**: Der objCode des Objekts, für das Änderungen abonniert sind. Die möglichen Werte für objCode sind in der folgenden Tabelle aufgeführt.

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
        <td scope="col">Genehmigung</td> 
        <td scope="col"><p>Genehmigung</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Genehmigungsphase</td> 
        <td scope="col"><p>approval_stage</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Teilnehmerin oder Teilnehmer der Genehmigungsphase</td> 
        <td scope="col"><p>approval_stage_participant</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Zuweisung</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Firma </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Dashboard</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Dokument</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Dokumentversion</p></td> 
        <td scope="col">DOCV </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Ausgabe</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Feld</p></td> 
        <td scope="col"><p>FIELD</p></td> 
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
        <td scope="col">HINWEIS</td> 
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
        <td scope="col"><p>Korrekturabzug-Genehmigung</p></td> 
        <td scope="col"><p>PRFAPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Eintrag</p></td> 
        <td scope="col"><p>RECORD</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Eintragstyp</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Bericht</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Personalplan</p></td> 
        <td scope="col"><p>STAFFP</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Parameterwert für den Personalplan</p></td> 
        <td scope="col"><p>SPVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Personalplanressource</p></td> 
        <td scope="col"><p>STAFFR</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Ressourcenattributwert für den Personalplan</p></td> 
        <td scope="col"><p>SPAVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Ressourcenattributwert für den Personalplan festgelegt</p></td> 
        <td scope="col"><p>SAVSET</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Ressourcenparameterwert für den Personalplan</p></td> 
        <td scope="col"><p>SRPVAL</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Aufgabe</p></td> 
        <td scope="col"><p>TASK</p></td> 
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
        <td scope="col">USER</td> 
       </tr> 
       <tr> 
        <td scope="col">Arbeitsbereich</td> 
        <td scope="col">WORKSPACE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (erforderlich)

   * **String**: Ein Wert, der den Ereignistyp darstellt, den das Objekt abonniert hat. Zu den verfügbaren Ereignistypen gehören:

      * CREATE
      * LÖSCHEN
      * AKTUALISIEREN

* URL (erforderlich)

   * **String**: Die URL des Endpunkts, an den Payloads von Abonnementereignissen über HTTP gesendet werden.

* authToken (erforderlich)

   * **String**: Das OAuth2-Bearer-Token, das zur Authentifizierung mit der im Feld „URL“ angegebenen URL verwendet wird.

## Erstellen von API-Anfragen für Ereignisabonnements

Nachdem Sie sichergestellt haben, dass der Benutzer bzw. die Benutzerin Administratorzugriff hat, und die Abonnementressource gebildet haben, können Sie Ereignisabonnements erstellen.

Verwenden Sie die folgende Syntax, um die URL zu erstellen.

**Anfrage-URL**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Anfrage-Header**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header-Name</p> </th> 
   <th> <p>Header-Wert</p> </th> 
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

**Beispiel für den Anfragetext:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

**Beispiel für den Antworttext**

```
{
    "id": <NEW SUBSCRIPTION ID>,
    "version": <NEW SUBSCRIPTION VERSION>
}
```

| Antwort-Code | Beschreibung |
|---|---|
| 201 (Erstellt) | Das Ereignisabonnement wurde erfolgreich erstellt. |
| 400 (Fehlerhafte Anfrage) | Das URL-Feld der Abonnementressource wurde als ungültig eingestuft. |
| 401 (Nicht autorisiert) | Die angegebene sessionID war leer oder ungültig. |
| 403 (Verboten) | Der Benutzer bzw. die Benutzerin, der bzw. die mit der angegebenen Sitzungs-ID übereinstimmt, hat keinen Administratorzugriff. |

Das Übergeben einer Abonnementressource als Hauptteil einer Anfrage (wobei der Inhaltstyp „application/json“ ist) führt dazu, dass ein Ereignisabonnement für das angegebene Objekt erstellt wird. Der Antwort-Code 201 (Erstellt) gibt an, dass das Abonnement erstellt wurde. Ein anderer Antwort-Code als 201 bedeutet, dass das Abonnement **NICHT** erstellt wurde.

>[!NOTE]
>
> Der Antwort-Header „Standort“ enthält den URI des neu erstellten Ereignisabonnements.

**Beispiel für Antwort-Header:**

| Antwort-Header | Beispiel |
|---|---|
| Content-Length | `→0` |
| Datum | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Standort | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Server | `→Apache-Coyote/1.1` |

## Abfrage von Ereignisabonnements

Verwenden Sie bei HTTP-Abfragen in Workfront die GET-Methode. Es gibt zwei Möglichkeiten, Ereignisabonnements abzufragen: Abfrage nach Abonnement-ID (siehe unten) oder Abfrage aller Ereignisabonnements.

### Abfrage aller Ereignisabonnements

Sie können alle Ereignisabonnements für eine Kundin oder einen Kunden abfragen oder Folgendes verwenden, um die Antwort zu verwalten. Sie können auch die folgenden Optionen verwenden, um die Antwort zu verwalten:

* **page**: Abfrageparameteroption zum Angeben der Anzahl der zurückzugebenden Seiten. Der Standardwert ist 1.
* **limit**: Abfrageparameteroption zum Angeben der pro Seite zurückzugebenden Ergebnisse. Der Standardwert ist 100 mit einem Maximum von 1.000.

Die Anfragesyntax zur Auflistung aller Ereignisabonnements für einen bestimmten Kunden bzw. eine bestimmte Kundin lautet wie folgt:

**Anfrage-URL**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Anfrage-Header:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header-Name</p> </th> 
   <th> <p>Header-Wert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID-Wert</p> </td> 
  </tr> 
 </tbody> 
</table>

**Antwort-Codes**

| Antwort-Code | Beschreibung |
|---|---|
| 200 (OK) | Die Anfrage wurde mit allen für den Kunden bzw. die Kundin gefundenen Ereignisabonnements zurückgegeben, die mit der angegebenen sessionID übereinstimmen. |
| 401 (Nicht autorisiert) | Die angegebene sessionID war leer. |
| 403 (Verboten) | Der Benutzer bzw. die Benutzerin, der bzw. die mit der angegebenen sessionID übereinstimmt, hat keinen Administratorzugriff. |


**Beispiel für Antwort-Header**

| Antwort-Header | Beispiel |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Datum | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Server | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


**Beispiel für einen Antworttext**

```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```

Wo

* **page** und **limit** sind die in der Anfrage angegebenen Werte oder der Standardwert, wenn keine Werte angegeben werden
* **page_count** ist die Gesamtzahl der Seiten, die abgefragt werden können.
* **total_count** ist die Gesamtzahl der Abonnements, die der Abfrage entsprechen.

### Abfrage nach Ereignisabonnement-ID

Sie können Ereignisabonnements über die ID des Ereignisabonnements abfragen. Die Anfragesyntax für die Auflistung von Ereignisabonnements sieht wie folgt aus:

**Anfrage-URL**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Anfrage-Header**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header-Name</p> </th> 
   <th> <p>Header-Wert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID-Wert</p> </td> 
  </tr> 
 </tbody> 
</table>

**Antwort-Codes**

| Antwort-Code | Beschreibung |
|---|---|
| 200 (OK) | Die Anfrage, die mit dem Ereignisabonnement zurückgegeben wird, das der angegebenen Abonnement-ID entspricht. |
| 401 (Nicht autorisiert) | Die angegebene sessionID war leer. |
| 403 (Verboten) | Der Benutzer bzw. die Benutzerin, der bzw. die mit der angegebenen sessionID übereinstimmt, hat keinen Administratorzugriff. |


**Beispiel für einen Antworttext**



```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```


## Versionierung von Ereignisabonnements

Workfront verfügt über zwei Versionen von Ereignisabonnements.

Durch die Möglichkeit, Ereignisabonnements zu aktualisieren oder herabzustufen, wird sichergestellt, dass bei Änderungen an der Struktur von Ereignissen bestehende Abonnements nicht unterbrochen werden. So können Sie ohne Unterbrechung Ihres Ereignisabonnements die neue Version testen.

Weitere Informationen zur Versionierung von Ereignisabonnements, einschließlich spezifischer Unterschiede zwischen der Version und wichtigen Termine, finden Sie unter [Versionierung von Ereignisabonnements](/help/quicksilver/wf-api/general/event-subs-versioning.md).

>[!NOTE]
>
>Wenn Sie Ihr Ereignisabonnement auf eine andere Version aktualisieren oder herabstufen, erhalten Sie für jede Ereigniszustellung während eines Zeitfensters von fünf Minuten nach der Versionsänderung doppelte Ereignisse. Die Duplikate enthalten je eines der Ereignisabonnements, Version 1 und Version 2. Dadurch wird sichergestellt, dass Sie keine Ereignisse aufgrund einer Änderung der Version des Ereignisabonnements verpassen.

### Änderung einer einzelnen Abonnementversion

Die Anfragesyntax zum Ändern der Version für ein einzelnes Abonnement lautet:

**Anfrage-URL**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>/version 
```

**Beispiel für Anfragetext**

```
{
    "version": "v2" 
}
```


**Beispiel für Antworttext (200)**

```
{
    "id": <SUBSCRIPTION ID>,
    "version": "v2" 
}
```

**Mögliche Antwort-Codes**

* 200
* 400
* 404


### Änderung mehrerer Abonnementversionen

Dieser Endpunkt ändert die Version mehrerer Abonnements anhand einer Liste von Abonnements oder einer Hervorhebung für alle Abonnements des Kunden bzw. der Kundin.

Die Anfragesyntax zum Ändern der Version für ein einzelnes Abonnement lautet:

**Anfrage-URL**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/version
```

**Beispiel für Anfragetexte**

* Anfragetext für Liste mit Abonnements

  ```
  {
      "subscriptionIds": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>],
      "version": "v2" 
  }
  ```

* Anfragetext für alle Abonnements eines Kunden bzw. einer Kundin

  ```
  {
      "allCustomerSubscriptions": true,
      "version": "v2" 
  }
  ```

**Beispiel für Antworttext (200)**

```
{
    "subscription_ids": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>, ...],
    "version": "v2" 
}
```

**Mögliche Antwort-Codes**

* 200
* 400

## Filtern von Ereignisabonnements

Durch das Filtern von Ereignisabonnements können Sie sicherstellen, dass Sie nur relevante Nachrichten erhalten. Durch das Erstellen von Filtern für Ihre Abonnements kann die Anzahl der Nachrichten, die Ihr Endpunkt verarbeiten muss, erheblich verringert werden.

Beispielsweise kann ein Ereignisabonnement des Typs **UPDATE – TASK** so eingerichtet werden, dass es nur dann ausgelöst wird, wenn der **newState** einer Ereignis-Payload den **taskStatus** als **aktuell** definiert.

>[!IMPORTANT]
>
>Die folgenden Attribute gelten für die Filterung von Ereignisabonnements

* Wenn ein Filterfeld einen nicht leeren Wert aufweist, werden nur Nachrichten mit einem **newState**, der die Filterschlüssel und -werte enthält, an die abonnierte URL gesendet
* Sie können nach benutzerdefinierten Daten filtern, die im **newState** UND/ODER **oldState** des Objekts enthalten sind
* Filter werden nur danach bewertet, ob sie einem bestimmten Wert entsprechen oder nicht
* Wenn Ihre Filtersyntax falsch ist oder nicht mit den Daten im **newState** der Payload übereinstimmt, wird keine Validierungsmeldung zurückgegeben, die darauf hinweist, dass ein Fehler aufgetreten ist
* Filter können nicht für ein Abonnement aktualisiert werden, das bereits vorhanden ist. Es muss ein neues Abonnement mit neuen Filterparametern erstellt werden.
* Auf ein einzelnes Abonnement können mehrere Filter angewendet werden. Das Abonnement wird nur bereitgestellt, wenn alle Filterbedingungen erfüllt sind.
* Das Anwenden mehrerer Filter auf ein einzelnes Abonnement entspricht der Verwendung des logischen Operators **UND**.
* Auf ein einzelnes Objekt können mehrere Ereignisabonnements angewendet werden, solange sich mindestens ein Feldparameter der Ereignisabonnements bei den einzelnen Ereignisabonnements unterscheidet.
* Wenn einem einzelnen Objekt mehrere Ereignisabonnements zugewiesen sind, können alle mit diesem Objekt verknüpften Ereignisabonnements an einen einzelnen Endpunkt zurückgegeben werden. Diese Vorgehensweise kann als gleichwertiger Ersatz für den logischen Operator **ODER** verwendet werden, der nicht mit Filterparametern festgelegt werden kann.
* Die folgenden Felder können nicht gefiltert werden:

   * DOCU.groups
   * RECORD.data
   * RECORD_TYPE.data
   * RECORD_TYPE.fields

### Verwenden von Vergleichsoperatoren

Sie können ein Vergleichsfeld zusammen mit dem Filterfeld angeben. Verwenden Sie in diesem Feld einen Vergleichsoperator, um nach Vergleichsergebnissen zu filtern. Sie können beispielsweise ein Abonnement für UPDATE – TASK erstellen, das nur dann eine Payload sendet, wenn der Aufgabenstatus NICHT gleich dem aktuellen Status ist. Sie können den folgenden Vergleichsoperator verwenden:

#### eq: equal

Dieser Filter ermöglicht den Empfang von Nachrichten, wenn die Änderung genau mit dem `fieldValue` im Filter übereinstimmt. Der Wert von `fieldValue` unterliegt der Groß-/Kleinschreibung.

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

#### ne: not equal

Dieser Filter ermöglicht den Empfang von Nachrichten, wenn die Änderung nicht genau mit dem `fieldValue` im Filter übereinstimmt. Der Wert von `fieldValue` unterliegt der Groß-/Kleinschreibung.

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

#### gt: greater than

Dieser Filter ermöglicht den Empfang von Nachrichten, wenn die Aktualisierung für den angegebenen `fieldName` größer als der Wert für `fieldValue` ist.

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

#### gte: greater than or equal to

Dieser Filter ermöglicht den Empfang von Nachrichten, wenn die Aktualisierung für den angegebenen `fieldName` größer oder gleich dem Wert für `fieldValue` ist.

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

#### lt: less than

Dieser Filter ermöglicht den Empfang von Nachrichten, wenn die Aktualisierung für den angegebenen `fieldName` kleiner als der Wert für `fieldValue` ist.

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

#### lte: less than or equal to

Dieser Filter ermöglicht den Empfang von Nachrichten, wenn die Aktualisierung des angegebenen `fieldName` kleiner oder gleich dem Wert für `fieldValue` ist.

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

#### contains

Dieser Filter ermöglicht den Empfang von Nachrichten, wenn die Änderung den `fieldValue` im Filter enthält. Der Wert von `fieldValue` unterliegt der Groß-/Kleinschreibung

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

#### containsOnly

Dieser Filter ermöglicht den Empfang von Nachrichten nur dann, wenn der vollständige Satz ausgewählter Werte genau mit dem fieldValue im Filter übereinstimmt, unabhängig von der Reihenfolge. Es dürfen keine zusätzlichen oder fehlenden Werte vorhanden sein.

>[!NOTE]
>
>Dies wird für Felder vom Typ Array (Mehrfachauswahl) verwendet. Dieses Beispielabonnement ermöglicht den Empfang von Nachrichten nur dann, wenn das Feld `groups` genau „Choice 3“ und „Choice 4“ enthält, ohne zusätzliche oder fehlende Werte und unabhängig von der Reihenfolge. Wenn eine Zeichenfolge oder eine Ganzzahl in `fieldValue` statt in einem Array angegeben wird, ermöglicht das Abonnement den Empfang von Nachrichten nur dann, wenn das Feld `groups` genau eine Option enthält und diese Option genau mit der in `fieldValue` angegebenen Zeichenfolge oder Ganzzahl übereinstimmt.


```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": [
                "Choice 3",
                "Choice 4"
            ],
            "state": "newState",
            "comparison": "containsOnly"
        }
    ]
}
```

#### notContains

Dieser Filter ermöglicht den Empfang von Nachrichten nur dann, wenn das angegebene Feld (`fieldName`) den angegebenen Wert (`fieldValue`) nicht enthält.

>[!NOTE]
>
>Dies wird für Felder vom Typ Array (Mehrfachauswahl) oder Zeichenfolge verwendet. Wenn das Feld eine Zeichenfolge ist, überprüfen wir, ob der angegebene Wert nicht in der Zeichenfolge enthalten ist (z. B. ist „Neu“ nicht in der Zeichenfolge „Projekt - Aktualisiert“ enthalten). Wenn das Feld ein Array ist und der angegebene Feldwert eine Zeichenfolge oder eine Ganzzahl ist, überprüfen wir, ob das Array den angegebenen Wert nicht enthält (z. B. „Auswahl 1“ nicht in [ „Auswahl 2“, „Auswahl 3“]). Das folgende Beispielabonnement ermöglicht den Empfang von Nachrichten nur dann, wenn die `groups`-Felder die Zeichenfolge „Gruppe 2“ nicht enthalten.

```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": "Group 2",
            "state": "newState",
            "comparison": "notContains"
        }
    ]
}
```

#### change

Dieser Filter ermöglicht den Empfang von Nachrichten nur dann, wenn das angegebene Feld (`fieldName`) in „oldState“ und „newState“ einen unterschiedlichen Wert aufweist. Durch die Aktualisierung anderer Felder neben dem angegebenen (`fieldName`) wird diese Änderung nicht zurückgegeben.

>[!NOTE]
>
>`fieldValue` im folgenden Filter-Array hat keine Auswirkungen.

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

Dieser Connector bewirkt, dass der Filter auf den neuen oder alten Status des Objekts angewendet wird, das erstellt oder aktualisiert wurde. Dies ist hilfreich, wenn Sie wissen möchten, wo eine Änderung von einer Sache zur anderen vorgenommen wurde.
`oldState` ist auf CREATE `eventTypes` nicht möglich.

>[!NOTE]
>
>Das Abonnement unten mit dem angegebenen Filter gibt nur Nachrichten zurück, bei denen der Name der Aufgabe `again` auf dem `oldState` enthält, wie er war, bevor eine Aktualisierung für die Aufgabe durchgeführt wurde.
>Ein Anwendungsfall hierfür wäre, die objCode-Nachrichten zu finden, die sich von einer Sache zur anderen geändert haben. So können Sie beispielsweise alle Aufgaben ermitteln, die von „Research Some name“ in „Research TeamName Some name“ geändert wurden

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

### Verwenden verschachtelter Filter

Das Ereignisabonnement unterstützt das Filtern verschachtelter Ereignisfelder mithilfe der verschachtelten Feldnamen. Um beispielsweise eine Nachricht zu filtern, bei der `newState.data.customField1 = 'myCustomFieldValue'` ist, kann das folgende Abonnement mit dem Filter erstellt werden:

```
{
    "objCode": "RECORD",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedRecords",
    "filters": [
        {
            "fieldName": "data",
            "fieldValue": {
                    "customField1": "myCustomFieldValue"
            },
            "comparison": "eq",
            "state": "newState"
        }
    ]
}
```

Doppelt verschachtelte Filter können ebenfalls adressiert werden.

```
"filters": [
    {
        "fieldName": "data",
        "fieldValue": {
            "fields": {
                "children": {
                    "customerId":"customer1234",
                    "name":"New Campaign"
                }
            }
        },
        "comparison": "eq",
        "state": "newState"
    }
],
"filterConnector": 'AND'
```


#### Leistung und Limits

So stellen Sie konsistente Leistung und Wartungsfreundlichkeit sicher:

* Jedes Abonnement unterstützt bis zu 10 Filtergruppen (wobei jede Gruppe mehrere Filter enthält).
* Jede Filtergruppe kann bis zu 5 Filter enthalten, um eine potenzielle Leistungsbeeinträchtigung während der Ereignisverarbeitung zu verhindern.
* Es werden bis zu 10 Filtergruppen (mit jeweils 5 Filtern) unterstützt. Beachten Sie jedoch, dass eine große Anzahl aktiver Abonnements mit komplexer Filterlogik zu einer Verzögerung bei der Ereignisauswertung führen kann.

Wenn Sie diese Beschränkungen überschreiten, sollten Sie Ihre Logik vereinfachen oder das Abonnement in mehrere kleinere aufteilen.

### Verwenden von Connector-Feldern

Im Feld `filterConnector` in der Abonnement-Payload können Sie auswählen, wie die Filter angewendet werden sollen. Der Standardwert ist „UND“, wobei die Filter alle `true` sein müssen, damit die Abonnementnachricht empfangen werden kann. Wenn „ODER“ angegeben ist, muss nur ein Filter übereinstimmen, damit die Abonnementnachricht empfangen werden kann.

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

### Verwenden von Filtergruppen

Mit Filtergruppen können Sie verschachtelte logische (UND/ODER) Bedingungen in Ihren Filtern für Ereignisabonnements erstellen.

Jede Filtergruppe kann Folgendes enthalten:

* Einen eigenen Connector (UND oder ODER).
* Mehrere Filter, die jeweils dieselbe Syntax und dasselbe Verhalten aufweisen wie eigenständige Filter.

>[!IMPORTANT]
>
>Eine Gruppe muss mindestens zwei Filter haben.


Alle Filter innerhalb einer Gruppe unterstützen Folgendes:

* Vergleichsoperatoren: eq, ne, gt, get, lt, lte, contains, notContains, containsOnly, changed.
* Statusoptionen: newState, oldState.
* Feld-Targeting: beliebiger gültiger Objektfeldname.

```
{
  "objCode": "TASK",
  "eventType": "UPDATE",
  "authToken": "token",
  "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
  "filters": [
    {
      "fieldName": "percentComplete",
      "fieldValue": "100",
      "comparison": "lt"
    },
    {
      "type": "group",
      "connector": "OR",
      "filters": [
        {
          "fieldName": "status",
          "fieldValue": "CUR",
          "comparison": "eq"
        },
        {
          "fieldName": "priority",
          "fieldValue": "1",
          "comparison": "eq"
        }
      ]
    }
  ],
  "filterConnector": "AND"
}
```

Das obige Beispiel enthält die folgenden Komponenten:

1. Den Filter der obersten Ebene (außerhalb der Gruppe):

   * `{ "fieldName": "percentComplete", "fieldValue": "100", "comparison": "lt" }`
   * Dieser Filter prüft, ob das Feld „percentComplete“ der aktualisierten Aufgabe kleiner als 100 ist.

1. Filtergruppe (verschachtelte Filter mit ODER):

   * `{ "type": "group", "connector": "OR", "filters": [ { "fieldName": "status", "fieldValue": "CUR", "comparison": "eq" }, { "fieldName": "priority", "fieldValue": "1", "comparison": "eq" } ] }`
   * Bei dieser Gruppe werden zwei interne Filter ausgewertet:

      * Der erste prüft, ob der Aufgabenstatus „CUR“ (aktuell) entspricht.
      * Der zweite prüft, ob die Priorität gleich „1“ (hohe Priorität) ist.
   * Da der Connector „ODER“ ist, wird diese Gruppe übergeben, wenn eine der Bedingungen erfüllt ist.

1. Connector der obersten Ebene (filterConnector: UND):
   * Der äußerste Connector zwischen den Filtern der obersten Ebene ist „UND“. Das bedeutet, dass sowohl der Filter der obersten Ebene als auch die Gruppe übergeben müssen, damit das Ereignis übereinstimmt.

1. Das Abonnement wird ausgelöst, wenn die folgenden Bedingungen erfüllt sind:
   * percentComplete ist kleiner als 100.
   * Entweder ist der Status „CUR“ oder die Priorität ist „1“.

>[!NOTE]
>
>Es gibt Beschränkungen, um bei der Verwendung von Filtergruppen eine konsistente Systemleistung sicherzustellen, darunter die folgenden:
>
>* Jedes Abonnement unterstützt bis zu 10 Filtergruppen (wobei jede Gruppe mehrere Filter enthält).
>* Jede Filtergruppe kann bis zu 5 Filter enthalten, um eine potenzielle Leistungsbeeinträchtigung während der Ereignisverarbeitung zu verhindern.
>* Es werden zwar bis zu 10 Filtergruppen (mit jeweils 5 Filtern) unterstützt, eine große Anzahl aktiver Abonnements mit komplexer Filterlogik kann jedoch zu einer Verzögerung bei der Ereignisauswertung führen.

## Löschen von Ereignisabonnements

Verwenden Sie beim Löschen von HTTP in Workfront die DELETE-Methode. Die Anfragesyntax zum Löschen eines einzelnen Ereignisabonnements nach Abonnement-ID lautet wie folgt:

**Anfrage-URL:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Anfrage-Header:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header-Name</p> </th> 
   <th> <p>Header-Wert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID-Wert </p> </td> 
  </tr> 
 </tbody> 
</table>

**Antwort-Codes:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Antwort-Code</p> </th> 
   <th> Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (kein Inhalt)</td> 
   <td>Der Server hat das Ereignisabonnement, das der angegebenen subscriptionID entspricht, erfolgreich entfernt.</td> 
  </tr> 
  <tr> 
   <td>401 (Nicht autorisiert)</td> 
   <td>Die angegebene sessionID war leer.</td> 
  </tr> 
  <tr> 
   <td>403 (Verboten)</td> 
   <td>Der Benutzer bzw. die Benutzerin, der bzw. die mit der angegebenen Sitzungs-ID übereinstimmt, hat keinen Administratorzugriff.</td> 
  </tr> 
  <tr> 
   <td>404 (Nicht gefunden)</td> 
   <td>Der Server konnte kein Ereignisabonnement finden, das der zum Löschen angegebenen subscriptionID entspricht.</td> 
  </tr> 
 </tbody> 
</table>

**Beispiel für Antwort-Header:**

| Antwort-Header | Beispiel |
|---|---|
| Datum | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Server | `→Apache-Coyote/1.1` |


**Beispiel für Antworttext:** Nicht zutreffend

## Beispiele für Ereignis-Payloads

Die Payload, die ein Benutzer bzw. eine Benutzerin erhält, hängt vom Objekttyp ab. Es gibt jedoch ein konsistentes Format, für das diese unterschiedlichen Payloads bereitgestellt werden.

Beispielsweise bleiben die folgenden Eigenschaften über alle Ereignis-Payloads hinweg konsistent:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Die in den Eigenschaften enthaltenen Werte variieren zwischen verschiedenen Objekten und Objekttypen, auch wenn sie im Format konsistent sind.

Nachfolgend finden Sie Beispiele für Payloads für ein UPDATE-Ereignis und ein CREATE-Ereignis. Beachten Sie, dass im UPDATE-Beispiel die Objekte „oldState“ und „newState“ identisch sind, während im CREATE-Beispiel das Objekt „oldState“ leer ist (nicht NULL).

Im Folgenden finden Sie eine Beispiel-Payload für ein UPDATE-Ereignis:

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "eventVersion": "v2",
                   "subscriptionVersion": "v2",
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
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
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

## Base 64-Codierung

Wenn ein Ereignisabonnement aufgrund eines Konflikts zwischen in Ihren Ereignisabonnements enthaltenen Sonderzeichen und Ihren Netzwerkeinstellungen abgelehnt wird, können Sie die Base64-Codierung verwenden, um Ihre Ereignisabonnements zu übergeben. Bei Base64 handelt es sich um ein Set von Codierungsschemata, die beliebige Daten in ein ASCII-Zeichenfolgenformat übersetzen können. Beachten Sie, dass Base64 keine Form der Sicherheitsverschlüsselung ist.

### Feld „base64Encoding“

Das Feld „base64Encoding“ ist ein optionales Feld, das verwendet wird, um die Base64-Codierung von Payloads für Ereignisabonnements zu aktivieren. Der Standardwert ist „false“ und die möglichen Werte sind „true“, „false“ und „ “ (leer).

### Beispiel für eine Anfrage mit dem Feld „base64Encoding“

Wenn eine Anfrage mit dem Feld „base64Encoding“ gestellt wird, das auf „true“ gesetzt ist, werden die Objekte **newState** und **oldState** in der Payload als Base64-Codierungszeichenfolgen bereitgestellt. Wenn das Feld „base64Encoding“ auf „false“ gesetzt ist, leer gelassen wird oder nicht in der Anfrage enthalten ist, wird die zurückgegebene Payload nicht in Base 64 codiert.

Im Folgenden finden Sie ein Beispiel für eine Anfrage, bei der das Feld „base64Encoding“ verwendet wird:

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

### Beispiele für Antwort-Payloads in Base 64-Codierung

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Veraltete Methode zum Abfragen aller Ereignisabonnements

Der folgende API-Endpunkt ist veraltet und sollte nicht für neue Implementierungen verwendet werden. Wir empfehlen auch, alte Implementierungen auf die oben im Abschnitt **Abfragen von Ereignisabonnements** beschriebene Methode umzustellen.

Sie können alle Ereignisabonnements für eine Kundin oder einen Kunden abfragen, wie durch den Wert „sessionID“ angegeben. Die Syntax der Anfragen zum Auflisten aller Ereignisabonnements für einen bestimmten Kunden bzw. eine bestimmte Kundin ist die folgende URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Anfrage-Header:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Header-Name</p> </th> 
   <th> <p>Header-Wert</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID-Wert </p> </td> 
  </tr> 
 </tbody> 
</table>

**Antwort-Codes:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Antwort-Code</p> </th> 
   <th> Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (kein Inhalt)</td> 
   <td>Die Anfrage hat erfolgreich alle für den Benutzer bzw. die Benutzerin gefundenen Ereignisabonnements zurückgegeben.</td> 
  </tr> 
  <tr> 
   <td>401 (Nicht autorisiert)</td> 
   <td>Die angegebene sessionID war leer.</td> 
  </tr> 
  <tr> 
   <td>403 (Verboten)</td> 
   <td>Der Benutzer bzw. die Benutzerin, der bzw. die mit der angegebenen sessionID übereinstimmt, hat keinen Administratorzugriff.</td> 
  </tr> 
 </tbody> 
</table>



### Beispiel für einen Antworttext

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
