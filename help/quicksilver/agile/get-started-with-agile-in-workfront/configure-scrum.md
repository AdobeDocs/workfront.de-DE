---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Konfigurieren von Scrum
description: Sie können die folgenden Optionen für Scrum-agile-Teams während oder nach der Erstellung des Teams konfigurieren.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '1793'
ht-degree: 0%

---

# Konfigurieren von [!UICONTROL scrum]

Sie können ein agiles Team in [!DNL Adobe Workfront] erstellen, wie in [Erstellen eines agilen Teams](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md) beschrieben. Beim Erstellen eines agilen Teams können Sie die Methodik auswählen, die das Team zum Abschließen seiner Arbeit verwendet. Sie können aus den folgenden Optionen auswählen:

* Scrum
* Kanban

In diesem Artikel wird beschrieben, wie Sie die Einstellungen für ein Scrum-Team konfigurieren. Nachdem Sie ein agiles Team erstellt und die Scrum-Methode ausgewählt haben, können Sie in diesem Artikel die folgenden Einstellungen aktualisieren:

* Ob Meldungen in Punkten oder Stunden geschätzt werden
* Die Statusspalten auf der agilen Storyboard für Iterationen und Projekte
* Zusätzliche Felder, die auf den Storykarten auf der Karte für die agile Meldung angezeigt werden
* Verwendung von Farbindikatoren für Meldungen auf der Landingpage
* Anwenden von Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration

Informationen zum Konfigurieren eines Kanban-Teams finden Sie unter [Konfigurieren von Kanban](/help/quicksilver/agile/get-started-with-agile-in-workfront/configure-kanban.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Teams bearbeiten</p>  </td> 
  </tr>

</tbody> 
</table>

*Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben.

## Konfigurieren, ob Meldungen in Punkten oder Stunden geschätzt werden

>[!NOTE]
>
>Diese Einstellung kann nicht geändert werden, wenn das Team über laufende Iterationen verfügt.

Sie können Geschichten so konfigurieren, dass sie entweder anhand von Punkten oder Stunden geschätzt werden.

So konfigurieren Sie, wie Geschichten für Ihr agile Team geschätzt werden:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!UICONTROL Workfront] und klicken Sie dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   Nur Teammitglieder mit einer [!UICONTROL Plan] - oder [!UICONTROL Work] -Lizenz sehen diese Option.\
   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Wählen Sie im Abschnitt **[!UICONTROL Agile]** im Bereich **[!UICONTROL Geschichten schätzen in]** aus, ob Sie Punkte oder Stunden zur Schätzung der Größe (Arbeitslast) von Geschichten verwenden möchten. Wenn Sie Punkte auswählen, geben Sie an, wie viele Stunden 1 Punkt entsprechen. (Der Standardwert ist 1 Punkt = 8 Stunden.) Dies ist die Anzahl der geplanten Stunden, die der Meldung hinzugefügt werden.

   **Beispiel:** Wenn Sie ausgewählt haben, Geschichten in Punkten und 1 Punkt gleich 8 Stunden zu schätzen, und eine Geschichte auf 3 Punkte geschätzt wird, werden 24 geplante Stunden zur Geschichte hinzugefügt.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Statusspalten auf der agilen Story-Pinnwand konfigurieren

Sie können konfigurieren, welche Spalten auf der agilen Story-Pinnwand für alle Iterationen angezeigt werden, die Ihrem Team zugewiesen sind, oder für ein bestimmtes Projekt.

