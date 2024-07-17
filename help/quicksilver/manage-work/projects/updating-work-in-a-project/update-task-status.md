---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierung des Aufgabenstatus
description: Sie können den Status einer Aufgabe aktualisieren, um andere darüber zu informieren, wo sich die Aufgabe befindet (und wie das Gesamtprojekt) und wie sie vorankommt.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

# Aktualisierung des Aufgabenstatus

Sie können den Status einer Aufgabe aktualisieren, um andere darüber zu informieren, wo sich die Aufgabe befindet (und wie das Gesamtprojekt) und wie sie vorankommt.

Die Standardstatus sind &quot;Neu&quot;, &quot;In Bearbeitung&quot;und &quot;Abgeschlossen&quot;. Ihr Adobe Workfront-Administrator kann benutzerdefinierte Status für Ihre Organisation hinzufügen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Sie können den Aufgabenstatus manuell aktualisieren oder Workfront automatisch aktualisieren lassen, wenn bestimmte Aktionen ausgeführt werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um Aufgaben manuell aktualisieren zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p> 
   Oder
   <p>Aktuell: Arbeit oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgabe verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Aktualisieren des Status von Aufgaben

* Wenn Sie eine Aufgabe als &quot;Abgeschlossen&quot;markieren, wird der prozentuale Abschluss der Aufgabe auf 100 % aktualisiert.
* Für übergeordnete Aufgaben gibt es die folgenden Szenarien:
   * Sie können den Status einer übergeordneten Aufgabe nicht auf &quot;Abgeschlossen&quot;aktualisieren, wenn der Zusammenfassungsabschlussmodus des Projekts auf &quot;Automatisch&quot;eingestellt ist und die Unteraufgaben nicht abgeschlossen sind.
   * Sie können den Status einer übergeordneten Aufgabe auf &quot;Abgeschlossen&quot;aktualisieren, wenn der Zusammenfassungsabschlussmodus des Projekts auf &quot;Manuell&quot;festgelegt ist und die Unteraufgaben abgeschlossen oder unvollständig sind.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](../manage-projects/edit-projects.md).

## Aufgabenstatus manuell aktualisieren

Sie können den Aufgabenstatus in den folgenden Bereichen von Workfront aktualisieren:

* Die Kopfzeile der Aufgabe auf der Aufgabenseite.
* das Feld Aufgabe bearbeiten beim Bearbeiten einer Aufgabe.
* den Abschnitt &quot;Aufgabendetails&quot;auf der Aufgabenseite.
* Wenn in einer Aufgabenliste oder einem Bericht das Feld Status in der Ansicht sichtbar ist.
* Im Bereich Zusammenfassung der Aufgabe.

So aktualisieren Sie den Aufgabenstatus in der Aufgabenüberschrift manuell:

1. Gehen Sie zu einer Aufgabe, für die Sie den Status aktualisieren möchten.
1. Klicken Sie in der Aufgabenkopfzeile auf das Feld **Status** und wählen Sie einen neuen Status aus.
1. Um einen visuellen Hinweis zum Abschluss der Aufgabe anzuzeigen, ziehen Sie die Blase unter **Prozent abgeschlossen** in die Kopfzeile der Aufgabe

   Oder

   Klicken Sie in die Blase in der Kopfzeile der Aufgabe, um einen Prozentsatz einzugeben.

   ![](assets/percent-complete-status-widgets-task-header.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um zusätzliche Informationen über die Aktualisierung bereitzustellen:

   * Um einen Hinweis zur Aktualisierung hinzuzufügen, gehen Sie zum Abschnitt **Aktualisierungen** und klicken Sie auf **Neuer Kommentar**. Geben Sie dann einen Hinweis ein.

     ![](assets/add-update-to-task.png)

   * Um bestimmte Benutzer über die Aktualisierung zu benachrichtigen, geben Sie deren Namen in das Feld **Personen oder Teams taggen** ein, das angezeigt wird, wenn Sie einen Kommentar eingeben. Weitere Informationen finden Sie unter [Taggen anderer Benutzer bei Updates](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Klicken Sie zum Aktualisieren des Übermittlungsdatums der Aufgabe auf **Aufgabendetails** und bearbeiten Sie dann das Feld **Übermittlungsdatum** . Weitere Informationen finden Sie unter [Aufgaben bearbeiten](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).


   >[!IMPORTANT]
   >
   >  Nur Aufgabenverantwortliche können das Veröffentlichungsdatum aktualisieren.

<!--old functionality in old commenting: 

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![](assets/drag-the-progress-bar-350x155.png)-->

## Automatisches Aktualisieren des Aufgabenstatus

Workfront aktualisiert den Status einer Aufgabe automatisch in einen anderen Status, wenn die in der folgenden Tabelle aufgelisteten Aktionen ausgeführt werden.

>[!NOTE]
>
>Die Status in der folgenden Tabelle sind standardmäßige Systemstatus. Ihr Workfront-Administrator oder ein Gruppenadministrator kann die Status in Ihrer Workfront-Instanz umbenennen. Informationen zum Erstellen und Verwalten von Status in Workfront finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Aktion</b></td> 
   <td><b>Originalstatus</b></td> 
   <td><b>Neuer Status</b></td> 
  </tr> 
  <tr> 
   <td>Aktualisieren Sie den Prozentsatz der abgeschlossenen Aufgaben auf 100 %</td> 
   <td>Neu oder in Bearbeitung</td> 
   <td>Abgeschlossen</td> 
  </tr> 
  <tr> 
   <td>Aktualisieren Sie den Prozentsatz der abgeschlossenen Aufgaben von 100 % auf eine niedrigere Zahl.</td> 
   <td>Abgeschlossen</td> 
   <td>In Arbeit</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klicken Sie auf die Schaltfläche Aufgabe starten , um die Arbeit an einer Aufgabe zu akzeptieren, die Ihnen zugewiesen ist</span> </td> 
   <td><span>Neu</span> </td> 
   <td> <p>Jeder Status, der mit der Schaltfläche Aufgabe starten in den Einstellungen des Home-Teams verknüpft ist.</p> <p>Weitere Informationen zum Ersetzen der Schaltfläche "Work On It"durch eine Schaltfläche "Start Task"finden Sie unter <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche "Work On It"durch eine Schaltfläche "Start"</a></span>.</p> <p>Tipp: <span>Durch Klicken auf die Schaltfläche "Rückgängig"<span data-mc-conditions="QuicksilverOrClassic.Quicksilver">nach dem Klicken auf "Aufgabe starten"wird der Status auf "Neu"zurückgesetzt.</span></span> </p> </td> 
  </tr> 
 </tbody> 
</table>
