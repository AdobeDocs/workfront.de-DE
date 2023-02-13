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
source-wordcount: '363'
ht-degree: 0%

---

# Hinzufügen einer Unteraufgabe zu einer vorhandenen Geschichte auf dem Kanban-Board

Beachten Sie beim Erstellen von Unteraufgaben für bestehende Meldungen Folgendes:

**Wenn die [!UICONTROL Modus für Zusammenfassungsabschluss] -Einstellung für das Projekt auf [!UICONTROL Manuell]:**

* Sie können eine übergeordnete Meldung mit Unteraufgaben in [!UICONTROL Fertig], wodurch die übergeordnete Meldung auf 100 % und die [!UICONTROL Status] nach [!UICONTROL Fertig]. Unteraufgaben werden nicht aktualisiert.
* So aktualisieren Sie die [!UICONTROL Prozent abgeschlossen] für die Geschichte müssen Sie sie über die [!UICONTROL Meldungen] oder aus dem [!UICONTROL Details] -Seite des -Objekts.

**Wenn die [!UICONTROL Modus für Zusammenfassungsabschluss] -Einstellung für das Projekt auf [!UICONTROL Automatisch]:**

* Sie können die übergeordnete Geschichte nicht übers Ganze verschieben. So aktualisieren Sie die [!UICONTROL Prozent abgeschlossen] für die Geschichte müssen Sie die [!UICONTROL Prozent abgeschlossen] für alle Unteraufgaben. Die [!UICONTROL Prozent abgeschlossen] für die Erzählung anhand der [!UICONTROL Prozent abgeschlossen] aller Unteraufgaben.
* Verschieben einer übergeordneten Geschichte mit Unteraufgaben in [!UICONTROL Fertig] aktualisiert die übergeordnete Meldung auf 100 % und die [!UICONTROL Status] nach [!UICONTROL Fertig]. Unteraufgaben werden auch auf 100 % aktualisiert und die [!UICONTROL Status] aktualisiert auf [!UICONTROL Fertig].

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Contribute] oder [!UICONTROL Verwalten] Zugriff auf die Aufgabe, in der sich die Unteraufgabe befindet</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Hinzufügen einer Unteraufgabe zu einem vorhandenen Artikel auf der [!UICONTROL Kanban] Pinnwand

1. Navigieren Sie zu [!UICONTROL Kanban] -Pinnwand, die die Geschichte enthält, der Sie eine Unteraufgabe hinzufügen möchten.
1. Klicken Sie auf den Namen der Aufgabe in der Kachel &quot;Geschichte&quot;auf der [!UICONTROL Kanban] Pinnwand.
1. Fügen Sie der Aufgabe eine Unteraufgabe hinzu, wie Sie sie in jeder anderen Aufgabenliste in [!DNL Workfront]wie in [Erstellen von Unteraufgaben](../../manage-work/tasks/create-tasks/create-subtasks.md).
