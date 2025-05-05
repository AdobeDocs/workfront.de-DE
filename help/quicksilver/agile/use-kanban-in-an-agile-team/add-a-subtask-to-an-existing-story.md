---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Eine Unteraufgabe zu einer vorhandenen Story auf dem Kanban-Board hinzufügen
description: Lesen Sie diesen Artikel, um zu erfahren, wie Sie Unteraufgaben für vorhandene Storys im Kanban-Board erstellen.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Eine Unteraufgabe zu einer vorhandenen Story auf dem Kanban-Board hinzufügen

Beachten Sie beim Erstellen von Unteraufgaben für vorhandene Storys Folgendes:

**Wenn die Einstellung [!UICONTROL Zusammenfassung - Fertigstellungsmodus] für das Projekt auf &quot;[!UICONTROL Manuell]:**

* Sie können eine übergeordnete Story mit Teilaufgaben nach [!UICONTROL Abgeschlossen] verschieben, wodurch die übergeordnete Story auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Abgeschlossen] aktualisiert wird. Teilaufgaben werden nicht aktualisiert.
* Um den [!UICONTROL Prozent abgeschlossen] für die Story zu aktualisieren, müssen Sie ihn über die Registerkarte [!UICONTROL Storys] oder über die Seite [!UICONTROL Details] des Objekts aktualisieren.

**Wenn die Einstellung [!UICONTROL Zusammenfassungsabschlussmodus] für das Projekt auf &quot;[!UICONTROL &quot; &#x200B;]:**

* Sie können die übergeordnete Story nicht über die Pinnwand verschieben. Um den [!UICONTROL Prozent abgeschlossen] für die Story zu aktualisieren, müssen Sie den [!UICONTROL Prozent abgeschlossen] für alle Teilaufgaben aktualisieren. Der [!UICONTROL Prozent abgeschlossen] für die Story wird anhand des [!UICONTROL Prozent abgeschlossen] aller Teilaufgaben berechnet.
* Wenn Sie eine übergeordnete Story mit Teilaufgaben nach [!UICONTROL Abgeschlossen] verschieben, wird die übergeordnete Story auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Abgeschlossen] aktualisiert. Teilaufgaben werden ebenfalls auf 100 % aktualisiert und der [!UICONTROL Status] wird auf [!UICONTROL Abgeschlossen] aktualisiert.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Work] oder höher</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Zugriff von [!UICONTROL Contribute] oder [!UICONTROL Manage] auf die Aufgabe, für die die Unteraufgabe ausgeführt wird</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eine Unteraufgabe zu einer vorhandenen Story auf dem Kanban[!UICONTROL Board &#x200B;]

1. Wechseln Sie zur [!UICONTROL Kanban]-Pinnwand, die die Story enthält, der Sie eine Unteraufgabe hinzufügen möchten.
1. Klicken Sie auf den Namen der Aufgabe auf der Story-Kachel auf dem [!UICONTROL Kanban]-Board.
1. Fügen Sie der Aufgabe wie in jeder anderen Aufgabenliste innerhalb von [!DNL Workfront] eine Unteraufgabe hinzu, wie in [Erstellen von Unteraufgaben](../../manage-work/tasks/create-tasks/create-subtasks.md) beschrieben.
