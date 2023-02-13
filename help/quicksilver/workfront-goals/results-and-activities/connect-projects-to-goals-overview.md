---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen
description: Sie können Projekte mit Zielen verknüpfen, um basierend auf dem tatsächlichen Fortschritt des Projekts anzugeben, wie das Ziel voranschreitet. Das Projekt wird zu einem Fortschrittsanzeiger für das Ziel.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Sie können Projekte mit Zielen verknüpfen, um basierend auf dem tatsächlichen Fortschritt des Projekts anzugeben, wie das Ziel voranschreitet. Das Projekt wird zu einem Fortschrittsanzeiger für das Ziel.

Indem Sie Projekte mit Zielen verbinden, können Sie die strategische Planung (Ziele) Ihrer Organisation mit der tatsächlichen Arbeit verbinden, die Ihre Mitarbeiter täglich leisten und abschließen (Projekte).

>[!IMPORTANT]
>
>Ziele auf Projektebene, die im Geschäftsfallbereich eines Projekts erstellt wurden, sind nicht mit strategischen Zielen verknüpft, die in Workfront-Zielen erstellt wurden. Weitere Informationen zu den Geschäftsfallprojektzielen finden Sie unter [Geschäftsfallziele erstellen](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Zugriffsanforderungen

<!--drafted for P&P release: replace the table below with this: 

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
   <td> <p>Zugriff auf Ziele bearbeiten</p> <p><b>NOTIZ</b>

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

Weitere Informationen zum Zugriff auf Workfront-Ziele finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../goal-management/access-needed-for-wf-goals.md).

## Überlegungen zum Verbinden von Projekten mit Zielen

* Sie können einem Ziel ein Projekt hinzufügen, das die folgenden Kriterien erfüllt:

   * Sie müssen mindestens über die Berechtigungen zum Anzeigen verfügen.

      >[!NOTE]
      >
      >Wenn Sie die Berechtigung zum Anzeigen des Projekts verlieren, nachdem Sie das Projekt an das Ziel angehängt haben, können Sie weiterhin Projektinformationen zum Ziel sehen, aber Sie können nicht mehr auf das Projekt zugreifen.

   * Das Projekt darf nicht den Status &quot;Tot&quot;haben.

* Sie können mehrere Projekte mit einem Ziel verknüpfen.
* Sie können dasselbe Projekt mit mehreren Zielen verknüpfen.
* Sie können den Fortschritt eines Projekts nicht manuell über das Ziel aktualisieren, an das das Projekt angehängt ist. Stattdessen berechnet Workfront den prozentualen Abschluss des Projekts und Workfront Goals berechnet den Zielfortschritt anhand dieses Prozentsatzes. Dadurch wird das Ziel in Echtzeit aktualisiert, nachdem der Prozentsatz des Projekts aktualisiert wurde.
* Die Projektdauer kann außerhalb des Zeitraums eines Ziels liegen. Wenn ein Projekt länger dauert als der Zieltermin, können Sie Ihr Ziel dennoch schließen und es als abgeschlossen betrachten. Der Zielprozentsatz für die Fertigstellung beträgt jedoch nicht 100 %. Der prozentuale Abschluss des Projekts aktualisiert das Ziel nicht mehr.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Wenn Sie ein an ein Ziel angehängtes Projekt löschen, wird das Projekt auch aus dem Ziel gelöscht.

   >[!CAUTION]
   >
   >Wenn das Ziel aktiv war, bevor Sie das Projekt gelöscht haben, und es keine weiteren Fortschrittsanzeigen für das Ziel gibt, wird das Ziel inaktiv.


## Hinzufügen von Projekten zu Zielen

1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-icon.png) (Entwurf für Shell: oder klicken Sie auf **Hauptmenü** ![](assets/three-line-main-menu-icon.png) in der oberen linken Ecke, sofern verfügbar.) , dann **Ziele**.
1. Klicken Sie in der Zielliste auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicken **Fortschrittsanzeigen** im linken Bereich.
1. Aus dem **Neuer Fortschrittsanzeiger** Dropdown-Menü, klicken Sie auf **Vorhandenes Projekt hinzufügen**.

   Das Feld Projekte zum Ziel hinzufügen wird angezeigt.
1. (Optional) Aktualisieren Sie die **Ansicht**, **Filter** oder **Gruppierung** durch Klicken auf die entsprechenden Symbole in der oberen rechten Ecke der Liste, um die Anzeige der Projektliste zu ändern.
1. (Optional) Klicken Sie auf die **Suche** icon ![](assets/search-icon.png) und geben Sie den Namen eines Projekts ein, um es schnell in der Liste zu finden.
1. Wählen Sie die Projekte aus, die Sie zum Ziel hinzufügen möchten, und klicken Sie dann auf **Hinzufügen**.

   Die ausgewählten Projekte werden zum Ziel hinzugefügt und im Abschnitt Fortschrittsindikatoren der Zielseite unter dem **Projekt** Gruppierung.

   Nachdem Sie das Ziel aktiviert haben, wird der Fortschritt des Ziels automatisch aktualisiert, sobald der Fortschritt eines Projekts aktualisiert wird. Informationen zum Aktivieren eines Ziels finden Sie unter [Aktivieren von Zielen in Adobe Workfront-Zielen](../goal-management/activate-goals.md).

## Suchen Sie nach Projektinformationen zu Zielen.

<p>
Die folgenden Projektinformationen sind auf der Zielebene im Abschnitt Fortschrittsindikatoren auf der Seite eines Ziels sichtbar:

</p>

<table>
  <tr>
   <td>Projektname
   </td>
   <td>Alle Änderungen am Projektnamen werden auch im verbundenen Projekt übernommen.
   </td>
  </tr>
  <tr>
   <td>Projektbesitzer
   </td>
   <td>Alle Änderungen im Projekteigentümer werden auch im verbundenen Projekt übernommen.
   </td>
  </tr>
    <tr>
   <td>Tatsächlicher Fortschritt
   </td>
   <td> <p>Der prozentuale Abschluss des Projekts. Sie können den Prozentsatz des Projekts, der vom Ziel abgeschlossen wurde, nicht manuell aktualisieren. Workfront berechnet sie automatisch anhand des Prozentsatzes, in dem die Aufgaben abgeschlossen sind. </p>
   </td>
  </tr>
  <tr>
   <td>Fortschritt
   </td>
   <td>Der prozentuale Abschluss des Projekts, dargestellt durch einen Balken. Jede Änderung des Prozentsatzes für den Abschluss des Projekts aktualisiert automatisch den Zielfortschritt, es sei denn, das Ziel ist geschlossen.
   </td>
  </tr>

</table>

## Zielinformationen zu Projekten suchen

Die folgenden Zielinformationen sind in einer Projektliste oder einem Bericht sichtbar:

| Zielinformation | Beschreibung |
|---|---|
| Ziele | Eine Liste aller Ziele, denen ein Projekt zugeordnet ist. |
| Zielhierarchie | Die Hierarchie, zu der ein Ziel gehört. Nur die übergeordneten Elemente des Ziels und des Ziels werden in diesem Feld angezeigt. Untergeordnete Ziele werden nicht angezeigt. |
| Anzahl verknüpfter Ziele | Die Anzahl der mit einem Projekt verknüpften Ziele. |
