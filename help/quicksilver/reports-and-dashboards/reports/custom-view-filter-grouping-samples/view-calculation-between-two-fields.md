---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: das Ergebnis einer Berechnung zwischen zwei Feldern einer Spalte anzeigen"
description: Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern anzuzeigen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Ansicht: das Ergebnis einer Berechnung zwischen zwei Feldern einer Spalte anzeigen

Sie können den Textmodus in einer Spalte verwenden, um eine Berechnung zwischen zwei Feldern anzuzeigen.

Wenn Sie beispielsweise die Anzahl der Wochentage zwischen zwei Daten ermitteln möchten, können Sie diese Differenz mithilfe der Textmodussyntax und Datenausdrücken berechnen.\
Sie können beispielsweise die Wochentagsdifferenz zwischen dem geplanten Abschlussdatum und dem tatsächlichen Abschlussdatum einer Aufgabe berechnen und das Ergebnis in einer Spalte anzeigen.

Sie können in dieser Berechnung zwei andere Daten verwenden (Tatsächlicher Start, tatsächlicher Abschluss, Voraussichtlicher Start, voraussichtlicher Abschluss usw.).\
Weitere Informationen zu berechneten Datenausdrücken finden Sie unter [Berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigen des Ergebnisses einer Berechnung zwischen zwei Feldern einer Spalte

So fügen Sie diese Spalte einer Aufgabenansicht hinzu:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht**.

1. Klicken **Spalte hinzufügen**, dann **In den Textmodus wechseln**.

1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:
   <pre>displayName=Wochentagsunterschied<br>textmode=true<br>valueExpression=WEEKDAYDIFF({scheduledCompletionDate},{ISTCompletionDate})<br>valueFormat=HTML</pre>

1. (Optional) Um die in der Ansicht angezeigten Werte in einer Gruppierung zusammenzufassen, gehen Sie wie folgt vor: [Gruppierung: das Ergebnis der Aggregation mehrerer berechneter Werte in einer Gruppierung anzeigen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Klicken **Speichern**, dann **Ansicht speichern**.
