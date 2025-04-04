---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Überprüfen Sie die Diagramme, um Trends beim Zielfortschritt in Adobe Workfront Goals zu verstehen
description: Im Abschnitt Diagramme der Adobe Workfront-Ziele können Sie den Gesamtzustand Ihrer Ziele und den zeitlichen Fortschritt einsehen. Die Diagramme in diesem Abschnitt schlüsseln den Fortschritt nicht nach Zielen auf, sondern bieten Ihnen stattdessen eine ganzheitliche Momentaufnahme des Fortschrittsstatus aller Ziele sowie ihres Fortschrittstrends in einem bestimmten Zeitraum.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: a64f6e507d74201cba1455fbbc6af77c2b7ba058
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 0%

---

# Überprüfen Sie die Diagramme, um die Zielfortschrittstrends in Adobe Workfront Goals zu verstehen

<!--Audited for P&P only: 4/2025-->

Im Abschnitt Diagramme der Adobe Workfront-Ziele können Sie den Gesamtzustand Ihrer Ziele und den zeitlichen Fortschritt einsehen. Die Diagramme in diesem Abschnitt schlüsseln den Fortschritt nicht nach Zielen auf, sondern bieten Ihnen stattdessen eine ganzheitliche Momentaufnahme des Fortschrittsstatus aller Ziele sowie ihres Fortschrittstrends in einem bestimmten Zeitraum.

>[!IMPORTANT]
>
>Im Bereich Diagramme wird für einen ausgewählten Zeitraum eine Gesamtanzahl von Zielen angezeigt. Workfront-Ziele berücksichtigen jedoch nur Ziele mit dem Status Aktiv und Geschlossen bei der Berechnung des Gesamtstatus für den Zielfortschritt und des Prozentsatzes abgeschlossen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> 
   <p>Für die neue Plan- und Lizenzstruktur:
  <ul><li>Ein Ultimate-Plan </li></ul>
   </p>
<p>Für die aktuelle Plan- und Lizenzstruktur: 
<ul><li> Ein Profi oder höher </li>
  <li>Eine Adobe Workfront-Ziellizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitwirkende oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
    <p> Neue Produktanforderung: Workfront</p>
    Oder
    <p>Aktuelle Produktanforderung: Zusätzlich zu einer Workfront-Lizenz müssen Sie eine Lizenz für Adobe Workfront Goals erwerben. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Zugriffsebene</p></td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzenden, einschließlich Workfront-Administratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) > **Ziele** in der oberen rechten Ecke.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

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

   Oder

   Klicken Sie **Baseline** am unteren Rand des Fortschrittsdiagramms, um den erwarteten Fortschritt aus dem Diagramm zu entfernen.

 
