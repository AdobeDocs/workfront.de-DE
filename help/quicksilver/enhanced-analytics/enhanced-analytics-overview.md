---
title: Erweiterte Analyse - Übersicht
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Enhanced Analytics ist ein leistungsstarkes Tool in Adobe Workfront mit vordefinierten Visualisierungen, mit denen Sie Projektdaten betrachten und Trends bei der Planung und beim Abschluss identifizieren können. Dieser Einblick in Ihre Projekte hilft Ihnen, Ihre aktuelle Arbeit zu verwalten und Ihre zukünftigen Arbeiten genauer zu planen.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 3%

---

# Erweiterte Analyse - Übersicht

>[!IMPORTANT]
>
>Enhanced Analytics wird in der Woche des 26. Mai aus Workfront entfernt. Workfront Data Connect ist eine neue, alternative Lösung und kann verwendet werden, um alle derzeit verwendeten Visualisierungen von Enhanced Analytics zu replizieren. <br>Weitere Informationen finden Sie im Handbuch [Erweiterte Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)Einstellung“.


Enhanced Analytics ist ein leistungsstarkes Tool in Adobe Workfront mit vordefinierten Visualisierungen, mit denen Sie Projektdaten betrachten und Trends bei der Planung und beim Abschluss identifizieren können. Dieser Einblick in Ihre Projekte hilft Ihnen, Ihre aktuelle Arbeit zu verwalten und Ihre zukünftigen Arbeiten genauer zu planen.

Die erweiterte Analyse kann Ihnen dabei helfen, Folgendes zu identifizieren:

* So planen Sie Projekte
* Wenn Arbeit zu Projekten hinzugefügt wird
* Der Arbeitsaufwand, der für verschiedene Projekte abgeschlossen wird
* Die Anzahl der Stunden oder Tage, die zum Abschließen eines Projekts erforderlich sind, im Vergleich zu den Stunden oder Tagen, für die ein Home-Team geplant ist
* Wie oft Benutzer während eines Projekts bestimmte Aktionen ausführen
* Der Fortschritt von Projekten sowie die einzelnen Aufgaben innerhalb eines Projekts

![Analytics](assets/nwe-full-screen-analytics-350x222.png)

