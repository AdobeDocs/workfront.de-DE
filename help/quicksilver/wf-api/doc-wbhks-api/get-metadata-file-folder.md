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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 2%

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
   <td>Die Kennung der Datei oder des Ordners, auf die der Webhook-Provider verweist. Dies unterscheidet sich von der Dokument-ID von Adobe Workfront. Um die Metadaten des Stammverzeichnisses abzurufen, verwenden Sie den Wert '/'.
   <p>Hinweis: Die maximale Länge der ID beträgt 255 Zeichen.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Reaktion

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
   <td>Zeichenfolge </td> 
   <td>Der Name des Dokuments oder Ordners</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>Zeichenfolge </td> 
   <td>Gibt an, ob es sich bei diesem Element um eine Datei oder einen Ordner handelt ('file' oder 'folder')</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Zeichenfolge </td> 
   <td>Die ID der Datei oder des Ordners.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Zeichenfolge </td> 
   <td> <p>Der URL-Pfad, der von einem Benutzer zum Anzeigen des Dokuments in einem Browserfenster verwendet wird. Die URL kann entweder vom Dokumentenanbieter oder vom nativen externen Speicheranbieter gehostet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Zeichenfolge </td> 
   <td> <p>Der URL-Pfad, den ein Benutzer zum Herunterladen des Dokuments in ein Browserfenster verwendet. Die URL kann entweder vom Dokumentenanbieter oder vom nativen externen Speicheranbieter gehostet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Zeichenfolge </td> 
   <td>Der MIME-Typ für die Datei. (optional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Zeichenfolge </td> 
   <td>Letzte Änderung dieser Datei (formatierter RFC 3339-Zeitstempel)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Lang</td> 
   <td> Die Größe der Datei in Byte. (optional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Boolesch</td> 
   <td> Gibt an, ob diese Datei oder dieser Ordner für den authentifizierten Benutzer schreibgeschützt ist.(optional) </td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"My Document",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"2014065T 17:39:45.251Z",<br>size: "32554694"<br></pre>

>[!NOTE]
>
>Die Fehlerbehandlung sollte für alle API-Aufrufe einheitlich sein. Weitere Informationen finden Sie unten im Abschnitt &quot;Umgang mit Fehlern&quot;.
