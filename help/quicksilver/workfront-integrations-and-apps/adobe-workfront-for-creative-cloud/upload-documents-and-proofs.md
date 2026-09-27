---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Hochladen von Dokumenten und Testsendungen aus der [!DNL Adobe Workfront plugin] in die [!DNL Creative Cloud]
description: Hochladen von Dokumenten und Testsendungen aus der [!DNL Adobe Workfront plugin] in die [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
TQID: 'https://experienceleague.adobe.com/bZsOnrrwZ7ksCaoM3jfIyeTO00XqG1hDTEmG5VmWOcA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%
---
# Hochladen von Dokumenten und Testsendungen aus der [!DNL Adobe Workfront plugin] in die [!DNL Creative Cloud]

Sie können Ihre Projekte als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in [!DNL Adobe Workfront] zu speichern.

>[!NOTE]
>
>Das Hochladen von Dokumenten und Testsendungen wird derzeit in Premiere Pro und After Effects nicht unterstützt.


## Dokumenteinschränkungen

In diesem Abschnitt werden bekannte Dokumenteinschränkungen in der [!DNL Workfront for Adobe Creative Cloud plugins] beschrieben.

### Neue Dokumentversionen akzeptieren nur eine Datei zum Hochladen

Da [!DNL Workfront] Dokumente nicht mehrere Dateien enthalten können, müssen bestimmte Einstellungen deaktiviert werden, um neue Dokumentversionen in Workfront hochladen zu können.

>[!NOTE]
>
>Wenn Sie mehrere Dateien generieren müssen, können Sie stattdessen einen Korrekturabzug erstellen. Der neue Korrekturabzug wird nicht mit dem Originaldokument verknüpft.



So ändern Sie Ihren Schalter wieder in eine einzelne Datei in [!DNL InDesign]:

1. Öffnen Sie **Dialogfeld Exportdateieinstellungen**.

   ![Dateiexporteinstellungen](assets/file-export-settings.png)

1. Suchen Sie den Asset-Typ, den Sie exportieren möchten, und passen Sie die Einstellungen wie unten beschrieben an:

   <table>
    <tr>
    <td><strong>PDF und PDF-PRINT</strong>
    </td>
    <td>Deaktivieren Sie <strong>Separate PDF-Dateien erstellen</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Wählen Sie <strong>Bereiche</strong> aus und geben Sie eine einzelne Seitenzahl ein. 
    <p>
    <strong>Hinweis</strong>: Wenn Sie das vollständige Dokument hochladen möchten, müssen Sie einen Korrekturabzug erstellen. 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB und EPUB-FIXED</strong>
    </td>
    <td>Keine Anpassungen erforderlich.
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>Keine Anpassungen erforderlich.
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>Wählen Sie <strong>Bereiche</strong> aus und geben Sie eine einzelne Seitenzahl ein. 
    <p>
    <strong>Hinweis</strong>: Wenn Sie das vollständige Dokument hochladen möchten, müssen Sie einen Korrekturabzug erstellen. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Wählen Sie <strong>Bereiche</strong> aus und geben Sie eine einzelne Seitenzahl ein. 
    <p>
    <strong>Hinweis</strong>: Wenn Sie das vollständige Dokument hochladen möchten, müssen Sie einen Korrekturabzug erstellen. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Keine Anpassungen erforderlich. 
    </td>
    </tr>
    </table>
