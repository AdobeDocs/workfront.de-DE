---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Eine Unteraufgabe zu einer vorhandenen Story auf dem Kanban-Board hinzufügen
description: Lesen Sie diesen Artikel, um zu erfahren, wie Sie Unteraufgaben für vorhandene Storys im Kanban-Board erstellen.
author: Courtney
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/Wbiao1UjwOzItIGJkh1E9A81RcUfLDJqgYjRDL46qvQ'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 14%
---
# Hinzufügen einer Unteraufgabe zu einer vorhandenen Story auf dem Kanban-Board

Beachten Sie beim Erstellen von Unteraufgaben für vorhandene Storys Folgendes:

**Wenn die Einstellung [!UICONTROL Zusammenfassung - Fertigstellungsmodus] für das Projekt auf &quot;[!UICONTROL Manuell]:**

* Sie können eine übergeordnete Story mit Teilaufgaben nach [!UICONTROL Abgeschlossen] verschieben, wodurch die übergeordnete Story auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Abgeschlossen] aktualisiert wird. Teilaufgaben werden nicht aktualisiert.
* Um den [!UICONTROL Prozent abgeschlossen] für die Story zu aktualisieren, müssen Sie ihn über die Registerkarte [!UICONTROL Storys] oder über die Seite [!UICONTROL Details] des Objekts aktualisieren.

**Wenn die Einstellung [!UICONTROL Zusammenfassungsabschlussmodus] für das Projekt auf &quot;[!UICONTROL &quot; ]:**

* Sie können die übergeordnete Story nicht über die Pinnwand verschieben. Um den [!UICONTROL Prozent abgeschlossen] für die Story zu aktualisieren, müssen Sie den [!UICONTROL Prozent abgeschlossen] für alle Teilaufgaben aktualisieren. Der [!UICONTROL Prozent abgeschlossen] für die Story wird anhand des [!UICONTROL Prozent abgeschlossen] aller Teilaufgaben berechnet.
* Wenn Sie eine übergeordnete Story mit Teilaufgaben nach [!UICONTROL Abgeschlossen] verschieben, wird die übergeordnete Story auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Abgeschlossen] aktualisiert. Teilaufgaben werden ebenfalls auf 100 % aktualisiert und der [!UICONTROL Status] wird auf [!UICONTROL Abgeschlossen] aktualisiert.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Work oder höher</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Zugriff auf die Aufgabe, für die die Teilaufgabe ausgeführt wird, gewähren oder verwalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Eine Unteraufgabe zu einer vorhandenen Story auf dem Kanban[!UICONTROL Board ]

1. Wechseln Sie zur [!UICONTROL Kanban]-Pinnwand, die die Story enthält, der Sie eine Unteraufgabe hinzufügen möchten.
1. Klicken Sie auf den Namen der Aufgabe auf der Story-Kachel auf dem [!UICONTROL Kanban]-Board.
1. Fügen Sie der Aufgabe wie in jeder anderen Aufgabenliste innerhalb von [!DNL Workfront] eine Unteraufgabe hinzu, wie in [Erstellen von Unteraufgaben](../../manage-work/tasks/create-tasks/create-subtasks.md) beschrieben.
