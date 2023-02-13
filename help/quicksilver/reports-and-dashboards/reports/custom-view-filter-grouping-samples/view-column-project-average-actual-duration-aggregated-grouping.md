---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht und Gruppierung: Projekt anzeigen Tatsächliche Dauer aggregiert durch den Durchschnitt in einer Gruppierung"
description: Sie können die folgende Spalte zu einem Projektbericht hinzufügen, um die tatsächliche Dauer als Durchschnitt in einer Gruppierung anzuzeigen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Ansicht und Gruppierung: Projekt anzeigen Tatsächliche Dauer aggregiert durch den Durchschnitt in einer Gruppierung

Sie können die folgende Spalte zu einem Projektbericht hinzufügen, um die tatsächliche Dauer als Durchschnitt in einer Gruppierung anzuzeigen.

![project_with_aggregate_current_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## Anzeigen der tatsächlichen Projektdauer, aggregiert durch den Durchschnitt in einer Gruppierung

So fügen Sie diese Spalte einer Projektansicht hinzu:

1. (Empfohlen) Um die besten Ergebnisse zu erzielen und den aggregierten Durchschnittswert der tatsächlichen Dauer anzuzeigen, muss Ihrer Projektliste oder Ihrem Bericht eine Gruppierung hinzugefügt werden.\
   Weitere Informationen zum Erstellen von Gruppierungen finden Sie im Artikel [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Wechseln Sie zu einer vorhandenen Projektansicht.
1. Erweitern Sie das Dropdown-Menü Ansicht und wählen Sie **Ansicht anpassen**.
1. Klicken **Spalte hinzufügen**.
1. Klicken **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über die **In dieser Spalte anzeigen** und klicken Sie auf **Klicken, um Text zu bearbeiten**.

1. Entfernen Sie den gesamten Text im Feld Textmodus und ersetzen Sie ihn durch den folgenden Code:

   <pre>aggregator.displayFormat=composite <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valueField=currentDurationMinutes <br>aggregator.valueFormat=val <br>displayName=Tatsächliche Projektdauer <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=currentDurationMinutes <br>textmode=true <br>valueField=effectiveDurationMinutes <br>valueFormat=related#M:D <br>viewalias=actualduration</pre>

1. Klicken **Ansicht speichern**.
