---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Kanban konfigurieren
description: Sie können die folgenden Optionen für agile Kanban-Teams während oder nach der Erstellung des Teams konfigurieren.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# Konfigurieren [!UICONTROL Kanban]

Sie können die folgenden Optionen für agile Teams während oder nach der Erstellung des Teams konfigurieren. Sie erstellen ein agiles Team (Kanban oder Scrum) in [!DNL Adobe Workfront] wie in [Erstellen eines agilen Teams](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Konfigurieren, ob Meldungen in Punkten oder Stunden geschätzt werden

Sie können Geschichten so konfigurieren, dass sie entweder anhand von Punkten oder Stunden geschätzt werden.

So konfigurieren Sie, wie Geschichten für Ihr agile Team geschätzt werden:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** und wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.\
   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Agile]** im Abschnitt **[!UICONTROL Geschätzte Meldungen in]** festlegen, ob Sie Punkte oder Stunden zur Schätzung der Größe (Arbeitslast) von Meldungen verwenden möchten. Wenn Sie Punkte auswählen, geben Sie an, wie viele Stunden 1 Punkt entsprechen. (Der Standardwert ist 1 Punkt = 8 Stunden.) Dies ist die Anzahl der geplanten Stunden, die der Meldung hinzugefügt werden.

   **Beispiel:** Wenn Sie sich dafür entschieden haben, Geschichten in Punkten und 1 Punkt gleich 8 Stunden zu schätzen, und eine Geschichte auf 3 Punkte geschätzt wird, werden 24 geplante Stunden zu der Geschichte hinzugefügt.

1. Klicken **[!UICONTROL Änderungen speichern]**.

## Statusspalten auf der agilen Story-Pinnwand konfigurieren

Sie können die Status definieren, die auf der Story-Pinnwand für das agile Team vorhanden sind. Dies sind die einzigen Status, die auf dem Storyboard angezeigt werden.

So definieren Sie die Status, die für die mit dem agile Team verknüpfte Story-Pinnwand verfügbar sind:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!UICONTROL Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Agile]** -Abschnitt, suchen Sie die **[!UICONTROL Story Board]** Bereich.

1. (Optional) Klicken Sie auf **[!UICONTROL Spalte hinzufügen]** , um eine zusätzliche Statusspalte zum Storyboard hinzuzufügen.
1. (Optional) Ziehen Sie eine Statusspalte mit der Drag &amp; Drop-Anzeige, um die Statusspalten auf der Story-Pinnwand neu anzuordnen. Die erste Spalte kann nicht verschoben werden und Sie können keine andere Spalte vor die erste Spalte ziehen.

   ![Drag &amp; Drop](assets/agile-story-card-drag-and-drop.png)

1. Wählen Sie den Aufgabenstatus aus.

   >[!IMPORTANT]
   >
   >Es stehen nur gesperrte systemweite Status zur Auswahl zur Verfügung. Sie können keine gruppenspezifischen Status auswählen. Der Status der ersten Spalte entspricht immer **[!UICONTROL Neu]**.

   Sie können benutzerdefinierte Status hinzufügen, wenn Ihre [!DNL Workfront] -Administrator hat sie konfiguriert; benutzerdefinierte Status können wie unter [Erstellen oder Bearbeiten eines Status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicken **[!UICONTROL Änderungen speichern]**.

## Zusätzliche Felder konfigurieren, die auf den Storykarten auf der Karte für Mobilgeräte angezeigt werden sollen

Wenn Sie Felder zu Storykarten hinzufügen, sind die Felder beim Ausfüllen des Felds schreibgeschützt und nur sichtbar.

Standardmäßig werden die folgenden Datentypen auf der Storykarte für Aufgaben und Probleme angezeigt:

* Name der Meldung mit einem Link direkt zur Aufgabe oder zum Problem
* Der Projektname mit einem Link direkt zum Projekt
* Dieser Link wird nur für Meldungen angezeigt, nicht für Unteraufgaben
* Aufgabenbeschreibung oder Problembeschreibung
* Aktuelle Zusage
* Anzeigen und Bearbeiten der prozentualen Vollständigkeit entweder durch Anpassung der prozentualen Vollständigkeit selbst oder durch Anpassung der Anzahl der vollständigen Punkte oder Stunden
* Zugewiesene Benutzer

Sie können zusätzliche Daten (einschließlich benutzerdefinierter Daten) auf Storykarten anzeigen. Sie können aus verschiedenen Gründen zusätzliche Felder auf Storykarten anzeigen lassen. Beispielsweise können Sie die Kunden-ID anzeigen, wenn Sie innerhalb der Iteration an Geschichten für mehrere Kunden arbeiten, oder das Projekt-Startdatum oder das Projekt-Abschlussdatum anzeigen möchten.

>[!NOTE]
>
>Wenn Sie ein benutzerdefiniertes Feld auf einer Storykarte verwenden, darf es keinen Punkt/Punkt im Namen enthalten.

So konfigurieren Sie dem agile Team zugewiesene Storykarten, um zusätzliche Felder anzuzeigen:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.\
   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Agile]** -Abschnitt einen Feldnamen eingeben, um ihn zu finden.

   ![Zusätzliche Felder](assets/agile-additional-fields-kanban.png)

