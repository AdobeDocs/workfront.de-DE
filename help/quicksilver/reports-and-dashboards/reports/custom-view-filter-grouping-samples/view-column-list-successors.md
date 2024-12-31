---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen : Liste der Aufgabennachfolger in einer Spalte hinzufügen'
description: Sie können einer Aufgabenansicht eine Spalte hinzufügen, um eine Liste der Nachfolger der Aufgaben anzuzeigen. Die Spalte „Aufgabennachfolger“ enthält die Nummer des Nachfolgers sowie den Namen.
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 1%

---

# Anzeigen : Liste der Aufgabennachfolger in einer Spalte hinzufügen

<!--Audited: 11/2024-->

Sie können einer Aufgabenansicht eine Spalte hinzufügen, um eine Liste der Nachfolger der Aufgaben anzuzeigen. Die Spalte **Aufgabe** Nachfolger“ enthält die Nummer des Nachfolgers sowie den Namen.

![TASK_VIEW_WITH_A_LIST_OF_SUCCESSORS_PNG](assets/task-view-with-a-list-of-successors--350x118.png)

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
