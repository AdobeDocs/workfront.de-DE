---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Vorgänge nach Portfolio, Programm und Projekt'
description: Verwenden Sie diese Vorgangsgruppierung, um Vorgänge nach dem Portfolio, nach Programm und dann nach dem Projekt zu gruppieren, mit dem sie verknüpft sind.
author: Courtney
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 23%

---

# Gruppierung: Aufgaben nach Portfolio, Programm und Projekt

<!--Audited: 10/2024-->

Verwenden Sie diese Vorgangsgruppierung, um Vorgänge nach dem Portfolio, nach Programm und dann nach dem Projekt zu gruppieren, mit dem sie verknüpft sind.

![Portfolio-Programmprojektgruppierung](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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
   <p>Anbieter oder Anforderung zum Ändern eines Filters </p>
   <p>Standard oder Abo zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen zum Ändern eines Filters</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aufgaben nach Portfolio, Programm und Projekt gruppieren

So wenden Sie diese Gruppierung an:

1. Wechseln Sie zu einer Liste von Aufgaben.
1. Wählen Sie im Dropdown-Menü **Gruppierung** die Option **Neue Gruppierung** aus.
1. Klicken Sie auf **Gruppierung hinzufügen**.

1. Klicken Sie auf **In Textmodus wechseln**.
1. Entfernen Sie den Text im Bereich **Gruppe nach**.
1. Ersetzen Sie den Text durch folgenden Code:

   ```
   group.0.linkedname=project
   group.0.namekey=portfolio
   group.0.notime=false
   group.0.valuefield=project:portfolio:name
   group.0.valueformat=string
   group.1.linkedname=project
   group.1.namekey=program
   group.1.notime=false
   group.1.valuefield=project:program:name
   group.1.valueformat=string
   group.2.name=Project
   group.2.valuefield=project:name
   group.2.valueformat=HTML
   textmode=true
   ```

1. Klicken Sie auf **Fertig** > **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Gruppierungsnamen, und klicken Sie dann auf **Gruppierung speichern**.

