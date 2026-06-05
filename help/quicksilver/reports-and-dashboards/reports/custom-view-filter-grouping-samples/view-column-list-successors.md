---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen : Liste der Aufgabennachfolger in einer Spalte hinzufügen'
description: Sie können einer Aufgabenansicht eine Spalte hinzufügen, um eine Liste der Nachfolger der Aufgaben anzuzeigen. Die Spalte „Aufgabennachfolger“ enthält die Nummer des Nachfolgers sowie den Namen.
author: Courtney
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/4fHIzHGFKODGd4UpJAANsFoI-FpzOptq8qyIp0IFgZ0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 22%

---

# Ansicht: Liste der Aufgabennachfolger in einer Spalte hinzufügen

<!--Audited: 11/2024-->

Sie können einer Aufgabenansicht eine Spalte hinzufügen, um eine Liste der Nachfolger der Aufgaben anzuzeigen. Die Spalte **Aufgabe** Nachfolger“ enthält die Nummer des Nachfolgers sowie den Namen.

![TASK_VIEW_WITH_A_LIST_OF_SUCCESSORS_PNG](assets/task-view-with-a-list-of-successors--350x118.png)

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


## Liste der Aufgabennachfolger in einer Spalte hinzufügen

So fügen Sie diese Spalte einer Aufgabenansicht hinzu:

1. Zu einer Aufgabenliste gehen.
1. Erweitern Sie das **Ansicht** Dropdown-Menü und klicken Sie auf **Neue Ansicht**.
1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie **Wechseln Sie in den Textmodus** und klicken Sie dann auf **Textmodus bearbeiten**.
1. Entfernen Sie den gesamten Text im Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
