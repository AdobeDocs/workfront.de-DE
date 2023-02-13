---
title: Erweiterte Analyse - Übersicht
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Verbesserte Analysen sind ein leistungsstarkes Tool in Adobe Workfront mit vordefinierten Visualisierungen, mit dem Sie Projektdaten untersuchen und Trends mit Planung und Abschluss identifizieren können. Diese Einblicke in Ihre Projekte helfen Ihnen bei der Verwaltung Ihrer aktuellen Arbeit und ermöglichen Ihnen eine genauere Planung für zukünftige Arbeiten.
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 2%

---

# Erweiterte Analyse - Übersicht

Verbesserte Analysen sind ein leistungsstarkes Tool in Adobe Workfront mit vordefinierten Visualisierungen, mit dem Sie Projektdaten untersuchen und Trends mit Planung und Abschluss identifizieren können. Diese Einblicke in Ihre Projekte helfen Ihnen bei der Verwaltung Ihrer aktuellen Arbeit und ermöglichen Ihnen eine genauere Planung für zukünftige Arbeiten.

Die erweiterte Analyse kann Ihnen dabei helfen, Folgendes zu identifizieren:

* Die Projektplanung
* Wann Arbeiten zu Projekten hinzugefügt werden
* Umfang der für verschiedene Projekte abgeschlossenen Arbeiten
* Die für den Abschluss eines Projekts erforderlichen Stunden oder Tage im Vergleich zu den Stunden oder Tagen, zu denen ein Heimteam geplant ist
* Wie oft Benutzer bestimmte Aktionen während eines Projekts durchführen
* Der Fortschritt der Projekte sowie die einzelnen Aufgaben innerhalb eines Projekts

![](assets/nwe-full-screen-analytics-350x222.png)

