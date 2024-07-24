---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Aufgaben zuweisen
description: Sie können Benutzern, Rollen oder Teams Aufgaben zuweisen, um anzugeben, wer für die Erfüllung der Aufgaben verantwortlich ist. Sie können eine Aufgabe mehreren Ressourcen gleichzeitig zuweisen.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 7b0da61c301fe8f1f24aa27a469952fbd46987c5
workflow-type: tm+mt
source-wordcount: '1985'
ht-degree: 1%

---

# Aufgaben zuweisen

<!--Audited: 07/2024-->

<!--remove the span class preview from everywhere but the Rate Card roles references must stay in yellow; replace the intro with preview and fast track only but not sure if with the link to third quarter release?!-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>.

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Überblick über die Version des vierten Quartals 2024](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md).</span>

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

Die Anzahl der einer Aufgabe zugewiesenen Benutzer und der Zeitplan des Aufgabenbesitzers können die geplanten Daten einer Aufgabe ändern, was zu einer Änderung der Zeitleiste des Projekts führt. Informationen zu den Auswirkungen der Zuweisung mehrerer Benutzer zu einer Aufgabe finden Sie unter [Übersicht über die Änderung von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Zusätzlich zu diesem Artikel empfehlen wir, die folgenden Artikel zu lesen, um weitere Informationen zum Zuweisen von Aufgaben zu erhalten:

* [Übersicht über die Änderung von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Smart-Zuweisungen vornehmen](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Erweiterte Zuweisungen erstellen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Ändern mehrerer Benutzerzuweisungen in einer Aufgabenliste](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Projektübersicht planen](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Übersicht über das geplante Abschlussdatum der Aufgabe](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Das geplante Abschlussdatum des Projekts festlegen](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Systemweite Projektanvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Zugriffsanforderungen

<!-- Audited: 07/2024-->

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p>
   <p>Aktuell: Arbeit oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>


*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Überlegungen zur Mehrfachzuweisung von Stellenrollen, Teams und Benutzern

Beachten Sie beim Zuweisen mehrerer Ressourcen zu einem Arbeitselement Folgendes:

* Benutzern kann mehr als eine Auftragsrolle mit ihrem Profil zugeordnet sein. Informationen zum Zuordnen von Benutzern zu Vorgangsrollen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Wenn Sie einer Aufgabe oder einem Problem mehrere Benutzer zuweisen, wird der erste von Ihnen ausgewählte Benutzer automatisch zum Eigentümer der Aufgabe oder des Problems bestimmt.
Anweisungen zum Ändern finden Sie in den Informationen zur Option &quot;Primär machen&quot;im Artikel [Erweiterte Zuweisungen erstellen](create-advanced-assignments.md).

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
   <p>Informationen über die primäre Rolle eines Benutzers und andere Rollen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Profil eines Benutzers bearbeiten</a>.</p>
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
1. Klicken Sie im Feld **Zuweisungen** in der Kopfzeile der Aufgabe auf **Zuweisen zu** .

   Oder

   Klicken Sie auf den Namen der Zuweisungen, falls die Aufgabe bereits zugewiesen ist.

   ![Arbeitsaufträge](assets/assignments-box-in-task-header.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein, den/das Sie zuweisen möchten, und klicken Sie dann auf den Namen, wenn er/sie in der Liste angezeigt wird.


     >[!TIP]
     >
     >Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
     >
     >Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     >
     ><span class="preview">Beim Hinzufügen einer Auftragsrollenzuweisung können Sie nach der Auftragsrolle oder dem Ort suchen. Wählen Sie in der Liste Auftragsrollen eine Rolle aus, um die standardmäßige Abrechnungsrate für die Zuweisung zu verwenden, oder wählen Sie eine Auftragsrolle für die Ratenkarte aus, um die Abrechnungsrate aus der Ratenkarte zu verwenden. Weitere Informationen zu Ratenkarten finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


   * (Bedingt) Klicken Sie auf einen der Namen in den Listen <span class="preview">**Vorgeschlagene Zuweisungen**</span>, **Benutzer und Teams** oder **Auftragsrollen** oder <span class="preview">**Rollen der Ratenkarten**</span> , wenn sie angezeigt werden. Weitere Informationen finden Sie unter [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     Sie können mit der Eingabe des Namens jedes Benutzers, Teams oder Auftrags beginnen, der der Aufgabe zuzuweisen, und diese dann auswählen, wenn sie in der Liste angezeigt wird.

   * Klicken Sie auf **Erweitert** .

     Informationen zum Erstellen erweiterter Zuweisungen finden Sie unter [Erstellen erweiterter Zuweisungen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Klicken Sie auf **Speichern**.
1. (Optional und bedingt) Klicken Sie im rechten Bereich der Aufgabe auf das Symbol **X** neben dem Namen der Zuweisung, um eine Zuweisung zu entfernen, wenn Sie auf **Erweitert** geklickt haben.

## Aufgabe in einer Liste zuweisen

Sie können Aufgaben in einer Liste oder einem Bericht zuweisen, wenn eines der Zuweisungsfelder in der Listenansicht sichtbar ist. Auf diese Weise können Aufgaben schneller zugewiesen werden. In diesem Artikel wird beschrieben, wie Sie Zuweisungen für eine Aufgabe in einer Liste ändern. Informationen zum Ändern mehrerer Zuweisungen für mehrere Aufgaben in einer Liste finden Sie unter [Ändern mehrerer Benutzerzuweisungen in einer Aufgabenliste](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Je nachdem, welches Feld in der Ansicht sichtbar ist, können Sie der Aufgabe die folgenden Entitäten zuweisen:

| Feld | Zugewiesene Entitäten |
|---|---|
| **Zuweisen zu** | Benutzer zuweisen |
| **Zugeordnet** | Benutzer zuweisen |
| **Arbeitsaufträge** | Zuweisen von Benutzern, Auftragsrollen oder Teams |

So weisen Sie Aufgaben in einer Liste zu:

1. Rufen Sie eine Liste von Aufgaben auf, für die in der Ansicht die Felder &quot;Zugeordnet&quot;, &quot;Zugeordnet&quot;oder &quot;Zuweisungen&quot;vorhanden sind.
1. (Optional) Klicken Sie auf das Dropdownmenü **Automatisches Speichern** und wählen Sie eine der folgenden Optionen aus:

   | Option | Optionsbeschreibung |
   |---|---| 
   | Automatisch speichern | Änderungen an den Aufgaben werden automatisch gespeichert und können nicht rückgängig gemacht werden |
   | Manuell speichern | Sie müssen Ihre Änderungen manuell speichern. Sie können Ihre Änderungen vor dem Speichern wiederherstellen. |
   | Zeitleistenplanung | Sie müssen Ihre Änderungen manuell speichern. Sie können Ihre Änderungen vor dem Speichern wiederherstellen. Das Speichern Ihrer Änderungen und aller Projektabhängigkeiten ist schneller als bei der Auswahl von Manuelles Speichern. |

   Weitere Informationen zum Speichern von Aufgaben beim Bearbeiten in einer Liste finden Sie unter [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Führen Sie einen der folgenden Schritte aus, um Aufgaben zuzuweisen:

   * Klicken Sie in die Felder **Zugeordneter Benutzer** oder **Zugeordneter Benutzer** und geben Sie den Namen eines aktiven Benutzers ein, den Sie der Aufgabe zuweisen möchten, und klicken Sie dann auf ihn, wenn er in der Liste angezeigt wird.
   * Klicken Sie in das Feld **Zuweisungen** und geben Sie den Namen eines aktiven Benutzers, einer aktiven Rolle oder eines aktiven Teams ein, den bzw. das Sie der Aufgabe zuweisen möchten. Klicken Sie dann auf die Aufgabe, wenn sie in der Liste angezeigt wird.

     >[!TIP]
     >
     >Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
     >
     >Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >
     ><span class="preview">Beim Hinzufügen einer Auftragsrollenzuweisung können Sie nach der Auftragsrolle oder dem Ort suchen. Wählen Sie eine Auftragsrolle aus, um die standardmäßige Abrechnungsrate für die Zuweisung zu verwenden, oder wählen Sie eine Ratenkartenrolle aus, um die Abrechnungsrate auf der Ratenkarte zu verwenden. Weitere Informationen zu Ratenkarten finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>


1. (Bedingt) Wenn dies im Feld **Zuweisungen** sichtbar ist, klicken Sie auf das Symbol **Personen** in der oberen rechten Ecke des Zuweisungsfelds, um das Feld **Erweiterte Zuweisungen** zu öffnen und erweiterte Zuweisungen zu erstellen.

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
1. (Bedingt) Stellen Sie sicher, dass die Option **Automatisches Speichern** ausgewählt ist, wenn Sie sich auf einer Liste von Aufgaben unter einem Projekt befinden.

   >[!IMPORTANT]
   >
   >Aufgaben können beim manuellen Speichern von Aufgaben in einem Projekt nicht stapelweise bearbeitet werden.

1. Wählen Sie mehrere Aufgaben in der Aufgabenliste aus.
1. Klicken Sie auf **Bearbeiten**.

   Das Dialogfeld **Aufgaben bearbeiten** wird geöffnet.

1. Wählen Sie im Bereich **Zuweisungen** das Feld **Bevollmächtigter** aus und geben Sie dann den Namen eines Benutzers, einer Rolle oder eines Teams ein, die bzw. das Sie allen Aufgaben zuweisen möchten.

   >[!IMPORTANT]
   >
   >Wenn eine der Aufgaben bereits zugewiesen ist, werden die hier angegebenen Ressourcen zu den Aufgaben hinzugefügt, anstatt die vorhandenen Ressourcen für die Aufgaben zu ersetzen.

1. (Optional) Wählen Sie das Optionsfeld in der Spalte **Aufgabeneigentümer** aus, um anzugeben, welche Ressource der primäre Verantwortliche oder Eigentümer der Aufgabe ist, wenn Sie der Aufgabe mehr als eine Ressource zuweisen. Dies ist nicht für Teams verfügbar.
1. (Bedingt) Geben Sie die &quot;**Zuordnung %**&quot; für jede Ressource an, die der Aufgabe zugewiesen ist, wenn für alle ausgewählten Aufgaben der Typ &quot;Dauer&quot;bestimmt oder &quot;Berechnete Zuweisung&quot;ausgewählt ist. Dies gibt an, wie viel Zeit diese Ressourcen für das Abschließen der Aufgabe verbringen sollen. Dies ist nur für Benutzer und Aufgabenrollen verfügbar.

   Oder

   Geben Sie für jede Ressource, die der Aufgabe zugewiesen ist, den Betrag von **Stunden** an, wenn für alle ausgewählten Aufgaben der Typ Einfach für die Dauer ausgewählt ist. Die Gesamtstundenzahl für alle Ressourcen sollte der Anzahl der geplanten Stunden für die Aufgabe entsprechen.

   >[!IMPORTANT]
   >
   >Sie können den Zuordnungsprozentsatz oder die Anzahl der Stunden pro Ressource nicht angeben, wenn die ausgewählten Aufgaben unterschiedliche Typen der Dauer oder die ausgewählten Aufgaben unterschiedliche Typen der Dauer aufweisen.

   Weitere Informationen zum Typ der Dauer für Aufgaben finden Sie unter [Übersicht über die Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Optional) Wählen Sie im Dropdown-Menü **Rolle auswählen** in der Spalte **Rolle des Empfängers** eine Rolle aus, die der Benutzer für die Aufgabe erfüllen soll, wenn Sie Aufgaben Benutzer zuweisen. Wenn Sie keine Rolle auswählen, wählt Workfront automatisch die Primäre Rolle des Benutzers aus.

1. (Optional) Wenn Sie vorhandene Bevollmächtigte aus allen Aufgaben entfernen möchten, führen Sie einen der folgenden Schritte aus:

   1. Beginnen Sie mit der Eingabe des Namens eines Benutzers, einer Rolle oder eines Teams, den/das Sie aus der Aufgabe entfernen möchten, wählen Sie ihn aus, wenn er in der Liste angezeigt wird, und klicken Sie auf **Zuweisung entfernen** , um weitere Verantwortliche zu entfernen.
   1. Klicken Sie auf **Alle vorhandenen Zuweisung entfernen** , um alle Bevollmächtigten aus allen ausgewählten Aufgaben zu entfernen.

1. Klicken Sie auf **Änderungen speichern**.
1. (Optional und bedingt) Wenn die Felder Zugeordnet oder Zuweisungen in Ihrer Aufgabenliste angezeigt werden, klicken Sie in eine dieser Spalten für eine Aufgabe und klicken Sie dann auf das Symbol **X** neben dem Namen eines Verantwortlichen, um sie aus der Aufgabe zu entfernen.

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


