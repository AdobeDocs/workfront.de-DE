---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Überprüfen Sie Diagramme, um die Trends beim Zielfortschritt in Adobe Workfront-Zielen zu verstehen.
description: Sie können den allgemeinen Zustand Ihrer Ziele und ihren Fortschritt rechtzeitig im Abschnitt Diagramme der Adobe Workfront-Ziele anzeigen. Die Diagramme in diesem Abschnitt zeigen nicht den Fortschritt der einzelnen Ziele, sondern geben Ihnen eine ganzheitliche Übersicht über den Fortschrittsstatus aller Ziele sowie über den zeitlichen Fortschrittstrend in einem bestimmten Zeitraum.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Überprüfen Sie Diagramme, um die Trends beim Zielfortschritt in Adobe Workfront-Zielen zu verstehen.

<!-- drafted mostly for P&P release-->

Sie können den allgemeinen Zustand Ihrer Ziele und ihren Fortschritt rechtzeitig im Abschnitt Diagramme der Adobe Workfront-Ziele anzeigen. Die Diagramme in diesem Abschnitt zeigen nicht den Fortschritt der einzelnen Ziele, sondern geben Ihnen eine ganzheitliche Übersicht über den Fortschrittsstatus aller Ziele sowie über den zeitlichen Fortschrittstrend in einem bestimmten Zeitraum.

>[!IMPORTANT]
>
>Sie können die Gesamtanzahl Ihrer Ziele im Abschnitt Diagramme für einen ausgewählten Zeitraum anzeigen. Bei den Workfront-Zielen werden jedoch nur Ziele mit dem Status Aktiv und Abgeschlossen berücksichtigt, wenn der Gesamtfortschrittsstatus des Ziels und der Prozentsatz seiner Fertigstellung berechnet werden.

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

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

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
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Ziele anzeigen oder höher</p> <p><b>NOTIZ</b><p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Zugriff auf Adobe Workfront-Ziele gewähren</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <div> 
     <p>Anzeigen oder Höhere Berechtigungen für Ziele</p> 
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Grafiktypen in Workfront Goals

Die folgenden Diagramme sind im Abschnitt Diagramme oder Workfront-Ziele verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Das Zielgesundheitdiagramm</td> 
   <td> <p>Ein Diagramm mit der folgenden Darstellung:</p> 
    <ul> 
     <li>Eine Gesamtzahl der Ziele für den ausgewählten Zeitraum. Ziele mit einem beliebigen Status werden berücksichtigt. </li> 
     <li>Der Fortschrittsstatus von Zielen mit dem Status "Aktiv"und "Geschlossen".</li> 
    </ul> <p>Informationen zur Berechnung des Fortschrittsstatus von Workfront Goals finden Sie unter <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Übersicht über den Zielfortschritt und die Bedingungen in Adobe Workfront-Zielen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Das Zielfortschrittsdiagramm</td> 
   <td> <p>Ein Liniendiagramm, das die während der Zieldauer vorgenommenen Aktualisierungen an Zielen in wöchentlichen Schritten anzeigt. Das Zielfortschrittsdiagramm enthält Folgendes:</p> 
    <ul> 
     <li>Durchschnittliche erwartete und tatsächliche Prozentzahl aller aktiven und geschlossenen Ziele im ausgewählten Zeitraum. Der prozentuale Gesamtfortschritt wird in wöchentliche, von Knoten markierte Inkrementierungen unterteilt. </li> 
     <li>Gesamtdurchschnitt des Fortschritts bei aktiven und abgeschlossenen Zielen seit der Vorwoche. </li> 
    </ul> <p>Tipp: Im Zielfortschrittsdiagramm werden möglicherweise keine Informationen angezeigt, wenn außerhalb des ausgewählten Zeitraums Aktualisierungen an den Zielen vorgenommen werden. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Überprüfen des Zielfortschritts in Diagrammen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) > **Ziele** in der oberen rechten Ecke.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dadurch wird der Workfront-Zielbereich geöffnet.

