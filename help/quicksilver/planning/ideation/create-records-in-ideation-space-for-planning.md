---
title: Erstellen von Planungsdatensätzen aus Ideation Space Briefs
description: Mit der Ideation Space, einer neuen Funktion von Adobe Workfront Planning, können Sie Briefs in Planungsunterlagen umwandeln. Exportierte Briefs erstellen neue Datensätze oder aktualisieren vorhandene. In diesem Artikel wird beschrieben, wie Sie mit dem Ideation-Bereich vorhandene Planungsdatensätze erstellen oder bearbeiten können.
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 2%

---


# Erstellen von Planungsdatensätzen aus Ideation Space Briefs

<!--
Will this release JUST to preview? If not - hide the preview portion below
-->

<!--
I started with this under Records first but what if Ideation will be added to other products and it will generate record types in those products? keep it here so it can be moved, if needed, to a standalone product one day?
-->

<!--
*********************** IMPORTANT ***************
THIS ARTICLE HAS 2 DRAFTS IN 2 SEPARATE AREAS FROM CLAUDE - THEY WERE CREATED AT DIFFERENT TIMES - WHICH ONE WOULD YOU KEEP OR MERGE THEM INTO ONE ARTICLE
-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Es ist nur im Rahmen des Programms **Ideation Space Beta** verfügbar. </span>

