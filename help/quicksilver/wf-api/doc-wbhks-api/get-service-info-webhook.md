---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Abrufen von Informationen über den Service
description: Abrufen von Informationen über den Service
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 1%

---


# Abrufen von Informationen über den Service (noch nicht implementiert)

>[!NOTE]
>
>Das Veröffentlichungsdatum für diese Funktion ist noch nicht festgelegt.

Gibt Informationen zum Service zurück, z. B. Funktionen. Adobe Workfront verwendet diese Informationen, um die Benutzeroberfläche in Workfront anzupassen. Wenn die Webhook-Implementierung beispielsweise benutzerdefinierte Aktionen enthält, sollte die JSON diese Vorgänge in der JSON-Datei auflisten. Benutzer können dann diese Aktionen von Workfront aus aufrufen.

**URL**

GET /serviceInfo

## Abfrageparameter

Keine. Darüber hinaus sollten Aufrufe an diesen Endpunkt keine Authentifizierung erfordern.

## Antwort

JSON mit Informationen zu diesem Service

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
   <td>webhookVersion </td> 
   <td>Zeichenfolge </td> 
   <td>Die Webhook-Version, die von diesem Service implementiert wird. Dies ist die Versionsnummer, die oben in dieser Spezifikation aufgeführt ist.</td> 
  </tr> 
  <tr> 
   <td>Version </td> 
   <td>Zeichenfolge </td> 
   <td>Die interne Versionsnummer für diesen Service. Diese Nummer wird vom Webhook-Dienstleister festgelegt und dient nur zu Informationszwecken.<br><br></td> 
  </tr> 
  <tr> 
   <td>Verleger </td> 
   <td>Zeichenfolge </td> 
   <td>Der Name des Unternehmens, das die Webhook-Implementierung bereitstellt.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Zeichenfolge </td> 
   <td>Eine Liste mit den API-Endpunkten, die von diesem Service implementiert wurden. Damit kann sichergestellt werden, dass die Benutzeroberfläche in Workfront die vom Webhook-Anbieter bereitgestellten Funktionen widerspiegelt. Jedes Element in der Liste muss den Namen des Endpunkts enthalten (z. B. „Suche„).</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Zeichenfolge</td> 
   <td>  <p>Eine Liste mit den benutzerdefinierten Vorgängen, die von diesem Webhook implementiert wurden. Jedes Listenelement enthält einen Namen und einen Anzeigenamen. Der Anzeigename wird im Dropdown-Menü „Dokumentaktionen“ in Workfront angezeigt. Durch Klicken auf das Element in der Dropdown-Liste wird die Aktion im Webhook aufgerufen, indem der /customAction-Endpunkt aufgerufen wird.</p></td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** `https://www.acme.com/api/serviceInfo`

Rückgabe

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
