---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Über die Zuordnung von Dateien in  [!DNL Adobe Workfront Fusion]
description: Einige Module können Dateien verarbeiten. Diese Module können entweder eine Ausgabedatei zurückgeben, die zur weiteren Verarbeitung gesendet werden soll, oder verlangen, dass eine Datei zur Verarbeitung an sie übergeben wird. Bevor diese Module zur Verarbeitung von Dateien zusammenarbeiten können, müssen sie einander zugeordnet werden.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Über die Zuordnung von Dateien in [!DNL Adobe Workfront Fusion]

Einige Module können Dateien verarbeiten. Diese Module können entweder eine Ausgabedatei zurückgeben, die zur weiteren Verarbeitung gesendet werden soll, oder verlangen, dass eine Datei zur Verarbeitung an sie übergeben wird. Bevor diese Module zur Verarbeitung von Dateien zusammenarbeiten können, müssen sie einander zugeordnet werden.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr>  </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Zuordnen von Dateien

Für Module, die mit Dateien arbeiten können, sind zwei Informationen erforderlich:

* Dateiname
* Dateiinhalt (Daten)

Wenn Sie eine Datei zuordnen, wählen Sie die Module in Ihrem Szenario aus, aus denen Sie die Daten abrufen möchten. Der Dateiname und der Dateiinhalt werden dann automatisch wie gewünscht zugeordnet.

>[!NOTE]
>
>Wenn Sie eine Datei über eine URL verarbeiten müssen, empfehlen wir, die Datei mit dem Modul `HTTP > Get a File` von der URL herunterzuladen und sie dann vom Modul `HTTP > Get a File` dem Feld des gewünschten Moduls in Ihrem Szenario zuzuordnen.

>[!INFO]
>
>**Beispiel:** Dieses Beispiel zeigt, wie Sie Dokumente von [!DNL Adobe Workfront] in [!DNL Google Drive] herunterladen können. Der Trigger [!DNL Workfront] [!UICONTROL Überwachungsdatensatz] gibt detaillierte Informationen zu den einzelnen Dokumenten zurück, einschließlich des Namens und der Kennung.
>
>Das nächste Modul, [!UICONTROL Dokument herunterladen], lädt die tatsächlichen Daten herunter, damit sie auf Google Drive hochgeladen werden können.
>
>Um diese Informationen [!DNL Google Drive] zuzuordnen, damit sie hochgeladen werden können, müssen Sie die Quelldatei angeben, der die Informationen zugeordnet werden. Wenn Sie unter der Quelldatei die Option [!DNL Workfront] > [!UICONTROL Dokument herunterladen] auswählen, ordnet [!DNL Workfront Fusion] den Dateinamen und den Dateiinhalt zu, sodass das Dokument aus [!DNL Workfront] in den angegebenen Google-Ordner hochgeladen wird.
>
>![](assets/wf-download-document-350x605.png)
>
>Wenn Sie die Datei jedoch umbenennen und die Daten unverändert lassen möchten, können Sie die Option [!UICONTROL Zuordnung] verwenden, um den Dateinamen und den Dateiinhalt separat zuzuordnen. Geben Sie den vollständigen Dateinamen einschließlich der Erweiterung ein. Textformate und binäre Formate wie Fotos, Videos und PDF werden unterstützt.
>
>![](assets/use-the-map-option-350x358.png)
