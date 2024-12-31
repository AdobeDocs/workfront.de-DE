---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Informationen zum Zuordnen von Dateien in  [!DNL Adobe Workfront Fusion]
description: Einige Module können Dateien verarbeiten. Diese Module können entweder eine Ausgabedatei zurückgeben, die zur weiteren Verarbeitung gesendet werden soll, oder sie erfordern, dass eine Datei zur Verarbeitung an sie übergeben wird. Bevor diese Module zusammenarbeiten können, um Dateien zu verarbeiten, müssen sie einander zugeordnet werden.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---

# Zuordnungsdateien in [!DNL Adobe Workfront Fusion]

Einige Module können Dateien verarbeiten. Diese Module können entweder eine Ausgabedatei zurückgeben, die zur weiteren Verarbeitung gesendet werden soll, oder sie erfordern, dass eine Datei zur Verarbeitung an sie übergeben wird. Bevor diese Module zusammenarbeiten können, um Dateien zu verarbeiten, müssen sie einander zugeordnet werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr>  </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Zuordnen von Dateien

Module, die mit Dateien arbeiten können, benötigen zwei Informationen:

* Dateiname
* Dateiinhalt (Daten)

Beim Zuordnen einer Datei wählen Sie die Module in Ihrem Szenario aus, aus denen Sie die Daten abrufen möchten. Der Dateiname und der Dateiinhalt werden dann automatisch so zugeordnet, wie sie sind.

>[!NOTE]
>
>Wenn Sie eine Datei über eine URL verarbeiten müssen, empfehlen wir die Verwendung des `HTTP > Get a File`-Moduls , um die Datei über die URL herunterzuladen, und dann die Zuordnung der Datei aus dem `HTTP > Get a File`-Modul zum Feld des gewünschten Moduls in Ihrem Szenario.

>[!INFO]
>
>**Beispiel:** Dieses Beispiel zeigt, wie Dokumente von [!DNL Adobe Workfront] nach [!DNL Google Drive] heruntergeladen werden. Der [!DNL Workfront] Trigger [!UICONTROL Watch Record] gibt detaillierte Informationen zu jedem Dokument zurück, einschließlich seines Namens und seiner ID.
>
>Das nächste Modul [!UICONTROL Dokument herunterladen] lädt die eigentlichen Daten herunter, damit sie auf das Google-Laufwerk hochgeladen werden können.
>
>Um diese Informationen [!DNL Google Drive] zuzuordnen, damit sie hochgeladen werden können, müssen Sie die Quelldatei angeben, aus der die Informationen zugeordnet werden sollen. Wenn Sie die Option [!DNL Workfront] > [!UICONTROL Dokument herunterladen] unter der Quelldatei auswählen, ordnet [!DNL Workfront Fusion] den Dateinamen und den Dateiinhalt zu, sodass das Dokument aus [!DNL Workfront] in den angegebenen Google-Ordner hochgeladen wird.
>
>![](assets/wf-download-document-350x605.png)
>
>Wenn Sie die Datei jedoch umbenennen, die Daten jedoch unverändert lassen möchten, können Sie die Option [!UICONTROL Zuordnen] verwenden, um den Dateinamen und den Dateiinhalt separat zuzuordnen. In diesem Fall geben Sie den vollständigen Dateinamen einschließlich der Erweiterung ein. Textformate und Binärformate wie Fotos, Videos und PDF werden unterstützt.
>
>![](assets/use-the-map-option-350x358.png)