* [Konfigurieren von Statusspalten für Iterationen](#configure-status-columns-for-iterations)
* [Konfigurieren von Statusspalten für Projekte](#configure-status-columns-for-projects)

### Konfigurieren von Statusspalten für Iterationen {#configure-status-columns-for-iterations}

Sie können die Status definieren, die auf der Story-Pinnwand für das agile Team vorhanden sind. Dies sind die einzigen Status, die auf dem Storyboard angezeigt werden.

So definieren Sie die Status, die für die mit dem agile Team verknüpfte Story-Pinnwand verfügbar sind:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   Nur Teammitglieder mit einer [!UICONTROL Plan] - oder [!UICONTROL Work] -Lizenz sehen diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Suchen Sie im Abschnitt **[!UICONTROL Agile]** den Bereich **[!UICONTROL Meldungsbrett]** .

1. (Optional) Klicken Sie auf **[!UICONTROL Spalte hinzufügen]** , um eine zusätzliche Statusspalte zur Storyboard-Pinnwand hinzuzufügen.
1. (Optional) Ziehen Sie eine Statusspalte mit der Drag &amp; Drop-Anzeige, um die Statusspalten auf der Story-Pinnwand neu anzuordnen. Die erste Spalte kann nicht verschoben werden und Sie können keine andere Spalte vor die erste Spalte ziehen.

   ![Ziehen und Ablegen](assets/agile-story-card-drag-and-drop.png)

1. Wählen Sie sowohl den Status der Aufgabe als auch des Problems aus. Aufgabenstatus werden als Spaltentitel für jede Spalte auf der Story-Pinnwand angezeigt. Der Problemstatus, den Sie für die Zuordnung zum Aufgabenstatus auswählen. Wenn Sie also ein Problem in eine andere Spalte des Storyboards verschieben, ändert sich der Problemstatus in den hier gezeigten Problemstatus und nicht in den Namen der Spalte im Storyboard (der den Aufgabenstatus widerspiegelt).

   >[!IMPORTANT]
   >
   >Zur Auswahl stehen nur gesperrte systemweite Status zur Verfügung. Gruppenspezifische Status können nicht ausgewählt werden. Außerdem entspricht der Status der ersten Spalte immer **[!UICONTROL Neu]**.

   Sie können benutzerdefinierte Status hinzufügen, wenn Ihr [!DNL Workfront] -Administrator sie konfiguriert hat. Benutzerdefinierte Status können wie in [Status erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) beschrieben konfiguriert werden.

   >[!NOTE]
   >
   >Bei der Auswahl des Problemstatus wird in der dritten Spalte immer standardmäßig [!UICONTROL Geschlossen] verwendet. Wenn Sie über mehr als drei Spalten verfügen, müssen Sie die Spalten manuell aktualisieren, um den korrekten Status widerzuspiegeln.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

### Konfigurieren von Statusspalten für Projekte {#configure-status-columns-for-projects}

Informationen zum Konfigurieren von Statusspalten für ein Projekt finden Sie im Abschnitt [Erstellen oder Anpassen einer [!UICONTROL Agile]-Ansicht](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) im Artikel [Ansichten in  [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md) erstellen oder bearbeiten.

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

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!UICONTROL Workfront] und klicken Sie dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.\
   Nur Teammitglieder mit einer [!UICONTROL Plan] - oder [!UICONTROL Work] -Lizenz sehen diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Geben Sie im Abschnitt **[!UICONTROL Agile]** einen Feldnamen ein, um ihn zu finden.

   ![Zusätzliche Felder](assets/agile-additional-fields-scrum.png)

1. Wählen Sie den Namen des Felds aus, das Sie hinzufügen möchten.
1. Geben Sie den **[!UICONTROL Anzeigenamen]** für das Feld ein, das auf der Meldung oder Ausgabekarte angezeigt werden soll.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Konfigurieren der Verwendung von Farbindikatoren für Meldungen auf der Landingpage

Standardmäßig sind die Story-Pinnwände in einer agilen Iteration entsprechend dem Projekt, mit dem die Geschichte verknüpft ist, farbcodiert. Jedem Projekt wird eine beliebige Farbe auf dem Story Board zugewiesen. Sie können dieses Standardverhalten für jedes agile Team ändern. Farben für agile Geschichten können mit der Priorität einer Geschichte, dem Besitzer usw. verknüpft werden.

So ändern Sie das Verhalten, wie Farben Geschichten für ein agiles Team zugewiesen werden:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   Nur Teammitglieder mit einer [!UICONTROL Plan] - oder [!UICONTROL Work] -Lizenz sehen diese Option.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Wählen Sie im Abschnitt [!UICONTROL Agile] im Bereich [!UICONTROL Kartenfarbe mit ] verknüpfen eine der folgenden Optionen aus:

   * **[!UICONTROL Projekt]**: Farben sind mit dem Projekt verknüpft, mit dem die Geschichte verknüpft ist. (Wenn eine Geschichte erstellt wird, muss sie mit einem Projekt verknüpft sein, wie in [Erstellen einer Agile Story](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md) beschrieben. Alle Aufgaben desselben Projekts werden in derselben Farbe angezeigt.
   * **[!UICONTROL Freies Formular]**: Alle Karten werden standardmäßig als blau angezeigt, bis ein Benutzer die Farbe manuell ändert, wie unter [[!UICONTROL Meldungen nach Farbe kategorisieren] auf der Trommelplatine](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md) beschrieben.
   * **[!UICONTROL Priorität]**: Farben werden wie folgt mit der Priorität der Geschichte verknüpft:

      * Hoch = rot
      * Medium = Gelb
      * Niedrig = Grün\

        Wenn Ihr Systemadministrator benutzerdefinierte Prioritäten für Ihr [!DNL Workfront]-System konfiguriert hat, ist die höchste Priorität rot, die zweithöchste gelb und die dritthöchste grün.
   * **[!UICONTROL Aufgabeneigentümer]**: Alle Geschichten mit demselben Hauptverantwortlichen haben dieselbe Farbe. Der primäre Verantwortliche ist der Benutzer, der der Aufgabe zuerst zugewiesen wurde.


1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Konfigurieren der Anwendung von Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration

Wenn Sie ein Arbeitselement zu einer Scrum-Iteration hinzufügen, werden das geplante Startdatum und das geplante Abschlussdatum des Arbeitselements standardmäßig so geändert, dass sie mit dem Start- und Enddatum der Iteration übereinstimmen. Sie können festlegen, dass die ursprünglichen Daten für alle Arbeitselemente des Teams beibehalten werden.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe] Workfront und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)
1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.\
   Nur Teammitglieder mit einer [!UICONTROL Plan] - oder [!UICONTROL Work] -Lizenz sehen diese Option.
1. Wählen Sie im Abschnitt [!UICONTROL Agile] im Bereich [!UICONTROL Wenn ein Arbeitselement zu einem Iterationsbereich hinzugefügt wird] aus den folgenden Optionen:

   * **[!UICONTROL Ändern Sie das geplante Startdatum und das geplante Abschlussdatum entsprechend dem Start- und Enddatum der Iteration]**: Wenn Arbeitselemente zu einer Iteration hinzugefügt werden, werden die Arbeitselementdaten in die Iterationsdaten geändert.\

     Weitere Informationen zur Änderung von Datumsangaben finden Sie im Abschnitt [Auswirkungen des Hinzufügens von Meldungen auf Aufgabendaten verstehen](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) im Artikel [Meldungen zu einer vorhandenen Iteration hinzufügen](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL Ändern Sie nicht das geplante Startdatum und das geplante Abschlussdatum entsprechend dem Iterationsbeginn und -enddatum]**: Wenn Arbeitselemente einer Iteration hinzugefügt werden, behalten die Arbeitselemente ihre ursprünglichen Daten bei.

   Wenn Sie die Datumsoption ändern, werden die Daten für Arbeitselemente, die sich bereits in der Iteration befinden, nicht angepasst.

   Diese Optionen können sich auf das Datum auswirken, an dem Teams den Iterationen der anderen Arbeitselemente zuweisen. Beispielsweise ändert Team A die Arbeitselementdaten in die Iterationsdaten und Team B ändert die Arbeitselementdaten nicht. Wenn Team B der Iteration von Team A ein Arbeitselement zuweist, werden die Daten der Arbeitselemente geändert. Wenn jedoch Team A der Iteration von Team B ein Arbeitselement zuweist, ändern sich die Daten nicht.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
