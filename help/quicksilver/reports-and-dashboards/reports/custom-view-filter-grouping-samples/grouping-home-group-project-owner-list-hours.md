---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Hauptgruppe des Projektbesitzers in einer Stundenliste'
description: Sie können den Namen der Hauptgruppe des Projektbesitzers in einer Stundenliste oder einem Bericht anzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: 6491ab9b-c09e-4bdb-99c2-56bb44f66947
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Gruppierung: Hauptgruppe des Projektbesitzers in einer Stundenliste

<!--Audited: 10/2024-->

Sie können den Namen der Hauptgruppe des Projektbesitzers in einer Stundenliste oder einem Bericht anzeigen.

Die Gruppierung gruppiert die Ergebnisse auch nach dem Namen des Projektbesitzers und dem Projektnamen.

![grouping_for_project_owner_home_group.png](assets/grouping-for-project-owner-home-group-350x51.png)

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

## Nach Hauptgruppe des Projektbesitzers in einer Stundenliste gruppieren

Um diese Gruppierung anzuwenden:

1. Zu einer Stundenliste gehen.
1. Wählen Sie **Dropdown-Menü** Gruppierung“ **Neue Gruppierung** aus.

1. Klicken Sie **In Textmodus wechseln**.
1. Entfernen Sie den Text im Bereich **Gruppieren nach**.
1. Ersetzen Sie den Text durch den folgenden Code:

```
group.0.displayname=Home Group of Project Owner
group.0.valuefield=project:owner:homeGroup:name
group.0.valueformat=HTML
group.1.displayname=Project Owner
group.1.linkedname=projectOwnerMM
group.1.namekey=view.relatedcolumn
group.1.namekeyargkey.0=projectOwnerMM
group.1.namekeyargkey.1=name
group.1.valuefield=projectOwnerMM:name
group.1.valueformat=string
group.2.displayname=Project Name
group.2.linkedname=project
group.2.namekey=view.relatedcolumn
group.2.namekeyargkey.0=project
group.2.namekeyargkey.1=name
group.2.valuefield=project:name
group.2.valueformat=string
textmode=true
```

1. Klicken Sie **Fertig** > **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Namen der Gruppierung und klicken Sie dann auf **Gruppierung speichern**.
