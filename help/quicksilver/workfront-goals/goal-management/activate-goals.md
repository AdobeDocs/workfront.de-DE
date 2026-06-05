---
product-previous: workfront-goals
navigation-topic: goal-management
title: Aktivieren von Zielen in Adobe Workfront
description: Wenn Sie ein Ziel erstellen, wird es von Adobe Workfront Goals mit dem Status Entwurf gespeichert. Entworfene Ziele sind nicht Teil des Zielmanagements.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/XVvr-M58-7ZXp7eIvYrmUoHheCgRVGavWqRxzoyYOM4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 440
ht-degree: 15%

---

# Aktivieren von Zielen in Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Wenn Sie ein Ziel erstellen, wird es von Adobe Workfront Goals mit dem Status Entwurf gespeichert. Entworfene Ziele sind nicht Teil des Zielmanagements.

Um zu verfolgen, wie nahe Sie einem Ziel sind, indem Sie dessen Fortschritt aktualisieren, müssen Sie es aktivieren. Dadurch wird der Status in „Aktiv“ geändert.

Informationen zum Erstellen eines Ziels finden Sie unter [Erstellen von Zielen in Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Sie müssen ein Ziel aktivieren, bevor Sie den Fortschritt seiner Ergebnisse und Aktivitäten aktualisieren können.


## Zugriffsanforderungen

>[!NOTE]
>
>Ihr Unternehmen kann sich dafür entscheiden, Adobe Workfront Goals weiterhin zu verwenden, wenn es dieses Paket in der Vergangenheit erworben hat. Weitere Informationen erhalten Sie bei Ihrer Kundenbetreuung.
>
>Adobe Workfront Goals ist nicht mehr erhältlich.

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
  <tr>
  <td> <p>Adobe Workfront-Paket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p><p><b>NOTIZ</b></p>
<p>Wenden Sie sich an Ihren Workfront-Support-Mitarbeiter, wenn Sie ein anderes Workfront-Paket haben.</p>
   </td> 
  </tr> 
  <tr>
 <td role="rowheader">Konfigurationen der Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Systemadministratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>
-->

## Voraussetzungen

Um ein Ziel zu aktivieren, muss das Ziel mit einer Fortschrittsanzeige wie einer Aktivität, einem Ergebnis oder einem Projekt verknüpft oder mit einem anderen aktiven Ziel ausgerichtet sein.

Führen Sie mindestens einen der folgenden Schritte aus, um ein Ziel aktivieren zu können:

* Ergebnis zum Ziel hinzufügen

  Weitere Informationen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Hinzufügen einer Aktivität zum Ziel

  Weitere Informationen finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Verbinden eines Projekts mit dem Ziel

  Weitere Informationen finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront Goals](../results-and-activities/connect-projects-to-goals-overview.md).

* Ein weiteres Ziel an dem Ziel ausrichten, das Sie aktivieren möchten

  Weitere Informationen finden Sie unter [Ausrichten von Zielen durch Verbinden in Adobe Workfront-](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Aktivieren von Zielen

Sie können Ziele aktivieren, die Sie erstellt haben, oder ein Ziel, für das Sie über Verwaltungsberechtigungen verfügen.

1. Navigieren Sie zu einem Ziel, das Sie aktivieren möchten. Die Zielseite wird geöffnet.

1. Klicken Sie auf das **Mehr** Menü ![Mehr](../goal-management/assets/more-icon.png) rechts neben dem Zielnamen und klicken Sie dann auf **Aktivieren**.

   ![Mehr Menü erweitert](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   Der Zielstatus ändert sich in Aktiv. Sie können jetzt den Fortschritt beim Ziel verfolgen. Das Ziel wird im Abschnitt Einchecken angezeigt und wird in den Diagrammabschnitten der Workfront-Ziele berücksichtigt
