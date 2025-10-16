---
content-type: reference
product-area: reporting;projects
keywords: berechnet,Aggregate,Erweitert,Ansichten
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Zeigt das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung an'
description: Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern in der Ansicht eines Berichts oder einer Liste anzuzeigen. Jede Zeile zeigt die Berechnung für jedes Objekt im Bericht oder in der Liste an.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Gruppierung: Zeigt das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung an

<!--Audited: 10/2024-->

Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern in der Ansicht eines Berichts oder einer Liste anzuzeigen. Jede Zeile zeigt die Berechnung für jedes Objekt im Bericht oder in der Liste an.

Beispielsweise können Sie den Unterschied zwischen tatsächlichen und geplanten Stunden in einer dritten Spalte namens Arbeitssaldo für jede Aufgabe in einem Aufgabenbericht anzeigen. Weitere Informationen zu berechneten Datenausdrücken finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Sie können den aggregierten Wert mehrerer berechneter Ansichtselemente in derselben Spalte in einer Gruppierung anzeigen, indem Sie der `aggregator` Zeile der Spalte, die den berechneten Wert enthält, eine Berechnung hinzufügen. Sie können beispielsweise die Summe der Stunden des Arbeitssaldos aller Aufgaben in der Gruppierung des Berichts oder der Liste für die Spalte „Arbeitssaldo“ aggregieren (anzeigen). In diesem Artikel wird beschrieben, wie Sie dies tun können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen

1. Um zu einem Aufgabenbericht zu wechseln, klicken Sie auf **Berichtsaktionen** > **Bearbeiten**.
1. Klicken Sie auf **Gruppierungen** auf **Gruppierung hinzufügen** und geben Sie **Projektname** in das Feld **Gruppieren nach** ein. Wählen Sie dann **Projekt > Name** aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie auf der Registerkarte **Spalten (Ansicht** auf **Spalte hinzufügen** und geben Sie dann **Geplante Stunden** in das Feld **In dieser Spalte anzeigen** ein und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   >[!TIP]
   >
   >Beginnen Sie immer damit, so viele Informationen wie möglich über die Standardschnittstelle hinzuzufügen, bevor Sie Informationen im Textmodus bearbeiten. Fügen Sie Felder hinzu, die den meisten Informationen, die Sie für die Berechnung erstellen möchten, am nächsten liegen oder diese enthalten.

1. Wählen Sie **Feld Diese Spalte zusammenfassen nach** die Option **Summe**.
1. Klicken **in der hinzugefügten Spalte auf** In Textmodus wechseln) und dann auf **Textmodus bearbeiten**.
1. Ersetzen Sie den Text im Feld durch das folgende Textmodusbeispiel:

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
   >Um den aggregierten Wert in der Gruppierung zu erhalten und die aggregierte Differenz zwischen den Feldern „Geplante Stunden“ und „Tatsächliche Stunden“ anzuzeigen, geben Sie dieselbe Gleichung in die `aggregator.valuefield` ein. Die für die Spalte Geplante Stunden verwendete `aggregator.displayformat` konvertiert Minuten in Stunden. Da das Feld Geplante Stunden als Platzhalter verwendet wurde, muss diese Zeile nicht angepasst werden.
   >
   >
   >Die `minutesAsHoursString` Definition der `aggregator.displayformat` bedeutet, dass es nicht notwendig ist, jedes Feld durch 60 zu teilen, wie es bei der `valueexpression` für die Ergebnisse geschieht. In diesem `aggregator.valuefield=workRequired` wird zu: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.
1. Klicken Sie auf **Fertig**.
1. Klicken Sie **Speichern+Schließen**.
