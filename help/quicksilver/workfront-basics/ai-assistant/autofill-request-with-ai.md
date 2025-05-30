---
title: Automatisches Ausfüllen einer Anfrage mit KI
content-type: reference
description: Sie können KI verwenden, um Anfragefelder automatisch auszufüllen.
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: a3e93311277bc5b68063e0ec1cbdcce3a40eb3dd
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# Automatisches Ausfüllen einer Anfrage mit KI

>[!NOTE]
>
>Diese Funktion ist derzeit Teil einer geschlossenen Beta-Version. Um diese Funktion aktivieren zu lassen, wenden Sie sich bitte an sargism@adobe.com.
>
>Um sich für die Closed Beta zu qualifizieren, muss Ihr Unternehmen die Anforderungen für die Verwendung des Workfront AI Assistant erfüllen. Weitere Informationen finden Sie unter [Voraussetzungen für den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

KI kann Ihnen helfen, Anfragefelder automatisch auszufüllen. Es kann Feldwerte basierend auf früheren Anfragen vorschlagen oder sie aus Text analysieren, z. B. E-Mails oder hochgeladene Dokumente.

Sie können diese Vorschläge vor dem Absenden der Anfrage genehmigen oder ablehnen.

Das automatische Ausfüllen überschreibt keine bereits ausgefüllten Felder.

## Vorschläge beim Ausfüllen des Formulars einholen

Das automatische Ausfüllen kann Feldwerte beim Ausfüllen des Formulars vorschlagen. Wenn Sie Werte in die Anfragefelder eingeben, vergleicht Workfront diese Werte mit vorherigen Anfragen. Wenn der eingegebene Wert eng mit anderen Feldwerten in ähnlichen Kontexten in früheren Anfragen korreliert, schlägt Workfront diese Werte vor.

Wenn beispielsweise eine Klinik immer denselben Abrechnungscode verwendet, schlägt Workfront vor, dass sich der Abrechnungscode bei Eingabe des Kliniknamens im entsprechenden Feld befindet.

So verwenden Sie Vorschläge basierend auf früheren Anfragen:

1. Erstellen Sie eine Anfrage.

   Anweisungen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Felder ausfüllen.

   Beim Ausfüllen von Feldern können andere Felder Vorschläge anzeigen.

1. Wählen Sie für jeden Feldvorschlag unter diesem Feld **Akzeptieren** oder **Ablehnen** aus.

   Oder

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

## Abrufen von Vorschlägen aus einer Textaufforderung

Das automatische Ausfüllen kann Feldwerte basierend auf Text vorschlagen, z. B. E-Mails. Sie fügen einen Textblock ein, und Workfront verarbeitet den Text, um auf der Grundlage des Texts Feldwerte vorzuschlagen.

Wenn die E-Mail beispielsweise „Dies ist am 1. Juni fällig“ enthält und das Anfrageformular ein Feld für das Fälligkeitsdatum hat, schlägt Workfront für diesen Feldwert den 1. Juni vor.

Diese Art von Vorschlag überprüft auch frühere Anfragen nach ähnlichen Kontexten. Wenn in der Eingabeaufforderung beispielsweise erwähnt wird, dass die Anfrage für einen bestimmten Client gilt, kann Workfront die Rechnungsadresse für diesen Client basierend auf vorherigen Anfragen automatisch suchen und eingeben.

Sie können Text einfügen, der auf das gesamte Formular oder auf einen einzelnen Abschnitt des Formulars angewendet wird.

So verwenden Sie Vorschläge basierend auf einer eingefügten Textaufforderung:

1. Erstellen Sie eine Anfrage.

   Anweisungen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Um die Textaufforderung auf das gesamte Formular anzuwenden, klicken Sie auf das KI-Symbol ![AI-Symbol](assets/request-prompt-icon.png) unter dem Formularnamen.

   Oder

   Um die Textaufforderung auf einen einzelnen Abschnitt anzuwenden, klicken Sie auf das KI![Symbol „KI](assets/request-prompt-icon.png)Symbol neben dem Abschnittsnamen.

1. Fügen Sie den Text in das Eingabeaufforderungsfeld ein.
1. Klicken Sie **Formular ausfüllen**.

   Workfront generiert Vorschläge für das Formular.
1. Wählen Sie für jeden Feldvorschlag unter diesem Feld **Akzeptieren** oder **Ablehnen** aus.

   Oder

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

## Abrufen von Vorschlägen basierend auf einem hochgeladenen Dokument

Das automatische Ausfüllen kann Feldwerte basierend auf einem hochgeladenen Dokument vorschlagen.

Diese Art von Vorschlag überprüft auch frühere Anfragen nach ähnlichen Kontexten. Wenn in der Eingabeaufforderung beispielsweise erwähnt wird, dass die Anfrage für einen bestimmten Client gilt, kann Workfront die Rechnungsadresse für diesen Client basierend auf vorherigen Anfragen automatisch suchen und eingeben.

### Leitplanken beim Hochladen von Dokumenten

#### Unterstützte Dateitypen

Die folgenden Dateitypen werden unterstützt:

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XLSX

#### Unterstützte Dateigröße

Jede Datei kann bis zu 100 MB groß sein

#### Anzahl Dateien

Sie können bis zu 50 Dateien (Seiten, Folien oder Blätter) hochladen.

>[!IMPORTANT]
>
>Dokumente werden in eine Reihe von Bildern konvertiert, die jeweils als separate Datei betrachtet werden.
>
>Sie können beispielsweise einen PowerPoint mit 50 Folien oder 5 Word-Dokumente mit jeweils 10 Seiten hochladen.

#### Andere Best Practices

Beachten Sie beim Hochladen eines Dokuments für das automatische Ausfüllen Folgendes:

* Das automatische Ausfüllen ist derzeit für das lateinische Alphabet optimiert.
* Es wird empfohlen, eine Textgröße von 8 Punkten oder mehr zu verwenden.
* Das automatische Ausfüllen kann Probleme mit Bildern im Dokument haben, z. B. gedrehte oder verzerrte Bilder, Diagramme und das Zählen oder Verwenden räumlicher Gründe für Objekte in Bildern.
* Wie immer empfehlen wir, die Ergebnisse vor dem Senden der Anfrage auf Korrektheit zu überprüfen.

### Dokument hochladen, um eine Anfrage automatisch auszufüllen

Sie können ein Dokument hochladen, das auf das gesamte Formular oder auf einen einzelnen Abschnitt des Formulars angewendet werden soll.

1. Erstellen Sie eine Anfrage.

   Anweisungen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Um das Dokument auf das gesamte Formular anzuwenden, klicken Sie auf das KI![Symbol „KI](assets/request-prompt-icon.png) unter dem Formularnamen.

   Oder

   Um das Dokument auf einen einzelnen Abschnitt anzuwenden, klicken Sie auf das KI![Symbol „KI](assets/request-prompt-icon.png)Symbol neben dem Abschnittsnamen.

1. Klicken Sie **Dateien hochladen** und wählen Sie dann die Datei aus Ihrem Datei-Manager aus.

   Oder

   Ziehen Sie das Dokument aus Ihrem Datei-Manager in das Feld **Dateien hochladen, um das Anfrageformular automatisch**.
1. Klicken Sie **Formular ausfüllen** oder **Abschnitt ausfüllen**.

   Workfront generiert Vorschläge für das Formular.
1. Wählen Sie für jeden Feldvorschlag unter diesem Feld **Akzeptieren** oder **Ablehnen** aus.

   Oder

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