<span class="preview">Weitere Informationen finden Sie unter [Erste Schritte mit dem Ideenraum für Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Mit der Ideation Space, einer neuen Funktion von Adobe Workfront Planning, können Sie Briefs in Planungsunterlagen umwandeln. Exportierte Briefs erstellen neue Datensätze oder aktualisieren vorhandene.

In diesem Artikel wird beschrieben, wie Sie mit dem Ideation-Bereich vorhandene Planungsdatensätze erstellen oder bearbeiten können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul> 
<li><p>Beliebige Workfront oder Workflows mit einem Planungspaket</p></li>
ODER
<li><p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Zusätzliche Produkte</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workflow-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> 
   <ul>
   <li><p>Sie müssen der Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p>   </li>
   <li><p>Die Einstellung Ideenraum deaktivieren in Ihrer Zugriffsebene muss deaktiviert sein</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Tragen Sie Berechtigungen oder höhere Berechtigungen zum Arbeitsbereich und Datensatztyp bei, dem Sie Datensätze hinzufügen möchten </p>
      <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
      <p>Anzeigen von Berechtigungen für Workfront-Objekte, um sie zu Briefs hinzuzufügen <!--not sure if this is available--></p>
      <p>Editor-Berechtigungen für den Ideenraum zum Erstellen von Briefs</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing-Benutzerrollen</p></td> 
   <td><p><ul><li>Jede GenStudio-Benutzerrolle für den Zugriff auf Kampagnen, Produkte und Personas</li>
   <li>GenStudio System Manager für den Zugriff auf Aktivierungen <!--and Events--></li></ul>
   Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Benutzerrollen und -berechtigungen</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Überlegungen zur Verwendung des Ideenraums zum Erstellen von Datensätzen

* Sie können den Ideationsbereich nur von Workfront Planning aus starten, während Sie Datensätze erstellen oder bearbeiten. Der Ideationsraum existiert außerhalb von Workfront Planning nicht.
* Für den Zugriff auf den Ideationsbereich sind ein Arbeitsbereich und ein Datensatztyp in Workfront Planning erforderlich.
* Neue Datensätze beginnen immer mit Platzhalterinhalten, unabhängig davon, wie Sie sie erstellen.
* Wenn Sie einen Planungsdatensatz löschen, der mit einer Ideenübersicht verknüpft ist, bleibt die Übersichtsübersicht im Ideenraum, und die zugehörige Arbeitsfläche im Ideenraum wird nicht gelöscht.
* Die Synchronisation von Informationen erfolgt nur vom Ideationsraum bis zur Workfront-Planung. Es gibt keine Rückwärts- oder automatische Synchronisation von einem Planungsdatensatz mit der Ideation Space Brief.
* Die folgenden Szenarien treten auf, wenn Felder in Workfront Planning erstellt, bearbeitet oder entfernt werden:

  * Neue Felder, die für Datensätze erstellt wurden, die mit Ideenbeschreibungen verknüpft sind, werden täglich zur Zusammenfassung hinzugefügt. Neue Felder erscheinen leer in der Ideenbeschreibung.
  * Entfernte Felder bleiben auf dem Brief und behalten ihre vorherigen Werte.
  * Umbenannte Felder aktualisieren ihre Namen in der Zusammenfassung.
* Sie können Dokumente als Karten im Ideationsbereich hinzufügen. Dazu gehören auch Bilder.

  Die folgenden Dateitypen werden unterstützt: PDF, Excel, CSV, PNG (und andere Bildformate), Word, PowerPoint. Videos werden nicht unterstützt.

  Alle hochgeladenen Dokumente werden im Backend zur Verarbeitung in PDF konvertiert.
* Sie können Datensätze direkt aus Workfront Planning per Drag-and-Drop in den Bereich ziehen, sodass sie wie manuell hochgeladene Dateien aussehen.

## Erstellen von Datensätzen mithilfe des Ideationsbereichs

1. Klicken Sie auf der Landingpage von Workfront Planning auf die Karte für einen Arbeitsbereich, den Sie verwalten können.
1. Klicken Sie auf die Karte für einen Datensatztyp, dem Sie Datensätze hinzufügen können.
1. Führen Sie einen der folgenden Schritte aus, um einen Datensatz zu erstellen:

   * Klicken Sie in einer beliebigen Ansicht der Seite mit dem Datensatztyp auf **Neuer Datensatz** in der oberen rechten Ecke der Seite und im Feld **Wählen Sie eine Methode zum Hinzufügen Ihrer Datensätze aus** klicken Sie auf **Öffnen Sie den Ideationsbereich** und klicken Sie dann auf **Fortfahren**.
   * Scrollen Sie nach unten in der Datensatztabelle, klicken Sie auf **Neue Zeile** und dann auf **Ideationsbereich öffnen**.

     >[!TIP]
     >
     >Wenn Sie **Nicht anzeigen** auswählen, wird die zukünftige Eingabeaufforderung endgültig geschlossen. Wenn Sie auf das Schließen **Symbol (X** klicken, wird dieses Feld geschlossen, aber es wird wieder angezeigt, wenn Sie das nächste Mal einen Inline-Datensatz hinzufügen.

   ![Neues Eintragsfeld mit der Schaltfläche „Ideationsraum öffnen“](assets/new-record-creation-picker-with-ideation.png)

   Der Bereich Ideen wird in einer neuen Registerkarte mit einer leeren Eingabeaufforderung geöffnet.

   Der Datensatz wird sofort mit Platzhaltertext erstellt.

1. (Optional) Klicken Sie im **auf** Vorhandene Zusammenfassung verwenden“, um ein vorhandenes Dokument zu suchen und hinzuzufügen, das der Ideationsbereich zum Erstellen der Zusammenfassung und des zukünftigen Datensatzes verwendet.

   ![Leere kurze Eingabeaufforderung für Ideen](assets/empty-ideation-prompt.png)

1. (Optional) Klicken Sie auf **Vorherige Arbeitsflächen öffnen** <!--accurate??--> Symbol ![Vorhandene Briefs öffnen](assets/open-existing-briefs-icon.png) in der oberen rechten Ecke des Eingabeaufforderungsfelds, um vorhandene Briefs zu öffnen

1. In der **Woran arbeiten Sie?** Im Eingabeaufforderungsfeld wird beschrieben, welche Art von Datensatz erstellt werden soll.

   Je mehr Details Sie teilen, desto nützlicher sind die Informationen aus dem Ideenraum. Geben Sie beispielsweise eine Beschreibung der geplanten Kampagne ein: „Zurück zur Schule für eine Marketing-Agentur“.

1. Klicken Sie **Ideating starten**.

   Der Ideationsbereich durchläuft die folgenden Schritte, während er Ihre Idee aufbaut: <!--check some of these in the UI - there might have been UI text changes-->

   1. Ihr Ziel und Kontext verstehen
   2. Überprüfen Sie Ihren Raum und ausgewählte Materialien
   3. Sammeln von Beweisen aus Dokumenten, Web und Daten
   4. Zusammenfassen der Ergebnisse in einer Forschungszusammenfassung
   5. Erstellen und Verfeinern von Karten mit Zitaten

   Während dieses Vorgangs sehen Sie den Ideation Space, der aktiv verbundene Workfront-Planungsdaten oder Informationen im Internet durchsucht.

   Sie kann beispielsweise nach vorhandenen Programmen, Produkten, Rollen oder Regionen sowie nach ähnlichen online verfügbaren Konzepten suchen. <!--check on this with Et-->

   Wenn die Idee abgeschlossen ist, werden die folgenden Dinge zum Ideationsraum hinzugefügt:

   * Eine Zusammenfassung der KI-Ergebnisse, die mit mehreren Karten verknüpft ist, mit detaillierten Informationen zu den zu berücksichtigenden Punkten. Die Detailkarten werden in einem neuen Abschnitt angezeigt. Ein Connector gibt an, welcher Kartenabschnitt zu welcher Zusammenfassung gehört.

   * Eine **Brief**-Datei in der linken unteren Ecke des Ideenraums. Die Zusammenfassung ist ein Entwurf des zukünftigen Datensatzes und wird als Detailseite eines Datensatzes angezeigt.

   ![Ideenkarte mit Verzweigungen](assets/ideation-card-with-branched-off-additional-cards.png)

1. Fügen Sie weitere Informationen zum Ideenraum hinzu, um die Erstellung Ihres Briefs abzuschließen.

1. (Bedingt) Wenn die Zusammenfassung abgeschlossen ist, klicken Sie auf das Vorschaubild in der linken unteren Ecke und dann auf eine der folgenden Aktionen:

   * **In Datei exportieren** um eine Datei zu erstellen
   * **In Workfront Planning exportieren**, um einen Planungsdatensatz zu erstellen

   Informationen zum Hinzufügen und Exportieren von Elementen zur Zusammenfassung finden Sie unter [Erstellen von Briefs im Bereich Ideen](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md).

   Dadurch wird die Erstellung des Datensatzes mit den zusätzlichen Informationen abgeschlossen und dem ursprünglich ausgewählten Datensatztyp hinzugefügt.

## Bearbeiten vorhandener Datensätze im Ideationsbereich

Sie können den Ideationsbereich aus vorhandenen Datensätzen öffnen, um sie zu aktualisieren.

Es ist nicht möglich, Datensätze im Ideationsbereich stapelweise zu bearbeiten.

1. Wechseln Sie zu einem vorhandenen Datensatz in Workfront Planning und öffnen Sie dessen Detailseite.

1. Klicken Sie **Öffnen im Ideationsbereich**. Dadurch wird der Ideationsbereich in einer neuen Registerkarte geöffnet.

   Wenn bereits eine Idee für den Datensatz vorhanden ist, wird dieser Bereich geöffnet.

   Wenn keine Idee existiert, erzeugt sie einen Ideenraum und eine kurze.

   >[!TIP]
   >
   >Massenbearbeitung von Datensätzen mit dem Ideationsbereich ist nicht verfügbar.

   <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->

1. Fahren Sie mit der Bearbeitung der Zusammenfassung fort, wie im Abschnitt [Erstellen von Datensätzen mithilfe des Ideenraums](#create-records-using-the-ideation-space) in diesem Artikel beschrieben.






<!-- this is from Claude, but rephrased and included most of this above: 

## Step 5: Open the Workfront Planning Records panel

To bring real Workfront Planning records into your canvas (rather than just AI-generated ideas), click the **records icon** in the left-hand toolbar (third icon down). This opens the **Workfront Planning Records** panel, listing all **Connected Record types** available in your Planning environment — for example:

- Products
- Regions
- Personas
- Channels
- Activations
- Project
- Test Record
- Experience Manager Assets

## Step 6: Drag real records onto the canvas

Search or browse within a record type (e.g., **Products** or **Personas**), then drag the record you want directly onto the canvas. In the example, an existing **Nike product** record and a **Deep testing** persona record were both dragged in and positioned near the relevant concept cards.

This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning, grounding the ideation in real data rather than hypothetical entities.


![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)

---

## Step 7: Refine with follow-up prompts

Use the **Ask anything** box in the bottom-right corner at any time to refine the canvas — for example, typing `regenerate` against a specific card to have Catalyze redo that section using updated context. Catalyze will re-run its reasoning steps (searching, synthesizing, citing) and update the affected cards in place.

---

## Step 8: Review the full canvas

Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.), and a **Campaign Brief** summary card in the corner pulling it all together.



![Full canvas overview](images/06_full_canvas_overview.png)

---

## Tips

- **Be specific in Step 2** — richer campaign descriptions produce more relevant, better-grounded cards.
- **Check citations** before trusting a generated fact — click **Sources** on any card.
- **Mix AI cards with real records** — dragging in actual Products, Personas, Regions, etc. keeps the canvas tied to your real Planning data, not just AI speculation.
- Responses are AI-generated and may be inaccurate — always verify against the linked sources before finalizing a record.

***************SECOND DRAFT FROM CLAUDE*******************
# Creating and Managing Records with Catalyze Ideation

> This workflow reflects the Closed Beta experience and is expected to evolve before Open Beta and GA. Confirm current behavior before publishing to customers.

This guide explains how to create and ideate on records using Catalyze within Workfront Planning. It covers all entry points, system behavior, data sync rules, and file-upload support.

## Before you start

- You must have access to a record list within Workfront Planning.
- Catalyze always opens in a **new browser tab** — this is consistent across every entry point.
- Any record created through Catalyze starts with **placeholder text** until you begin ideating.

## Option 1: Create a record via the top-level "New Record" button

1. Navigate to your record list in Workfront Planning.
2. Click the **New Record** button at the top of the page.
3. From the dropdown menu, select **Ideate in Catalyze**.
4. A new browser tab opens automatically, launching the Catalyze canvas.
5. A new record is created in Workfront Planning with placeholder text.
6. Begin ideation directly in Catalyze.

**Additional access from the record view:** Open the newly created record and, in its detail modal, click **Ideate in Catalyze**. This opens Catalyze in a new tab (same behavior as above).

## Option 2: Create a record via inline record creation (bottom of table)

1. Scroll to the bottom of the record table.
2. Click **New Record**.
3. The record is created immediately with placeholder text.
4. A pop-up appears with these options:
   - **Open Catalyze** — launches Catalyze in a new browser tab
   - **Don't Show Again** — permanently dismisses the future prompt
   - **X (Close)** — closes the pop-up; it will reappear next time
5. Click **Open Catalyze** to begin ideation.

## Working with existing records

**Contextual actions (bottom selection bar)**
- **Single record selected:** an "Ideate in Canvas" / "Open in Canvas" action appears.
  - If a canvas already exists, it opens that canvas.
  - If no canvas exists, it creates a new one.
- **Multiple records selected:** the Ideate/Open in Canvas action is **not available** — bulk ideation is not supported.

**Record detail panel**
- If no canvas is connected, an **Ideate in Catalyze** button appears in the record header.
- If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
- If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.

**When can you create a canvas for a record?**
A canvas can be created for a record that is in Workfront Planning and still in **draft** state (not yet marked "ready").

## Record deletion behavior

If a Planning record linked to a Catalyze canvas is deleted:
- The canvas remains intact in Catalyze.
- No data is removed from Catalyze.

## Data synchronization rules

**Sync direction:** One-way only, from Catalyze → Workfront Planning. There is no reverse or automatic sync from Planning back to Catalyze.

**Export process:**
1. In Catalyze, click **Export to Planning**.
2. Data is pushed to the connected Workfront Planning record.
3. The export **overwrites all existing field data** in the record.

**Important notes:**
- Changes made directly in Workfront Planning do **not** sync back to Catalyze.
- Data refresh in Workfront Planning is manual only (Beta behavior) — there is no scheduled/automatic sync.
- Schema updates do sync one direction: once connected, Planning schema changes propagate to Catalyze daily — added fields appear empty, removed fields keep their prior values, and renamed fields update in place.

## Uploading documents into the Catalyze canvas

- Files can be added as a "document card" on the canvas — this works the same whether the file is an image or another document type.
- You can drag and drop files directly from Workfront Planning onto the canvas, and they appear the same way as manually uploaded files.
- All uploaded documents are converted to PDF on the backend for processing.
- Supported file types (as of the Aug 2026 beta): **PDF, Excel, CSV, PNG (and likely other image formats), Word, PowerPoint.**
- **Not supported:** video files.
- You can include images directly in a prompt and Catalyze will recognize their content, though small-format legibility is still being refined.

## Key takeaways

- Use **Ideate in Catalyze** to connect records to the AI-assisted ideation workflow.
- Catalyze always launches in a separate browser tab.
- New records always start with placeholder content, regardless of entry point.
- Data flow between Catalyze and Planning is manual and one-directional (Catalyze → Planning).
- Deleting a Planning record does not delete its associated Catalyze canvas.

-->


<!--
Internal info: 

## The Ideation space and Adobe GenStudio

Adobe GenStudio for Performance Marketing is Adobe's end-to-end content supply chain solution, spanning five stages:

1. Strategy and Ideation
2. Workflow and Planning
3. Asset Management
4. Creation and Production
5. Delivery and Activation

The Ideation space fits in the **Strategy and Ideation** stage — the front door of the content supply chain — and is designed to work natively with the rest of GenStudio, so the briefs and strategic direction it generates flow directly into Workfront Planning for execution.
-->


