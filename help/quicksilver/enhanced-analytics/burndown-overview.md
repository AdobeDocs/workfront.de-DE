---
title: Anzeigen der Burndown-Visualisierung in erweiterten Analysen
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Burndown-Visualisierung zeigt den Burndown eines bestimmten Projekts im Zeitverlauf und hilft Ihnen, die Beziehung zwischen dem Projektzustand, der Geschwindigkeit und den verbleibenden Stunden (oder Tagen) zu verstehen.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# Anzeigen der Burndown-Visualisierung in erweiterten Analysen

>[!IMPORTANT]
>
>Enhanced Analytics wird in der Woche des 26. Mai aus Workfront entfernt. Workfront Data Connect ist eine neue, alternative Lösung und kann verwendet werden, um alle derzeit verwendeten Visualisierungen von Enhanced Analytics zu replizieren. <br>Weitere Informationen finden Sie im Handbuch [Erweiterte Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)Einstellung“.


<!-- Audited: 12/2023 -->

Die Burndown-Visualisierung zeigt den Burndown eines bestimmten Projekts im Zeitverlauf und hilft Ihnen, die Beziehung zwischen dem Projektzustand, der Geschwindigkeit und den verbleibenden Stunden (oder Tagen) zu verstehen.

![Beispiel für ein erweitertes Analyse-Burndown](assets/burndown120623.png)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>
      <p>Neu: Beliebig</p>
      <p>oder</p>
      <p>Aktuell: Unternehmen oder höher</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
      <p>Neu: Licht oder höher</p>
      <p>oder</p>
      <p>Aktuell: Überprüfung oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen</p> </td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Voraussetzungen für die Verwendung der erweiterten Analyse finden Sie im Abschnitt „Voraussetzungen“ in [Übersicht über die erweiterte Analyse](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung für Burndown

Die durchgezogene blaue Linie zeigt die geplante Geschwindigkeit vom Startdatum bis zum geplanten Abschlussdatum. Diese Linie wird angepasst, wenn Arbeiten hinzugefügt, entfernt oder aktualisiert werden, und ändert sich in eine gestrichelte vertikale Linie, wenn das Projekt das geplante Abschlussdatum erreicht.

![Geplante Geschwindigkeit](assets/burndown-planned-line.png)

Die tatsächliche Linie zeigt die Anzahl der Stunden - oder Tage -, die im Laufe der Zeit für das Projekt aufgewendet wurden. Die Farbe dieser Linie zeigt den Zustand des Projekts jeden Tag an:

* **Grün**: Das Projekt ist am Ziel.

  ![Im Zielbereich](assets/burndown-green.png)

* **Orange**: Das Projekt ist in Gefahr.

  ![Gefährdet](assets/burndown-orange.png)

* **Red**: Das Projekt ist in Schwierigkeiten.

  ![In Schwierigkeiten](assets/burndown-red.png)

Weitere Informationen zu diesen Projektbedingungen finden Sie unter [Übersicht über Projektbedingung und Bedingungstyp](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Wenn die tatsächliche Linie vertikal nach oben bewegt wird, wurde dem Projekt Arbeit hinzugefügt. Wenn die Linie vertikal nach unten bewegt wird, wurden die Arbeiten für das Projekt entfernt oder abgeschlossen.

Unter der x-Achse der Visualisierung sehen Sie weitere Informationen darüber, wie sich Aufgaben und Stunden - oder Tage - an einem bestimmten Tag geändert haben (den hinzugefügten Betrag, den abgeschlossenen Betrag und die Differenz zwischen den beiden).

Wenn Sie alle diese Informationen in der Burndown-Visualisierung sehen, können Sie Folgendes ermitteln:

* Zustand des einzelnen Projekts im Zeitverlauf
* Auswirkungen von Problemen (oder ungeplanten Arbeiten) auf die geplanten Arbeiten
* Welche Ereignisse haben Ihr Projekt über das ursprüngliche Abschlussdatum hinaus verlängert?

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Anzeigen der Burndown-Visualisierung

{{step1-to-analytics}}

1. (Optional) Um einen anderen Datumsbereich zu verwenden, wählen Sie im Datumsbereichsfilter Neues Start- und Enddatum aus.

   ![Daten auswählen](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Filters für den Datumsbereich finden Sie unter [Anwenden von Filtern in der erweiterten Analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie den Projektdatensatz einschränken müssen, wählen Sie die gewünschten Filter aus und wenden Sie sie an.

   Weitere Informationen zum Hinzufügen von Filtern in der erweiterten Analyse finden Sie unter [Anwenden von Filtern in der erweiterten Analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nachdem Sie Filter hinzugefügt haben, werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. (Optional) Um einen Datumsbereich heranzuzoomen, wählen Sie einen Punkt auf der Visualisierung für den Beginn Ihres Datumsbereichs und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert, und es wird automatisch ein Zeitrahmenfilter erstellt.

   ![Zeitrahmen-Filter](assets/timeframe-filter-350x220.png)

1. Klicken Sie in der Flugplan- oder Projekt-Treemap-Visualisierung auf ein Projekt, um weitere Informationen anzuzeigen.

   Burndown und Aufgaben in Flugvisualisierungen werden angezeigt.

   >[!NOTE]
   >
   >Weitere Informationen zu diesen anderen Visualisierungen finden Sie unter:
   >
   >   * [Sehen Sie sich die Flugplanvisualisierung in Enhanced Analytics an](../enhanced-analytics/flight-plan-overview.md)
   >   * [Anzeigen der Projekt-Treemap-Visualisierung in Enhanced Analytics](../enhanced-analytics/project-treemap-overview.md)
   >   * [Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Optional) Ändern Sie die Ansicht von „Geplante Stunden“ in **Dauer**.

   Geplante Stunden sind standardmäßig ausgewählt.

   >[!NOTE]
   >
   >Durch Auswahl von **Dauer** werden alle Stundeninformationen in Tage geändert.\
   >![Dauer des Burndowns](assets/duration-burndown-350x112.png)\
   >Weitere Informationen zur Dauer im erweiterten Analysebereich finden Sie im Abschnitt „Ansicht der Dauer“ in [Übersicht über die erweiterte Analyse](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Klicken Sie auf einen beliebigen Punkt im Liniendiagramm.

   Das genaue Datum wird angezeigt, und unter dem Diagramm werden weitere Informationen zu Aufgaben und Stunden - oder Tagen - für den ausgewählten Tag angezeigt.

   ![Burndown-Details](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Wenn die tatsächliche Geschwindigkeit eine flache Linie ist, die entlang der X-Achse (inline mit 0 Stunden oder 0 Tagen) der Visualisierung verläuft, bedeutet dies, dass keine geplanten Stunden - oder Tage - zum Projekt hinzugefügt wurden.\
   >Wenn die tatsächliche Geschwindigkeit eine flache Linie über der X-Achse ist (inline mit einer Anzahl von Stunden oder Tagen) und nie absinkt, bedeutet dies, dass innerhalb des gefilterten Zeitraums keine Aufgaben abgeschlossen wurden.

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie auf **Export**-Symbol ![Export-](assets/export.png)) in der oberen rechten Ecke der Visualisierung und wählen Sie das Exportformat aus:

   * Diagramm (PNG)
   * Datentabelle (XSLX)

1. (Optional) Um Details zum Fortschritt von Aufgaben im ausgewählten Projekt anzuzeigen, sehen Sie sich die Aufgaben in der Flugvisualisierung an, die unter der Burndown-Visualisierung angezeigt wird. Weitere Informationen finden Sie unter [Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
