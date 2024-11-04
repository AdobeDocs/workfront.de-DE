---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Anzeigen des Ergebnisses einer Berechnung zwischen zwei Feldern einer Spalte'
description: Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern anzuzeigen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Ansicht: Anzeigen des Ergebnisses einer Berechnung zwischen zwei Feldern einer Spalte

<!--Audited: 11/2024-->

Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern anzuzeigen.

Wenn Sie beispielsweise die Anzahl der Wochentage zwischen zwei Daten ermitteln möchten, können Sie diese Differenz mithilfe der Textmodussyntax und Datenausdrücken berechnen.\
Sie können beispielsweise die Wochentagsdifferenz zwischen dem geplanten Abschlussdatum und dem tatsächlichen Abschlussdatum einer Aufgabe berechnen und das Ergebnis in einer Spalte anzeigen.

Sie können in dieser Berechnung zwei andere Daten verwenden (Tatsächlicher Start, tatsächlicher Abschluss, Voraussichtlicher Start, voraussichtlicher Abschluss usw.).\
Weitere Informationen zu berechneten Datenausdrücken finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Anzeigen des Ergebnisses einer Berechnung zwischen zwei Feldern einer Spalte

So fügen Sie diese Spalte einer Aufgabenansicht hinzu:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Klicken Sie im Dropdownmenü **Ansicht** auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen** und dann auf **Wechseln zum Textmodus** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Optional) Um die in der Ansicht angezeigten Werte in einer Gruppierung zu aggregieren, führen Sie die unter [Gruppierung: Zeigen Sie das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md) beschriebenen Schritte an.
1. Klicken Sie auf **Fertig** und dann auf **Ansicht speichern**.
