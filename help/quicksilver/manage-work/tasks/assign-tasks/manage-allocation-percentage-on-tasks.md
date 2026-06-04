---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Verwalten der prozentualen Benutzerzuweisung oder Rollenzuweisung bei Aufgaben
description: Der Zuordnungsprozentsatz gibt an, wie lange eine zugewiesene Ressource an einem Tag an einem Vorgang arbeiten soll. Er ist der Prozentsatz eines Arbeitstages (gemäß dem Benutzer- oder Projektzeitplan), an dem eine Ressource während der gesamten Dauer des Vorgangs zugewiesen wird.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/tpBEkOgTsJSJ-dk-gKZ6uLyCk4j4vP4nMIQ5-ciHMAI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 444
ht-degree: 11%

---

# Verwalten des Prozentsatzes der Benutzer- oder Rollenzuweisung bei Aufgaben

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->


Der Zuordnungsprozentsatz gibt an, wie lange eine zugewiesene Ressource an einem Tag an einem Vorgang arbeiten soll. Er ist der Prozentsatz eines Arbeitstages (gemäß dem Benutzer- oder Projektzeitplan), an dem eine Ressource während der gesamten Dauer des Vorgangs zugewiesen wird.

Sie können den Zuordnungsprozentsatz ändern, wenn Sie erweiterte Zuweisungen zu einer Aufgabe vornehmen.

>[!NOTE]
>
>Wenn Sie Benutzende einer Arbeit zuweisen, wirkt sich ihre Verfügbarkeit entsprechend den Zeitplänen auf die geplanten und erwarteten Termine von Aufgaben und Problemen aus. Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <p>Work oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Aufgaben bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td>
   <td><p>Tragen Sie zur Aufgabe bei oder erhöhen Sie die Berechtigungen.</p>
   <p>Bearbeiten Sie die Berechtigungen, um den Zuordnungsprozentsatz im Feld Aufgabe bearbeiten zu aktualisieren.</p>
   <!--
   Not true anymore: 
   <p><b>NOTE</b></p>
   <p> You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a>.</p>
   -->
   </td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

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

   Abhängig vom Workfront- oder Workflow-Paket Ihres Unternehmens wird möglicherweise einer dieser Bildschirme angezeigt.

   ![Ändern des Zuordnungsprozentsatzes](assets/advanced-assignments-allocation-percentage.png)

   ![Ändern des Zuordnungsprozentsatzes](assets/new-aa-allocation-by-percentage.png)

1. Klicken Sie auf **Speichern**.
