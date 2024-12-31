---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Stunden mit Informationen zur übergeordneten Aufgabe'
description: Diese Stundenansicht zeigt den Namen der Aufgabe, in der die Stunden protokolliert wurden, sowie den Namen der übergeordneten Aufgabe an.
author: Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Anzeigen: Stunden mit Informationen zur übergeordneten Aufgabe

<!--Audited: 11/2024-->

Diese Stundenansicht zeigt den Namen der Aufgabe, in der die Stunden protokolliert wurden, sowie den Namen der übergeordneten Aufgabe an.

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

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

## Stunden mit Informationen zur übergeordneten Aufgabe anzeigen

1. Zu einer Stundenliste gehen.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Entfernen Sie im Bereich **Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln**.
1. Klicken Sie **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:



   ```
   column.0.aggregator.displayformat=doubleAsString
   column.0.aggregator.function=SUM
   column.0.aggregator.namekey=hours
   column.0.aggregator.valuefield=hours
   column.0.aggregator.valueformat=doubleAsDouble
   column.0.descriptionkey=hours
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=doubleAsDouble(hours)
   column.0.namekey=hours.abbr
   column.0.querysort=hours
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=hours
   column.0.valueformat=doubleAsString
   column.0.width=150
   column.1.descriptionkey=task
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=task:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=task:objCode
   column.1.link.valueformat=val
   column.1.linkedname=task
   column.1.listsort=nested(task).string(name)
   column.1.namekey=task
   column.1.querysort=task:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=task:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Parent Task Name
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=task:parent:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=task:objCode
   column.2.link.valueformat=val
   column.2.linkedname=task
   column.2.listsort=nested(task:parent).string(name)
   column.2.name=Parent Task Name
   column.2.querysort=task:parent:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=task:parent:name
   column.2.valueformat=HTML
   column.2.width=150
   ```

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.

