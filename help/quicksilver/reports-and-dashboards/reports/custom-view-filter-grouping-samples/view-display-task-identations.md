---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Aufgabeneinzüge in einer Aufgabenliste anzeigen'
description: In dieser Aufgabenansicht können Sie der Spalte Aufgabenname Code hinzufügen, um die Aufgaben anzuzeigen, die entsprechend der Arbeitsaufschlüsselstruktur des Projekts eingerückt sind.
author: Courtney
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 19%

---

# Ansicht: Einrückung von Aufgaben in einer Aufgabenliste anzeigen

<!--Audited: 11/2024-->

In dieser Aufgabenansicht können Sie der Spalte Aufgabenname Code hinzufügen, um die Aufgaben anzuzeigen, die entsprechend der Arbeitsaufschlüsselstruktur des Projekts eingerückt sind.

![Aufgabeneinzug anzeigen](assets/view-text-mode-indentation-task-list-350x171.png)

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

## Aufgabeneinzüge in einer Spalte einer Aufgabenliste anzeigen

1. Zu einer Aufgabenliste gehen.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen** und geben Sie „Aufgabenname“ in das Feld **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie in der neuen Spalte auf **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text in der `valuefield=` Zeile und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Task hierarchy
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
