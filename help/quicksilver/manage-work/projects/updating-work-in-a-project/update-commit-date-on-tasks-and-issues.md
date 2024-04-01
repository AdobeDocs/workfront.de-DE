---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen
description: Sie können das Übermittlungsdatum einer Aufgabe oder eines Problems, dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zu den Zusendedaten in Adobe Workfront finden Sie unter Übersicht über das Datum der Übermittlung .
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 55e8fc5ce8f3b4065f6c974bf77da4e91e66090f
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---


# Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen

Sie können das Übermittlungsdatum einer Aufgabe oder eines Problems, dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zum Festlegen von Datumswerten in Adobe Workfront finden Sie unter [Datum bestätigen - Übersicht](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Zugriffsanforderungen

<!--Audited: 01/2024-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
   Für die neuen Lizenzen:
   <ul>
   <li><p>Standard für Aufgaben</p> </li>
   <li><p>Beitragende oder höher für Probleme</p></li>
   </ul>
   Für aktuelle Lizenzen:
<ul>
   <li><p>Arbeit oder höher für Aufgaben</p></li> 
   <li><p>Anfrage oder höher für Probleme</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben oder Probleme verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Bevor Sie beginnen, müssen Sie der Aufgabe oder dem Problem zugewiesen sein, für die Sie das Veröffentlichungsdatum aktualisieren müssen.

## Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen

Die Aktualisierung des Veröffentlichungsdatums ist für Aufgaben und Probleme identisch.

1. Gehen Sie zu einer Aufgabe oder einem Problem, die bzw. dem Sie als **Inhaber**.

   Weitere Informationen dazu, wie Sie herausfinden, wer der Aufgabeneigentümer für ein Problem oder eine Aufgabe ist, finden Sie im Abschnitt [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Klicks **Aufgabendetails** oder **Problemdetails** im linken Bereich.
1. Klicks **Übersicht** um sie zu erweitern.
1. Aktualisieren Sie die **Datum der Übermittlung** -Feld.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klicken Sie auf **Änderungen speichern**.

   Nach dieser Änderung geschieht Folgendes: 

   * Das Datum der Übermittlung und das geplante Abschlussdatum der Aufgabe bzw. des Problems sind nicht mehr dasselbe.

     Stattdessen werden das Bestätigungsdatum und das geplante Abschlussdatum der Aufgabe oder des Problems identisch.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Der Projekteigentümer wird in den In-App-Benachrichtigungen darüber benachrichtigt, dass Sie ein neues Veröffentlichungsdatum für die Aufgabe oder das Problem vorgeschlagen haben.
   * Der Projekteigentümer wird im Abschnitt Updates darüber benachrichtigt, dass Sie ein neues Veröffentlichungsdatum vorgeschlagen haben. Zu diesem Zeitpunkt kann er das geplante Abschlussdatum der Aufgabe oder des Problems entsprechend dem von Ihnen vorgeschlagenen Zustimmungsdatum aktualisieren. Diese Funktion wird im neuen Kommentierungserlebnis nicht unterstützt. Weitere Informationen finden Sie unter [Die neue Kommentarfunktion](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     Informationen zu den Benachrichtigungen und Aktualisierungen, die durch diese Änderung ausgelöst werden, finden Sie im Abschnitt &quot;Benachrichtigungen und Aktualisierungen, die durch Änderung des Zusagedatums ausgelöst werden&quot;im Artikel [Datum bestätigen - Übersicht](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->