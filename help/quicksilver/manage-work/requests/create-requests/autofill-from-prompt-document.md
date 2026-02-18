---
title: Verwenden von Form Fill powered by AI zum Ausfüllen einer Anfrage mithilfe von Eingabeaufforderungen oder Dokumenten
content-type: reference
description: Sie können KI zum automatischen Ausfüllen von Anfragefeldern verwenden, indem Sie eine Eingabeaufforderung eingeben oder ein Dokument angeben.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: 8dc094718999af291443bd1a703cdc742d13f57e
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 3%

---

# Verwenden von Form Fill powered by AI zum Ausfüllen einer Anfrage mithilfe von Eingabeaufforderungen oder Dokumenten

>[!NOTE]
>
>Um diese Funktion nutzen zu können, muss Ihr Unternehmen die Anforderungen für die Verwendung des Workfront AI Assistant erfüllen. Weitere Informationen finden Sie unter [Voraussetzungen für den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

Mit KI-Formularausfüllen können Sie Anfragefelder basierend auf einer von Ihnen eingegebenen Eingabeaufforderung automatisch ausfüllen. Es kann auch Felder basierend auf Text ausfüllen, z. B. E-Mails oder hochgeladene Dokumente. Sie können diese Vorschläge vor dem Absenden der Anfrage genehmigen oder ablehnen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <td> <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Um das Ausfüllen eines Formulars mit KI mithilfe einer Eingabeaufforderung oder eines Dokuments zu ermöglichen, müssen **alle** der folgenden Bedingungen erfüllt sein:

* Ihr Unternehmen muss zu Adobe IMS (Identity Management System) migriert sein
* Adobe Unified Experience muss aktiviert sein
* Ihr Unternehmen muss über einen Select-, Prime- oder Ultimate Workfront-Plan verfügen
* Adobe muss über eine unterzeichnete Adobe Gen AI-Vereinbarung verfügen

  Weitere Informationen zum Unterzeichnen des Vertrags finden Sie unter [Unterschreiben des Adobe Gen AI-](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)) im Artikel KI-Assistent - Übersicht.
* Der KI-Assistent muss in den Systemeinstellungen Ihrer Organisation aktiviert sein. Dieser wird von Ihrem Workfront-Administrator verwaltet.

  Weitere Informationen zum Aktivieren des KI-Assistenten in den Systemeinstellungen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Überlegungen zur Verwendung von Formularausfüllen mit KI

Beachten Sie bei der Verwendung von Formularausfüllen auf Basis von KI Folgendes

* KI-Formularausfüllung überschreibt keine Felder, die Sie bereits ausgefüllt haben.
* Benutzer erhalten keine Vorschläge für Daten, auf die sie sonst keinen Zugriff hätten.

<!--
* Files that you use in Form Fill powered by AI are uploaded to Azure storage for 24 hours. This is necessary for document processing. 
* All files uploaded to Azure are currently stored in US Azure clusters for the 24 hour storage window. 
-->

## Abrufen von Vorschlägen aus einer Textaufforderung

Das Ausfüllen eines KI-Formulars kann Feldwerte basierend auf Text wie E-Mails vorschlagen. Sie fügen einen Textblock ein, und Workfront verarbeitet den Text, um auf der Grundlage des Texts Feldwerte vorzuschlagen.

Wenn die E-Mail beispielsweise „Dies ist am 1. Juni fällig“ enthält und das Anfrageformular ein Feld für das Fälligkeitsdatum hat, würde das Ausfüllen des KI-Formulars für diesen Feldwert den 1. Juni vorschlagen.

Beim Ausfüllen eines Formulars prüft Workfront auch frühere Anfragen auf ähnliche Kontexte. Wenn in der Eingabeaufforderung beispielsweise erwähnt wird, dass die Anfrage für einen bestimmten Client gilt, kann Workfront die Rechnungsadresse für diesen Client basierend auf vorherigen Anfragen automatisch suchen und eingeben.

Sie können Text einfügen, der auf das gesamte Formular oder auf einen einzelnen Abschnitt des Formulars angewendet wird.

So verwenden Sie Vorschläge basierend auf einer eingefügten Textaufforderung:

1. Erstellen Sie eine Anfrage.

   Anweisungen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Um die Textaufforderung auf das gesamte Formular anzuwenden, klicken Sie auf das KI-Symbol ![AI-Symbol](assets/request-prompt-icon.png) unter dem Formularnamen.

   ODER

   Um die Textaufforderung auf einen einzelnen Abschnitt anzuwenden, klicken Sie auf das KI![Symbol „KI](assets/request-prompt-icon.png)Symbol neben dem Abschnittsnamen.

1. Fügen Sie den Text in das Eingabeaufforderungsfeld ein.
1. Klicken Sie **Formular ausfüllen**.

   Workfront generiert Vorschläge für das Formular.
1. Wählen Sie für jeden Feldvorschlag **Feld** Akzeptieren“ oder **Ablehnen** aus.

   ![Vorschlag annehmen oder ablehnen](assets/accept-reject-suggestion.png)

   ODER

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

   >[!NOTE]
   >
   >Alle nicht überprüften Vorschläge werden automatisch akzeptiert, wenn Sie die Anfrage senden.

### Beispiele für Textaufforderungen

Diese Beispiele zeigen Aufforderungen zu verschiedenen Möglichkeiten, wie die KI auf andere Projekte verweisen kann.

#### Verweisen auf eine frühere Kundenkampagne

>[!BEGINSHADEBOX]

Erstellen Sie eine ähnliche Kampagnenanfrage wie bei der Einführung im 2. Quartal, diesmal jedoch für den Unternehmensbereich Automotive. Beibehalten des Lieferumfangs und des Zielgruppenprofils.

>[!ENDSHADEBOX]

