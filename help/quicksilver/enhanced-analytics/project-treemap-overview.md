---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: Anzeigen der Projekt-Treemap-Visualisierung in Enhanced Analytics
description: Die Projekt-Treemap-Visualisierung ist eine Ansicht von Stunden - oder Tagen -, die in einem bestimmten Zeitfenster bearbeitet wurden, verglichen mit anderen Arbeitsschritten in der Größe. Auf diese Weise können Sie nachvollziehen, wie viel Zeit Benutzer für ein Projekt haben.
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Anzeigen der Projekt-Treemap-Visualisierung in Enhanced Analytics

<!-- Audited: 12/2023 -->

Die Projekt-Treemap-Visualisierung ist eine Ansicht von Stunden - oder Tagen -, die in einem bestimmten Zeitfenster bearbeitet wurden, verglichen mit anderen Arbeitsschritten in der Größe. Auf diese Weise können Sie nachvollziehen, wie viel Zeit Benutzer für ein Projekt haben.

![](assets/project-treemap-350x126.png){width="700"}

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-Abo</a></td> 
   <td> <p>Unternehmen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a></td> 
   <td>   <p>Neu:</p> 
   <ul><li>Licht oder höher</li></ul>
   <p>Aktuell:</p>
   <ul><li>Überprüfen oder höher</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Voraussetzungen für die Verwendung von Enhanced Analytics finden Sie im Abschnitt &quot;Voraussetzungen&quot;unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Grundlegendes zur Projekt-Treemap-Visualisierung

Die Kästchen in der Projekt-Treemap-Visualisierung stellen Projekte dar, und die Größe der Kästchen zeigt einen Vergleich der Zeit, die für verschiedene Projekte verbracht wurde. Je größer die Kiste ist, desto mehr Zeit wird für das Projekt benötigt.

Die Projekt-Treemap-Visualisierung besteht aus:

* **Kleinere, hellblaue Boxen**: Projekte mit weniger Stunden oder Tagen werden als kleinere Kästchen mit hellblauer Farbe angezeigt.

  ![](assets/project-treemap-smaller-box.png)

* **Größere, dunkelblaue Kisten**: Projekte mit mehr Stunden - oder Tagen - werden als größere Kästchen mit dunkelblauer Farbe angezeigt.

  ![](assets/project-treemap-larger-box-350x205.png)

* **Mittlere, blaue Boxen**: Projekte, die zwischen den beiden Kategorien liegen, werden als mittelgroße Kästchen mit einem Blau-Schatten zwischen den dunkelblauen und den hellblauen Farben angezeigt. Für mittelgroße Kisten gibt es 3 mögliche blaue Schattierungen.

Die Legende auf der rechten Seite zeigt eine Aufschlüsselung der abgeschlossenen Stunden für jeden Blau-Schatten. Diese Legende ist dynamisch und wird entsprechend den Daten aktualisiert.

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>Wenn Sie sich die Projekt-Treemap-Visualisierung nach Dauer statt nach geplanten Stunden ansehen, zeigt diese Legende eine Aufschlüsselung der Tage, die für jeden Blau-Schatten gearbeitet wurden.\
>![](assets/project-treemap-days-worked.png)>

Anhand dieser Informationen können Sie Folgendes feststellen:

* Die Priorität der Dinge, an denen im ausgewählten Datumsbereich gearbeitet wird.
* Für welche Teams Zeit verbringen.
* Wenn sich Teams auf die richtigen Dinge konzentrieren.
* Wenn auf ein bestimmtes Projekt geklickt wird, wie stark sich der Umfang eines Projekts in diesem Zeitraum geändert hat.

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Anzeigen der Projekt-Treemap-Visualisierung

1. Klicken Sie auf das Symbol Hauptmenü . ![](assets/main-menu-icon-16x12.png), wählen Sie **Analytics**.
1. (Optional) Wenn Sie einen anderen Datumsbereich verwenden möchten, wählen Sie im Filter für den Datumsbereich die neuen Start- und Enddaten aus.

   ![](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Datumsbereichfilters finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie den Projektdatensatz einschränken müssen, wählen Sie die Filter aus, die Sie verwenden möchten, und wenden Sie sie an.

   Weitere Informationen zum Hinzufügen von Filtern in der erweiterten Analyse finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nach dem Hinzufügen von Filtern werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. (Optional) Klicken Sie zum Ändern der Projektsortierung auf die Schaltfläche **Sortieren nach** in der oberen rechten Ecke der Projekt-Treemap-Visualisierung und wählen Sie dann eine neue Sortieroption aus:

   * **A - Z**
   * **Z - A**
   * **Geplantes Abschlussdatum**
   * **Geplantes Startdatum**

   Alle anderen Visualisierungen auf der Seite werden entsprechend Ihrer Sortierungsauswahl aktualisiert.

1. (Bedingt) Wenn Ihr Datensatz mehr als 50 Projekte enthält, können Sie mit den Pfeilen in der linken unteren Ecke der Visualisierung von einer Gruppe von 50 Projekten zur nächsten navigieren.

   Alle anderen Visualisierungen auf der Seite werden entsprechend Ihrer Seitenauswahl aktualisiert.

   ![](assets/pagination-350x118.png)

1. (Optional) Ändern Sie die Ansicht von **geplante Stunden** nach **duration**.

   Geplante Stunden ist standardmäßig ausgewählt.

1. Bewegen Sie den Mauszeiger über ein Projekt, um die Projektbedingung sowie die Anzahl der geplanten Gesamtstunden, die Anzahl der insgesamt abgeschlossenen Stunden und die durchschnittliche Anzahl der pro Tag im Projekt verbrachten Stunden anzuzeigen.

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >Wenn Sie die Option **duration** -Ansicht werden die folgenden Details zur Dauer angezeigt:
   >
   >* **Geplanter Zeitrahmen**: Die Anzahl der geplanten Tage, um das Projekt abzuschließen.
   >* **Arbeitstage**: Die geplante Dauer für jede Aufgabe, die innerhalb des oben ausgewählten Datumsbereichs abgeschlossen wurde, dividiert durch die Anzahl der Stunden pro Tag.
   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >Weitere Informationen zur Dauer finden Sie im Abschnitt &quot;Ansicht der Dauer&quot;unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie auf das **Symbol &quot;Exportieren&quot;** ![](assets/export.png) Wählen Sie oben rechts in der Visualisierung das Exportformat aus:

   * **Diagramm (PNG)**
   * **Datentabelle (XSLX)**

1. Klicken Sie auf ein Projekt, um die Niederlassung und Aufgaben in den Flugvisualisierungen zu öffnen und einen tieferen Einblick in den Beitrag von Aufgaben und Stunden - oder Tagen - zur Größe eines Projekts zu erhalten.

Weitere Informationen zur Aufschlüsselungsvisualisierung finden Sie unter [Anzeigen der Niederschlagsvisualisierung in der erweiterten Analyse](../enhanced-analytics/burndown-overview.md). Weitere Informationen zu den Aufgaben in der Flugvisualisierung finden Sie unter [Anzeigen der Aufgaben in der Flugvisualisierung in Enhanced Analytics](../enhanced-analytics/tasks-in-flight-overview.md).

