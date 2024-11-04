---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht und Gruppierung: Anzeige der tatsächlichen Projektdauer, aggregiert durch den Durchschnitt in einer Gruppierung"
description: Sie können die folgende Spalte zu einem Projektbericht hinzufügen, um die tatsächliche Dauer als Durchschnitt in einer Gruppierung anzuzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Ansicht und Gruppierung: Anzeige der tatsächlichen Projektdauer, aggregiert nach dem Durchschnitt in einer Gruppierung

<!--Audited: 11/2024-->

Sie können die folgende Spalte in einer Projektansicht hinzufügen, um die tatsächliche Dauer als Durchschnitt in einer Gruppierung anzuzeigen.

![project_with_aggregate_current_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## Anzeigen der tatsächlichen Projektdauer, aggregiert durch den Durchschnitt in einer Gruppierung

So fügen Sie diese Spalte einer Projektansicht hinzu:

1. Wechseln Sie zu einer Projektliste.
1. (Erforderlich) Um den aggregierten Durchschnittswert der tatsächlichen Dauer des Projekts anzuzeigen, muss Ihrer Projektliste eine Gruppierung hinzugefügt werden.\
   Weitere Informationen zum Erstellen von Gruppierungen finden Sie im Artikel [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
1. Erweitern Sie das Dropdownmenü **Ansicht** und wählen Sie **Ansicht anpassen** aus.
1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie auf **Wechseln zum Textmodus** und dann auf **Textmodus bearbeiten**.
1. Entfernen Sie den gesamten Text im Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. Klicken Sie auf **Fertig** und dann auf **Ansicht speichern**.
1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
