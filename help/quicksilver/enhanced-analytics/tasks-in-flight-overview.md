---
title: Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Aufgaben in der Flugvisualisierung zeigt, wie viele Aufgaben (innerhalb der angewendeten Filterkriterien) für ein Projekt gerade ausgeführt werden, wie viel Arbeit in Prozent für jede Aufgabe abgeschlossen ist und wie terminiert die Aufgaben sind.
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 59e021aa3ae66e4fc8d9ce9eb57616f948e6cd90
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 4%

---

# Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics

>[!IMPORTANT]
>
>Enhanced Analytics wird in der Woche des 26. Mai aus Workfront entfernt. Workfront Data Connect ist eine neue, alternative Lösung und kann verwendet werden, um alle derzeit verwendeten Visualisierungen von Enhanced Analytics zu replizieren. <br>Weitere Informationen finden Sie im Handbuch [Erweiterte Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)Einstellung“.


Die Aufgaben in der Flugvisualisierung zeigt, wie viele Aufgaben (innerhalb der angewendeten Filterkriterien) für ein Projekt gerade ausgeführt werden, wie viel Arbeit in Prozent für jede Aufgabe abgeschlossen ist und wie terminiert die Aufgaben sind.

![Aufgaben im Flug](assets/tasks-in-flight-possible-replacement-350x104.png)

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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> <p>Zugriff auf Aufgaben anzeigen (Um Aufgaben zu aktualisieren, benötigen Sie Bearbeitungszugriff auf Aufgaben.)</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat.<br>Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigung zum Anzeigen von Projekt- und Aufgabenobjekten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Voraussetzungen für die Verwendung der erweiterten Analyse finden Sie im Abschnitt „Voraussetzungen“ in [Übersicht über die erweiterte Analyse](../enhanced-analytics/enhanced-analytics-overview.md).

## Verstehen der Aufgaben in der Flugvisualisierung

Die Visualisierung Aufgaben im Flugplan zeigt die folgenden Aufgabendetails:

* **Geplante Aufgabendauer**: Die Länge einer Vorgangsleiste gibt die geplante Dauer an, die auf dem Start- und Abschlussdatum der Aufgabe basiert.

  ![Aufgaben während der Flugdauer](assets/tasks-in-flight-duration-350x80.png)

* **Work Effort abgeschlossen**: Die dunkelblaue Farbe in einer Taskleiste zeigt den Umfang der für eine Aufgabe abgeschlossenen Arbeit an. Dieser Prozentsatz der Fertigstellung wird rechts neben der Taskleiste angezeigt.

  ![Aufgaben im Flug dunkelblau](assets/tasks-in-flight-dark-blue-350x35.png)

* **Verbleibender Arbeitsaufwand**: Die hellblaue Farbe in einer Aufgabenleiste zeigt den Arbeitsaufwand an, der für eine Aufgabe abgeschlossen werden muss.

  ![Aufgaben im Flug hellblau](assets/tasks-in-flight-light-blue-350x35.png)

Anhand dieser Informationen können Sie Folgendes feststellen:

* Wo sich der Arbeitsaufwand konzentriert hat.
* Welche Aufgaben ein Projekt gefährden könnten.
* Wie nah eine Aufgabe an der Fertigstellung ist.
* Mit wem Sie über eine bestimmte Aufgabe reden müssen.

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Anzeigen der Aufgaben in der Flugvisualisierung

1. Klicken Sie auf das Hauptmenüsymbol ![Hauptmenüsymbol](assets/main-menu-icon-16x12.png) und wählen Sie dann **Analytics**.
1. (Optional) Um einen anderen Datumsbereich zu verwenden, wählen Sie im Datumsbereichsfilter Neues Start- und Enddatum aus.

   ![Datumsbereich auswählen](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Filters für den Datumsbereich finden Sie unter [Anwenden von Filtern in der erweiterten Analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie den Projektdatensatz einschränken müssen, wählen Sie die gewünschten Filter aus und wenden Sie sie an.

   Weitere Informationen zum Hinzufügen von Filtern in der erweiterten Analyse finden Sie unter [Anwenden von Filtern in der erweiterten Analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nachdem Sie Filter hinzugefügt haben, werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. Klicken Sie in der Flugplan- oder Projekt-Treemap-Visualisierung auf ein Projekt, um weitere Informationen anzuzeigen.

   Burndown und Aufgaben in Flugvisualisierungen werden angezeigt.

   >[!NOTE]
   >
   >Weitere Informationen zu diesen anderen Visualisierungen finden Sie unter:
   >
   >   
   >   
   >   * [Sehen Sie sich die Flugplanvisualisierung in Enhanced Analytics an](../enhanced-analytics/flight-plan-overview.md)
   >   * [Anzeigen der Projekt-Treemap-Visualisierung in Enhanced Analytics](../enhanced-analytics/project-treemap-overview.md)
   >   * [Anzeigen der Burndown-Visualisierung in Enhanced Analytics](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. (Optional) Um einen Datumsbereich heranzuzoomen, wählen Sie einen Punkt auf der Visualisierung für den Beginn Ihres Datumsbereichs und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und ein Zeitrahmenfilter wird erstellt.

   ![Zeitrahmen-Filter](assets/timeframe-filter-350x220.png)

1. (Optional) Um zu ändern, wie die Aufgaben sortiert werden, klicken Sie auf das Menü **Sortieren nach** und wählen Sie dann eine neue Sortieroption aus:

   * **Abschlussdatum**
   * **Alphabetisch von A-Z**
   * **Projektstrukturplan** (Diese Option entspricht der Reihenfolge, in der die Aufgaben im Projekt angezeigt werden.)

   Alle anderen Visualisierungen auf der Seite werden aktualisiert, damit sie Ihrer Sortierauswahl entsprechen.

1. Überprüfen Sie den Fortschritt der Aufgaben im ausgewählten Projekt und bewegen Sie dann den Mauszeiger über eine bestimmte Aufgabe, um die Anzahl der geplanten Stunden, das geplante Fälligkeitsdatum und den Abschlussprozentsatz anzuzeigen.

   ![Aufgaben in Flugdetails](assets/tasks-in-flight-task-details-350x242.png)

1. Klicken Sie auf eine Aufgabe, um die Aufgabendetails auf der rechten Seite des Bildschirms zu öffnen, wo Sie weitere Informationen über die Aufgabe sehen, Aktualisierungen anzeigen oder eingeben oder Änderungen an der Aufgabe vornehmen können.

   ![Aufgabendetails](assets/task-details-qs-350x675.png)

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie **Export**![ Export](assets/export.png)Symbol „Exportieren“ in der oberen rechten Ecke der Visualisierung und wählen Sie dann das Exportformat aus:

   * **Diagramm (PNG)**
   * **Datentabelle (XSLX)**

