---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Probleme mit Genehmigungsinformationen'
description: Die folgende Ansicht eines Problems zeigt den Genehmigungsprozess, den Schritt, die Namen der genehmigenden Personen und den Status des Problems vor der Genehmigung. Auf einige dieser Felder kann nicht über den standardmäßigen Interface Builder zugegriffen werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Anzeigen: Probleme mit Genehmigungsinformationen

<!--Audited: 11/2024-->

Die folgende Ansicht eines Problems zeigt den Genehmigungsprozess, den Schritt, die Namen der genehmigenden Personen und den Status des Problems vor der Genehmigung. Auf einige dieser Felder kann nicht über den standardmäßigen Interface Builder zugegriffen werden.

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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

## Probleme mit Genehmigungsinformationen anzeigen

1. Zu einer Problemliste gehen.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Entfernen Sie im Bereich **Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte, klicken Sie auf **Wechseln in den Textmodus** und dann **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=40
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=220
   column.1.descriptionkey=assignedto
   column.1.linkedname=assignedTo
   column.1.listsort=nested(assignedTo).string(name)
   column.1.namekey=assignedto
   column.1.querysort=assignedTo:name
   column.1.shortview=true
   column.1.stretch=0
   column.1.valuefield=assignedTo:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.descriptionkey=role
   column.2.linkedname=role
   column.2.listsort=nested(role).string(name)
   column.2.namekey=role
   column.2.querysort=role:name
   column.2.shortview=false
   column.2.stretch=25
   column.2.valuefield=role:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Approval Process Name
   column.3.linkedname=direct
   column.3.listsort=string(name)
   column.3.name=Approval Process Name
   column.3.querysort=name
   column.3.shortview=false
   column.3.stretch=35
   column.3.valuefield=approvalProcess:name
   column.3.valueformat=HTML
   column.3.width=220
   column.4.description=Approval Step Name
   column.4.linkedname=direct
   column.4.listsort=string(name)
   column.4.name=Approval Step Name
   column.4.querysort=name
   column.4.shortview=false
   column.4.stretch=0
   column.4.valuefield=currentApprovalStep:name
   column.4.valueformat=HTML
   column.4.width=220
   column.5.description=Previous Status
   column.5.linkedname=direct
   column.5.listsort=string(name)
   column.5.name=Previous Status
   column.5.querysort=name
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=previousStatus
   column.5.valueformat=HTML
   column.5.width=220
   column.6.linkedname=direct
   column.6.listsort=HTML(approversString)
   column.6.namekey=approver.plural.abbr
   column.6.querysort=approversString
   column.6.shortview=false
   column.6.stretch=0
   column.6.valuefield=approversString
   column.6.valueformat=HTML
   column.6.viewalias=approver.plural
   column.6.width=200
   ```

1. Klicken Sie **Fertig** > **Ansicht speichern**.
1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
