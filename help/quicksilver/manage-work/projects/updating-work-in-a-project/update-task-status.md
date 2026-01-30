---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aufgabenstatus aktualisieren
description: Sie können den Status einer Aufgabe aktualisieren, um andere darüber zu informieren, wo sich die Aufgabe (und das gesamte Projekt) befindet und wie sie voranschreitet.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 4%

---

# Aufgabenstatus aktualisieren

<!--Audited: 10/2024-->

Sie können den Status einer Aufgabe aktualisieren, um andere darüber zu informieren, wo sich die Aufgabe (und das gesamte Projekt) befindet und wie sie voranschreitet.

Die Standardstatus sind „Neu“, „In Bearbeitung“ und „Abgeschlossen“. Ihr Adobe Workfront-Administrator kann benutzerdefinierte Status für Ihr Unternehmen hinzufügen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Sie können den Aufgabenstatus manuell aktualisieren oder zulassen, dass Workfront ihn automatisch aktualisiert, wenn bestimmte Aktionen ausgeführt werden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Work oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgabe</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p> 
   Or
   <p>Current: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen zur Aktualisierung des Aufgabenstatus

* Wenn Sie eine Aufgabe als abgeschlossen markieren, wird der Prozentsatz der Fertigstellung der Aufgabe auf 100 % aktualisiert.
* Die folgenden Szenarien existieren für übergeordnete Aufgaben:
   * Sie können den Status einer übergeordneten Aufgabe nicht auf „Abgeschlossen“ aktualisieren, wenn der Fertigstellungsmodus Zusammenfassung des Projekts auf „Automatisch“ eingestellt ist und die Teilaufgaben nicht abgeschlossen sind.
   * Sie können den Status einer übergeordneten Aufgabe auf Abgeschlossen aktualisieren, wenn der Fertigstellungsmodus Zusammenfassung des Projekts auf Manuell festgelegt ist und die Teilaufgaben abgeschlossen oder unvollständig sind.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](../manage-projects/edit-projects.md).

## Aufgabenstatus manuell aktualisieren

Sie können den Aufgabenstatus in den folgenden Bereichen aktualisieren:

* Die Aufgabenkopfzeile auf der Aufgabenseite
* Das Feld Aufgabe bearbeiten beim Bearbeiten einer Aufgabe.
* Der Abschnitt Aufgabendetails auf der Aufgabenseite.
* In einer Aufgabenliste oder einem Bericht, wenn das Feld Status in der Ansicht sichtbar ist.
* Im Bedienfeld Zusammenfassung der Aufgabe.

So aktualisieren Sie den Aufgabenstatus in der Aufgabenkopfzeile manuell:

1. Wechseln Sie zu einer Aufgabe, für die Sie den Status aktualisieren möchten.
1. Klicken Sie in der Aufgabenkopfzeile auf das Feld **Status** und wählen Sie einen neuen Status aus.
1. Um einen visuellen Hinweis auf den Abschluss der Aufgabe zu geben, ziehen Sie den Kreis unter **Prozent abgeschlossen** in die Kopfzeile der Aufgabe.

   ODER

   Doppelklicken Sie in die Blase **Prozent abgeschlossen**, um manuell einen neuen Prozentsatz einzugeben.

   ![Aufgabenkopfzeile der Status-Widgets „Prozent abgeschlossen“](assets/percent-complete-status-widgets-task-header.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um zusätzliche Informationen zur Aktualisierung bereitzustellen:

   * Um einen Hinweis zur Aktualisierung hinzuzufügen, gehen Sie zum Abschnitt **Aktualisierungen** und klicken Sie auf **Neuer Kommentar** und geben Sie dann einen Hinweis ein.

     ![Hinzufügen einer Aktualisierung zu einer Aufgabe](assets/add-update-to-task.png)

   * Um bestimmte Benutzer über die Aktualisierung zu benachrichtigen, geben Sie ihre Namen in das Feld **Personen oder Teams taggen** ein, das angezeigt wird, wenn Sie einen Kommentar eingeben. Weitere Informationen finden Sie unter [Andere bei Updates taggen](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Um das Commit-Datum der Aufgabe zu aktualisieren, klicken Sie auf **Aufgabendetails** und bearbeiten Sie dann das Feld **Commit-**&quot;. Weitere Informationen finden Sie unter [Aufgaben bearbeiten](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).


   >[!IMPORTANT]
   >
   >  Nur Aufgabenzugewiesene können das Commit-Datum aktualisieren.

<!--old functionality in old commenting: 

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![Drag the progress bar]](assets/drag-the-progress-bar-350x155.png)-->

## Aufgabenstatus automatisch aktualisieren

Workfront aktualisiert automatisch den vorhandenen Aufgabenstatus auf einen anderen Status, wenn die in der folgenden Tabelle aufgeführten Aktionen ausgeführt werden.

>[!NOTE]
>
>Die in der folgenden Tabelle aufgeführten Statuswerte sind standardmäßige Systemstatus. Ihr Workfront-Administrator oder ein Gruppenadministrator kann die Status in Ihrer Workfront-Instanz umbenennen. Informationen zum Erstellen und Verwalten von Status in Workfront finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Aktion</b></td> 
   <td><b>Originalzustand</b></td> 
   <td><b>Neuer Status</b></td> 
  </tr> 
  <tr> 
   <td>Prozentuale Fertigstellung der Aufgabe auf 100 % aktualisieren</td> 
   <td>Neu oder in Bearbeitung</td> 
   <td>Abgeschlossen</td> 
  </tr> 
  <tr> 
   <td>Prozentuale Fertigstellung der Aufgabe von 100 % auf eine niedrigere Zahl aktualisieren</td> 
   <td>Abgeschlossen</td> 
   <td>In Arbeit</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicken Sie auf die Schaltfläche Aufgabe starten , um die Bearbeitung einer Ihnen zugewiesenen Aufgabe anzunehmen</span> </td> 
   <td><span>Neu</span> </td> 
   <td> <p>Jeder Status, der mit der Schaltfläche Aufgabe starten in den Einstellungen Ihres Home-Teams verknüpft ist.</p> <p>Informationen zum Ersetzen der Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Aufgabe starten“ finden Sie <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Starten“</a></span>.</p> <p>Tipp: <span>Klicken</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">auf die Schaltfläche „Rückgängig“, </span> Sie auf „Aufgabe starten“ geklickt haben, wird der Status auf „Neu“ zurückgesetzt. </p> </td> 
  </tr> 
 </tbody> 
</table>
