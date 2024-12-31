---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Probleme mit dem Auflösen von Objektdetails'
description: Diese Anfrageansicht zeigt den Namen und den abgeschlossenen Prozentsatz des Lösungsobjekts des Problems an, sodass der Problemurheber auch ohne Zugriff auf die Lösungsaufgabe oder das Projekt Einblick in den Fortschritt des Problems erhalten kann.
author: Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Anzeigen: Probleme mit dem Auflösen von Objektdetails

<!--Audited: 11/2024-->

Diese Anfrageansicht zeigt den Namen und den abgeschlossenen Prozentsatz des Lösungsobjekts des Problems an, sodass der Problemurheber auch ohne Zugriff auf die Lösungsaufgabe oder das Projekt Einblick in den Fortschritt des Problems erhalten kann.

In dieser Ansicht werden mit dem Tag `sharecol=true` mehrere Felder unter derselben Spaltenüberschrift kombiniert. Weitere Informationen zum `sharecol`-Tag finden Sie unter [Ansicht: Zusammenführungsinformationen aus mehreren Spalten in einer gemeinsamen Spalte](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu:<ul><li>Mitwirkende zum Ändern einer Ansicht</li><li>Standard zum Ändern eines Berichts</li></ul></p><p>Oder</p>Aktuell:<ul><li>Änderung einer Ansicht anfordern</li><li>Planen der Änderung eines Berichts</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Probleme mit dem Auflösen von Objektdetails anzeigen

1. Zu einer Problemliste gehen.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Entfernen Sie **Bereich „Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte, klicken Sie auf **Wechseln in den Textmodus** und klicken Sie dann auf **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   column.0.querysort=name
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=sourceobject
   column.1.linkedname=direct
   column.1.listsort=nested(referenceObject).HTML(name)
   column.1.namekey=sourceobject.abbr
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=referenceObject:name
   column.1.valueformat=HTML
   column.1.viewalias=source
   column.1.width=100
   column.2.descriptionkey=assignedto
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=assignedTo:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=assignedTo:objCode
   column.2.link.valueformat=val
   column.2.linkedname=assignedTo
   column.2.listsort=nested(assignedTo).string(name)
   column.2.namekey=assignedto
   column.2.querysort=assignedTo:name
   column.2.shortview=false
   column.2.stretch=25
   column.2.valuefield=assignedTo:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.descriptionkey=entrydate
   column.3.linkedname=direct
   column.3.listsort=atDateAsAtDate(entryDate)
   column.3.namekey=entrydate.abbr
   column.3.querysort=entryDate
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=entryDate
   column.3.valueformat=atDate
   column.3.width=150
   column.4.descriptionkey=description
   column.4.linkedname=direct
   column.4.listsort=string(description)
   column.4.namekey=description.abbr
   column.4.querysort=description
   column.4.shortview=false
   column.4.stretch=75
   column.4.valuefield=description
   column.4.valueformat=HTML
   column.4.width=150
   column.5.descriptionkey=status
   column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum
   column.5.linkedname=direct
   column.5.listsort=string(status)
   column.5.namekey=status.abbr
   column.5.querysort=status
   column.5.shortview=false
   column.5.stretch=0
   column.5.type=enum
   column.5.valuefield=status
   column.5.valueformat=val
   column.5.width=150
   column.6.displayname=Resolving Object Name
   column.6.linkedname=resolveTask
   column.6.namekey=view.relatedcolumn
   column.6.namekeyargkey.0=resolveTask
   column.6.namekeyargkey.1=name
   column.6.querysort=resolveTask:name
   column.6.sharecol=true
   column.6.textmode=true
   column.6.valuefield=resolveTask:name
   column.6.valueformat=HTML
   column.7.displayname=
   column.7.linkedname=resolveOpTask
   column.7.namekey=view.relatedcolumn
   column.7.namekeyargkey.0=resolveOpTask
   column.7.namekeyargkey.1=name
   column.7.querysort=resolveOpTask:name
   column.7.sharecol=true
   column.7.textmode=true
   column.7.valuefield=resolveOpTask:name
   column.7.valueformat=HTML
   column.8.displayname=
   column.8.linkedname=resolveProject
   column.8.namekey=view.relatedcolumn
   column.8.namekeyargkey.0=resolveProject
   column.8.namekeyargkey.1=name
   column.8.querysort=resolveProject:name
   column.8.textmode=true
   column.8.valuefield=resolveProject:name
   column.8.valueformat=HTML
   column.9.displayname=Resolving Object Percent Complete
   column.9.textmode=true
   column.9.valueexpression=IF(ISBLANK({resolveTask}.{ID}),{resolveProject}.{percentComplete},IF(ISBLANK({resolveProject}.{ID}),{resolveTask}.{percentComplete},''))
   column.9.valueformat=doubleAsPercentRounded
   ```

1. Klicken Sie **Fertig** > **Ansicht speichern**.
1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
