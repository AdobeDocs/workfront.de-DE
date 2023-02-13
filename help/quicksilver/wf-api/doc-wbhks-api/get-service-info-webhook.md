---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Informationen zum Dienst erhalten
description: Informationen zum Dienst erhalten
author: John
feature: Workfront API
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 4%

---


# Informationen zum Dienst abrufen (noch nicht implementiert)

>[!NOTE]
>
>Das Veröffentlichungsdatum für diese Funktion ist noch nicht festgelegt.

Gibt Informationen zum Dienst zurück, z. B. Funktionen und Funktionen. Adobe Workfront verwendet diese Informationen, um die Benutzeroberfläche in Workfront anzupassen. Wenn die Webhook-Implementierung beispielsweise einige benutzerdefinierte Aktionen enthält, sollte die JSON diese Vorgänge in der JSON auflisten. Benutzer können diese Aktionen dann über Workfront aufrufen.

**URL**

GET /serviceInfo

## Abfrageparameter

Keine. Darüber hinaus sollten Aufrufe an diesen Endpunkt keine Authentifizierung erfordern.

## Antwort

JSON mit Informationen zu diesem Dienst

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
   <td>Die von diesem Dienst implementierte Webhook-Version. Dies ist die Versionsnummer, die oben in dieser Spezifikation aufgeführt ist.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Zeichenfolge </td> 
   <td>Die interne Versionsnummer für diesen Dienst. Diese Nummer wird vom Webhook-Dienstleister bestimmt und nur zu Informationszwecken verwendet.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher </td> 
   <td>Zeichenfolge </td> 
   <td>Der Name des Unternehmens, das die Webhook-Implementierung bereitstellt.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Zeichenfolge </td> 
   <td>Eine Liste mit den von diesem Dienst implementierten API-Endpunkten. Dies kann verwendet werden, um sicherzustellen, dass die Benutzeroberfläche in Workfront die vom Webhook-Provider bereitgestellten Funktionen widerspiegelt. Jedes Element in der Liste muss den Namen des Endpunkts enthalten (z. B. "Suche").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Zeichenfolge</td> 
   <td>  <p>Eine Liste mit den von diesem Webhook implementierten benutzerdefinierten Vorgängen. Jedes Listenelement enthält einen Namen und einen Anzeigenamen. Der Anzeigename wird im Dropdown-Menü "Dokumentaktionen"in Workfront angezeigt. Durch Klicken auf das Element in der Dropdown-Liste wird die Aktion im Webhook aufgerufen, indem der Endpunkt /customAction aufgerufen wird.</p></td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** `https://www.acme.com/api/serviceInfo`

return

```
{
webhook version: “1.2”, version: “1.0”, publisher: “Acme, LLC”, availableEndpoints: [“files”, “metadata”, “search”, “download”
“thumbnail”, “uploadInit”, “upload” ], customActions [
{
name: “archive”, displayName: “Archive” 
}, 
{name: “doSomethingElse”, displayName: “Do Something” }, 
] 
}
```