1. Wählen Sie den Namen des Felds aus, das Sie hinzufügen möchten.
1. Geben Sie die **[!UICONTROL Anzeigename]** für das Feld, das auf der Meldung oder der Ausgabekarte angezeigt wird.
1. Klicken **[!UICONTROL Änderungen speichern]**.

## Konfigurieren der Grenze für laufende Arbeit (WIP)

Kanban in [!DNL Workfront] ermöglicht Ihnen, die Arbeitszeit des Teams zu steuern, indem Sie die Anzahl der Aufgaben begrenzen, die in der [!UICONTROL In Bearbeitung] in der Spalte [!UICONTROL Kanban] Pinnwand.

Wenn das WIP-Limit konfiguriert ist, können Sie das WIP-Limit anzeigen oder es sogar über die [!UICONTROL Kanban] Landingpage, wie beschrieben in [Verwalten Sie die Grenze für laufende Arbeiten (WIP) auf der [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

So begrenzen Sie die WIP für Ihr Kanban-Team:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Kanban-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Agile]** im Abschnitt **[!UICONTROL Methode]** -Abschnitt, stellen Sie sicher, dass Kanban ausgewählt ist.

1. Im **[!UICONTROL Story Board]** im Abschnitt **[!UICONTROL WIP LIMIT]** -Feld die maximal zulässige Anzahl von Elementen in jeder Spalte der [!UICONTROL Kanban] agile Story Board. Sie können für jede Spalte einen anderen Grenzwert festlegen. Die Höchstgrenze, die Sie für jede Spalte festlegen können, beträgt 100.\
   Wenn diese Einstellung festgelegt ist, zeigt das WIP-Limit eine Warnmeldung auf der [!UICONTROL Kanban] agile Storyboard jedes Mal, wenn die Grenze für eine Spalte auf der Storyboard überschritten wird. Diese Warnmeldung wird nur angezeigt, wenn das WIP-Limit zum ersten Mal überschritten wird. Diese Warnmeldung wird nicht für Spalten angezeigt, deren Status mit [!UICONTROL Fertig].\
   Das WIP-Limit ist lediglich eine visuelle Warnung und schränkt Ihr Team nicht ein, mehr Elemente in einer Spalte als das von Ihnen festgelegte Limit zu haben.

   ![WIP-Beschränkung](assets/wip-limit-350x193.png)

1. Klicken **Änderungen speichern**.

## Konfigurieren von Storys, die automatisch aus dem Backlog hinzugefügt werden sollen

Sie können Storys aus dem Backlog so konfigurieren, dass sie automatisch zur ersten Spalte auf der [!UICONTROL Kanban] -Pinnwand unmittelbar nachdem ein Element aus dieser Spalte verschoben wurde.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Kanban-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Auswählen **[!UICONTROL Automatisch nächsten Story aus dem Backlog hinzufügen]** , um Meldungen zu konfigurieren, die automatisch aus dem Rückstand zur ersten Spalte auf der [!UICONTROL Kanban] Story Board.

   Dies geschieht jedes Mal, wenn eine Meldung in eine Spalte auf der Storyboard verschoben wird, die den Status Abgeschlossen darstellt (Status, der mit Abgeschlossen übereinstimmt). Wenn die Meldung aus dem Rückstand hinzugefügt wird, wird die Meldung mit der höchsten Priorität zum Storyboard hinzugefügt. Wählen Sie diese Option aus, um das nächste Element aus dem Rückstand zu konfigurieren, das automatisch zum **[!UICONTROL In Bearbeitung]** Spalte, wenn ein Element aus der **[!UICONTROL In Bearbeitung]** Spalte.

1. Klicken **[!UICONTROL Änderungen speichern]**.

## Konfigurieren Sie, wie lange Karten auf der Seite bleiben [!UICONTROL Kanban] Pinnwand

Sie können festlegen, wie lange abgeschlossene Karten auf der [!UICONTROL Kanban] Pinnwand. Aufgaben, die von der [!UICONTROL Kanban] Die Pinnwand kann weiterhin in ihrem ursprünglichen Projekt aufgerufen werden.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Kanban-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie das Kanban-Team aus.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **Edit**.

   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Anzahl der Tage Abgeschlossene Karten bleiben auf der Kanban-Pinnwand]** aus.
1. Klicken **[!UICONTROL Änderungen speichern]**.
