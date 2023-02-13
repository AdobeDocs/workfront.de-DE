---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen
description: Sie können das Übermittlungsdatum einer Aufgabe oder eines Problems, dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zu den Zusendedaten in Adobe Workfront finden Sie unter Übersicht über das Datum der Übermittlung .
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen

Sie können das Übermittlungsdatum einer Aufgabe oder eines Problems, dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zum Festlegen von Datumswerten in Adobe Workfront finden Sie unter [Datum bestätigen - Übersicht](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Zugriffsanforderungen

<!--drafted for P&P

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   For the current licenses:
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   For legacy licenses:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher für Aufgaben</p> 
   <p>Anfrage oder höher für Probleme</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben oder Probleme verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie der Aufgabe oder dem Problem zugewiesen sein, für die Sie das Veröffentlichungsdatum aktualisieren müssen.

## Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen

Die Aktualisierung des Veröffentlichungsdatums ist für Aufgaben und Probleme identisch.

1. Gehen Sie zu einer Aufgabe oder einem Problem, die bzw. dem Sie als **Aufgabeneigentümer**.

   Weitere Informationen dazu, wie Sie herausfinden, wer der Aufgabeneigentümer für ein Problem oder eine Aufgabe ist, finden Sie im Abschnitt [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Klicken Sie auf Bearbeiten in der Aufgaben- oder Problemkopfzeile

   Oder

   Klicken **Aufgabe starten** oder **Startproblem** , wenn die Schaltfläche Bearbeiten in Ihrer Umgebung angepasst wurde, um anzugeben, dass Sie derzeit am Arbeitselement arbeiten.

   Zu diesem Zeitpunkt sind das Zustimmungsdatum und das geplante Abschlussdatum der Aufgabe oder des Problems identisch.

1. (Optional) Wenn Sie auf Aufgabe starten oder Problem starten geklickt haben, klicken Sie auf **Rückgängig** in der linken unteren Ecke des Bildschirms. Das Datum für das Bestätigen wird entfernt.

   Weitere Informationen zum Ersetzen der Schaltfläche &quot;Work On It&quot;durch eine Schaltfläche &quot;Start&quot;finden Sie unter  [Ersetzen der Schaltfläche &quot;Work On It&quot;durch die Schaltfläche Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

   >[!TIP]
   >
   >Die Option zum Rückgängigmachen Ihrer Auswahl zum Starten Ihrer Arbeit ist nicht verfügbar, wenn Sie auf **Arbeiten daran**.

1. Klicken **Updates** Klicken Sie im linken Bereich auf das **Neue Aktualisierung starten** >**Datum der Übermittlung**

   Oder

   Klicken **Aufgabendetails** oder **Problemdetails** Klicken Sie im linken Bereich auf **Datum der Übermittlung** und wählen Sie ein neues Datum aus dem Kalender aus. Klicken Sie dann auf **Änderungen speichern**.
   ![](assets/commit-date-calendar-picker-in-updates-stream-nwe-350x452.png)

   Nach dieser Änderung geschieht Folgendes: 

   * Das Datum der Veröffentlichung und das Datum des geplanten Abschlusses sind nicht mehr dasselbe.

      Stattdessen werden das Bestätigungsdatum und das geplante Abschlussdatum der Aufgabe oder des Problems identisch.

      ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Die Änderungen werden automatisch gespeichert, wenn Sie im Bereich Updates ein neues Datum auswählen.
   * Der Projekteigentümer wird darüber informiert, dass Sie ein neues Veröffentlichungsdatum für die Aufgabe oder das Problem vorgeschlagen haben, und kann zu diesem Zeitpunkt das geplante Abschlussdatum der Aufgabe oder des Problems aktualisieren, um es an das von Ihnen vorgeschlagene Zustimmungsdatum anzupassen.

      ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

      Informationen zu den Benachrichtigungen und Aktualisierungen, die durch diese Änderung ausgelöst werden, finden Sie im Abschnitt . [Durch Änderung des Zusagedatums ausgelöste Benachrichtigungen und Aktualisierungen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) im Artikel [Datum bestätigen - Übersicht](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
