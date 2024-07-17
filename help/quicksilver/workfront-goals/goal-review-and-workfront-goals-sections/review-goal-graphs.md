---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Überprüfen Sie Diagramme, um die Trends beim Zielfortschritt in Adobe Workfront-Zielen zu verstehen.
description: Sie können den allgemeinen Zustand Ihrer Ziele und ihren Fortschritt rechtzeitig im Abschnitt Diagramme der Adobe Workfront-Ziele anzeigen. Die Diagramme in diesem Abschnitt zeigen nicht den Fortschritt der einzelnen Ziele, sondern geben Ihnen eine ganzheitliche Übersicht über den Fortschrittsstatus aller Ziele sowie über den zeitlichen Fortschrittstrend in einem bestimmten Zeitraum.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 0%

---

# Überprüfen Sie Diagramme, um die Trends beim Zielfortschritt in Adobe Workfront-Zielen zu verstehen.

<!-- drafted mostly for P&P release-->

Sie können den allgemeinen Zustand Ihrer Ziele und ihren Fortschritt rechtzeitig im Abschnitt Diagramme der Adobe Workfront-Ziele anzeigen. Die Diagramme in diesem Abschnitt zeigen nicht den Fortschritt der einzelnen Ziele, sondern geben Ihnen eine ganzheitliche Übersicht über den Fortschrittsstatus aller Ziele sowie über den zeitlichen Fortschrittstrend in einem bestimmten Zeitraum.

>[!IMPORTANT]
>
>Sie können die Gesamtanzahl Ihrer Ziele im Abschnitt Diagramme für einen ausgewählten Zeitraum anzeigen. Bei den Workfront-Zielen werden jedoch nur Ziele mit dem Status Aktiv und Abgeschlossen berücksichtigt, wenn der Gesamtfortschrittsstatus des Ziels und der Prozentsatz seiner Fertigstellung berechnet werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> 
   <p>Für den neuen Plan und die Lizenzstruktur:
  <ul><li>Ein ultimativer Plan </li>
  Oder
  <li>Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. </li></ul> </p>
<p>Für den aktuellen Plan und die Lizenzstruktur: 
<ul><li> A Pro oder höher </li>
  <li>Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitarbeiter oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderungen, eine der folgenden: </p>
<ul>
<li>Ein Select- oder Prime-Adobe Workfront-Plan und eine zusätzliche Adobe Workfront Goals-Lizenz.</li>
<li>Ein Ultimate Workfront-Plan, der standardmäßig Workfront-Ziele enthält. </li></ul>
 <p>Oder</p>
 <p>Aktuelle Produktanforderungen: Ein Workfront-Plan und eine zusätzliche Lizenz für Adobe Workfront Goals. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Zugriffsebene</p></td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen oder Anzeigen höherer Berechtigungen zum Ziel</p>
  <p>Berechtigungen für das Ziel verwalten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
     <li>Der Fortschrittsstatus von Zielen mit dem Status Aktiv und Geschlossen .</li> 
    </ul> <p>Informationen dazu, wie Workfront Goals den Fortschrittsstatus berechnet, finden Sie unter <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Übersicht über den Zielfortschritt und die Bedingungen in Adobe Workfront Goals</a>.</p> </td> 
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

1. Klicken Sie oben rechts auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png) > **Ziele** .

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dadurch wird der Workfront-Zielbereich geöffnet.

1. Klicken Sie im linken Bereich auf **Diagramme** .

   ![](assets/graphs-in-left-panel.png)

   Der Abschnitt Diagramme wird angezeigt.

   Standardmäßig sind die im Abschnitt Diagramme angezeigten Ziele durch die folgenden Kriterien eingeschränkt:

   * Die auf den Bereich &quot;Diagramme&quot;angewendeten Filter.
   * Ziele, die den Status &quot;Aktiv&quot;und &quot;Entwurf&quot;aufweisen.

1. (Optional) Wählen Sie den Informationstyp aus, der angezeigt werden soll, indem Sie die Filter in der oberen rechten Ecke des Bereichs Diagramme aktualisieren.

   Weitere Informationen zu Filterzielen finden Sie unter [Informationen in Adobe Workfront-Zielen filtern](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Wenn Sie sich für die Anzeige von mehr als einem Zeitraum ausgewählt haben, werden für jeden Zeitraum ein Konsistenzdiagramm (Messung) sowie ein Fortschrittsdiagramm (Linie) angezeigt.

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

   * **Wochendatum**: Der Monat, der Tag und das Jahr der ausgewählten Woche.
   * **Fortschritt**: Ein Durchschnitt des tatsächlichen Prozentsatzes, der für alle Ziele der ausgewählten Woche erreicht wurde.
   * **Grundlinie**: Durchschnittliche Fertigstellung des erwarteten Prozentsatzes aller Ziele für die ausgewählte Woche.

1. (Optional) Klicken Sie unten im Fortschrittsdiagramm auf **Fortschritt** , um die tatsächliche Gesamtfortschrittszeile zu entfernen.

   Oder

   Klicken Sie unten im Fortschrittsdiagramm auf **Grundlinie** , um den erwarteten Fortschritt aus der Grafik zu entfernen.

 
