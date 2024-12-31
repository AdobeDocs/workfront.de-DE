---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Hochladen von Dokumenten und Testsendungen aus dem [!DNL Adobe Workfront plugin]  in den [!DNL Creative Cloud]
description: Hochladen von Dokumenten und Testsendungen aus dem [!DNL Adobe Workfront plugin]  in den [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
source-git-commit: 0ca335bf0db934d23f607d3f8ce7cfb67e629053
workflow-type: tm+mt
source-wordcount: '242'
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

   ![](assets/file-export-settings.png)

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
