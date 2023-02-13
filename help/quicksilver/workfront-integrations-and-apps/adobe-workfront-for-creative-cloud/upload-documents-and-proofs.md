---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Hochladen von Dokumenten und Testsendungen aus dem [!DNL Adobe Workfront plugin] der [!DNL Creative Cloud]
description: Hochladen von Dokumenten und Testsendungen aus dem [!DNL Adobe Workfront plugin] der [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 67952bf88a782595e13e559bfbc14ce1c622d432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Hochladen von Dokumenten und Testsendungen aus dem [!DNL Adobe Workfront plugin] der [!DNL Creative Cloud]

Sie können Ihre Projekte als Dokumente hochladen, um sie schnell zu überprüfen und zu genehmigen oder einfach in [!DNL Adobe Workfront].

>[!NOTE]
>
>Das Hochladen von Dokumenten und Testsendungen wird derzeit in Premiere Pro und After Effects nicht unterstützt.


## Dokumenteinschränkungen

In diesem Abschnitt werden die bekannten Dokumenteinschränkungen im Abschnitt [!DNL Workfront for Adobe Creative Cloud plugins].

### Neue Dokumentversionen akzeptieren nur eine Datei zum Hochladen

weil [!DNL Workfront] Dokumente dürfen nicht mehrere Dateien enthalten. Bestimmte Einstellungen müssen deaktiviert sein, damit neue Dokumentversionen in Workfront hochgeladen werden können.

>[!NOTE]
>
>Wenn Sie mehrere Dateien generieren müssen, können Sie stattdessen einen Testversand erstellen. Der neue Testversand wird nicht mit dem Originaldokument verknüpft.



So ändern Sie Ihren Wechsel zurück zu einer einzelnen Datei in [!DNL InDesign]:

1. Öffnen Sie die **Festlegen der Exportdateieinstellungen** Dialogfeld.

   ![](assets/file-export-settings.png)

1. Suchen Sie den Asset-Typ, den Sie exportieren möchten, und passen Sie die Einstellungen wie unten beschrieben an:

   <table>
    <tr>
    <td><strong>PDF und PDF-PRINT</strong>
    </td>
    <td>Auswahl aufheben <strong>Separate PDF-Dateien erstellen</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Auswählen <strong>Bereiche</strong> und geben Sie eine Seitenzahl ein. 
    <p>
    <strong>Hinweis</strong>: Wenn Sie das vollständige Dokument hochladen möchten, müssen Sie einen Testversand erstellen. 
    </td>
    </tr>
    <tr>
    <td><strong>ePub und EPUB FIXED</strong>
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
    <td>Auswählen <strong>Bereiche</strong> und geben Sie eine Seitenzahl ein. 
    <p>
    <strong>Hinweis</strong>: Wenn Sie das vollständige Dokument hochladen möchten, müssen Sie einen Testversand erstellen. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Auswählen <strong>Bereiche</strong> und geben Sie eine Seitenzahl ein. 
    <p>
    <strong>Hinweis</strong>: Wenn Sie das vollständige Dokument hochladen möchten, müssen Sie einen Testversand erstellen. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Keine Anpassungen erforderlich. 
    </td>
    </tr>
    </table>
