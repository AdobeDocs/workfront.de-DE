---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Aufgaben zuweisen
description: Sie können Benutzern, Rollen oder Teams Aufgaben zuweisen, um anzugeben, wer für die Erfüllung der Aufgaben verantwortlich ist. Sie können eine Aufgabe mehreren Ressourcen gleichzeitig zuweisen.
author: Alina
feature: Work Management
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '1901'
ht-degree: 1%

---

# Aufgaben zuweisen

{{highlighted-preview}}

Sie können Benutzern, Stellenrollen oder Teams Aufgaben zuweisen, um anzugeben, wer für die Erfüllung der Aufgaben verantwortlich ist. Sie können eine Aufgabe mehreren Ressourcen gleichzeitig zuweisen.

>[!TIP]
>
>Sie können mehrere Benutzer, Auftragsrollen oder Teams zuweisen. Sie können nur aktive Benutzer, Stellenrollen und Teams zuweisen.
>
>Wenn ein Benutzer, eine Rolle oder ein Team zugewiesen wurde, bevor sie deaktiviert wurden, bleiben sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
>
>* Weisen Sie das Arbeitselement aktiven Ressourcen erneut zu.
>* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team erneut zu.
>

Die Anzahl der einer Aufgabe zugewiesenen Benutzer und der Zeitplan des Aufgabenbesitzers können die geplanten Daten einer Aufgabe ändern, was zu einer Änderung der Zeitleiste des Projekts führt. Informationen zu den Auswirkungen der Zuweisung mehrerer Benutzer zu einer Aufgabe finden Sie unter [Übersicht über das Ändern von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Zusätzlich zu diesem Artikel empfehlen wir, die folgenden Artikel zu lesen, um weitere Informationen zum Zuweisen von Aufgaben zu erhalten:

* [Übersicht über das Ändern von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Smart-Zuweisungen vornehmen](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Erweiterte Zuweisungen erstellen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Projektübersicht planen](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Übersicht über die geplante Aufgabe - Abschlussdatum](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Festlegen des geplanten Abschlussdatums des Projekts](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Zugriffsanforderungen

<!--drafted for P&P - replace table below with this:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Benutzer</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen oder höhere Berechtigungen zu Aufgaben</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zur Mehrfachzuweisung von Stellenrollen, Teams und Benutzern

Beachten Sie beim Zuweisen mehrerer Ressourcen zu einem Arbeitselement Folgendes:

* Benutzern kann mehr als eine Auftragsrolle mit ihrem Profil zugeordnet sein. Informationen zum Zuordnen von Benutzern zu Aufgabenrollen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Wenn Sie einer Aufgabe oder einem Problem mehrere Benutzer zuweisen, wird der erste von Ihnen ausgewählte Benutzer automatisch zum Eigentümer der Aufgabe oder des Problems bestimmt.
Anweisungen zum Ändern finden Sie in den Informationen zur Option Primär machen im Artikel [Erweiterte Zuweisungen erstellen](create-advanced-assignments.md).

* Ein Team kann kein Primärer Verantwortlicher für eine Aufgabe oder ein Problem sein. Nur Benutzer oder Aufgabenrollen können als Primär für Aufgaben oder Probleme gekennzeichnet werden.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Aufgaben und Probleme in einem Projekt können zuerst einem oder mehreren Teams oder Auftragsprofilen zugewiesen werden. Wenn das Projekt startbereit ist, müssen sie möglicherweise auch Benutzern zugewiesen werden:

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Teams</td>
   <td>Wenn Sie eine Aufgabe einem Team zuweisen und auch einen Benutzer zuweisen, bleibt die Aufgabe dem Team und dem Benutzer zugewiesen, auch wenn der Benutzer nicht Mitglied des Teams ist.</td>
  </tr>
  <tr>
   <td>Aufgabengebiete</td>
   <td><p>Wenn Sie einer oder mehreren Rollen eine Aufgabe oder ein Problem zuweisen und dann auch einen Benutzer zuweisen, entscheidet gemäß den folgenden Regeln, welche Vorgangsrolle dem zusätzlichen Benutzer zugeordnet werden soll (falls vorhanden):</p>
     <ul>
      <li>Wenn nur eine Auftragsrolle zugewiesen ist und sie mit der (in ihrem Profil konfigurierten) Hauptrolle des Benutzers übereinstimmt, wird die Aufgabe oder das Problem nur diesem Benutzer zugewiesen.</li>
      <li>Wenn mehrere Rollen zugewiesen sind und mindestens eine der Rollen des Benutzers übereinstimmt, wird die Aufgabe bzw. das Problem dem Benutzer zugewiesen (die Rolle wird nach dem Zufallsprinzip ausgewählt, wenn mehrere Übereinstimmungen vorliegen), zusammen mit allen zusätzlichen zugewiesenen Rollen</li>
      <li>Wenn mindestens eine Auftragsrolle zugewiesen ist und keine Übereinstimmung mit den Benutzerrollen vorliegt, wird die Aufgabe bzw. das Problem sowohl der Rolle bzw. den Rollen als auch dem Benutzer zugewiesen.</li>
     </ul>
   <p>Informationen über die primäre Rolle eines Benutzers und andere Rollen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Benutzerprofil bearbeiten</a>.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Zuweisen einer einzelnen Aufgabe

1. Gehen Sie zu einer Aufgabe, die Sie zuweisen möchten.
1. Klicken **Zuweisen zu** im **Zuweisungen** in der Kopfzeile der Aufgabe oder des Problems.

   Oder

   Klicken Sie auf den Namen der Zuweisungen, falls die Aufgabe oder das Problem bereits zugewiesen wurde.

   ![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein, den/das Sie zuweisen möchten, und klicken Sie dann auf den Namen, wenn er/sie in der Liste angezeigt wird.


     >[!TIP]
     >
     >Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
     >
     ><span class="preview">Beim Hinzufügen einer Auftrags-Rollenzuweisung können Sie nach der Auftragsrolle oder dem Ort suchen. Wählen Sie die System-/Standardauftragsrolle aus, um die standardmäßige Abrechnungsrate für die Zuweisung zu verwenden, oder wählen Sie eine Ratenkarten-Auftragsrolle aus, um die Abrechnungsrate aus der Ratenkarte zu verwenden. Weitere Informationen zu Ratenkarten finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * (Bedingt) Klicken Sie auf einen der Namen im **Vorgeschlagene Zuweisungen** Liste, wenn diese Liste angezeigt wird. Weitere Informationen finden Sie unter [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

   * Klicken **Erweitert**

     Informationen zum Ausführen erweiterter Zuweisungen finden Sie unter [Erweiterte Zuweisungen erstellen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Klicken Sie auf **Speichern**.
1. (Optional und bedingt) Klicken Sie auf die **X-Symbol** neben dem Namen der Zuweisung im rechten Bereich der Aufgabe, um eine Zuweisung zu entfernen, wenn Sie auf **Erweitert**.

## Aufgabe in einer Liste zuweisen

Sie können Aufgaben in einer Liste oder einem Bericht zuweisen, wenn eines der Zuweisungsfelder in der Listenansicht sichtbar ist. Auf diese Weise können Aufgaben schneller zugewiesen werden. In diesem Artikel wird beschrieben, wie Sie Zuweisungen für eine Aufgabe in einer Liste ändern. Informationen zum Ändern mehrerer Zuweisungen für mehrere Aufgaben in einer Liste finden Sie unter [Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Je nachdem, welches Feld in der Ansicht sichtbar ist, können Sie der Aufgabe die folgenden Entitäten zuweisen:

| Feld | Zugewiesene Entitäten |
|---|---|
| **Zuweisen zu** | Benutzer zuweisen |
| **Zugewiesen** | Benutzer zuweisen |
| **Arbeitsaufträge** | Zuweisen von Benutzern, Auftragsrollen oder Teams |

So weisen Sie Aufgaben in einer Liste zu:

1. Rufen Sie eine Liste von Aufgaben auf, für die in der Ansicht die Felder &quot;Zugeordnet&quot;, &quot;Zugeordnet&quot;oder &quot;Zuweisungen&quot;vorhanden sind.
1. (Optional) Klicken Sie auf die **Automatische Speicherung** aus dem Dropdown-Menü und wählen Sie aus den folgenden Optionen aus:

   | Option | Optionsbeschreibung |
   |---|---| 
   | Automatisch speichern | Änderungen an den Aufgaben werden automatisch gespeichert und können nicht rückgängig gemacht werden |
   | Manuell speichern | Sie müssen Ihre Änderungen manuell speichern. Sie können Ihre Änderungen vor dem Speichern wiederherstellen. |
   | Zeitleistenplanung | Sie müssen Ihre Änderungen manuell speichern. Sie können Ihre Änderungen vor dem Speichern wiederherstellen. Das Speichern Ihrer Änderungen und aller Projektabhängigkeiten ist schneller als bei der Auswahl von Manuelles Speichern. |

   Weitere Informationen zum Speichern von Aufgaben beim Bearbeiten in einer Liste finden Sie unter [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Führen Sie einen der folgenden Schritte aus, um Aufgaben zuzuweisen:

   * Klicken Sie in die **Zugeordnet zu** oder **Zugeordnet** und beginnen Sie mit der Eingabe des Namens eines aktiven Benutzers, den Sie der Aufgabe zuweisen möchten, und klicken Sie dann auf diesen, wenn er in der Liste angezeigt wird.
   * Klicken Sie in die **Zuweisungen** eingeben und den Namen eines aktiven Benutzers, einer aktiven Rolle oder eines Teams eingeben, das bzw. das Sie der Aufgabe zuweisen möchten, und klicken Sie dann auf sie, wenn sie in der Liste angezeigt wird.

     >[!TIP]
     >
     >Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
     >
     ><span class="preview">Beim Hinzufügen einer Auftrags-Rollenzuweisung können Sie nach der Auftragsrolle oder dem Ort suchen. Wählen Sie die System-/Standardauftragsrolle aus, um die standardmäßige Abrechnungsrate für die Zuweisung zu verwenden, oder wählen Sie eine Ratenkarten-Auftragsrolle aus, um die Abrechnungsrate aus der Ratenkarte zu verwenden. Weitere Informationen zu Ratenkarten finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. (Bedingt) Wenn im **Zuweisungen** und klicken Sie auf das **Personen** in der oberen rechten Ecke des Zuweisungsfelds, um die **Erweiterte Zuweisungen** und erstellen Sie erweiterte Zuweisungen.

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   Weitere Informationen finden Sie unter [Erweiterte Zuweisungen erstellen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Sie können keine erweiterten Zuweisungen aus den Feldern Zugeordnet oder Zugeordnet vornehmen.

1. Nachdem Sie Ihre Bevollmächtigten zur Aufgabe hinzugefügt haben, drücken Sie die Eingabetaste oder klicken Sie auf eine beliebige Stelle auf der Seite, um Ihre Änderungen zu speichern, wenn Sie Automatisches Speichern ausgewählt haben. Klicken Sie andernfalls auf **Speichern**.

## Weisen Sie einem Benutzer mehrere Aufgaben zu

1. Gehen Sie zu einer Liste der Aufgaben, die Sie stapelweise zuweisen möchten.
1. (Bedingt) Stellen Sie sicher, dass die Variable **Automatische Speicherung** ausgewählt ist, wenn Sie sich auf einer Liste von Aufgaben im Rahmen eines Projekts befinden.

   >[!IMPORTANT]
   >
   >Aufgaben können beim manuellen Speichern von Aufgaben in einem Projekt nicht stapelweise bearbeitet werden.

1. Wählen Sie mehrere Aufgaben in der Aufgabenliste aus.
1. Klicken **Bearbeiten**.

   Die **Aufgaben bearbeiten** wird geöffnet.

1. Im **Zuweisungen** Bereich, wählen Sie die **Bevollmächtigter** und geben Sie dann den Namen eines Benutzers, einer Rolle oder eines Teams ein, die/das Sie allen Aufgaben zuweisen möchten.

   >[!IMPORTANT]
   >
   >Wenn eine der Aufgaben bereits zugewiesen ist, werden die hier angegebenen Ressourcen zu den Aufgaben hinzugefügt, anstatt die vorhandenen Ressourcen für die Aufgaben zu ersetzen.

1. (Optional) Wählen Sie das Optionsfeld im **Aufgabeneigentümer** gibt an, welche Ressource der primäre Verantwortliche oder Eigentümer der Aufgabe ist, wenn Sie der Aufgabe mehr als eine Ressource zuweisen. Dies ist nicht für Teams verfügbar.
1. (Bedingt) Geben Sie die **Zuteilung %** für jede Ressource, die der Aufgabe zugewiesen ist, wenn alle ausgewählten Aufgaben über eine Dauer verfügen, die vom Aufwandstyp bestimmt oder berechnet wurde. Dies gibt an, wie viel Zeit diese Ressourcen für das Abschließen der Aufgabe verbringen sollen. Dies ist nur für Benutzer und Vorgangsrollen verfügbar.

   Oder

   Geben Sie den Betrag von **Stunden** für jede Ressource, die der Aufgabe zugewiesen ist, wenn für alle ausgewählten Aufgaben der Typ Einfache Dauer ausgewählt ist. Die Gesamtstundenzahl für alle Ressourcen sollte der Anzahl der geplanten Stunden für die Aufgabe entsprechen.

   >[!IMPORTANT]
   >
   >Sie können den Zuordnungsprozentsatz oder die Anzahl der Stunden pro Ressource nicht angeben, wenn die ausgewählten Aufgaben unterschiedliche Typen der Dauer oder die ausgewählten Aufgaben unterschiedliche Typen der Dauer aufweisen.

   Informationen zum Typ der Dauer für Aufgaben finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Optional) Wählen Sie eine Rolle aus, die der Benutzer für die Aufgabe aus dem **Rolle auswählen** Dropdown-Menü im **Rolle des Bevollmächtigten** Spalte, wenn Sie Aufgaben Benutzer zuweisen. Wenn Sie keine Rolle auswählen, wählt Workfront automatisch die Primäre Rolle des Benutzers aus.

1. (Optional) Wenn Sie vorhandene Bevollmächtigte aus allen Aufgaben entfernen möchten, führen Sie einen der folgenden Schritte aus:

   1. Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein, den/das Sie aus der Aufgabe entfernen möchten, wählen Sie ihn aus, wenn er/sie in der Liste angezeigt wird, und klicken Sie auf **Zuweisung entfernen** , um weitere Bevollmächtigte zu entfernen.
   1. Klicken **Alle vorhandenen Zuweisung entfernen** um alle Bevollmächtigten aus allen ausgewählten Aufgaben zu entfernen.

1. Klicken **Änderungen speichern**.
1. (Optional und bedingt) Wenn die Felder Zugeordnet oder Zuweisungen in Ihrer Aufgabenliste angezeigt werden, klicken Sie in eine dieser Spalten für eine Aufgabe und klicken Sie dann auf die Schaltfläche **X-Symbol** neben dem Namen eines Bevollmächtigten, um ihn aus der Aufgabe zu entfernen.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


