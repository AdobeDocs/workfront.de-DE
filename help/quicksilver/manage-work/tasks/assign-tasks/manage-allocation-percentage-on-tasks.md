---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Verwalten der prozentualen Benutzerzuweisung oder Rollenzuweisung bei Aufgaben
description: Der Zuordnungsprozentsatz gibt an, wie lange eine zugewiesene Ressource an einem Tag an einem Vorgang arbeiten soll. Er ist der Prozentsatz eines Arbeitstages (gemäß dem Benutzer- oder Projektzeitplan), an dem eine Ressource während der gesamten Dauer des Vorgangs zugewiesen wird.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 1%

---

# Verwalten des Prozentsatzes der Benutzer- oder Rollenzuweisung bei Aufgaben

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->


Der Zuordnungsprozentsatz gibt an, wie lange eine zugewiesene Ressource an einem Tag an einem Vorgang arbeiten soll. Er ist der Prozentsatz eines Arbeitstages (gemäß dem Benutzer- oder Projektzeitplan), an dem eine Ressource während der gesamten Dauer des Vorgangs zugewiesen wird.

Sie können den Zuordnungsprozentsatz ändern, wenn Sie erweiterte Zuweisungen zu einer Aufgabe vornehmen.

>[!NOTE]
>
>Wenn Sie Benutzende einer Arbeit zuweisen, wirkt sich ihre Verfügbarkeit entsprechend den Zeitplänen auf die geplanten und erwarteten Termine von Aufgaben und Problemen aus. Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Arbeit oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Aufgaben bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td>
   <td><p>Tragen Sie zur Aufgabe bei oder erhöhen Sie die Berechtigungen.</p>
   <p>Bearbeiten Sie die Berechtigungen, um den Zuordnungsprozentsatz im Feld Aufgabe bearbeiten zu aktualisieren, wenn Sie Aufgaben mit dem alten Erlebnis bearbeiten. Sie können den Zuordnungsprozentsatz im Feld Aufgabe bearbeiten nicht mehr verwalten, wenn Sie Aufgaben in der neuen -Version bearbeiten.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Aufgaben bearbeiten</a>.</p></td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

## Überlegungen zur Änderung der prozentualen Zuteilungen für Aufgaben

* Benutzern wird standardmäßig ein gleicher Prozentsatz der Zeit für Aufgaben zugewiesen, denen sie zugewiesen sind.
* Sie können den Zuordnungsprozentsatz für Benutzer und Aufgabengebiete, die Aufgaben zugewiesen sind, nur dann manuell ändern, wenn der Dauertyp der Aufgabe „Berechnet“, „Arbeit“ oder „Arbeitsaufwand“ ist.

  Weitere Informationen finden Sie unter [Übersicht über Aufgabendauer und -typ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Die prozentuale Zuordnung für Teams, die Aufgaben zugewiesen sind, kann nicht geändert werden.
* Die prozentuale Zuordnung für Benutzende und den Problemen zugewiesenen Aufgabengebieten kann nicht geändert werden.

## Ändern der prozentualen Zuordnung des Benutzers oder der Funktion für eine Aufgabe

1. Wechseln Sie zu einem Vorgang, für dessen Ressourcen Sie die prozentuale Zuordnung ändern.
1. Klicken Sie in **Aufgabenkopfzeile auf den** „Arbeitsaufträge“ und dann auf **Erweitert**.

1. Stellen Sie sicher **dass der** Dauertyp“ der Aufgabe einer der folgenden ist:

   * Berechnete Arbeit
   * Leistungsgesteuert

   >[!TIP]
   >
   >* Für den Typ „Berechnete Zuweisungsdauer“ verwendet Workfront die folgende Formel, um den Zuordnungsprozentsatz jedes Empfängers zu berechnen: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Für den Typ Einfache Dauer können Sie die jeder Ressource zugewiesenen Stunden schätzen, nicht den Zuordnungsprozentsatz.

1. Ändern Sie das **Zuweisungen** für jeden Aufgabenempfänger.

   Sie können nur den Zuordnungsprozentsatz für Benutzer- und Aufgabenrollenzuweisungen ändern.

   Sie können den Zuordnungsprozentsatz für ein Team, das einer Aufgabe zugewiesen ist, nicht ändern.

   ![Ändern des Zuordnungsprozentsatzes](assets/advanced-assignments-allocation-percentage.png)

1. Klicken Sie auf **Speichern**.
