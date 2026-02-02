---
product-area: projects
navigation-topic: create-tasks
title: Wiederkehrende Aufgaben erstellen
description: Sie können wiederkehrende Aufgaben für Aufgaben erstellen, die Sie im Rahmen eines einzelnen Projekts wiederholen müssen.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '890'
ht-degree: 3%

---

# Wiederkehrende Aufgaben erstellen

<!--Audited: 01/2024-->

Sie können wiederkehrende Aufgaben für Aufgaben erstellen, die Sie im Rahmen eines einzelnen Projekts wiederholen müssen.

Allgemeine Informationen zu wiederkehrenden Aufgaben, einschließlich der Auswirkungen der Bearbeitung vorhandener wiederkehrender Aufgaben, finden Sie unter [Übersicht über wiederkehrende Aufgaben](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

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
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt mit der Möglichkeit zum Hinzufügen von Aufgaben oder höher hinzufügen</p> 
   <p>Wenn Sie eine Aufgabe erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für die Aufgabe</p> 
    </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p> 
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> 
   <p>When you create a task you automatically receive Manage permissions to the task</p> 
   <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator. For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Erstellen einer wiederkehrenden Aufgabe

>[!NOTE]
>
>Sie können eine wiederkehrende Aufgabe nicht erstellen, indem Sie eine vorhandene Aufgabe ändern. Sie müssen eine Aufgabe von Grund auf neu erstellen.

1. Wechseln Sie zu dem Projekt, in dem Sie eine wiederkehrende Aufgabe erstellen möchten, und klicken Sie dann im linken Bedienfeld auf **Aufgaben** Abschnitt.
1. Klicken Sie auf **Neue Aufgabe**.

   Das Dialogfeld Neue Aufgabe wird angezeigt.

   ![Aufgabe erstellen - kleiner Bildschirm](assets/nwe-create-task-small-screen-350x272.png)

1. Klicken Sie auf **Weitere Optionen** und geben Sie dann einen Namen für die Aufgabe in das Feld **Aufgabenname** ein.
1. Aktualisieren Sie die Aufgabe wie beim Hinzufügen einer neuen Aufgabe. Weitere Informationen zum Hinzufügen einer neuen Aufgabe finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   Die Dauer und die geplanten Stunden für eine neue wiederkehrende Aufgabe entsprechen der Dauer und den geplanten Stunden für jedes Vorkommen. Die Dauer der übergeordneten Aufgabe ist die Zeit zwischen dem geplanten Startdatum der frühesten Aufgabe und dem geplanten Abschlussdatum der letzten Aufgabe. Die geplanten Stunden der übergeordneten Aufgabe sind die Gesamtstunden aller geplanten Stunden aus allen Vorfällen.

1. Klicken Sie **linken** auf „Übersicht“.
1. Scrollen Sie nach unten zum Abschnitt **Wiederholungszeitplan** und wählen Sie dann die Option **Dies zu einer wiederkehrenden Aufgabe machen** aus.

   ![Abschnitt „Wiederholungszeitplan“ für neue wiederkehrende Aufgaben](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. Wählen **in der Dropdown** Liste „Häufigkeit“ die Anzahl der Zeiteinheiten, zu denen die Aufgabe ausgeführt werden soll, und den Typ der Zeiteinheiten aus. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Intervalltyp</th> 
      <th>Beschreibung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Day</strong> </td> 
      <td> <p>Die Aufgabe wird täglich, alle 2 Tage, alle 3 Tage usw. wiederholt, je nach ausgewählter Kadenz. Sie können Aufgaben so konfigurieren, dass sie bis zu jedem 6. Tag wiederholt werden. Die Standardeinstellung ist 1 Tag. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Arbeitstag</strong> </td> 
      <td> <p> Die Aufgabe wird je nach ausgewählter Kadenz an jedem Arbeitstag, allen 2 Arbeitstagen, allen 3 Arbeitstagen usw. wiederholt. Sie können Aufgaben so konfigurieren, dass sie bis zu jedem 6. Arbeitstag wiederholt werden.</p> <p>Diese Option verwendet den vom Systemadministrator definierten Standardzeitplan, wie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Erstellen eines Zeitplans</a> beschrieben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Woche</strong> </td> 
      <td> <p> Die Aufgabe wird jede Woche, alle 2 Wochen, alle 3 Wochen usw. wiederholt, je nach ausgewählter Kadenz.</p> <p>Wählen <strong> im Feld </strong> den Wochentag aus, an dem jede Aufgabe ausgeführt werden soll. Sie können mehrere Tage auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Month</strong> </td> 
      <td> <p>Die Aufgabe wird monatlich, alle 2 Monate, alle 3 Monate usw. wiederholt, je nach ausgewählter Kadenz. Sie können zwischen 1 und 12 Monaten wählen. </p> <p>Wählen <strong> im Feld „Wiederholungen</strong> eine der folgenden Optionen aus, wenn die Aufgabe ausgeführt werden soll:</p> 
       <ul> 
        <li> <p><strong>Jeden Monat an Tag &lt;Monatsdatum&gt;</strong> </p> <p>Sie können Tage von 1 bis 30 auswählen oder "<strong>" </strong>. Sie können beispielsweise „Jeden Monat am 30.“ auswählen. </p> </li> 
        <li> <p><strong>Jeden Monat am &lt;number&gt; &lt;Tag der Woche&gt;</strong> </p> <p>Im ersten Dropdown-Menü können Sie eine Zahl zwischen 1 und 4 für die Zahl der Woche im Monat auswählen oder Sie können „Letzte“ auswählen. </p> <p>Im zweiten Dropdown-Menü können Sie einen beliebigen Wochentag auswählen. </p> <p>Sie können beispielsweise „Jeden Monat am 2. Dienstag“ auswählen. </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wenn mit dem Zeitplan des Projekts eine Zeitplanausnahme verknüpft ist, können wiederkehrende Aufgaben während der Ausnahme nicht gestartet werden. Wiederkehrende Aufgaben, die während der Zeitplanausnahme auftreten, sind so geplant, dass sie am ersten Geschäftstag nach der Ausnahme beginnen. Weitere Informationen zu Zeitplanausnahmen finden Sie im Artikel [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. Wählen **im Feld** das Datum und die Uhrzeit aus, zu der die wiederkehrenden Aufgaben beginnen sollen.
1. Wählen Sie **Feld** das Datum und die Uhrzeit aus, zu der die wiederkehrenden Aufgaben abgeschlossen werden sollen

   ODER

   Wählen Sie **Nach `<number>` Vorkommen**, um anzugeben, wie oft die wiederkehrende Aufgabe ausgeführt werden soll. Workfront erstellt für die Aufgaben dieselbe Anzahl von Wiederholungen wie für die Zahl, die Sie in diesem Feld angeben.

1. Klicken Sie auf **Aufgabe erstellen.**

   Die Aufgabenliste wird angezeigt. Die wiederkehrende Aufgabe wird als übergeordnete Aufgabe erstellt, und alle Wiederholungen sind ihre untergeordneten Elemente. Workfront generiert automatisch die Namen der untergeordneten Aufgaben, wobei der Name verwendet wird, den Sie für das übergeordnete Element eingegeben haben, gefolgt von einer Zahl. Die wiederkehrenden Aufgaben werden am Ende der Aufgabenliste platziert.

   Weitere Informationen dazu, welche Felder von der übergeordneten wiederkehrenden Aufgabe automatisch ausgefüllt werden, finden Sie unter [Übersicht über wiederkehrende Aufgaben](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![Wiederkehrende Aufgaben in Aufgabenliste](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Optional) Ändern Sie jede wiederkehrende Aufgabe wie jede andere Aufgabe im Projekt.

   Sie können beispielsweise Zuweisungen, Vorgänger und Dauer hinzufügen und alle anderen Informationen zur Aufgabe ändern, einschließlich benutzerdefinierter Felder.

   >[!IMPORTANT]
   >
   >Wenn Sie die übergeordnete Wiederholung ändern, nachdem die untergeordneten Elemente einzeln geändert wurden, kann dies zu unterschiedlichen Informationen zwischen den untergeordneten Elementen oder zwischen den untergeordneten Elementen und den übergeordneten Elementen führen. Weitere Informationen finden Sie unter [Übersicht über wiederkehrende Aufgaben](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
