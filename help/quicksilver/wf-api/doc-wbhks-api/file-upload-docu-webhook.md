---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Datei-Upload über Dokument-Webhooks
description: Datei-Upload über Dokument-Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 1%

---


# Datei-Upload über Dokument-Webhooks

Das Hochladen einer Datei in einen Dokumentspeicheranbieter ist ein zweistufiger Prozess, für den zwei separate API-Endpunkte erforderlich sind. Adobe Workfront beginnt den Upload-Prozess mit dem Aufruf von /uploadInit . Dieser Endpunkt gibt eine Dokument-ID zurück, die beim Hochladen der Dokument-Bytes an /upload übergeben wird. Je nach dem zugrunde liegenden Dokumentenspeichersystem kann es erforderlich sein, ein Dokument mit einer Länge von null zu erstellen und den Inhalt des Dokuments dann später zu aktualisieren.

In Version 1.1 dieser Spezifikation können die Dokument-ID und Dokumentversions-ID hinzugefügt werden, um zusätzliche Informationen von Workfront abzurufen.

**Beispiel:** Wenn das Dokumentenverwaltungssystem zusätzliche Informationen zum Dokument benötigt, könnte der Webhook-Implementierungs-Code die Dokument-ID verwenden, um diese Informationen mithilfe der RESTful-API von Workfront abzurufen. Als Best Practice empfiehlt es sich, diese Informationen aus benutzerdefinierten Datenfeldern im Dokument zu generieren, das die Aufgabe, das Problem oder das Projekt enthält.

## POST-Methode

**URL**

POST/uploadInit

### Abfrageparameter

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>-Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>Die ID des übergeordneten Ordners, wie vom Webhook-Anbieter referenziert.</td> 
  </tr> 
  <tr> 
   <td>Dateiname </td> 
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

Die Metadaten für die Datei, wie vom Endpunkt /metadata definiert. Dazu gehört die vom Anbieter verwendete Dokument-ID.

**Beispiel:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT-Methode

Lädt die Bytes eines Dokuments in den Webhook-Anbieter hoch.

**URL**

PUT/Upload

## Abfrageparameter

| -Name  | Beschreibung |
|---|---|
| ID  |  Die Dokument-ID, die gerade erstellt wurde. |


**Anfragetext**

Die Rohdaten-Inhaltsbytes für das Dokument.

**Antwort**

```
{
result: "success"
}
```

oder

```
{
result: "fail"
}
```

**Beispiel**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

Antwort

```
{
result:"success"
}
```
