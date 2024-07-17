---
content-type: reference
product-area: reporting;projects
keywords: calculated,aggregates,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen'
description: Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern in der Ansicht eines Berichts oder einer Liste anzuzeigen. Jede Zeile zeigt die Berechnung für jedes Objekt im Bericht oder in der Liste an.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Gruppierung: Anzeige des Ergebnisses der Aggregation mehrerer berechneter Werte in einer Gruppierung

Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern in der Ansicht eines Berichts oder einer Liste anzuzeigen. Jede Zeile zeigt die Berechnung für jedes Objekt im Bericht oder in der Liste an.

Beispielsweise können Sie den Unterschied zwischen tatsächlichen und geplanten Stunden in einer dritten Spalte mit dem Namen Work Balance für jede Aufgabe in einem Aufgabenbericht anzeigen. Weitere Informationen zu berechneten Datenausdrücken finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Sie können den aggregierten Wert mehrerer berechneter Ansichtselemente in derselben Spalte in einer Gruppierung anzeigen, indem Sie der Zeile `aggregator` der Spalte, die den berechneten Wert enthält, eine Berechnung hinzufügen. Sie können beispielsweise die Anzahl der Arbeitsbilanzstunden aller Aufgaben in der Gruppierung des Berichts oder der Liste für die Spalte &quot;Arbeitsstand&quot;aggregieren (die Summe anzeigen). In diesem Artikel wird beschrieben, wie Sie dies tun.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zur Änderung einer Gruppierung </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Gruppierung zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen

1. Klicken Sie in einen Aufgabenbericht auf **Berichtaktionen** > **Bearbeiten**.
1. Klicken Sie auf der Registerkarte **Gruppierungen** auf **Gruppierung hinzufügen**, geben Sie im Feld **Gruppieren Sie Ihren Bericht** > **Zuerst nach** den Wert **Projektnamen** ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

1. Klicken Sie auf der Registerkarte **Spalten(Ansicht)** auf **Spalte hinzufügen**, geben Sie dann im Feld **In dieser Spalte anzeigen** den Wert **Geplante Stunden** ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   >[!TIP]
   >
   >Beginnen Sie immer mit dem Hinzufügen so vieler Informationen über die Standard-Benutzeroberfläche, bevor Sie Informationen im Textmodus bearbeiten. Fügen Sie die Felder hinzu, die am nächsten sind oder die die meisten Informationen enthalten, die für die Berechnung, die Sie vornehmen möchten, erforderlich sind.

1. Wählen Sie im Feld **Zusammenfassen dieser Spalte nach** die Option **Summe** und klicken Sie dann auf **Fertig**.
1. Klicken Sie in der hinzugefügten Spalte auf **In den Textmodus wechseln** .
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Ersetzen Sie die Zeilen `valuefield ` und `aggregator.valuefield` durch die Zeilen, die im folgenden Textmodus hervorgehoben sind:

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
   >Um den aggregierten Wert in der Gruppierung abzurufen und den aggregierten Unterschied zwischen den Feldern &quot;Geplante Stunden&quot;und &quot;Tatsächliche Stunden&quot;anzuzeigen, geben Sie dieselbe Gleichung in die Zeile `aggregator.valuefield` ein. Die für die Spalte &quot;Geplante Stunden&quot;verwendete `aggregator.displayformat` wandelt Minuten in Stunden um. Da das Feld &quot;Geplante Stunden&quot;als Platzhalter verwendet wurde, muss diese Zeile nicht angepasst werden.
   >
   >
   >Die `minutesAsHoursString`-Definition der Zeile `aggregator.displayformat` bedeutet, dass es nicht notwendig ist, jedes Feld durch 60 zu teilen, wie es auf der `valueexpression` für die Ergebnisse getan wird. In diesem `aggregator.valuefield=workRequired` wird: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Klicken Sie auf **Speichern+Schließen**.