1. Klicken **Diagramme** im linken Bereich.

   ![](assets/graphs-in-left-panel.png)

   Der Abschnitt Diagramme wird angezeigt.

   Standardmäßig sind die im Abschnitt Diagramme angezeigten Ziele durch die folgenden Kriterien eingeschränkt:

   * Die auf den Bereich &quot;Diagramme&quot;angewendeten Filter.
   * Ziele, die den Status &quot;Aktiv&quot;und &quot;Entwurf&quot;aufweisen.

1. (Optional) Wählen Sie den Informationstyp aus, der angezeigt werden soll, indem Sie die Filter in der oberen rechten Ecke des Bereichs Diagramme aktualisieren.

   Weitere Informationen zum Filtern von Zielen finden Sie unter [Informationen in Adobe Workfront-Zielen filtern](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   Wenn Sie sich für die Anzeige von mehr als einem Zeitraum ausgewählt haben, werden für jeden Zeitraum ein Konsistenzdiagramm (Messung) sowie ein Fortschrittsdiagramm (Linie) angezeigt.

1. Überprüfen Sie die Informationen in der unten stehenden Tabelle, wenn Sie das Zielgesundheitsdiagramm lesen.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Gesamtzahl der Ziele | Die Zahl am unteren Rand des Diagramms gibt die Anzahl aller Ziele im ausgewählten Zeitraum in allen ausgewählten Status an. |
   |---|---|
   | Durchschnittliche prozentuale Aufschlüsselung | Oben im Diagramm zeigt diese Zahl den durchschnittlichen Prozentsatz der Vollständigkeit aktiver und geschlossener Ziele im ausgewählten Zeitraum an. |
   | Ziele und Fortschritt | Die Anzahl der Ziele für jedes Fortschrittsstatussegment, wenn Sie den Mauszeiger über die Segmente der Grafik bewegen. In den Segmenten werden nur Ziele mit dem Status Aktiv oder Geschlossen gezählt. |


1. Überprüfen Sie die Informationen in der folgenden Tabelle, wenn Sie das Zielfortschrittsdiagramm lesen.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Grundlegender Fortschritt</td> 
      <td>Die grüne Steigung zeigt den erwarteten Gesamtdurchschnitt der vollständigen aktiven und geschlossenen Ziele für den ausgewählten Zeitraum in Prozent an. Alle Ziele innerhalb eines Zeitraums werden voraussichtlich erreicht, sodass der Ausgangsfortschritt am Ende des Zeitraums immer 100 % beträgt. </td> 
     </tr> 
     <tr> 
      <td>Tatsächlicher Fortschritt</td> 
      <td> <p>Die blaue Linie zeigt den tatsächlichen Gesamtdurchschnitt der vollständigen Ziele in Prozent für den ausgewählten Zeitraum in wöchentlichen Schritten an. Jede Woche während der Dauer des Ziels wird durch einen Knoten in der Zeile markiert. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Bewegen Sie den Mauszeiger über einen Wochenknoten in das Zielfortschrittsdiagramm und überprüfen Sie Folgendes:

   * **Wochendatum**: Monat, Tag und Jahr der ausgewählten Woche.
   * **Fortschritt**: Durchschnittliche tatsächliche prozentuale Gesamtanzahl aller Ziele für die ausgewählte Woche.
   * **Grundlinie**: Durchschnittliche Fertigstellung des erwarteten Prozentsatzes aller Ziele für die ausgewählte Woche.

1. (Optional) Klicken Sie auf **Fortschritt** unten im Fortschrittsdiagramm, um die tatsächliche Gesamtfortschrittslinie zu entfernen

   Oder

   Klicken **Grundlinie** unten im Fortschrittsdiagramm, um den erwarteten Fortschritt aus der Grafik zu entfernen.

 
