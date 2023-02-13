---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Über die Zuordnung von Dateien in [!DNL Adobe Workfront Fusion]
description: Einige Module können Dateien verarbeiten. Diese Module können entweder eine Ausgabedatei zurückgeben, die zur weiteren Verarbeitung gesendet werden soll, oder verlangen, dass eine Datei zur Verarbeitung an sie übergeben wird. Bevor diese Module zur Verarbeitung von Dateien zusammenarbeiten können, müssen sie einander zugeordnet werden.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Über die Zuordnung von Dateien in [!DNL Adobe Workfront Fusion]

Einige Module können Dateien verarbeiten. Diese Module können entweder eine Ausgabedatei zurückgeben, die zur weiteren Verarbeitung gesendet werden soll, oder verlangen, dass eine Datei zur Verarbeitung an sie übergeben wird. Bevor diese Module zur Verarbeitung von Dateien zusammenarbeiten können, müssen sie einander zugeordnet werden.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr>  </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Zuordnen von Dateien

Für Module, die mit Dateien arbeiten können, sind zwei Informationen erforderlich:

* Dateiname
* Dateiinhalt (Daten)

Wenn Sie eine Datei zuordnen, wählen Sie die Module in Ihrem Szenario aus, aus denen Sie die Daten abrufen möchten. Der Dateiname und der Dateiinhalt werden dann automatisch wie gewünscht zugeordnet.

>[!NOTE]
>
>Wenn Sie eine Datei über eine URL verarbeiten müssen, empfehlen wir die Verwendung der `HTTP > Get a File` -Modul, um die Datei von der URL herunterzuladen, und ordnen Sie dann die Datei aus der `HTTP > Get a File` in das Feld des gewünschten Moduls in Ihrem Szenario.

>[!INFO]
>
>**Beispiel:** In diesem Beispiel wird gezeigt, wie Dokumente von heruntergeladen werden [!DNL Adobe Workfront] nach [!DNL Google Drive]. Die [!DNL Workfront] Trigger [!UICONTROL Aufzeichnen von Aufnahmen] gibt detaillierte Informationen zu den einzelnen Dokumenten zurück, einschließlich Name und Kennung.
>
>das nächste Modul, [!UICONTROL Dokument herunterladen], lädt die tatsächlichen Daten herunter, damit sie auf Google Drive hochgeladen werden können.
>
>Zuordnen dieser Informationen zu [!DNL Google Drive] Damit sie hochgeladen werden kann, müssen Sie die Quelldatei angeben, der die Informationen zugeordnet werden. Wenn Sie die [!DNL Workfront] > [!UICONTROL Dokument herunterladen] Option unter der Quelldatei, [!DNL Workfront Fusion] ordnet Dateinamen und Dateiinhalt so zu, dass das Dokument aus [!DNL Workfront] wird in den angegebenen Ordner Google hochgeladen.
>
>![](assets/wf-download-document-350x605.png)
>
>Wenn Sie die Datei jedoch umbenennen und die Daten unverändert lassen möchten, können Sie die [!UICONTROL Zuordnung] -Option, um den Dateinamen und den Dateiinhalt separat zuzuordnen. Geben Sie den vollständigen Dateinamen einschließlich der Erweiterung ein. Textformate und binäre Formate wie Fotos, Videos und PDF werden unterstützt.
>
>![](assets/use-the-map-option-350x358.png)
