---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Abrufen von Metadaten für eine Datei oder einen Ordner
description: Abrufen von Metadaten für eine Datei oder einen Ordner
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
TQID: https://experienceleague.adobe.com/H04UQeyhGw-FdXDwaRZs5PSXnN-YErVptHWn-78INYo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 17%

---

# Abrufen von Metadaten für eine Datei oder einen Ordner

Gibt Metadaten für die angegebene Datei oder den angegebenen Ordner zurück.

**URL**

GET /metadata?id=[document or folder ID]

## Abfrageparameter

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>Die ID der Datei oder des Ordners, auf die bzw. den der Webhook-Anbieter verweist. Dies unterscheidet sich von der Dokument-ID von Adobe Workfront. Um die Metadaten des Stammverzeichnisses abzurufen, verwenden Sie den Wert "/".
   <p>Hinweis: Die maximale Länge für die ID beträgt 255 Zeichen.</p></td> 
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
   <th>Name </th> 
   <th>Typ </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>String </td> 
   <td>Der Name des Dokuments oder Ordners</td> 
  </tr> 
  <tr> 
   <td>Art </td> 
   <td>String </td> 
   <td>Gibt an, ob es sich bei diesem Element um eine Datei oder einen Ordner ('Datei' oder 'Ordner') handelt</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String </td> 
   <td>Die ID der Datei oder des Ordners.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Zeichenfolge </td> 
   <td> <p>Der URL-Pfad, der von einem Benutzer zum Anzeigen des Dokuments in einem Browser-Fenster verwendet wird. Die URL kann entweder vom Dokumentanbieter oder vom nativen externen Speicheranbieter gehostet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Zeichenfolge </td> 
   <td> <p>Der URL-Pfad, der von einem Benutzer zum Herunterladen des Dokuments in einem Browser-Fenster verwendet wird. Die URL kann entweder vom Dokumentanbieter oder vom nativen externen Speicheranbieter gehostet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String </td> 
   <td>Der MIME-Typ für die Datei. (optional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String </td> 
   <td>Letzter Änderungszeitpunkt dieser Datei (formatierter RFC 3339-Zeitstempel)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Lang</td> 
   <td> Die Größe der Datei in Byte. (optional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Boolesch</td> 
   <td> Gibt an, ob diese Datei oder dieser Ordner für den authentifizierten Benutzer schreibgeschützt ist. (Optional) </td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:„Mein Dokument“,<br>kind:„file“<br>id“:„12345“,<br>viewLink:“https://www.acme.com/viewDocument?id=12345",<br>downloadLink:“https://www.acme.com/downloadDocument?id=12345",<br>mimeType:„image/png“,<br>dateModified:„20140605T17:39:45.251Z“,<br>size: „32554694“<br>}</pre>

>[!NOTE]
>
>Die Fehlerbehandlung sollte bei allen API-Aufrufen konsistent sein. Einzelheiten finden Sie im Abschnitt „Fehlerbehandlung“ weiter unten.
