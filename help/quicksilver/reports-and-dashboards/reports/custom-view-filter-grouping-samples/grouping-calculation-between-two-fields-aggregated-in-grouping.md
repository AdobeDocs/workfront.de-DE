---
content-type: reference
product-area: reporting;projects
keywords: Berechnet,Aggregate,Erweitert,Ansichten
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Zeigt das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung an'
description: Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern in der Anzeige eines Berichts oder einer Liste anzuzeigen. Jede Zeile zeigt die Berechnung für jedes Objekt in dem Bericht oder der Liste an.
author: Courtney
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 10%

---

# Gruppierung: Das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen

<!--Audited: 10/2024-->

Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern in der Anzeige eines Berichts oder einer Liste anzuzeigen. Jede Zeile zeigt die Berechnung für jedes Objekt in dem Bericht oder der Liste an.

Sie können z. B. die Differenz zwischen den aktuellen Stunden und den geplanten Stunden in einer dritten Spalte mit der Bezeichnung Arbeitsbilanz für jeden Vorgang in einem Vorgangsbericht anzeigen. Weitere Informationen zu berechneten Datenausdrücken finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Sie können den aggregierten Wert mehrerer berechneter Ansichtselemente in derselben Spalte in einer Gruppe anzeigen, indem Sie der Zeile `aggregator` der Spalte, die den berechneten Wert enthält, eine Berechnung hinzufügen. Sie können z. B. den Stundenbetrag für den Arbeitssaldo aller Vorgänge in der Berichtsgruppe oder der Liste für die Spalte &quot;Arbeitssaldo&quot; aggregieren (die Summe anzeigen). In diesem Artikel wird beschrieben, wie Sie dies tun können.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Anbieter oder Anforderung zum Ändern eines Filters </p>
   <p>Standard oder Abo zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen zum Ändern eines Filters</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen

1. Wechseln Sie zu einem Aufgabenbericht, und klicken Sie auf **Berichtsaktionen** > **Bearbeiten**.
1. Klicken Sie auf der Registerkarte **Gruppierungen** auf **Gruppierung hinzufügen**, geben Sie **Projektname** im Feld **Gruppe von** ein, und wählen Sie dann **Projekt > Name** aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie auf der Registerkarte **Spalten(Ansicht)** auf **Spalte hinzufügen**, geben Sie dann im Feld **In dieser Spalte anzeigen** **Geplante Stunden** ein, und wählen Sie diese Spalte aus, wenn sie in der Liste angezeigt wird.

   >[!TIP]
   >
   >Beginnen Sie immer mit dem Hinzufügen so vieler Informationen über die Standardschnittstelle, bevor Sie Informationen im Textmodus bearbeiten. Fügen Sie Felder hinzu, die den meisten Informationen für die Berechnung, die Sie vornehmen möchten, am nächsten kommen oder diese enthalten.

1. Wählen Sie im Feld **Diese Spalte zusammenfassen nach** die Option **Summe** aus.
1. Klicken Sie in der hinzugefügten Spalte auf **In Textmodus wechseln**, und klicken Sie dann auf **Textmodus bearbeiten**.
1. Ersetzen Sie den Text im Feld durch das folgende Beispiel für den Textmodus:

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >Um den aggregierten Wert in der Gruppierung abzurufen, um die aggregierte Differenz zwischen den Feldern &quot;Geplante Stunden&quot; und &quot;Aktuelle Stunden&quot; anzuzeigen, geben Sie dieselbe Gleichung in die Zeile `aggregator.valuefield` ein. Die `aggregator.displayformat`, die für die Spalte &quot;Geplante Stunden&quot; verwendet wird, konvertiert Minuten in Stunden. Da das Feld &quot;Geplante Stunden&quot; als Platzhalter verwendet wurde, muss diese Linie nicht angepasst werden.
   >
   >
   >Die `minutesAsHoursString`-Definition der `aggregator.displayformat`-Zeile bedeutet, dass es nicht erforderlich ist, jedes Feld durch 60 zu teilen, wie dies auf `valueexpression` für die Ergebnisse erfolgt ist. In diesem `aggregator.valuefield=workRequired` wird zu: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.
1. Klicken Sie auf **Fertig**.
1. Klicken Sie auf **Speichern+Schließen**.
