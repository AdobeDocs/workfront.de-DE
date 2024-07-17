---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Hinzufügen einer Unteraufgabe zu einer vorhandenen Geschichte auf dem Kanban-Board
description: Lesen Sie diesen Artikel, um zu erfahren, wie Sie Unteraufgaben für bestehende Geschichten auf dem Kanban-Board erstellen.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Hinzufügen einer Unteraufgabe zu einer vorhandenen Geschichte auf dem Kanban-Board

Beachten Sie beim Erstellen von Unteraufgaben für bestehende Meldungen Folgendes:

**Wenn die Einstellung [!UICONTROL Zusammenfassungsabschlussmodus] für das Projekt auf [!UICONTROL Manuell] festgelegt ist:**

* Sie können eine übergeordnete Meldung mit Unteraufgaben in [!UICONTROL Complete] verschieben, wodurch die übergeordnete Meldung auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Complete] aktualisiert wird. Unteraufgaben werden nicht aktualisiert.
* Um den [!UICONTROL Percent Complete] für die Meldung zu aktualisieren, müssen Sie ihn auf der Registerkarte [!UICONTROL Meldungen] oder auf der Seite [!UICONTROL Details] des Objekts aktualisieren.

**Wenn die Einstellung [!UICONTROL Zusammenfassungsabschlussmodus] für das Projekt auf [!UICONTROL Automatisch] festgelegt ist:**

* Sie können die übergeordnete Geschichte nicht übers Ganze verschieben. Um den [!UICONTROL Percent Complete] für die Meldung zu aktualisieren, müssen Sie den [!UICONTROL Percent Complete] für alle Unteraufgaben aktualisieren. Die [!UICONTROL Prozent abgeschlossen] für die Meldung wird basierend auf der [!UICONTROL Prozent abgeschlossen] aller Unteraufgaben berechnet.
* Wenn Sie eine übergeordnete Meldung mit Unteraufgaben auf [!UICONTROL Fertig stellen] verschieben, wird die übergeordnete Meldung auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Fertig stellen] aktualisiert. Unteraufgaben werden auch auf 100 % aktualisiert und der [!UICONTROL Status] wird auf [!UICONTROL Abgeschlossen] aktualisiert.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Contribute] oder [!UICONTROL] Zugriff auf die Aufgabe verwalten, in der sich die Unteraufgabe befindet</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Hinzufügen einer Unteraufgabe zu einer vorhandenen Geschichte auf der [!UICONTROL Kanban]-Pinnwand

1. Gehen Sie zur [!UICONTROL Kanban]-Pinnwand, die die Geschichte enthält, in der Sie eine Unteraufgabe hinzufügen möchten.
1. Klicken Sie auf der Pinnwand [!UICONTROL Kanban] auf den Namen der Aufgabe auf der Kachel &quot;Geschichte&quot;.
1. Fügen Sie der Aufgabe eine Unteraufgabe hinzu, wie Sie es in jeder anderen Aufgabenliste innerhalb von [!DNL Workfront] tun würden, wie in [Unteraufgaben erstellen](../../manage-work/tasks/create-tasks/create-subtasks.md) beschrieben.
