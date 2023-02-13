---
title: Anzeigen der Visualisierung der Ressourcenkapazität in Enhanced Analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Visualisierung der Ressourcenkapazität zeigt an, ob ein Team vorbei ist, unterhalb der Kapazitäten ist oder nicht. Diese Berechnung basiert auf - EDIT ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Anzeigen der Visualisierung der Ressourcenkapazität in Enhanced Analytics

Die Visualisierung der Ressourcenkapazität zeigt an, ob ein Team vorbei ist, unterhalb der Kapazitäten ist oder nicht.

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
   <td> <p>Anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Voraussetzungen für die Verwendung von Enhanced Analytics finden Sie im Abschnitt &quot;Voraussetzungen&quot;unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung der Ressourcenkapazität

Die Visualisierung der Ressourcenkapazität zeigt an, ob ein Team vorbei ist, unterhalb der Kapazitäten ist oder nicht. Diese Berechnung basiert auf:

* **Verfügbare Kapazität**: Gesamtstundenzahl, die ein Heimteam für die Arbeit in dem gefilterten Zeitraum zur Verfügung hat

   >[!NOTE]
   >
   >Wenn Sie sich einen zukünftigen Zeitraum ansehen, wird die verfügbare Kapazität anhand der Kapazität des Teams für die letzten sieben Tage berechnet. Aus diesem Grund werden geplante PTO nicht berücksichtigt.

* **Geplante Kapazität**: Gesamtsumme der geplanten Arbeitsstunden, die das Heimteam in dem gefilterten Zeitraum erwarten würde

Dieser Vergleich der geplanten Arbeitszeiten eines Heimteams mit den tatsächlichen geplanten Arbeitszeiten kann Ihnen dabei helfen festzustellen, ob Sie dem Heimteam nicht genügend Arbeit zuweisen oder ob es bei diesen Arbeitsstunden möglicherweise zu einem Burnout kommt.

![](assets/resource-capacity-350x110.png)

In der Visualisierung der Ressourcenkapazität sehen Sie die folgenden Details:

* **Geplante Kapazität**: Der blaue Kreis steht in Übereinstimmung mit dem Namen des Startseiten-Teams für die Anzahl der geplanten Stunden, die dem Startseiten-Team zugewiesen sind.

   ![](assets/resource-capacity-blue-circle.png)

* **Tatsächliche Kapazität**: Entsprechend dem Namen des Startseiten-Teams stellt die vertikale Zeile die Anzahl der Stunden dar, die für das Startseiten-Team verfügbar sind.

   ![](assets/resource-capacity-vertical-line.png)

* **Überkapazitäten**: Wenn die horizontale Linie und der blaue Kreis rechts neben der vertikalen Linie angezeigt werden, wurde dem Heimteam mehr Arbeit zugewiesen, als sie in der Anzahl der verfügbaren Stunden vervollständigen können. Dies bedeutet, dass das Team möglicherweise über die Kapazität für den gefilterten Zeitraum verfügt. Die verbleibende Anzahl der Stunden, die das Team abschließen muss, wird rechts neben dem blauen Kreis angezeigt.

   ![](assets/resource-capacity-over-capacity.png)

* **Kapazität**: Wenn die horizontale Linie und der blaue Kreis links neben der vertikalen Linie angezeigt werden, verfügt das Startseiten-Team über mehr verfügbare Stunden als die Anzahl der geplanten Arbeitsstunden, die ihnen zugewiesen wurden. Dies bedeutet, dass das Team für den gefilterten Zeitraum möglicherweise nicht in der Lage ist. Links neben dem blauen Kreis wird die zusätzliche Anzahl der Stunden angezeigt, die das Startseiten-Team für die Arbeit zur Verfügung hat.

   ![](assets/resource-capacity-under-capacity.png)

Wenn Sie den Mauszeiger über eine Zeile bewegen, werden die genaue Anzahl der Stunden für die geplante Kapazität und die verfügbare Kapazität sowie die Anzahl der Stunden angezeigt, die das Heimteam verbringt oder zu wenig Kapazität hat.

Anhand dieser Informationen können Sie Folgendes feststellen:

* Wenn das Heimteam überzugewiesen oder unterzugewiesen wurde.
* Die größten Projekte waren, auf die sich das Heimteam konzentrierte.
* Welche Heimteams stehen zur Arbeit zur Verfügung.

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung der Ressourcenkapazität anzeigen

1. Klicken Sie auf das Symbol Hauptmenü . ![](assets/main-menu-icon-16x12.png), wählen Sie **Analytics**.
1. Wählen Sie im linken Bereich die Option **Personen**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Optional) Wenn Sie einen anderen Datumsbereich verwenden möchten, wählen Sie im Filter für den Datumsbereich die neuen Start- und Enddaten aus.

   ![](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Datumsbereichfilters finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie Ihren Team-Filter nicht festgelegt haben, fügen Sie den Team-Filter hinzu und wählen Sie die einzelnen Teams aus, für die Daten angezeigt werden sollen.

   Weitere Informationen zum Hinzufügen von Filtern in der erweiterten Analyse finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nach dem Hinzufügen von Filtern werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. (Optional) Wenn Sie einen Datumsbereich vergrößern möchten, wählen Sie einen Punkt auf der Visualisierung für den Anfang Ihres Datumsbereichs aus und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und es wird ein Zeitrahmen-Filter erstellt.

   ![](assets/timeframe-filter-350x220.png)

1. Bewegen Sie den Mauszeiger über die Startseite, um zu sehen, wie viele Stunden noch geplant werden können, wie viele Stunden das Heimteam voraussichtlich abschließen wird und wie viele Stunden insgesamt gearbeitet wurden, d. h. über, unter oder nach Kapazität.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie auf das **Symbol &quot;Exportieren&quot;** ![](assets/export.png) Wählen Sie oben rechts in der Visualisierung das Exportformat aus:

   * **Diagramm (PNG)**
   * **Datentabelle (XSLX)**

1. Klicken Sie auf einen Startseiten-Teamnamen, um weitere Informationen in der Visualisierung der Teamkapazität anzuzeigen.

   Weitere Informationen zur Visualisierung der Teamkapazität finden Sie unter [Visualisierung der Teamkapazität in der erweiterten Analyse anzeigen](../enhanced-analytics/team-capacity-overview.md).


