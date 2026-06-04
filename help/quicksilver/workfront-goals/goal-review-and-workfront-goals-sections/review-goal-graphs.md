---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Überprüfen Sie die Diagramme, um Trends beim Zielfortschritt in Adobe Workfront Goals zu verstehen
description: Im Abschnitt Diagramme der Adobe Workfront-Ziele können Sie den Gesamtzustand Ihrer Ziele und den zeitlichen Fortschritt einsehen. Die Diagramme in diesem Abschnitt schlüsseln den Fortschritt nicht nach Zielen auf, sondern bieten Ihnen stattdessen eine ganzheitliche Momentaufnahme des Fortschrittsstatus aller Ziele sowie ihres Fortschrittstrends in einem bestimmten Zeitraum.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/urDVf7lFxl90prTZq1jsqAWD8Q-vZ6sdbnw0LIeY5Qk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 913
ht-degree: 8%

---

# Überprüfen von Diagrammen, um die Trends beim Zielfortschritt in Adobe Workfront Goals zu verstehen

<!--Audited for P&P only: 4/2025-->

Im Abschnitt Diagramme der Adobe Workfront-Ziele können Sie den Gesamtzustand Ihrer Ziele und den zeitlichen Fortschritt einsehen. Die Diagramme in diesem Abschnitt schlüsseln den Fortschritt nicht nach Zielen auf, sondern bieten Ihnen stattdessen eine ganzheitliche Momentaufnahme des Fortschrittsstatus aller Ziele sowie ihres Fortschrittstrends in einem bestimmten Zeitraum.

>[!IMPORTANT]
>
>Im Bereich Diagramme wird für einen ausgewählten Zeitraum eine Gesamtanzahl von Zielen angezeigt. Workfront-Ziele berücksichtigen jedoch nur Ziele mit dem Status Aktiv und Geschlossen bei der Berechnung des Gesamtstatus für den Zielfortschritt und des Prozentsatzes abgeschlossen.

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
 <td role="rowheader">Adobe Workfront-Lizenz</td>
 <td>
 <p>Mitwirkende oder höher</p>
<p>Anfragende oder höher</p></td>
 </tr>
  <tr>
 <td role="rowheader">Konfiguration der Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
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
    Or
    <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
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

## Diagrammtypen in Workfront Goals

Die folgenden Diagramme sind im Abschnitt Diagramme für Workfront-Ziele verfügbar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Diagramm zur Zielgesundheit</td> 
   <td> <p>Ein Messdiagramm, das Folgendes anzeigt:</p> 
    <ul> 
     <li>Eine Gesamtzahl von Zielen für den ausgewählten Zeitraum. Ziele mit beliebigem Status werden berücksichtigt. </li> 
     <li>Der Fortschrittsstatus von Zielen mit dem Status Aktiv und Geschlossen.</li> 
    </ul> <p>Informationen dazu, wie Workfront Goals den Fortschrittsstatus berechnet, finden Sie unter <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Übersicht über den Zielfortschritt und die Bedingung in Adobe Workfront Goals</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Die Grafik für den Zielfortschritt</td> 
   <td> <p>Ein Liniendiagramm, das die an den Zielen vorgenommenen Aktualisierungen in wöchentlichen Schritten während der Dauer des Ziels anzeigt. Das Diagramm Zielfortschritt zeigt Folgendes an:</p> 
    <ul> 
     <li>Ein durchschnittlicher erwarteter und tatsächlicher abgeschlossener Prozentsatz aller aktiven und geschlossenen Ziele im ausgewählten Zeitraum. Der Fortschritt in Prozent abgeschlossen wird in wöchentliche Inkremente unterteilt, die durch -Knoten gekennzeichnet sind. </li> 
     <li>Der durchschnittliche Gesamtfortschritt für aktive und geschlossene Ziele seit der Vorwoche. </li> 
    </ul> <p>Tipp: Das Diagramm zum Zielfortschritt zeigt möglicherweise keine Informationen an, wenn außerhalb des ausgewählten Zeitraums Aktualisierungen an den Zielen vorgenommen werden. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Überprüfen des Zielfortschritts in Diagrammen

