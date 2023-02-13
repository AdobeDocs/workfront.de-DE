---
content-type: reference
product-area: reporting;projects
keywords: calculated,aggregates,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
title: "Gruppierung: das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen"
description: Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern in der Ansicht eines Berichts oder einer Liste anzuzeigen. Jede Zeile zeigt die Berechnung für jedes Objekt im Bericht oder in der Liste an.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Gruppierung: das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen

Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern in der Ansicht eines Berichts oder einer Liste anzuzeigen. Jede Zeile zeigt die Berechnung für jedes Objekt im Bericht oder in der Liste an.

Beispielsweise können Sie den Unterschied zwischen tatsächlichen und geplanten Stunden in einer dritten Spalte mit dem Namen Work Balance für jede Aufgabe in einem Aufgabenbericht anzeigen. Weitere Informationen zu berechneten Datenausdrücken finden Sie unter [Berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Sie können den aggregierten Wert mehrerer berechneter Ansichtselemente in derselben Spalte in einer Gruppierung anzeigen, indem Sie der `aggregator` Zeile der Spalte, die den berechneten Wert enthält. Sie können beispielsweise die Anzahl der Arbeitsbilanzstunden aller Aufgaben in der Gruppierung des Berichts oder der Liste für die Spalte &quot;Arbeitsstand&quot;aggregieren (die Summe anzeigen). In diesem Artikel wird beschrieben, wie Sie dies tun.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen

1. Gehen Sie zu einem Aufgabenbericht, klicken Sie auf **Berichtaktionen** > **Bearbeiten**.
1. Im **Gruppierungen** Registerkarte, klicken Sie auf **Gruppierung hinzufügen** und beginnen Sie mit der Eingabe **Projektname** im **Gruppieren Ihres Berichts** > **Zuerst durch** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Im **Spalten (Ansicht)** Registerkarte, klicken Sie auf **Spalte hinzufügen**, und beginnen Sie dann mit der Eingabe **Geplante Stunden** im **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   >[!TIP]
   >
   >Beginnen Sie immer mit dem Hinzufügen so vieler Informationen über die Standard-Benutzeroberfläche, bevor Sie Informationen im Textmodus bearbeiten. Fügen Sie die Felder hinzu, die am nächsten sind oder die die meisten Informationen enthalten, die für die Berechnung, die Sie vornehmen möchten, erforderlich sind.

1. Im **Zusammenfassen dieser Spalte nach** Feld, wählen Sie **Summe** Klicken Sie auf **Fertig**.
1. Klicken **In den Textmodus wechseln** in der von Ihnen hinzugefügten Spalte.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Ersetzen Sie die `valuefield ` und `aggregator.valuefield` Zeilen mit den im folgenden Textmodus hervorgehobenen Zeilen:

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
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") viewalias=workrequired displayname=Work Balance
   ```

   >[!TIP]
   >
   >Um den aggregierten Wert in der Gruppierung zu erhalten und die aggregierte Differenz zwischen den Feldern &quot;Geplante Stunden&quot;und &quot;Tatsächliche Stunden&quot;anzuzeigen, müssen Sie dieselbe Gleichung in die `aggregator.valuefield` Linie. Die `aggregator.displayformat` für die Spalte &quot;Geplante Stunden&quot;verwendet wird, werden Minuten in Stunden umgewandelt. Da das Feld &quot;Geplante Stunden&quot;als Platzhalter verwendet wurde, muss diese Zeile nicht angepasst werden.
   >
   >
   >Die `minutesAsHoursString` Definition der `aggregator.displayformat` bedeutet, dass es nicht notwendig ist, jedes Feld wie auf der `valueexpression` für die Ergebnisse. In diesem `aggregator.valuefield=workRequired` wird: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Klicken **Speichern+Schließen**.
