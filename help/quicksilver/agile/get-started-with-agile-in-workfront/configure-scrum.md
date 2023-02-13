---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Konfigurieren von Scrum
description: Sie können die folgenden Optionen für Scrum-agile-Teams während oder nach der Erstellung des Teams konfigurieren.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 0%

---

# Konfigurieren [!UICONTROL Scrum]

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

>[!NOTE]
>
>Diese Einstellung kann nicht geändert werden, wenn das Team über laufende Iterationen verfügt.

Sie können Geschichten so konfigurieren, dass sie entweder anhand von Punkten oder Stunden geschätzt werden.

So konfigurieren Sie, wie Geschichten für Ihr agile Team geschätzt werden:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!UICONTROL Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** und wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.\
   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Agile]** im Abschnitt **[!UICONTROL Geschätzte Meldungen in]** festlegen, ob Sie Punkte oder Stunden zur Schätzung der Größe (Arbeitslast) von Meldungen verwenden möchten. Wenn Sie Punkte auswählen, geben Sie an, wie viele Stunden 1 Punkt entsprechen. (Der Standardwert ist 1 Punkt = 8 Stunden.) Dies ist die Anzahl der geplanten Stunden, die der Meldung hinzugefügt werden.

   **Beispiel:** Wenn Sie sich dafür entschieden haben, Geschichten in Punkten und 1 Punkt gleich 8 Stunden zu schätzen, und eine Geschichte auf 3 Punkte geschätzt wird, werden 24 geplante Stunden zu der Geschichte hinzugefügt.

1. Klicken **[!UICONTROL Änderungen speichern]**.

## Statusspalten auf der agilen Story-Pinnwand konfigurieren

Sie können konfigurieren, welche Spalten auf der agilen Story-Pinnwand für alle Iterationen angezeigt werden, die Ihrem Team zugewiesen sind, oder für ein bestimmtes Projekt.

