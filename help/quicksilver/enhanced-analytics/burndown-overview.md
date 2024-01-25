---
title: Anzeigen der Niederschlagsvisualisierung in der erweiterten Analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Niederschlagsvisualisierung zeigt den Niedergang eines bestimmten Projekts im Zeitverlauf und hilft Ihnen, die Beziehung zwischen Projektbedingung, Geschwindigkeit und verbleibenden Stunden - oder Tagen zu verstehen.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Anzeigen der Niederschlagsvisualisierung in der erweiterten Analyse

<!-- Audited: 12/2023 -->

Die Niederschlagsvisualisierung zeigt den Niedergang eines bestimmten Projekts im Zeitverlauf und hilft Ihnen, die Beziehung zwischen Projektbedingung, Geschwindigkeit und verbleibenden Stunden - oder Tagen zu verstehen.

![Beispiel für einen optimierten Analyseaufbau](assets/burndown120623.png)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>
      <p>Neu: Beliebig</p>
      <p>oder</p>
      <p>Aktuell: Business oder höher</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
      <p>Neu: Licht oder höher</p>
      <p>oder</p>
      <p>Aktuell: Überprüfen oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
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

Voraussetzungen für die Verwendung von Enhanced Analytics finden Sie im Abschnitt &quot;Voraussetzungen&quot;unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Grundlegendes zur Aufschlüsselungsvisualisierung

Die durchgehende blaue Linie zeigt die geplante Geschwindigkeit vom Startdatum bis zum geplanten Abschlussdatum an. Diese Zeile wird angepasst, wenn die Arbeit hinzugefügt, entfernt oder aktualisiert wird, und sie wird in eine gestrichelte vertikale Linie umgewandelt, wenn das Projekt das geplante Abschlussdatum erreicht.

![Geplante Geschwindigkeit](assets/burndown-planned-line.png)

Die tatsächliche Zeile zeigt die Anzahl der Stunden - oder Tage - an, die im Zeitverlauf für das Projekt verbracht wurden. Die Farbe dieser Zeile zeigt die tägliche Bedingung des Projekts an:

* **Grün**: Das Projekt wurde ausgewählt.

  ![Zielgruppe](assets/burndown-green.png)

* **Orange**: Das Projekt ist in Gefahr.

  ![Risiko](assets/burndown-orange.png)

* **Rot**: Das Projekt ist in Schwierigkeiten.

  ![In Schwierigkeiten](assets/burndown-red.png)

Weitere Informationen zu diesen Projektbedingungen finden Sie unter [Übersicht über Projektbedingung und Bedingungstyp](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Wenn die tatsächliche Zeile vertikal nach oben bewegt wird, wurde dem Projekt Arbeit hinzugefügt. Wenn die Linie vertikal nach unten bewegt wird, wurde die Arbeit für das Projekt entfernt oder abgeschlossen.

Unter der X-Achse der Visualisierung können Sie weitere Informationen darüber sehen, wie sich Aufgaben und Stunden - oder Tage - an einem bestimmten Tag geändert haben (hinzugefügter Betrag, abgeschlossener Betrag und Differenz zwischen den beiden).

Wenn Sie alle diese Informationen in der Aufschlüsselungsvisualisierung anzeigen, können Sie Folgendes feststellen:

* Die Gesundheit des einzelnen Projekts im Zeitverlauf
* Auswirkungen der eingetretenen (oder ungeplanten) Arbeiten auf die geplante Arbeit
* Welche Ereignisse haben Ihr Projekt nach dem ursprünglichen Abschlussdatum erweitert?

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Ansicht der Niederschlagsvisualisierung

{{step1-to-analytics}}

1. (Optional) Wenn Sie einen anderen Datumsbereich verwenden möchten, wählen Sie im Filter für den Datumsbereich die neuen Start- und Enddaten aus.

   ![Datumsangaben auswählen](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Datumsbereichfilters finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie den Projektdatensatz einschränken müssen, wählen Sie die Filter aus, die Sie verwenden möchten, und wenden Sie sie an.

   Weitere Informationen zum Hinzufügen von Filtern in der erweiterten Analyse finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nach dem Hinzufügen von Filtern werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. (Optional) Wenn Sie einen Datumsbereich vergrößern möchten, wählen Sie einen Punkt auf der Visualisierung für den Anfang Ihres Datumsbereichs aus und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und es wird automatisch ein Zeitrahmen-Filter erstellt.

   ![Zeitrahmen-Filter](assets/timeframe-filter-350x220.png)

1. Klicken Sie in der Visualisierung Flugplan oder Projekt-Treemap auf ein Projekt, um weitere Informationen anzuzeigen.

   Die Niederschläge und Aufgaben in den Flugvisualisierungen werden angezeigt.

   >[!NOTE]
   >
   >Weitere Informationen zu diesen anderen Visualisierungen finden Sie unter:
   >
   >   * [Anzeigen der Visualisierung des Flugplans in der erweiterten Analyse](../enhanced-analytics/flight-plan-overview.md)
   >   * [Anzeigen der Projekt-Treemap-Visualisierung in Enhanced Analytics](../enhanced-analytics/project-treemap-overview.md)
   >   * [Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. (Optional) Ändern Sie die Ansicht von den geplanten Stunden in **duration**.

   Geplante Stunden ist standardmäßig ausgewählt.

   >[!NOTE]
   >
   >Auswählen **duration** ändert alle Stundeninformationen in Tage.\
   >![Duration-Burndown](assets/duration-burndown-350x112.png)\
   >Weitere Informationen zur Dauer im Bereich &quot;Erweiterte Analyse&quot;finden Sie im Abschnitt &quot;Ansicht der Dauer&quot;unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. Klicken Sie auf einen beliebigen Punkt im Liniendiagramm.

   Unter dem Diagramm wird das genaue Datum angezeigt und weitere Informationen zu Aufgaben und Stunden - oder Tagen - für den ausgewählten Tag werden angezeigt.

   ![Details zur Verteilung](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >Wenn die tatsächliche Geschwindigkeit eine flache Linie ist, die entlang der x-Achse verläuft (inline mit 0 Stunden oder 0 Tagen) der Visualisierung, bedeutet dies, dass dem Projekt keine geplanten Stunden oder Tage hinzugefügt wurden.\
   >Wenn die tatsächliche Geschwindigkeit eine flache Linie über der x-Achse ist (inline mit einer Anzahl von Stunden oder Tagen), die nie zurückgeht, bedeutet dies, dass innerhalb des gefilterten Zeitraums keine Aufgaben abgeschlossen wurden.

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie auf das **Export** icon ![Symbol &quot;Exportieren&quot;](assets/export.png) in der oberen rechten Ecke der Visualisierung und wählen Sie das Exportformat aus:

   * Diagramm (PNG)
   * Datentabelle (XSLX)

1. (Optional) Um Details über den Fortschritt von Aufgaben im ausgewählten Projekt anzuzeigen, sehen Sie sich die Aufgaben in der Flugvisualisierung an, die unter der Aufschlüsselungsvisualisierung angezeigt wird. Weitere Informationen finden Sie unter [Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
