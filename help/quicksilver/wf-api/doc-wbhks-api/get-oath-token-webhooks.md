---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Abrufen von OAuth2-Token
description: Abrufen von OAuth2-Token
author: Becky
feature: Workfront API
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 4%

---


# Abrufen von OAuth2-Token

## Abrufen von OAuth2-Token

Gibt das OAuth2-Aktualisierungstoken und Zugriffstoken für einen authentifizierten Benutzer zurück. Dies wird einmal aufgerufen, wenn der Benutzer einen Dokumentanbieter bereitstellt. Nachfolgende Aufrufe werden durchgeführt, um ein aktualisiertes Zugriffstoken zu erhalten.

**URL**

POST /any/url

Die URL kann konfiguriert werden und entspricht dem URL-Wert des Token-Endpunkts auf der Setup-Seite der benutzerdefinierten Integration.

### Abfrageparameter

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Name</th>
   <th>Erforderlich</th>
   <th>Beschreibung</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>yes</td>
   <td><p>Zu den Werten gehören "authorization_code"oder "refresh_token". Der angegebene Wert gibt an, welcher der beiden Parameter an diesen API-Aufruf übergeben wird: Code oder refresh_token.</p></td>
  </tr>
  <tr>
   <td>code</td>
   <td>abhängig</td>
   <td><p>Der Autorisierungscode, der an Adobe Workfront gesendet wird, nachdem der Benutzer auf die Schaltfläche "Grant" geklickt hat. Dies ist nur erforderlich, wenn der Fördertyp "authorization_code"ist. Der Autorisierungscode sollte kurzlebig sein und in der Regel innerhalb von 10 Minuten oder weniger ablaufen.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>abhängig</td>
   <td><p>Dies ist nur erforderlich, wenn nachfolgende Aufrufe durchgeführt werden, um ein neues access_token abzurufen, da das vorherige access_token abgelaufen ist. Setzen Sie beim Senden dieses Werts den Parameter grant_type auf "refresh_token".</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>yes</td>
   <td>Die in Workfront für diese benutzerdefinierte Integration konfigurierte Client-ID.</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>yes</td>
   <td> Der Client Secret , der in Workfront für diese benutzerdefinierte Integration konfiguriert wurde.</td>
  </tr>
 </tbody>
</table>

 

## Antwort

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Name</th>
   <th>Typ </th>
   <th>Beschreibung</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>Zeichenfolge</td>
   <td><p>Ein Token, mit dem autorisierte API-Aufrufe im Namen des Benutzers durchgeführt werden. Dies sollte ablaufen, um nicht autorisierte API-Aufrufe zu verhindern.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>Zeichenfolge</td>
   <td><p>Ein langlebiges Token, das zum Abrufen eines neuen access_token durch Aufruf dieser API-Methode verwendet wird.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>long</td>
   <td><p>(optional) Die Zeit (in Sekunden) bis zum Ablauf des access_token (im Allgemeinen 3.600).</p></td>
  </tr>
 </tbody>
</table>

**Beispiel**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## Antwort

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