* [Konfigurieren von Statusspalten für Iterationen](#configure-status-columns-for-iterations)
* [Konfigurieren von Statusspalten für Projekte](#configure-status-columns-for-projects)

### Konfigurieren von Statusspalten für Iterationen {#configure-status-columns-for-iterations}

Sie können die Status definieren, die auf der Story-Pinnwand für das agile Team vorhanden sind. Dies sind die einzigen Status, die auf dem Storyboard angezeigt werden.

So definieren Sie die Status, die für die mit dem agile Team verknüpfte Story-Pinnwand verfügbar sind:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Agile]** -Abschnitt, suchen Sie die **[!UICONTROL Story Board]** Bereich.

1. (Optional) Klicken Sie auf **[!UICONTROL Spalte hinzufügen]** , um eine zusätzliche Statusspalte zum Storyboard hinzuzufügen.
1. (Optional) Ziehen Sie eine Statusspalte mit der Drag &amp; Drop-Anzeige, um die Statusspalten auf der Story-Pinnwand neu anzuordnen. Die erste Spalte kann nicht verschoben werden und Sie können keine andere Spalte vor die erste Spalte ziehen.

   ![Drag &amp; Drop](assets/agile-story-card-drag-and-drop.png)

1. Wählen Sie sowohl den Status der Aufgabe als auch des Problems aus. Aufgabenstatus werden als Spaltentitel für jede Spalte auf der Story-Pinnwand angezeigt. Der Problemstatus, den Sie für die Zuordnung zum Aufgabenstatus auswählen. Wenn Sie also ein Problem in eine andere Spalte des Storyboards verschieben, ändert sich der Problemstatus in den hier gezeigten Problemstatus und nicht in den Namen der Spalte im Storyboard (der den Aufgabenstatus widerspiegelt).

   >[!IMPORTANT]
   >
   >Es stehen nur gesperrte systemweite Status zur Auswahl zur Verfügung. Sie können keine gruppenspezifischen Status auswählen. Der Status der ersten Spalte entspricht immer **[!UICONTROL Neu]**.

   Sie können benutzerdefinierte Status hinzufügen, wenn Ihre [!DNL Workfront] -Administrator hat sie konfiguriert; benutzerdefinierte Status können wie unter [Erstellen oder Bearbeiten eines Status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >Bei der Auswahl des Problemstatus wird in der dritten Spalte immer standardmäßig [!UICONTROL Geschlossen]. Wenn Sie über mehr als drei Spalten verfügen, müssen Sie die Spalten manuell aktualisieren, um den korrekten Status widerzuspiegeln.

1. Klicken **[!UICONTROL Änderungen speichern]**.

### Konfigurieren von Statusspalten für Projekte {#configure-status-columns-for-projects}

Informationen zum Konfigurieren von Statusspalten für ein Projekt finden Sie im Abschnitt . [Erstellen oder Anpassen von [!UICONTROL Agile] Ansicht](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) im Artikel [Erstellen oder Bearbeiten von Ansichten in [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

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

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!UICONTROL Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.\
   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Agile]** -Abschnitt einen Feldnamen eingeben, um ihn zu finden.

   ![Zusätzliche Felder](assets/agile-additional-fields-scrum.png)

1. Wählen Sie den Namen des Felds aus, das Sie hinzufügen möchten.
1. Geben Sie die **[!UICONTROL Anzeigename]** für das Feld, das auf der Meldung oder der Ausgabekarte angezeigt wird.
1. Klicken **[!UICONTROL Änderungen speichern]**.

## Konfigurieren der Verwendung von Farbindikatoren für Meldungen auf der Landingpage

Standardmäßig sind die Story-Pinnwände in einer agilen Iteration entsprechend dem Projekt, mit dem die Geschichte verknüpft ist, farbcodiert. Jedem Projekt wird eine beliebige Farbe auf dem Story Board zugewiesen. Sie können dieses Standardverhalten für jedes agile Team ändern. Farben für agile Geschichten können mit der Priorität einer Geschichte, dem Besitzer usw. verknüpft werden.

So ändern Sie das Verhalten, wie Farben Geschichten für ein agiles Team zugewiesen werden:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Im [!UICONTROL Agile] im Abschnitt [!UICONTROL Kartenfarbe zuordnen zu] -Bereich aus den folgenden Optionen auswählen:

   * **[!UICONTROL Projekt]**: Farben sind mit dem Projekt verknüpft, an das die Geschichte gebunden ist. (Wenn eine Geschichte erstellt wird, muss sie mit einem Projekt verknüpft sein, wie unter [Erstellen einer Agile Story](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Alle Aufgaben desselben Projekts werden in derselben Farbe angezeigt.
   * **[!UICONTROL Kostenlose Form]**: Alle Karten werden standardmäßig als blau angezeigt, bis ein Benutzer die Farbe manuell ändert, wie unter [[!UICONTROL Kategorisieren von Meldungen nach Farbe] auf der Scrum-Pinnwand](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Priorität]**: Farben sind mit der Priorität der Geschichte wie folgt verknüpft:

      * Hoch = Rot
      * Mittel = Gelb
      * Niedrig = Grün\

         Wenn Ihr Systemadministrator benutzerdefinierte Prioritäten für Ihre [!DNL Workfront] -System ist die höchste Priorität rot, die zweithöchste gelb und die dritthöchste grün.
   * **[!UICONTROL Aufgabeneigentümer]**: Alle Geschichten mit dem gleichen Hauptverantwortlichen haben dieselbe Farbe. Der primäre Verantwortliche ist der Benutzer, der der Aufgabe zuerst zugewiesen wurde.


1. Klicken **[!UICONTROL Änderungen speichern]**.

## Konfigurieren der Anwendung von Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration

Wenn Sie ein Arbeitselement zu einer Scrum-Iteration hinzufügen, werden das geplante Startdatum und das geplante Abschlussdatum des Arbeitselements standardmäßig so geändert, dass sie mit dem Start- und Enddatum der Iteration übereinstimmen. Sie können die ursprünglichen Daten für alle Arbeitselemente des Teams beibehalten.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe] Workfront, und klicken Sie dann auf **[!UICONTROL Teams]**.
1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.\
   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.
1. Im [!UICONTROL Agile] im Abschnitt [!UICONTROL Wenn ein Arbeitselement zu einer Iteration hinzugefügt wird] -Bereich aus den folgenden Optionen auswählen:

   * **[!UICONTROL Ändern Sie das geplante Startdatum und das geplante Abschlussdatum entsprechend dem Start- und Enddatum der Iteration.]**: Wenn Arbeitselemente zu einer Iteration hinzugefügt werden, werden die Arbeitselementdaten in die Iterationsdaten geändert.\

      Weiterführende Informationen zur Änderung von Datumsangaben finden Sie im Abschnitt . [Erfahren Sie, wie sich das Hinzufügen von Meldungen auf Aufgabendaten auswirkt](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) im Artikel [Hinzufügen von Meldungen zu einer vorhandenen Iteration](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL Ändern Sie weder das geplante Startdatum noch das geplante Abschlussdatum entsprechend dem Start- und Enddatum der Iteration.]**: Wenn Arbeitselemente einer Iteration hinzugefügt werden, behalten die Arbeitselemente ihre ursprünglichen Daten bei.

   Wenn Sie die Datumsoption ändern, werden die Daten für Arbeitselemente, die sich bereits in der Iteration befinden, nicht angepasst.

   Diese Optionen können sich auf das Datum auswirken, an dem Teams den Iterationen der anderen Arbeitselemente zuweisen. Beispielsweise ändert Team A die Arbeitselementdaten in die Iterationsdaten und Team B ändert die Arbeitselementdaten nicht. Wenn Team B der Iteration von Team A ein Arbeitselement zuweist, werden die Daten der Arbeitselemente geändert. Wenn jedoch Team A der Iteration von Team B ein Arbeitselement zuweist, ändern sich die Daten nicht.

1. Klicken **[!UICONTROL Änderungen speichern]**.
