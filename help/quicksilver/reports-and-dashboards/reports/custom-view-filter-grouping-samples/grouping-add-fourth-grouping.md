---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Eine vierte Gruppierung zu einer Liste hinzufügen'
description: Ein Matrixbericht kann vier Gruppierungen enthalten. Weitere Informationen zu Matrixberichten finden Sie unter Erstellen eines Matrixberichts.
author: Nolan
feature: Reports and Dashboards
exl-id: 1147a47b-c6e2-496e-b202-eefeb500054e
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Gruppierung: Eine vierte Gruppierung zu einer Liste hinzufügen

<!--Audited: 10/2024-->

Ein Matrixbericht kann vier Gruppierungen enthalten. Weitere Informationen zu Matrixberichten finden Sie unter [Erstellen eines Matrixberichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

Ein Standardbericht kann über die Standardschnittstelle nur drei Gruppierungen enthalten. Um in einem Standardbericht eine vierte Gruppierung hinzuzufügen, müssen Sie den Textmodus verwenden.

![Four_groupings_in_a_standard_report.png](assets/four-tier-grouping-for-tasks-350x239.png)

Angenommen, Sie haben einen Aufgabenbericht, der nach Projektname, Fortschrittsstatus und geplantem Abschlussdatum gruppiert ist, aber Sie möchten den Bericht auch nach Zugewiesenem Namen gruppieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen einer vierten Gruppierung zu einer Liste

So fügen Sie eine vierte Gruppierung hinzu:

1. Klicken Sie **In Textmodus wechseln**.
1. Entfernen Sie den Text im Bereich **Bericht gruppieren**.
1. Ersetzen Sie den Text in dem angezeigten Feld durch den folgenden Code:

   ```
   group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br>group.0.valuefield=project:name<br>group.0.valueformat=string<br>group.1.enumclass=com.attask.common.constants.ProgressStatusEnum<br>group.1.enumtype=TASK<br>group.1.linkedname=direct<br>group.1.namekey=progressStatus<br>group.1.type=enum<br>group.1.valuefield=progressStatus<br>group.1.valueformat=val<br>group.2.groupdatesby=WY<br>group.2.linkedname=direct<br>group.2.namekey=plannedCompletionDate<br>group.2.notime=false<br>group.2.valuefield=plannedCompletionDate<br>group.2.valueformat=atDateAsWeekString<br><strong>group.3.valuefield=assignedTo:name</strong><br style="font-weight: bold;"><strong>group.3.valueformat=HTML</strong><br>textmode=true
   ```

1. Klicken Sie **Fertig** und dann **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Namen für die Gruppierung und klicken Sie dann auf **Gruppierung speichern**.
