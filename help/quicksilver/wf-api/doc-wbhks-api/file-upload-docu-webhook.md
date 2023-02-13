---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Datei-Upload über Document Webhooks
description: Datei-Upload über Document Webhooks
author: John
feature: Workfront API
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: b117eb11e4e9325e6249687448d3de98a11e5e00
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%

---


# Datei-Upload über Document Webhooks

Das Hochladen einer Datei in einen Dokumentenspeicheranbieter ist ein zweistufiger Prozess, der zwei separate API-Endpunkte erfordert. Adobe Workfront startet den Upload-Prozess durch Aufruf von /uploadInit . Dieser Endpunkt gibt eine Dokument-ID zurück, die beim Hochladen der Dokument-Bytes an /upload übergeben wird. Je nach zugrunde liegendem Dokumentenspeicher kann es erforderlich sein, ein Dokument mit einer Länge von null zu erstellen und den Inhalt des Dokuments später zu aktualisieren.

Wird Version 1.1 dieser Spezifikation hinzugefügt, können die Dokument-ID und die Dokumentversions-ID verwendet werden, um zusätzliche Informationen aus Workfront abzurufen.

**Beispiel:** Wenn das Document Management-System zusätzliche Informationen zum Dokument benötigt, kann der Webhook-Implementierungscode die Dokument-ID verwenden, um diese Informationen mithilfe der Workfront-RESTful-API abzurufen. Als Best Practice empfiehlt sich, diese Informationen aus benutzerdefinierten Datenfeldern im Dokument zu erhalten, die Aufgaben, Probleme oder Projekte enthalten.

## POST

**URL**

POST /uploadInit

### Abfrageparameter

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
   <td>parentId </td> 
   <td>Die übergeordnete Ordner-ID, wie vom Webhook-Provider referenziert.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>Der Name des Dokuments</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Die Workfront-Dokument-ID (in Version 1.1 hinzugefügt)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Die Workfront-Dokumentversions-ID (in Version 1.1 hinzugefügt) </td> 
  </tr> 
 </tbody> 
</table>

## Antwort

Die Metadaten für die Datei, wie vom Endpunkt /metadata definiert. Dazu gehört die Dokument-ID, die vom Provider verwendet wird.

**Beispiel:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT-Methode

Lädt die Bytes eines Dokuments in den Webhook-Provider hoch.

**URL**

PUT /upload

## Abfrageparameter

| Name  | Beschreibung |
|---|---|
| id  |  Die Dokument-ID, die gerade erstellt wurde. |


**Anfrageinhalt**

Die rohen Inhalts-Bytes für das Dokument.

**Reaktion**

```
{
result: “success”
}
```

oder

```
{
result: “fail”
}
```

**Beispiel**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

response

```
{
result:"success"
}
```