Weitere Informationen zum Verwalten der aktuellen Arbeit und der Planung für die künftige Arbeit mit der erweiterten Analyse finden Sie unter [Verbesserte Lernpfade für Analysen](https://one.workfront.com/s/enhanced-analytics-program).

## Voraussetzungen

Um auf den Bereich &quot;Erweiterte Analyse&quot;zuzugreifen, müssen Sie:

* Sie haben einen Business- oder Enterprise-Plan.

   Weitere Informationen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

* Bitten Sie Ihren Workfront-Administrator, Ihrer Layoutvorlage erweiterte Analysen hinzuzufügen.

   Weitere Informationen finden Sie unter [Verbesserte Analyse: Hinzufügen von Analysen zu Layoutvorlagen](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

Um Informationen zu Projekten und Aufgaben anzuzeigen, müssen Sie:

* Sie haben die Berechtigung Anzeigen für die Bereiche Projekte und Aufgaben in Ihrer Zugriffsebene.

   Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Sie verfügen über Anzeigeberechtigungen für bestimmte Aufgaben und/oder Projekte.

   Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter [Zugriff auf Objekte anfordern](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## Best Practices für erweiterte Analysen

Verwenden Sie Vorlagen mit genauen geplanten Stunden und Tagen für die Dauer, um die besten Daten für Ihre Projekte zu erhalten. Außerdem müssen Sie sicherstellen, dass Ihre Benutzer die unten stehenden Felder so genau wie möglich eingeben und aktualisieren.

>[!NOTE]
>
>Einige der folgenden Felder sind Berechnungen, die Workfront anhand von vom Benutzer eingegebenen Informationen durchführt. Diese Felder können nicht manuell aktualisiert werden.

* Geplante Stunden

   Dies ist das wichtigste Feld, das ausgefüllt werden muss.

   >[!NOTE]
   >
   >Wenn Ihre Teams keine geplanten Stunden verwenden, können Sie dennoch einige Daten sehen, die auf der Projektdauer basieren.\
   >Weitere Informationen finden Sie im Abschnitt . [Ansicht &quot;Dauer&quot;](#duration-view) in diesem Artikel.

* Projektname

   Der Name sollte beschreibend für das Projekt sein.

* Projektbedingung
* Projektstatus
* Vorgesehenes Projektstartdatum
* Geplantes Abschlussdatum
* Tatsächliches Projektstartdatum
* Tatsächliches Projektende
* Projektdauer Stunden
* Tatsächliche Projektzeiten
* Aufgabenstatus (Dazu gehört das Kennzeichnen von abgeschlossenen Aufgaben.)
* Aufgabenname
* Task Percent Complete
* Geplantes Startdatum der Aufgabe
* Für die Aufgabe geplantes Abschlussdatum

>[!IMPORTANT]
>
>Es kann bis zu 24 Stunden dauern, bis Änderungen an Aufgaben und Projekten in der erweiterten Analyse berücksichtigt werden.

## Ansicht &quot;Dauer&quot; {#duration-view}

Standardmäßig basieren die Visualisierungen der Aufschlüsselung und der Projekt-Treemap auf geplanten Stunden. Wenn Ihre Teams keine geplanten Stunden verwenden, können Sie sich diese Visualisierungen basierend auf der Projektdauer ansehen.

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
   >8 Stunden ist die Standardnummer für **Typische Stunden pro Arbeitstag**. Ein Adobe Workfront-Administrator kann die **Typische Stunden pro Arbeitstag** Einstellung unter **Einrichtung** > **Projektvoreinstellungen** > **Projekte** > **Zeitpläne**.\
   >Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Informationen über die geplante Dauer finden Sie unter [Übersicht über die Projektdauer](../manage-work/projects/planning-a-project/project-duration.md).

## Tastaturbefehle

Sie können die folgenden Tasten auf Ihrer Tastatur verwenden, um bestimmte Aktionen im Bereich &quot;Erweiterte Analyse&quot;zu navigieren oder durchzuführen:

| Schlüssel | Aktion |
|---|---|
| **Tab.** | Navigieren Sie zu jedem Element auf der Seite sowie zu einer Tabelle mit Informationen zu jeder Visualisierung, die nicht auf der Seite angezeigt wird. |
| **Eingabe** | Öffnen Sie das Kalender-Widget, löschen Sie einen vorhandenen Filter, öffnen Sie die Filteroptionen hinzufügen, aktivieren/deaktivieren Sie die Filterwerte, wenden Sie einen erstellten Filter an, öffnen Sie die Exportoptionen für jede Visualisierung, öffnen Sie die Dropdown-Menüs für die Dropdown-Liste der Dropdown-Menüs für die Dropdown-Liste, Aufgaben im Flug und Projekt-Treemap-Visualisierungen |
| **Pfeiltasten** | Navigieren Sie zu Datumsangaben im Kalender-Widget durch Filteroptionen beim Hinzufügen eines Filters und durch Optionen in allen Dropdownmenüs der Visualisierungen. |
| **Leertaste** | Wählen Sie Datumsangaben im Kalender-Widget aus, wählen Sie beim Hinzufügen eines Filters einen Filtertyp aus, wählen Sie aus dem Dropdown-Menü einer jeden Visualisierung eine Exportoption aus und wählen Sie Optionen aus den Dropdown-Menüs im Dropdown-Menü der Dropdown-Liste, Aufgaben im Flug und Projekt-Treemap-Visualisierungen aus. |

{style=&quot;table-layout:auto&quot;}

Wenn Sie Software zum Lesen von Bildschirmen oder ein Plug-in verwenden, liest die Bildschirmlesehilfe die Informationen laut auf dem Bildschirm und beschreibt die Aktionen, die Sie ausführen, während Sie die oben aufgeführten Schlüssel verwenden.

## Erweiterte Analyseansichten und -funktionen

Weitere Informationen zu den Details einer bestimmten Funktion in Enhanced Analytics, den Aktionen, die Sie ausführen können, um weitere Einblicke zu erhalten, und den Informationen, die Sie aus diesen Daten lernen können, finden Sie in den folgenden Artikeln:

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
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">Filter in erweiterten Analysen anwenden</a> </td> 
   <td> <p>Sie können benutzerdefinierte Filter, Projektfeldfilter oder Teamfilter anwenden, um nur Projekte anzuzeigen, die bestimmten Kriterien entsprechen. Beim Hinzufügen von Filtern wird die Anzahl der Projekte entsprechend aktualisiert.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">Grundlegendes zu erweiterten Analyse-KPIs</a> </td> 
   <td> <p>Wichtige Leistungsindikatoren (KPIs) für alle Projekte innerhalb eines bestimmten Zeitraums befinden sich oben auf dem Bildschirm.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Anzeigen der Visualisierung des Flugplans in der erweiterten Analyse</a> </p> </td> 
   <td> <p>Die <b>Flugplan</b> -Visualisierung zeigt an, dass sich die Bedingung während der Lebensdauer eines Projekts geändert hat. Durch die Interaktion mit der Visualisierung erhalten Sie weitere Details zu bestimmten Daten. Wenn Sie ein Projekt auswählen, werden die Niederlassung und Aufgaben in den Flugvisualisierungen geöffnet.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">Anzeigen der Niederschlagsvisualisierung in der erweiterten Analyse</a> </td> 
   <td> <p>Die <b>Niederschlag</b> Die Visualisierung zeigt die geplante Geschwindigkeit eines Projekts in Bezug auf die tatsächlich für ein Projekt aufgewendete Zeit. Durch die Interaktion mit der Visualisierung erhalten Sie weitere Details zur Bedingung des Projekts an einem bestimmten Datum.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics</a> </td> 
   <td> <p>Die <b>Aufgaben während des Fluges</b> Visualisierung zeigt Ihnen den Status jeder Aufgabe innerhalb eines Projekts an. Durch die Interaktion mit der Visualisierung können Sie schnell und einfach Änderungen an einer Aufgabe vornehmen.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">Anzeigen der Visualisierung der Projektaktivität in der erweiterten Analyse</a> </td> 
   <td> <p>Die <b>Projektaktivität</b> Die Visualisierung zeigt eine Heatmap, die angibt, wann Benutzer einem Projekt zugewiesen sind, das sich bei Workfront angemeldet hat, den Aufgabenstatus in diesem Projekt geändert und Aufgaben in diesem Projekt abgeschlossen haben. Durch die Interaktion mit der Visualisierung können Sie diese Details für jeden Benutzer anzeigen. Sie können auch bestimmte Daten für diese Aktionen sowie die Anzahl der durchgeführten Aktionen anzeigen.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">Anzeigen der Projekt-Treemap-Visualisierung in Enhanced Analytics</a> </td> 
   <td> <p>Die <b>Projekt-Treemap</b> Die Visualisierung zeigt Ihnen, wie viel Zeit für einige Projekte im Vergleich zu anderen verbracht wurde. Durch die Interaktion mit der Visualisierung erhalten Sie Details zum Zustand des Projekts, zum geplanten Abschluss des Projekts und zum tatsächlichen Abschluss des Projekts.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Anzeigen der Aktivitäts-Visualisierung nach Team in Enhanced Analytics</a> </td> 
   <td> <p>Die <b>Aktivität nach Team</b> Die Visualisierung zeigt Ihnen eine Heatmap, die angibt, wann sich Benutzer in einem Startseiten-Team bei Workfront angemeldet haben, den Status einer Aufgabe geändert und eine Aufgabe abgeschlossen haben. Durch die Interaktion mit der Visualisierung können Sie diese Details für jeden einzelnen Benutzer anzeigen. Sie können auch bestimmte Daten für diese Aktionen sowie die Anzahl der durchgeführten Aktionen anzeigen.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">Anzeigen der Visualisierung der Ressourcenkapazität in Enhanced Analytics</a> </td> 
   <td> <p>Die <b>Ressourcenkapazität</b> Die Visualisierung zeigt Ihnen, welche Startseiten über die nötigen Kapazitäten verfügen, um mehr Arbeit zu leisten, und welche Startseiten mehr Arbeit zugewiesen haben, als sie abschließen können. Durch die Interaktion mit der Visualisierung können Sie weitere Details zu abgeschlossenen Arbeiten und verfügbaren Stunden für weitere Arbeiten anzeigen. Wenn Sie ein Team auswählen, wird die Visualisierung der Teamkapazität geöffnet.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">Visualisierung der Teamkapazität in der erweiterten Analyse anzeigen</a> </td> 
   <td> <p>Die <b>Teamkapazität</b> Die Visualisierung zeigt Ihnen einen Prozentsatz der Arbeit, die ein Heimteam aus der ihnen zugewiesenen Arbeit geleistet hat. Durch die Interaktion mit der Visualisierung können Sie geplante Stunden und geplante Stunden für ein bestimmtes Datum sowie den Kapazitätsprozentsatz anzeigen und feststellen, ob das Startseiten-Team an diesem Tag vorbei war, unterwegs war oder über Kapazität verfügte.</p> </td> 
  </tr> 
 </tbody> 
</table>
