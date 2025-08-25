---
title: Automatisches Ausfüllen einer Anfrage über Eingabeaufforderungen oder Dokumente
content-type: reference
description: Sie können KI zum automatischen Ausfüllen von Anfragefeldern verwenden, indem Sie eine Eingabeaufforderung eingeben oder ein Dokument angeben.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 2%

---

# Automatisches Ausfüllen einer Anfrage über Eingabeaufforderungen oder Dokumente

>[!NOTE]
>
>* Diese Funktion wird als offene Beta-Version nach dem folgenden Zeitplan verfügbar sein:
>
>   * Monatliche Version: 11. September 2025
>   * Vierteljährliche Veröffentlichung: 16. Oktober 2025
>
>* Um diese Funktion nutzen zu können, muss Ihr Unternehmen die Anforderungen für die Verwendung des Workfront AI Assistant erfüllen. Weitere Informationen finden Sie unter [Voraussetzungen für den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

KI kann Ihnen dabei helfen, Anfragefelder basierend auf einer von Ihnen eingegebenen Eingabeaufforderung automatisch auszufüllen. Es kann auch Felder basierend auf Text ausfüllen, z. B. E-Mails oder hochgeladene Dokumente. Sie können diese Vorschläge vor dem Absenden der Anfrage genehmigen oder ablehnen.

Das automatische Ausfüllen überschreibt keine bereits ausgefüllten Felder.

Benutzer erhalten keine Vorschläge für Daten, auf die sie sonst keinen Zugriff hätten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Mitwirkender oder höher</p>
   Oder
   <p>Aktuell: Anforderung oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p>  </td> 
  </tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Zugriff zum Hinzufügen von Anfragen zu einer Anfragewarteschlange</p> <p>Anzeigen von oder höheren Berechtigungen für die vorhandene Anfrage</p> <p>Informationen zum Einrichten einer Anfrage-Warteschlange finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anfrage-Warteschlange</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Um Anfragen mithilfe einer Eingabeaufforderung oder eines Dokuments automatisch auszufüllen **müssen** der folgenden Bedingungen zutreffen:

* Ihr Unternehmen muss Adobe IMS (Identity Management-System) verwenden
* Adobe Unified Experience muss aktiviert sein
* Ihr Unternehmen muss über einen Select-, Prime- oder Ultimate Workfront-Plan verfügen
* Adobe muss über eine unterzeichnete Adobe Gen AI-Vereinbarung verfügen

  Weitere Informationen zum Unterzeichnen des Vertrags finden Sie unter [Unterschreiben des Adobe Gen AI-](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)) im Artikel KI-Assistent - Übersicht.
* Der KI-Assistent muss in den Systemeinstellungen Ihrer Organisation aktiviert sein. Dieser wird von Ihrem Workfront-Administrator verwaltet.

  Weitere Informationen zum Aktivieren des KI-Assistenten in den Systemeinstellungen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

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
1. Wählen Sie für jeden Feldvorschlag **Feld** Akzeptieren“ oder **Ablehnen** aus.

   ![Vorschlag annehmen oder ablehnen](assets/accept-reject-suggestion.png)

   Oder

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

   >[!NOTE]
   >
   >Alle nicht überprüften Vorschläge werden automatisch akzeptiert, wenn Sie die Anfrage senden.

## Abrufen von Vorschlägen basierend auf einem hochgeladenen Dokument

Das automatische Ausfüllen kann Feldwerte basierend auf einem hochgeladenen Dokument vorschlagen.

Diese Art von Vorschlag überprüft auch frühere Anfragen nach ähnlichen Kontexten. Wenn in der Eingabeaufforderung beispielsweise erwähnt wird, dass die Anfrage für einen bestimmten Client gilt, kann Workfront die Rechnungsadresse für diesen Client basierend auf vorherigen Anfragen automatisch suchen und eingeben.

### Leitplanken beim Hochladen von Dokumenten

#### Unterstützte Dateitypen

Die folgenden Dateitypen werden unterstützt:

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### Unterstützte Dateigröße

Jede Datei kann bis zu 100 MB groß sein

#### Anzahl Dateien

Sie können bis zu 50 Dateien (Seiten, Folien oder Blätter) hochladen.

>[!IMPORTANT]
>
>Dokumente werden in eine Reihe von Bildern konvertiert, die jeweils als separate Datei betrachtet werden.
>
>Sie können beispielsweise einen PowerPoint mit 50 Folien oder 5 Word-Dokumente mit jeweils 10 Seiten hochladen.

#### Unterstützte Feldtypen

Workfront-Feldtypen beeinflussen, ob ein bestimmtes Feld automatisch ausgefüllt werden kann.

<table>
<tr>
<td><b>Unterstützt </b><br> Automatisches Ausfüllen kann ausfüllen</td>
<td><b>Nicht unterstützt</b> <br>Automatisches Ausfüllen wird nicht ausgefüllt</td>
</tr>
<tr>
<td>
<ul>
<li>Einzeiliger Text</li>
<li>Textbereich oder Absatz</li>
<li>Datumsfeld</li>
<li>Kontrollkästchen</li>
<li>Optionsfelder</li>
<li>Dropdown-Listen für Einzel- und Mehrfachauswahl</li>
</ul>
</td>
<td><li>Typeahead</li>
<li>Externer Lookup</li>
<li>Interne Suche</li>
<li>Referenz</li>
<li>Eingebettete WF-Felder planen</li>
</ul>
</td>
</tr>
</table>

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
1. Wählen Sie für jeden Feldvorschlag **Feld** Akzeptieren“ oder **Ablehnen** aus.

   ![Vorschlag annehmen oder ablehnen](assets/accept-reject-suggestion.png)

   Oder

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

   >[!NOTE]
   >
   >Alle nicht überprüften Vorschläge werden automatisch akzeptiert, wenn Sie die Anfrage senden.

## Fehlerbehebung

Wenn Sie nicht die erwarteten Vorschläge erhalten, kann dies auf eine der folgenden Ursachen zurückzuführen sein:

* Sie müssen mindestens einen Monat an Anfragedaten im System haben, bevor es Feldwerte aus früheren Anfragen vorschlagen kann.
* Sie haben möglicherweise die Leitplanken für den Dokument-Upload nicht befolgt, wenn Sie ein Dokument hochladen, aus dem Sie Vorschläge abrufen möchten. Weitere Informationen finden Sie unter [Leitplanken beim Hochladen von Dokumenten](#document-upload-guardrails) in diesem Artikel.
