---
title: Visualisierung der Teamkapazität in der erweiterten Analyse anzeigen
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Visualisierung der Teamkapazität zeigt die Gesamtkapazität eines Heimteams, ob sie überzugewiesen oder unterverteilt sind und wie dynamisch die Kapazität im Laufe der Zeit ist.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Visualisierung der Teamkapazität in der erweiterten Analyse anzeigen

<!-- Audited: 01/2024 -->

Die Visualisierung der Teamkapazität zeigt die Gesamtkapazität eines Heimteams, ob sie überzugewiesen oder unterverteilt sind und wie dynamisch die Kapazität im Laufe der Zeit ist.

![Teamkapazität](assets/team-capacity.png)

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
   <td role="rowheader">Übersicht über Adobe Workfront-Lizenzen</td>
   <td>
      <p>Neu: Licht oder höher</p>
      <p>oder</p>
      <p>Aktuell: Überprüfen oder höher</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Zugriff auf Projekte anzeigen</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Anzeigen </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Voraussetzungen für die Verwendung von Enhanced Analytics finden Sie im Abschnitt &quot;Voraussetzungen&quot;unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung der Teamkapazität

Die Visualisierung der Teamkapazität zeigt das Arbeitsvolumen an, das dem Startseiten-Team an einem bestimmten Tag zugewiesen wurde.

* **Burnout**: Wenn die dunkelblaue Füllfarbe über der gepunkteten Linie liegt, werden dem Heimteam mehr Arbeitsstunden zugewiesen, als in der Anzahl der Stunden, die das Team zur Arbeit zur Verfügung hat, abgeschlossen werden können. Dies deutet darauf hin, dass das Team überzugewiesen wurde und möglicherweise kurz vor dem Start steht.

  ![Überkapazitäten](assets/team-capacity-over-capacity.png)

* **Unangefochten**: Wenn die dunkelblaue Füllfarbe unter der gepunkteten Linie liegt, stehen dem Startseiten-Team mehr Arbeitsstunden zur Verfügung als die ihnen zugewiesene Arbeitszeit. Dies weist darauf hin, dass das Team nicht genügend Platz hat und möglicherweise nicht angefochten werden kann.

  ![Kapazität](assets/team-capacity-under-capacity.png)

* **Saldo**: Wenn die hellere oder transparentere blaue Füllfarbe direkt über, direkt unterhalb oder an der gepunkteten Linie liegt, hat das Heimteam eine Arbeitszeit zugewiesen, die es innerhalb der verfügbaren Arbeitszeiten abschließen kann. Dies deutet darauf hin, dass die Arbeitslast des Teams ausgeglichener ist.

  ![Kapazität](assets/team-capacity-at-capacity.png)

Wenn Sie den Mauszeiger über einen Punkt in der Visualisierung bewegen, werden die folgenden Details für einen bestimmten Tag angezeigt:

* **Geplante Stunden**: Dies ist die Anzahl der geplanten Arbeitsstunden, die das Team durchführen muss.
* **Verfügbare Stunden**: Dies ist die Anzahl der Arbeitsstunden, die das Team zur Arbeit zur Verfügung hat.
* **Kapazität**: Zusätzlich zu einem Kapazitätsprozentsatz werden auch die Bezeichnungen Kapazität, Unterkapazität oder Überkapazität angezeigt.

Anhand dieser Informationen können Sie Folgendes feststellen:

* Als das Zuhause-Team überzugewiesen oder unterzugewiesen wurde.
* Wenn das Heimteam täglich überverteilt oder unterzugewiesen ist.
* Wie konsistent die Arbeitslast eines Heimteams von Tag zu Tag ist.
* Wenn Sie Kapazitätsprobleme mit neuer Arbeit schaffen.

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung der Teamkapazität anzeigen

{{step1-to-analytics}}

1. Wählen Sie im linken Bereich die Option **Personen**.

   ![Personen auswählen](assets/people-area-cropped-qs-350x276.png)

1. (Optional) Wenn Sie einen anderen Datumsbereich verwenden möchten, wählen Sie im Filter für den Datumsbereich die neuen Start- und Enddaten aus.

   ![Filter für Datumsbereiche](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Datumsbereichfilters finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie Ihren Team-Filter nicht festgelegt haben, fügen Sie den Team-Filter hinzu und wählen Sie die Teams aus, für die Sie Daten anzeigen möchten.

   Weitere Informationen zum Hinzufügen von Filtern in der erweiterten Analyse finden Sie unter [Filter in erweiterten Analysen anwenden](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nach dem Hinzufügen von Filtern werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. Klicken Sie in der Visualisierung der Ressourcenkapazität auf ein Team, um weitere Informationen anzuzeigen.

   Die Visualisierung der Teamkapazität wird angezeigt.

   Weitere Informationen zur Visualisierung der Ressourcenkapazität finden Sie unter [Anzeigen der Visualisierung der Ressourcenkapazität in Enhanced Analytics](../enhanced-analytics/resource-capacity-overview.md).

1. (Optional) Wenn Sie einen Datumsbereich vergrößern möchten, wählen Sie einen Punkt auf der Visualisierung für den Anfang Ihres Datumsbereichs aus und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und es wird ein Zeitrahmen-Filter erstellt.

   ![Zeitrahmen-Filter](assets/timeframe-filter-350x220.png)

1. Bewegen Sie den Mauszeiger über einen Punkt auf der Diagrammlinie, um die geplanten Stunden und geplanten Stunden für das angegebene Datum sowie den Kapazitätsprozentsatz und die Frage zu sehen, ob das Heimteam zu der Zeit vorbei, unterwegs oder auf Kapazität war.

   ![Popup für Teamkapazität](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie auf das **Export** icon ![Symbol &quot;Exportieren&quot;](assets/export.png) Wählen Sie oben rechts in der Visualisierung das Exportformat aus:

   * Diagramm (PNG)
   * Datentabelle (XSLX)