Anwendungsfälle oder weitere Informationen zum Verwalten aktueller Arbeiten und zum Planen für die zukünftige Arbeit mit Enhanced Analytics finden Sie unter [Enhanced Analytics-Lernpfade](https://one.workfront.com/s/enhanced-analytics-program).

## Voraussetzungen

Um auf den erweiterten Analysebereich zuzugreifen, müssen Sie:

* Einen Business- oder Enterprise-Plan haben.

  Weitere Informationen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

* Bitten Sie Ihren Workfront-Administrator, Ihrer Layoutvorlage erweiterte Analysen hinzuzufügen.

  Weitere Informationen finden Sie unter [Erweiterte Analyse: Hinzufügen von Analysen zu Layout-Vorlagen](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Um Informationen zu Projekten und Aufgaben anzuzeigen, gehen Sie folgendermaßen vor:

* Berechtigung zum Anzeigen der Bereiche „Projekte“ und „Aufgaben“ auf Ihrer Zugriffsebene.

  Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Über Anzeigeberechtigungen für bestimmte Aufgaben und/oder Projekte verfügen.

  Weitere Informationen zum Anfordern von Zugriff finden Sie unter [Anfordern von Zugriff auf Objekte](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Best Practices für erweiterte Analysen

Um die besten Daten für Ihre Projekte zu erhalten, verwenden Sie Vorlagen mit genauen geplanten Stunden und Tagen. Außerdem müssen Sie sicherstellen, dass Ihre Benutzer die unten stehenden Felder so genau wie möglich eingeben und aktualisieren.

>[!NOTE]
>
>Einige der folgenden Felder sind Berechnungen, die Workfront basierend auf Informationen durchführt, die von Benutzenden eingegeben werden. Sie können diese Felder nicht manuell aktualisieren.

* Geplante Stunden

  Dies ist das wichtigste auszufüllende Feld.

  >[!NOTE]
  >
  >Wenn Ihre Teams keine geplanten Stunden verwenden, können Sie trotzdem einige Daten basierend auf der Projektdauer sehen.\
  >Weitere Informationen finden Sie im Abschnitt [Ansicht „Dauer](#duration-view) in diesem Artikel.

* Projektname

  Der Name sollte das Projekt beschreiben.

* Projektbedingung
* Projektstatus
* Geplantes Startdatum des Projekts
* Geplantes Abschlussdatum
* Tatsächliches Startdatum des Projekts
* Tatsächliches Enddatum des Projekts
* Projektdauer Stunden
* Tatsächliche Stunden des Projekts
* Aufgabenstatus (dies umfasst das Markieren von Aufgaben als abgeschlossen)
* Aufgabenname
* Prozentuale Abschlussrate der Aufgabe
* Geplantes Startdatum der Aufgabe
* Für die Aufgabe geplantes Abschlussdatum

>[!IMPORTANT]
>
>Es kann bis zu 24 Stunden dauern, bis Änderungen an Aufgaben und Projekten in Enhanced Analytics übernommen werden.

## Daueransicht {#duration-view}

Standardmäßig basieren die Burndown- und Projekt-Treemap-Visualisierungen auf geplanten Stunden. Wenn Ihre Teams keine geplanten Stunden verwenden, können Sie diese Visualisierungen auf Grundlage der Projektdauer anzeigen.

In Enhanced Analytics wird die Dauer eines Projekts anhand der folgenden Formeln berechnet:

* Geplanter Zeitrahmen:

  ```
  Planned Completion Date of the project - Start Date of the project
  ```

* Arbeitstage:

  ```
  Planned Duration for tasks completed in the selected date range / Typical hours per work day
  ```

  >[!NOTE]
  >
  >8 Stunden ist die Standardzahl für **Typische Stunden pro Arbeitstag**. Ein Adobe Workfront-Administrator kann die Einstellung **Typische Stunden pro Arbeitstag** unter **Setup** > **Projektvoreinstellungen** > **Projekte** > **Timelines** aktualisieren.\
  >Weitere Informationen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Informationen zur geplanten Dauer finden Sie unter [Übersicht über die Projektdauer](../manage-work/projects/planning-a-project/project-duration.md).

## Tastaturbefehle

Sie können die folgenden Tasten auf Ihrer Tastatur verwenden, um im erweiterten Analysebereich durch bestimmte Aktionen zu navigieren oder diese auszuführen:

| Schlüssel | Aktion |
|---|---|
| **tab** | Navigieren Sie zu jedem Element auf der Seite sowie zu einer Tabelle mit Informationen zu jeder Visualisierung, die nicht auf der Seite angezeigt wird |
| **Eingeben** | Öffnen Sie das Kalender-Widget, löschen Sie einen vorhandenen Filter, öffnen Sie die Filteroptionen hinzufügen, wählen/deaktivieren Sie Filterwerte, wenden Sie einen von Ihnen erstellten Filter an, öffnen Sie die Exportoptionen für jede Visualisierung, öffnen Sie die Dropdown-Menüs für die Burndown-Visualisierungen, Aufgaben im Flug und Projekt-Treemap-Visualisierungen |
| **Pfeiltasten** | Navigieren Sie zu Datumsangaben im Kalender-Widget, durch Filteroptionen beim Hinzufügen eines Filters und durch Optionen in allen Dropdown-Menüs in den Visualisierungen |
| **Leertaste** | Wählen Sie Datumsangaben im Kalender-Widget aus, wählen Sie beim Hinzufügen eines Filters einen Filtertyp aus, wählen Sie eine Exportoption aus dem Dropdown-Menü für jede Visualisierung aus und wählen Sie Optionen aus den Dropdown-Menüs für die Visualisierungen Burndown , Aufgaben im Flug und Projekt-Treemap aus |

{style="table-layout:auto"}

Wenn Sie eine Bildschirmlesehilfe oder ein Plug-in verwenden, liest die Bildschirmlesehilfe die Informationen auf dem Bildschirm laut vor und beschreibt die Aktionen, die Sie ausführen, während Sie die oben aufgeführten Tasten verwenden.

## Erweiterte Analyseansichten und -funktionen

Weitere Informationen zu den Details einer bestimmten Funktion in Enhanced Analytics, zu den Aktionen, die Sie durchführen können, um weitere Einblicke zu erhalten, und dazu, was Sie aus diesen Daten lernen können, finden Sie in den folgenden Artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Artikel</th> 
   <th>Erklärung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Anwenden von Filtern in Enhanced Analytics</a> </td> 
   <td> <p>Sie können benutzerdefinierte Filter, Projektfeldfilter oder Team-Filter anwenden, um nur Projekte anzuzeigen, die bestimmten Kriterien entsprechen. Beim Hinzufügen von Filtern wird die Anzahl der Projekte entsprechend aktualisiert.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Erfahren Sie mehr über die KPIs der erweiterten Analyse</a> </td> 
   <td> <p>Die wichtigsten Leistungsindikatoren (KPIs) für alle Projekte innerhalb eines bestimmten Zeitrahmens befinden sich oben im Bildschirm.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Sehen Sie sich die Flugplanvisualisierung in Enhanced Analytics an</a> </p> </td> 
   <td> <p>Die <b>Flugplan</b>-Visualisierung zeigt Ihnen, wie sich der Zustand im Laufe des Projekts geändert hat. Durch Interaktion mit der Visualisierung erhalten Sie weitere Details zu bestimmten Daten. Wenn Sie ein Projekt auswählen, werden der Burndown und die Aufgaben in Flugvisualisierungen geöffnet.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Anzeigen der Burndown-Visualisierung in Enhanced Analytics</a> </td> 
   <td> <p>Die <b>Burndown</b>-Visualisierung zeigt die geplante Geschwindigkeit eines Projekts im Vergleich zur tatsächlichen Anzahl der Stunden, die für ein Projekt aufgewendet wurden. Durch Interaktion mit der Visualisierung erhalten Sie weitere Details über den Zustand des Projekts an einem bestimmten Datum.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics</a> </td> 
   <td> <p>Die <b>Aufgaben im Flug</b> Visualisierung zeigt den Status jeder Aufgabe innerhalb eines Projekts an. Durch die Interaktion mit der Visualisierung können Sie schnell und einfach Änderungen an einer Aufgabe vornehmen.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Anzeigen der Visualisierung von Projektaktivitäten in Enhanced Analytics</a> </td> 
   <td> <p>Die <b>Projektaktivität</b>-Visualisierung zeigt Ihnen eine Heatmap, aus der ersichtlich ist, wann Benutzende, die einem Projekt zugewiesen sind, sich bei Workfront angemeldet haben, den Aufgabenstatus in diesem Projekt geändert haben und Aufgaben in diesem Projekt erledigt haben. Durch Interaktion mit der Visualisierung können Sie diese Details für jeden Benutzer anzeigen. Sie können auch bestimmte Daten für diese Aktionen sowie die Anzahl der Abschlüsse jeder Aktion sehen.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Anzeigen der Projekt-Treemap-Visualisierung in Enhanced Analytics</a> </td> 
   <td> <p>Die <b>Projekt-Treemap</b>-Visualisierung zeigt Ihnen, wie viel Zeit an einigen Projekten im Vergleich zu anderen verbracht wurde. Durch Interaktion mit der Visualisierung erhalten Sie Details zum Zustand des Projekts, zum geplanten Abschluss des Projekts und zum tatsächlichen Abschluss des Projekts.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Visualisierung „Aktivität nach Team“ in Enhanced Analytics anzeigen</a> </td> 
   <td> <p>Die <b>Aktivität nach Team</b>-Visualisierung zeigt eine Heatmap an, aus der ersichtlich ist, wann sich Benutzer eines Haupt-Teams bei Workfront angemeldet, den Status einer Aufgabe geändert und eine Aufgabe abgeschlossen haben. Durch Interaktion mit der Visualisierung können Sie diese Details für jeden einzelnen Benutzer anzeigen. Sie können auch bestimmte Daten für diese Aktionen sowie die Anzahl der Abschlüsse jeder Aktion sehen.</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>
