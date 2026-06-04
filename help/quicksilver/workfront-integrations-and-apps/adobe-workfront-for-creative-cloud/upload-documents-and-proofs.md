---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Hochladen von Dokumenten und Korrekturabzügen aus dem  [!DNL Adobe Workfront plugin]  in  [!DNL Creative Cloud]
description: Hochladen von Dokumenten und Korrekturabzügen aus dem  [!DNL Adobe Workfront plugin]  in  [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
TQID: https://experienceleague.adobe.com/bZsOnrrwZ7ksCaoM3jfIyeTO00XqG1hDTEmG5VmWOcA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 245
ht-degree: 5%

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
