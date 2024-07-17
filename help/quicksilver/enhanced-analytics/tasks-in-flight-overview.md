---
title: Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Aufgaben in der Flugvisualisierung zeigen an, wie viele Aufgaben (innerhalb der angewendeten Filterkriterien) für ein Projekt ausgeführt werden, wie hoch der Prozentsatz der für jede Aufgabe abgeschlossenen Aufgaben ist und wie planmäßig die Aufgaben ablaufen.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 4%

---

# Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics

Die Aufgaben in der Flugvisualisierung zeigen an, wie viele Aufgaben (innerhalb der angewendeten Filterkriterien) für ein Projekt ausgeführt werden, wie hoch der Prozentsatz der für jede Aufgabe abgeschlossenen Aufgaben ist und wie planmäßig die Aufgaben ablaufen.

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-Plan</a>*</td> 
   <td> <p>Unternehmen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> <p>Zugriff auf Aufgaben anzeigen (Um Aufgaben zu aktualisieren, benötigen Sie Zugriff auf Aufgaben bearbeiten.)</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt.<br>Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigung für Projekt- und Aufgabenobjekte anzeigen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Voraussetzungen für die Verwendung von Enhanced Analytics finden Sie im Abschnitt &quot;Voraussetzungen&quot;in der [Übersicht über erweiterte Analysen](../enhanced-analytics/enhanced-analytics-overview.md).

## Grundlegendes zu den Aufgaben in der Flugvisualisierung

Die Aufgaben in der Visualisierung des Flugplans zeigen die folgenden Aufgabendetails an:

* **Geplante Aufgabendauer**: Die Länge einer Taskleiste gibt die geplante Dauer an, die auf dem Startdatum und dem Abschlussdatum der Aufgabe basiert.

  ![](assets/tasks-in-flight-duration-350x80.png)

* **Abgeschlossener Arbeitsaufwand**: Die dunkelblaue Farbe in einer Aufgabenleiste gibt an, wie viel Arbeit für eine Aufgabe abgeschlossen wurde. Dieser Fertigstellungsprozentsatz wird rechts neben der Taskleiste angezeigt.

  ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **verbleibender Arbeitsaufwand**: Die hellblaue Farbe in einer Aufgabenleiste gibt an, wie viel Arbeit für eine Aufgabe ausgeführt werden muss.

  ![](assets/tasks-in-flight-light-blue-350x35.png)

Anhand dieser Informationen können Sie Folgendes feststellen:

* Wo der Arbeitsaufwand im Mittelpunkt stand.
* Welche Aufgaben ein Projekt gefährden könnten.
* Wie nah eine Aufgabe an der Fertigstellung ist.
* Mit wem Sie über eine bestimmte Aufgabe reden müssen.

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Überblick über erweiterte Analysen](../enhanced-analytics/enhanced-analytics-overview.md).

## Aufgaben in der Flugvisualisierung anzeigen

1. Klicken Sie auf das Hauptmenü-Symbol ![](assets/main-menu-icon-16x12.png) und wählen Sie dann **Analytics** aus.
1. (Optional) Wenn Sie einen anderen Datumsbereich verwenden möchten, wählen Sie im Filter für den Datumsbereich die neuen Start- und Enddaten aus.

   ![](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Datumsbereichfilters finden Sie unter [Anwenden von Filtern in Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie den Projektdatensatz einschränken müssen, wählen Sie die Filter aus, die Sie verwenden möchten, und wenden Sie sie an.

   Weitere Informationen zum Hinzufügen von Filtern in Enhanced Analytics finden Sie unter [Anwenden von Filtern in Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nach dem Hinzufügen von Filtern werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. Klicken Sie in der Visualisierung Flugplan oder Projekt-Treemap auf ein Projekt, um weitere Informationen anzuzeigen.

   Die Niederschläge und Aufgaben in den Flugvisualisierungen werden angezeigt.

   >[!NOTE]
   >
   >Weitere Informationen zu diesen anderen Visualisierungen finden Sie unter:
   >
   >   
   >   
   >   * [Anzeigen der Visualisierung des Flugplans in der erweiterten Analyse](../enhanced-analytics/flight-plan-overview.md)
   >   * [Anzeigen der Projekt-Treemap-Visualisierung in Enhanced Analytics](../enhanced-analytics/project-treemap-overview.md)
   >   * [Anzeigen der Aufschlüsselungsvisualisierung in der erweiterten Analyse](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. (Optional) Wenn Sie einen Datumsbereich vergrößern möchten, wählen Sie einen Punkt auf der Visualisierung für den Anfang Ihres Datumsbereichs aus und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und es wird ein Zeitrahmen-Filter erstellt.

   ![](assets/timeframe-filter-350x220.png)

1. (Optional) Um die Sortierung der Aufgaben zu ändern, klicken Sie auf das Menü **Sortieren nach** und wählen Sie dann eine neue Sortieroption aus:

   * **Abschlussdatum**
   * **Alphabetisch A-Z**
   * **Struktur der Aufschlüsselung der Arbeit** (Diese Option entspricht der Reihenfolge, in der die Aufgaben im Projekt angezeigt werden.)

   Alle anderen Visualisierungen auf der Seite werden entsprechend Ihrer Sortierungsauswahl aktualisiert.

1. Überprüfen Sie den Fortschritt der Aufgaben im ausgewählten Projekt und bewegen Sie dann den Mauszeiger über eine bestimmte Aufgabe, um die Anzahl der geplanten Stunden, das geplante Fälligkeitsdatum und den Fertigstellungsprozentsatz anzuzeigen.

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. Klicken Sie auf eine Aufgabe, um die Aufgabendetails auf der rechten Seite des Bildschirms zu öffnen, wo Sie weitere Informationen zur Aufgabe sehen, Aktualisierungen anzeigen oder eingeben oder Änderungen an der Aufgabe vornehmen können.

   ![](assets/task-details-qs-350x675.png)

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie oben rechts in der Visualisierung auf das Symbol **Exportieren** ![](assets/export.png) und wählen Sie dann das Exportformat aus:

   * **Diagramm (PNG)**
   * **Datentabelle (XSLX)**

