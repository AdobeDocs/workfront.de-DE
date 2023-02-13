---
product-previous: workfront-goals
navigation-topic: goal-management
title: Aktivieren von Zielen in Adobe Workfront-Zielen
description: Wenn Sie ein Ziel erstellen, speichert Adobe Workfront Goals es mit dem Status "Entwurf". Entworfene Ziele sind nicht Teil des Zielmanagements.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Aktivieren von Zielen in Adobe Workfront-Zielen

Wenn Sie ein Ziel erstellen, speichert Adobe Workfront Goals es mit dem Status &quot;Entwurf&quot;. Entworfene Ziele sind nicht Teil des Zielmanagements.

Um durch Aktualisierung des Fortschritts verfolgen zu können, wie nah Sie am Erreichen eines Ziels sind, müssen Sie es aktivieren. Dadurch wird der Status zu &quot;Aktiv&quot;geändert.

Informationen zum Erstellen eines Ziels finden Sie unter [Erstellen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Sie müssen ein Ziel aktivieren, bevor Sie den Fortschritt seiner Ergebnisse und Aktivitäten aktualisieren können.


## Zugriffsanforderungen

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die Adobe Workfront Goals erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Ziele oder höher bearbeiten</p> <p><b>NOTIZ</b>

<p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter:</p> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a> </p> </li> 
    <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Zugriff auf Adobe Workfront-Ziele gewähren</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <div> 
     <p>Berechtigungen für das Ziel verwalten</p> 
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

Um ein Ziel zu aktivieren, muss das Ziel mit einem Fortschrittsindikator wie einer Aktivität, einem Ergebnis, einem Projekt oder einem anderen aktiven Ziel verknüpft sein.

Führen Sie mindestens einen der folgenden Schritte aus, um ein Ziel aktivieren zu können:

* Hinzufügen eines Ergebnisses zum Ziel

   Weitere Informationen finden Sie unter [Hinzufügen von Ergebnissen zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Hinzufügen einer Aktivität zum Ziel

   Weitere Informationen finden Sie unter [Hinzufügen von Aktivitäten zu Zielen in Adobe Workfront-Zielen](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Projekt mit dem Ziel verbinden

   Weitere Informationen finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen](../results-and-activities/connect-projects-to-goals-overview.md).

* Ein anderes Ziel an das Ziel ausrichten, das aktiviert werden soll

   Weitere Informationen finden Sie unter [Ziele durch Verbinden in Adobe Workfront-Zielen ausrichten](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Ziele aktivieren

Sie können von Ihnen erstellte Ziele oder ein Ziel, für das Sie über Verwaltungsberechtigungen verfügen, aktivieren.

1. Gehen Sie zu einem Ziel, das Sie aktivieren möchten. Die Zielseite wird geöffnet.

1. Klicken Sie auf **Mehr** Menü ![](../goal-management/assets/more-icon.png) rechts neben dem Zielnamen, und klicken Sie dann auf **Aktivieren**.

   ![](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   Der Zielstatus ändert sich in &quot;Aktiv&quot;. Sie können jetzt den Fortschritt beim Ziel verfolgen. Das Ziel wird im Abschnitt &quot;Einchecken&quot;angezeigt und auch in den Diagrammen der Workfront-Ziele berücksichtigt.