#### Aufbauen auf einem vorhandenen Projekt

>[!BEGINSHADEBOX]

Verwenden Sie das gleiche Setup, das wir beim Projektstart (Projektname) im letzten Frühjahr hatten. Ich möchte eine digitale Werbekampagne mit demselben Executive-Publikum durchführen, aber mit aktualisierten Daten für dieses Quartal.

>[!ENDSHADEBOX]

#### Wiederverwenden eines Stils aus einer früheren Leistung

>[!BEGINSHADEBOX]

Bereiten Sie eine Anfrage ähnlich der Sommerförderungskampagne vor, die wir im letzten Jahr ausgeführt haben (Kundenfirma). Konzentrieren Sie sich auf Social-Media-Assets, behalten Sie Spanisch als primäre Sprache bei und passen Sie das Budget auf 75.000 Dollar an.

>[!ENDSHADEBOX]

#### Erweitern auf einen älteren Kampagnentyp

>[!BEGINSHADEBOX]

Nehmen Sie die Webinar-Reihe (Name der Kampagne) aus dem 1. Quartal als Referenz. Ich möchte denselben Registrierungs-Workflow und dieselben Assets, aber dieses Mal ist das Thema „KI in der Finanzplanung“ und das Publikum sind junge Profis.

>[!ENDSHADEBOX]

#### Wiederholen einer Anfrage für ein anderes Produkt

>[!BEGINSHADEBOX]

Richten Sie eine Kampagnenanfrage genauso ein wie das von uns behandelte Rebranding-Projekt (Client-Unternehmen), ersetzen Sie jedoch durch (neues Client-Unternehmen) als Client. Sorgen Sie dafür, dass alle Ergebnisse mit dem Unternehmens-Branding übereinstimmen.

>[!ENDSHADEBOX]

#### Erzählstil mit impliziten Verweisen

>[!BEGINSHADEBOX]

Wir planen eine Kampagne, die der Holiday Social Ads ähnelt, die wir letztes Jahr geschaltet haben. Das Budget sollte etwa 50.000 sein, das Ziel sollte die Lead-Generierung sein, und die Ergebnisse sollten Instagram- und TikTok-Assets umfassen.

>[!ENDSHADEBOX]


## Abrufen von Vorschlägen basierend auf einem hochgeladenen Dokument

Das Ausfüllen eines Formulars mit KI kann eine Anfrage mithilfe von Eingabeaufforderungen ausfüllen, oder Dokumente können Feldwerte basierend auf einem hochgeladenen Dokument vorschlagen.

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
<li>ODP</li>
</ul>
</td>
<td>
<ul>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
<li>PPTX</li>
</ul>
</td>
<td>
<ul>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>WEBP</li>
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
<td><b>Unterstützte </b><br> Formularausfüllung mit KI kann ausfüllen</td>
<td><b>Nicht unterstützt</b> <br>Formularausfüllen mit KI wird nicht ausgefüllt</td>
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

Beachten Sie beim Hochladen eines Dokuments zum Ausfüllen eines KI-Formulars Folgendes:

* Das Ausfüllen von KI-Formularen ist derzeit für das lateinische Alphabet optimiert.
* Es wird empfohlen, eine Textgröße von 8 Punkten oder mehr zu verwenden.
* Das Ausfüllen von KI-Formularen kann Probleme mit Bildern im Dokument haben, z. B. gedrehte oder verzerrte Bilder, Diagramme und das Zählen oder Verwenden räumlicher Gründe für Objekte in Bildern.
* Wie immer empfehlen wir, die Ergebnisse vor dem Senden der Anfrage auf Korrektheit zu überprüfen.

### Dokument hochladen, um eine Anfrage automatisch auszufüllen

Sie können ein Dokument hochladen, das auf das gesamte Formular oder auf einen einzelnen Abschnitt des Formulars angewendet werden soll.

1. Erstellen Sie eine Anfrage.

   Anweisungen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Um das Dokument auf das gesamte Formular anzuwenden, klicken Sie auf das KI![Symbol „KI](assets/request-prompt-icon.png) unter dem Formularnamen.

   ODER

   Um das Dokument auf einen einzelnen Abschnitt anzuwenden, klicken Sie auf das KI![Symbol „KI](assets/request-prompt-icon.png)Symbol neben dem Abschnittsnamen.

1. Klicken Sie **Dateien hochladen** und wählen Sie dann die Datei aus Ihrem Datei-Manager aus.

   ODER

   Ziehen Sie das Dokument aus Ihrem Datei-Manager in das Feld **Dateien hochladen, um das Anfrageformular automatisch**.
1. Klicken Sie **Formular ausfüllen** oder **Abschnitt ausfüllen**.

   Workfront generiert Vorschläge für das Formular.
1. Wählen Sie für jeden Feldvorschlag **Feld** Akzeptieren“ oder **Ablehnen** aus.

   ![Vorschlag annehmen oder ablehnen](assets/accept-reject-suggestion.png)

   ODER

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

   >[!NOTE]
   >
   >Alle nicht überprüften Vorschläge werden automatisch akzeptiert, wenn Sie die Anfrage senden.

## Fehlerbehebung

Wenn Sie nicht die erwarteten Vorschläge erhalten, kann dies auf eine der folgenden Ursachen zurückzuführen sein:

* Sie müssen mindestens einen Monat an Anfragedaten im System haben, bevor es Feldwerte aus früheren Anfragen vorschlagen kann.
* Sie haben möglicherweise die Leitplanken für den Dokument-Upload nicht befolgt, wenn Sie ein Dokument hochladen, aus dem Sie Vorschläge abrufen möchten. Weitere Informationen finden Sie unter [Leitplanken beim Hochladen von Dokumenten](#document-upload-guardrails) in diesem Artikel.
