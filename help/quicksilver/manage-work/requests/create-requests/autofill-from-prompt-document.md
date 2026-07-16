---
title: Verwenden der KI-gestützten Formularausfüllung zum Ausfüllen einer Anfrage mithilfe von Prompts oder Dokumenten
content-type: reference
description: Sie können KI zum automatischen Ausfüllen von Anfragefeldern verwenden, indem Sie eine Eingabeaufforderung eingeben oder ein Dokument angeben.
author: Alina, Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Z2t6RQBsQZK6MNRd3w2gWEY8k9YU48Jsco7pev7papM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 07a00836f60ce0bb4ee7fb0202c9458b0c1be406
workflow-type: tm+mt
source-wordcount: 1495
ht-degree: 7%

---

# Verwenden der KI-gestützten Formularausfüllung zum Ausfüllen einer Anfrage mithilfe von Prompts oder Dokumenten

>[!NOTE]
>
>Um diese Funktion nutzen zu können, muss Ihr Unternehmen die Anforderungen für die Verwendung des Workfront AI Assistant erfüllen. Weitere Informationen finden Sie unter [Voraussetzungen für den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

Mit KI-Formularausfüllen können Sie Anfragefelder basierend auf einer von Ihnen eingegebenen Eingabeaufforderung automatisch ausfüllen. Es kann auch Felder basierend auf Text ausfüllen, z. B. E-Mails oder hochgeladene Dokumente. Sie können diese Vorschläge vor dem Absenden der Anfrage genehmigen oder ablehnen.

Diese Funktion ist beim Erstellen einer Anfrage im Bereich Workfront-Anfragen sowohl für Workfront- als auch für Workfront Planning-Anfragen verfügbar.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront- oder Workflow-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p>
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

Um das Ausfüllen eines Formulars mit KI mithilfe einer Eingabeaufforderung oder eines Dokuments zu ermöglichen, müssen **alle** der folgenden Bedingungen erfüllt sein:

<!--
Remove me October 2026
* Your organization must have migrated to Adobe IMS (Identity Management System)
* The Adobe Unified Experience must be enabled
-->
* Ihr Unternehmen muss über ein Select-, Prime- oder Ultimate Workfront- oder Workflow-Paket verfügen
* Bei Adobe muss eine unterzeichnete Adobe GenAI-Vereinbarung hinterlegt sein

  Weitere Informationen zum Unterzeichnen des Vertrags finden Sie unter [Unterschreiben des Adobe Gen AI-](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)) im Artikel KI-Assistent - Übersicht.
* Der KI-Assistent muss in den Systemeinstellungen Ihrer Organisation aktiviert sein. Dieser wird von Ihrem Workfront-Administrator verwaltet.

  Weitere Informationen zum Aktivieren des KI-Assistenten in den Systemeinstellungen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Überlegungen zur Verwendung von Formularausfüllen mit KI

Beachten Sie bei der Verwendung von Formularausfüllen auf Basis von KI Folgendes

* KI-Formularausfüllung überschreibt keine Felder, die Sie bereits ausgefüllt haben.
* Benutzer erhalten keine Vorschläge für Daten, auf die sie sonst keinen Zugriff hätten.
* Felder, die von berechneten Daten abhängen, werden nicht unterstützt. Wenn beispielsweise Feld A ein berechnetes Feld ist und die Optionen von Feld B von Feld A abgeleitet sind, kann Feld B nicht automatisch ausgefüllt werden.

<!--
* Files that you use in Form Fill powered by AI are uploaded to Azure storage for 24 hours. This is necessary for document processing. 
* All files uploaded to Azure are currently stored in US Azure clusters for the 24 hour storage window. 
-->

## Aktivieren von Formularausfüllen mit KI für Ihre Organisation

>[!NOTE]
>
>Das Ausfüllen von Formularen mit künstlicher Intelligenz ist auf Organisationsebene aktiviert und kann für bestimmte Benutzer oder Zugriffsebenen nicht aktiviert oder deaktiviert werden.

Weitere Informationen finden Sie [Konfigurieren von Systemvoreinstellungen](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

<!--

This should point to the System Preferences article, since it's not a user function: 

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Click **System**, then under System, click **Preferences**.
1. In the AI preference section, turn on the **Enable AI** setting.
1. Turn on the **AI Form Fill** setting.
1. To disable Form Fill powered by AI, turn off **AI Form Fill**.

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

Das Ausfüllen von Formularen mit KI kann eine Anfrage mithilfe von Eingabeaufforderungen ausfüllen oder Feldwerte basierend auf einem hochgeladenen Dokument vorschlagen.

Diese Art von Vorschlag überprüft auch frühere Anfragen nach ähnlichen Kontexten. Wenn in der Eingabeaufforderung beispielsweise erwähnt wird, dass die Anfrage für einen bestimmten Client gilt, kann Workfront die Rechnungsadresse für diesen Client basierend auf vorherigen Anfragen automatisch suchen und eingeben.

### Leitplanken beim Hochladen von Dokumenten

#### Unterstützte Dateitypen

Die folgenden Dateitypen werden unterstützt:

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
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
<li>Externer Lookup</li>
<li>Interne Suche</li>
<li>Referenz</li>
<li>Eingebettete Workfront-Felder planen</li>
</ul>
</td>
<td><li>Typeahead</li>
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
* Mit KI-Formularausfüllen kann ein externer Wert für ein Suchfeld ausgefüllt werden. Wenn das externe Suchfeld jedoch eine Abhängigkeit von einem Formelfeld aufweist, kann die KI die Feldoptionen nicht genau abrufen und füllt diesen Feldwert nicht aus.


