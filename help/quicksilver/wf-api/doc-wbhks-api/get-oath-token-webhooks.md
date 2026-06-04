---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Abrufen von OAuth2-Token
description: Abrufen von OAuth2-Token
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
TQID: https://experienceleague.adobe.com/dspQLWwqjYdo3y9Trqv70ylGd1hFE-ynJaBU7-xLyxg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 10%

---

# Abrufen von OAuth2-Token

## Abrufen von OAuth2-Token

Gibt das OAuth2-Aktualisierungs-Token und Zugriffs-Token für einen authentifizierten Benutzer zurück. Dieser wird einmal aufgerufen, wenn der Benutzer einen Dokumentanbieter bereitstellt. Nachfolgende Aufrufe erfolgen, um ein aktualisiertes Zugriffstoken abzurufen.

**URL**

POST /any/url

Die URL ist konfigurierbar und entspricht dem Token-Endpunkt-URL-Wert auf der Seite „Benutzerdefiniertes Integrations-Setup“.

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
   <td>ja</td>
   <td><p>Die Werte umfassen „authorization_code“ oder „refresh_token“. Der angegebene Wert gibt an, welcher der beiden Parameter an diesen API-Aufruf übergeben wird: code oder refresh_token.</p></td>
  </tr>
  <tr>
   <td>Code</td>
   <td>Depends</td>
   <td><p>Der Autorisierungs-Code wird an Adobe Workfront gesendet, unmittelbar nachdem der Benutzer auf die Schaltfläche „Gewähren“ geklickt hat. Dies ist nur erforderlich, wenn der Gewährungstyp „authorization_code“ ist. Der Autorisierungs-Code sollte kurzlebig sein und im Allgemeinen in 10 Minuten oder weniger ablaufen.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>Depends</td>
   <td><p>Dies ist nur erforderlich, wenn nachfolgende Aufrufe zum Abrufen eines neuen Zugriffs-Tokens erfolgen, da das vorherige Zugriffs-Token abgelaufen ist. Wenn Sie diesen Wert senden, setzen Sie den Parameter grant_type auf „refresh_token“.</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>ja</td>
   <td>Die in Workfront für diese benutzerdefinierte Integration konfigurierte Client-ID.</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>ja</td>
   <td> Der in Workfront für diese benutzerdefinierte Integration konfigurierte geheime Clientschlüssel.</td>
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
   <td>String</td>
   <td><p>Ein Token, das verwendet wird, um autorisierte API-Aufrufe im Namen des Benutzers durchzuführen. Dieser sollte ablaufen, um nicht autorisierte API-Aufrufe zu verhindern.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>String</td>
   <td><p>Ein langlebiges Token, mit dem ein neues Zugriffs-Token abgerufen wird, indem diese API-Methode aufgerufen wird.</p></td>
  </tr>
  <tr>
   <td>expires_in </td>
   <td>long</td>
   <td><p>(Optional) Die Zeit (in Sekunden), bevor das Zugriffs-Token abläuft, im Allgemeinen 3.600.</p></td>
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
