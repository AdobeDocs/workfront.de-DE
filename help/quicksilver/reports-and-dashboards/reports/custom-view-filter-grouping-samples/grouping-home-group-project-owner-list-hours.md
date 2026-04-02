---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Hauptgruppe des Projektbesitzers in einer Stundenliste'
description: Sie können den Namen der Hauptgruppe des Projektbesitzers in einer Stundenliste oder einem Bericht anzeigen.
author: Courtney
feature: Reports and Dashboards
exl-id: 6491ab9b-c09e-4bdb-99c2-56bb44f66947
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 22%

---

# Gruppierung: Hauptgruppe des Projektbesitzers bzw. der Projektbesitzerin in einer Stundenliste

<!--Audited: 10/2024-->

Sie können den Namen der Hauptgruppe des Projektbesitzers in einer Stundenliste oder einem Bericht anzeigen.

Die Gruppierung gruppiert die Ergebnisse auch nach dem Namen des Projektbesitzers und dem Projektnamen.

![grouping_for_project_owner_home_group.png](assets/grouping-for-project-owner-home-group-350x51.png)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
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

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
