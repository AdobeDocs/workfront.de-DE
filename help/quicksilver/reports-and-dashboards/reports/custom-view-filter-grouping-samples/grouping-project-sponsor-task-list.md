---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Projektsponsor für eine Aufgabenliste'
description: Mit dieser Aufgabengruppen können Sie Aufgaben nach Projektsponsor gruppieren.
author: Courtney
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 27%

---

# Gruppierung: Projekt-Sponsor für eine Aufgabenliste

<!--Audited: 11/2024-->

Mit dieser Aufgabengruppen können Sie Aufgaben nach Projektsponsor gruppieren.

![Nach Projektsponsor gruppieren](assets/grouping--project-sponsor-for-a-task-350x189.png)

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

## Nach Projektsponsor für eine Aufgabenliste gruppieren


Um diese Gruppierung anzuwenden:

1. Zu einer Aufgabenliste gehen.
1. Wählen Sie **Dropdown-Menü** Gruppierung“ **Neue Gruppierung** aus.

1. Klicken Sie **In Textmodus wechseln**.
1. Entfernen Sie den Text im angezeigten Bereich und ersetzen Sie ihn durch den folgenden Code:

   ```
   group.0.name=Project Sponsor
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=string
   ```

1. Klicken Sie auf **Fertig**.
1. Aktualisieren Sie den Gruppierungsnamen und klicken Sie dann auf **Gruppierung speichern**.

