---
title: Anzeigen der Visualisierung des Flugplans in der erweiterten Analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Visualisierung des Flugplans zeigt, wie viele Projekte (innerhalb der angewandten Filterkriterien) abgewickelt wurden, welche Bedingungsänderungen während der gesamten Laufzeit dieser Projekte eingetreten sind und wie eng diese Projekte an die geplanten Fertigstellungsfristen gebunden waren.
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# Anzeigen der Visualisierung des Flugplans in der erweiterten Analyse

Die Visualisierung des Flugplans zeigt, wie viele Projekte (innerhalb der angewandten Filterkriterien) abgewickelt wurden, welche Bedingungsänderungen während der gesamten Laufzeit dieser Projekte eingetreten sind und wie eng diese Projekte an die geplanten Fertigstellungsfristen gebunden waren.

![](assets/flight-plan-350x132.png)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-Abo</a>*</td> 
   <td> <p>Unternehmen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt.<br>Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf das Projekt anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Voraussetzungen für die Verwendung von Enhanced Analytics finden Sie im Abschnitt &quot;Voraussetzungen&quot;unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung des Flugplans

In der tatsächlichen Dauer eines Projekts sehen Sie nur die folgenden Projektbedingungen:

* Im Zielbereich
* Gefährdet
* In Schwierigkeiten

Weitere Informationen zu Projektbedingungen finden Sie unter [Übersicht über Projektbedingung und Bedingungstyp](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Die Visualisierung des Flugplans zeigt die folgenden Projektdetails an:

* **Geplante Dauer**: Die horizontale blaue Linie stellt die geplante Länge des Projekts dar, wobei die Dreiecke an beiden Enden der Zeile das Start- und Enddatum angeben.

   ![](assets/planned-duration-line-350x37.png)

* **Tatsächliche Dauer**: Die dicke, farbige Linie unterhalb der geplanten Dauer stellt die tatsächliche Länge des Projekts dar. Die Farbe der Linie hängt von der Bedingung des Projekts zu dem bestimmten Zeitpunkt während der Projektlaufzeit ab.

   ![](assets/actual-duration-line.png)

* **Tatsächliche Bedingung**: Die dicke, farbige Linie zeigt auch den Zustand eines Projekts zu unterschiedlichen Zeitpunkten. Die Farbe der Zeile ändert sich je nach Projektbedingung:

   * **Grün**: In Target
   * **Orange**: Risiko
   * **Rot**: In Schwierigkeiten

   ![](assets/actual-condition-color.png)

Wenn Sie in der Visualisierung des Flugplans mit dem Mauszeiger über eine Projektzeile fahren, werden Informationen zum geplanten Zeitrahmen des Projekts, zur aktuellen Projektbedingung und - falls zutreffend - zur benutzerdefinierten Bedingung angezeigt. Um einen tieferen Überblick darüber zu erhalten, was sich auf die Dauer oder Bedingung ausgewirkt haben könnte, können Sie sich die anderen Visualisierungen im Bereich &quot;Erweiterte Analyse&quot;ansehen.

Anhand dieser Informationen können Sie Folgendes feststellen:

* Welche Ereignisse verlängern ein Projekt über das ursprünglich geplante Abschlussdatum hinaus.
* Wenn bei einem Projekt Probleme auftreten.
* Wie viele Projekte im selben Zeitraum geöffnet sind.
* Anzahl der aktiven Projekte.
* Welche Projekte benötigen besondere Aufmerksamkeit oder Unterstützung?

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung des Flugplans anzeigen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon-16x12.png), wählen Sie **Analytics**.
1. (Optional) Wenn Sie einen anderen Datumsbereich verwenden möchten, wählen Sie im Filter für den Datumsbereich die neuen Start- und Enddaten aus.

   ![](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Datumsbereichfilters finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie den Projektdatensatz einschränken müssen, wählen Sie die Filter aus, die Sie verwenden möchten, und wenden Sie sie an.

   Weitere Informationen zum Hinzufügen von Filtern in der erweiterten Analyse finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nach dem Hinzufügen von Filtern werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. (Optional) Wenn Sie einen Datumsbereich vergrößern möchten, wählen Sie einen Punkt auf der Visualisierung für den Anfang Ihres Datumsbereichs aus und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und es wird ein Zeitrahmen-Filter erstellt.

   ![](assets/timeframe-filter-350x220.png)

1. (Optional) Klicken Sie zum Ändern der Projektsortierung auf die Schaltfläche **Sortieren nach** in der oberen rechten Ecke der Visualisierung des Flugplans und wählen Sie dann eine neue Sortieroption aus:

   * **A – Z**
   * **Z – A**
   * **Geplantes Abschlussdatum**
   * **Geplantes Startdatum**

   Alle anderen Visualisierungen auf der Seite werden entsprechend Ihrer Sortierungsauswahl aktualisiert.

1. (Bedingt) Wenn Ihr Datensatz mehr als 50 Projekte enthält, können Sie mit den Pfeilen in der linken unteren Ecke der Visualisierung von einer Gruppe von 50 Projekten zur nächsten navigieren.

   Alle anderen Visualisierungen auf der Seite werden entsprechend Ihrer Seitenauswahl aktualisiert.

   ![](assets/pagination-350x118.png)

1. Bewegen Sie den Mauszeiger über das Diagramm der Projektleiste, um die blaue Datumszeile sowie die folgenden Details anzuzeigen:

   * Geplante Zeitleiste
   * Aktuelle Bedingung
   * Benutzerdefinierte Bedingung (falls zutreffend)

   ![](assets/project-bar-graph-350x143.png)

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie auf das **Export** icon ![](assets/export.png) Wählen Sie oben rechts in der Visualisierung das Exportformat aus:

   * **Diagramm (PNG)**
   * **Datentabelle (XSLX)**

1. Um weitere Projektinformationen anzuzeigen, klicken Sie auf ein Projekt in der Visualisierung, um die Aufschlüsselung und Aufgaben in den Flugvisualisierungen zu öffnen.

   Diese Visualisierungen können Ihnen dabei helfen, tiefere Einblicke in die Gründe zu erhalten, durch die das Projekt aus der Bahn gelaufen ist. Sie machen es auch einfach, in einem laufenden Projekt einzuchecken.\
   Weitere Informationen zur Aufschlüsselungsvisualisierung finden Sie unter [Anzeigen der Niederschlagsvisualisierung in der erweiterten Analyse](../enhanced-analytics/burndown-overview.md). Weitere Informationen zu den Aufgaben in der Flugvisualisierung finden Sie unter [Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics](../enhanced-analytics/tasks-in-flight-overview.md).

