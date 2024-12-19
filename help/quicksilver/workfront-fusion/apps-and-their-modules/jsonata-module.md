---
title: JSONata-Module
description: Der Adobe Workfront Fusion JSONata-Connector bietet ein Modul zur Verarbeitung von Daten im JSON-Format, damit Adobe Workfront Fusion weiter mit dem Dateninhalt arbeiten kann.
author: Becky
feature: Workfront Fusion
source-git-commit: b7a6ecd9089c3a5517c56b849b860d57a900dade
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 1%

---

# [!UICONTROL JSONata]-Module

Mit dem [!DNL Adobe Workfront Fusion] [!UICONTROL JSONata]-Connector können Sie JSON-Objekte abfragen. Dieses Modul erfordert keine Verbindung.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## JSONata-Modul und seine Felder

### Evaluate

Dieses Aktionsmodul fragt ein JSON-Objekt ab und gibt ein Array zurück.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ausdruck]</td> 
   <td>Geben Sie den Ausdruck ein, den Sie zum Auswerten des JSON-Objekts verwenden möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Daten] </td> 
   <td> Geben Sie das zu überprüfende JSON-Objekt ein.  </td> 
  </tr> 
  </tbody>
  </table>

>[!BEGINSHADEBOX]

**Beispiel**:

Das Ziel besteht darin, ein Array von Namen aus dem folgenden JSON-Objekt zurückzugeben:

```JSON
{
  "people": [
    { "name": "Alice", "age": 30 },
    { "name": "Bob", "age": 25 },
    { "name": "Charlie", "age": 35 }
  ]
}
```

1. Geben Sie im Ausdrucksfeld `people.name` ein.
1. Geben Sie im Datenfeld das JSON-Objekt ein.

Das -Modul gibt ein Array von Namen zurück, die aus dem JSON-Objekt abgerufen wurden.

>[!ENDSHADEBOX]