{{step1-to-goals}}

Dadurch wird der Bereich Workfront-Ziele geöffnet.

1. Klicken Sie **linken** auf „Diagramme“.

   ![Diagramme im linken Bedienfeld](assets/graphs-in-left-panel.png)

   Der Abschnitt Diagramme wird angezeigt.

   Standardmäßig werden die im Abschnitt Diagramme angezeigten Ziele durch die folgenden Kriterien eingeschränkt:

   * Die auf den Bereich Diagramme angewendeten Filter.
   * Ziele mit dem Status Aktiv und Entwurf

1. (Optional) Wählen Sie den Typ der Informationen aus, die angezeigt werden sollen, indem Sie die Filter in der oberen rechten Ecke des Abschnitts Diagramme aktualisieren.

   Weitere Informationen zum Filtern von Zielen finden Sie unter [Filtern von Informationen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Wenn Sie ausgewählt haben, mehr als einen Zeitraum anzuzeigen, werden für jeden Zeitraum ein Konsistenzdiagramm (Messgerät) sowie ein Fortschrittsdiagramm (Linie) angezeigt.

1. Überprüfen Sie die Informationen in der folgenden Tabelle, wenn Sie die Zielintegritätstabelle überprüfen.

   ![Tacho-Diagramm](assets/gauge-graph-wf-align-350x230.png)

   | Gesamtzahl der Ziele | Die Zahl am unteren Rand des Diagramms gibt die Anzahl aller Ziele im ausgewählten Zeitraum in allen ausgewählten Status an. |
   |---|---|
   | Durchschnittlicher Prozentsatz abgeschlossen | Am oberen Rand des Diagramms gibt diese Zahl den durchschnittlichen Prozentsatz der abgeschlossenen aktiven und geschlossenen Ziele in dem ausgewählten Zeitraum an. |
   | Ziele und ihr Fortschritt | Die Anzahl der Ziele für jedes Fortschrittsstatussegment, wenn Sie den Mauszeiger über die Segmente des Diagramms bewegen. Nur Ziele mit dem Status Aktiv oder Geschlossen werden in den Segmenten gezählt. |


1. Überprüfen Sie die Informationen in der folgenden Tabelle, wenn Sie die Tabelle für den Zielfortschritt überprüfen.

   ![Liniendiagramm](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Baseline-Fortschritt</td> 
      <td>Die grüne Steigungslinie gibt den erwarteten Gesamtdurchschnitt der abgeschlossenen aktiven und geschlossenen Ziele für den ausgewählten Zeitraum in Prozent an. Es wird erwartet, dass alle Ziele innerhalb eines Zeitraums abgeschlossen werden, sodass der grundlegende Fortschritt am Ende des Zeitraums immer 100 % beträgt. </td> 
     </tr> 
     <tr> 
      <td>Tatsächlicher Fortschritt</td> 
      <td> <p>Die blaue Linie zeigt den tatsächlichen prozentualen Gesamtdurchschnitt der aktiven und geschlossenen Ziele für den ausgewählten Zeitraum in wöchentlichen Schritten an. Jede Woche während der Dauer des Ziels wird durch einen Knoten in der Zeile markiert. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Bewegen Sie den Mauszeiger über einen Wochenknoten im Diagramm zum Zielfortschritt und überprüfen Sie Folgendes:

   * **Wochendatum**: Der Monat, Tag und das Jahr der ausgewählten Woche.
   * **Fortschritt**: Ein Durchschnitt des tatsächlichen Prozentsatzes der vollständigen Ziele für die ausgewählte Woche.
   * **Baseline**: Ein Durchschnitt des erwarteten Prozentsatzes der vollständigen Ziele für die ausgewählte Woche.

1. (Optional) Klicken Sie **Fortschritt** unten im Fortschrittsdiagramm, um die tatsächliche Gesamtfortschrittslinie zu entfernen

   ODER

   Klicken Sie **Baseline** am unteren Rand des Fortschrittsdiagramms, um den erwarteten Fortschritt aus dem Diagramm zu entfernen.


