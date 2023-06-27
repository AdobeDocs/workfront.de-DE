---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Zuordnen eines Arrays in [!DNL Adobe] Workfront Fusion
description: Sie können ein Array einem Modulfeld in Adobe Workfront Fusion zuordnen.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Zuordnen eines Arrays in [!DNL Adobe Workfront Fusion]

Ein Array ist ein spezieller Elementtyp, der Folgendes enthalten kann:

* Ein oder mehrere Textwerte (einfaches Array)
* Eine oder mehrere Sammlungen desselben Typs (komplexes Array)

>[!INFO]
>
>**Beispiel:** Die [!UICONTROL E-Mails ansehen] -Modul gibt eine Gruppe von Anhängen für jede E-Mail zurück. Jeder Anhang stellt eine Sammlung dar, die einen Namen, einen Inhalt, eine Größe usw. enthalten kann.

Weitere Informationen finden Sie unter [Elementdatentypen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Array zuordnen

1. Klicken Sie auf die Schaltfläche im Zielfeld.

   >[!INFO]
   >
   >  **Beispiel:** Im obigen Beispiel würden Sie auf die [!UICONTROL Anlage hinzufügen] für eine E-Mail.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Geben Sie in das angezeigte Feld das Element ein.

   Über den Bereich können Sie Felder auf die gleiche Weise zuordnen wie mit jedem anderen Elementtyp. Wenn Sie nicht jedes Element einzeln ausfüllen möchten, aber ein anderes Array dem Zielfeld zuordnen möchten, verwenden Sie die [!UICONTROL Zuordnung] Schaltfläche. Stellen Sie in diesem Fall sicher, dass beide Arrays (das Quell-Array und das Ziel-Array) dieselbe Struktur aufweisen.

   Sie können einem Array eine beliebige Anzahl von Elementen hinzufügen.

Sie können ein Array mithilfe eines Iterators in einzelne Bundles unterteilen. Weitere Informationen finden Sie unter [[!UICONTROL Iterator] -Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
