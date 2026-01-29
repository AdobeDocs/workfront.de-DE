---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Aufgaben zuweisen
description: Sie können Benutzern, Rollen oder Teams Aufgaben zuweisen, um anzugeben, wer für die Durchführung der Aufgaben verantwortlich ist. Sie können eine Aufgabe mehreren Ressourcen gleichzeitig zuweisen.
author: Lisa
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: b1d5122dd66d84a0e2a21f24eeb01fd3298374ad
workflow-type: tm+mt
source-wordcount: '2479'
ht-degree: 2%

---

# Aufgaben zuweisen

<!--Audited: 10/2025-->

<!--remove production/ preview and old/ new experience references at prod-->

<div class="preview">

Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Dieselben Funktionen sind ab einer Woche ab der Vorschau-Version auch in der Produktionsumgebung für alle Kunden verfügbar.

Weitere Informationen finden Sie unter [Versionsübersicht für das zweite Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).

</div>

Sie können Benutzern, Aufgabengebieten oder Teams Aufgaben zuweisen, um anzugeben, wer für die Durchführung der Aufgaben verantwortlich ist. Sie können eine Aufgabe mehreren Ressourcen gleichzeitig zuweisen.

>[!TIP]
>
>Sie können mehrere Benutzer, Aufgabengebiete oder Teams zuweisen. Sie können nur aktive Benutzer, Aufgabengebiete und Teams zuweisen.
>
>Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team zugewiesen wurde, bevor sie/er deaktiviert wurden, bleiben sie/sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
>
>* Weisen Sie das Arbeitselement den aktiven Ressourcen neu zu.
>* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team zu.
>

Die Anzahl der Benutzer, die einer Aufgabe zugewiesen sind, und der Zeitplan des Aufgabenbesitzers können die geplanten Termine einer Aufgabe ändern, was zu einer Änderung der Zeitleiste des Projekts führt. Informationen zur Auswirkung der Zuweisung mehrerer Benutzer zu einer Aufgabe finden Sie unter [Übersicht über das Ändern von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Zusätzlich zu diesem Artikel empfehlen wir, die folgenden Artikel zu lesen, um weitere Informationen zum Zuweisen von Aufgaben zu erhalten:

* [Übersicht über das Ändern von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [Smart Assignments - Übersicht](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Smart-Zuweisungen vornehmen](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Erweiterte Zuweisungen erstellen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Ändern mehrerer Benutzerzuweisungen in einer Aufgabenliste](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Projektübersicht planen](../../../manage-work/projects/planning-a-project/plan-project.md)
* [Übersicht über das geplante Abschlussdatum der Aufgabe](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [Legen Sie das geplante Abschlussdatum des Projekts fest](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Übersicht über die Zuweisung von Arbeit im Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Work oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Anzeigen von oder höherem Zugriff auf Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td>
   <td>Tragen Sie zur Aufgabe bei oder erhöhen Sie die Berechtigungen.</td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zu mehreren Zuweisungen an Aufgabengebiete, Teams und Benutzer

Beachten Sie Folgendes, wenn Sie einem Arbeitselement mehrere Ressourcen zuweisen:

* Benutzern kann mehr als ein Aufgabengebiet mit ihrem Profil zugeordnet sein. Informationen zum Verknüpfen von Benutzern mit Aufgabengebieten finden Sie unter [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Wenn Sie einer Aufgabe oder einem Problem mehr als einen Benutzer zuweisen, wird der erste von Ihnen ausgewählte Benutzer automatisch als Eigentümer der Aufgabe oder des Problems bestimmt.
Anweisungen zum Ändern dieses Werts finden Sie in den Informationen zur Option Primär machen im Artikel [Erstellen erweiterter Zuweisungen](create-advanced-assignments.md).

* Ein Team kann kein Primärer Beauftragter für eine Aufgabe oder ein Problem sein. Nur ein(e) Benutzende(r) oder ein Aufgabengebiet kann als Primärer(r) für eine Aufgabe oder ein Problem bestimmt werden.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* Aufgaben und Probleme in einem Projekt können zunächst einem oder mehreren Teams oder Aufgabengebieten zugewiesen werden. Wenn das Projekt startbereit ist, müssen sie möglicherweise auch Benutzern zugewiesen werden:

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Teams</td>
   <td>Wenn Sie einem Team eine Aufgabe zuweisen und auch einen Benutzer zuweisen, bleibt die Aufgabe dem Team und dem Benutzer zugewiesen, auch wenn der Benutzer kein Mitglied des Teams ist.</td>
  </tr>
  <tr>
   <td>Aufgabengebiete</td>
   <td><p>Wenn Sie eine Aufgabe oder ein Problem einer oder mehreren Rollen zuweisen und dann auch einen Benutzer bzw. eine Benutzerin zuweisen, entscheidet gemäß den folgenden Regeln, welches Aufgabengebiet mit dem zusätzlichen Benutzer bzw. der zusätzlichen Benutzerin (falls vorhanden) verknüpft werden soll:</p>
     <ul>
      <li>Wenn nur ein Aufgabengebiet zugewiesen ist und es mit der primären Rolle des Benutzers (in seinem Profil konfiguriert) übereinstimmt, wird die Aufgabe oder das Problem nur diesem Benutzer zugewiesen.</li>
      <li>Wenn mehrere Rollen zugewiesen sind und mindestens eine davon mit einer der anderen Rollen des Benutzers übereinstimmt, wird die Aufgabe oder das Problem dem Benutzer zugewiesen (die Rolle wird nach dem Zufallsprinzip ausgewählt, wenn mehrere Übereinstimmungen vorliegen), zusammen mit allen zusätzlichen Rollen, die zugewiesen werden</li>
      <li>Wenn mindestens ein Aufgabengebiet zugewiesen ist und es keine Übereinstimmungen mit den Aufgabengebieten des Benutzers gibt, wird die Aufgabe oder das Problem sowohl der Rolle bzw. den Rollen als auch dem Benutzer zugewiesen.</li>
     </ul>
   <p>Informationen zur primären Rolle eines Benutzers und anderen Rollen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Bearbeiten des Benutzerprofils</a>.</p>
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

## Einzelne Aufgabe zuweisen

1. Wechseln Sie zu einer Aufgabe, die Sie zuweisen möchten.
1. Klicken Sie **Zuweisen zu** im Feld **Zuweisungen** in der Kopfzeile der Aufgabe

   ODER

   Klicken Sie auf den Namen der Zuweisungen, wenn die Aufgabe bereits zugewiesen ist.

   ![Arbeitsaufträge](assets/assignments-from-task-header-0825.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Beginnen Sie mit der Eingabe des Namens eines Benutzers, eines Aufgabengebiets oder Teams, den/das Sie zuweisen möchten, und klicken Sie dann darauf, wenn es in der Liste angezeigt wird.

     >[!TIP]
     >
     >Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.
     >
     >Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Benutzerzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   * (Bedingt) Klicken Sie auf einen der Namen in den Listen **Benutzer und Teams** oder **Aufgabengebiete**, wenn sie angezeigt werden. Weitere Informationen finden Sie unter [Smart Assignments - Übersicht](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     Sie können den Namen eines Benutzers, Teams oder Aufgabengebiets eingeben, das der Aufgabe zugewiesen werden soll, und ihn dann auswählen, wenn er in der Liste angezeigt wird.

   * Klicken Sie auf **Erweitert**.

     Informationen zum Erstellen erweiterter Zuweisungen finden Sie unter [Erstellen erweiterter Zuweisungen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Klicken Sie auf **Speichern**.
1. (Optional und bedingt) Klicken Sie auf das Symbol **X** neben dem Namen der Zuweisung im rechten Bedienfeld der Aufgabe, um eine Zuweisung zu entfernen, wenn Sie auf **Erweitert** geklickt haben.

## Aufgabe in einer Liste zuweisen, wenn sie inline bearbeitet wird

Sie können Aufgaben in einer Liste oder einem Bericht zuweisen, wenn eines der Zuweisungsfelder in der Listenansicht sichtbar ist. Dies ist eine schnellere Möglichkeit, Aufgaben zuzuweisen. In diesem Artikel wird beschrieben, wie Sie Zuweisungen für eine Aufgabe in einer Liste ändern. Informationen zum Ändern mehrerer Zuweisungen für mehrere Aufgaben in einer Liste finden Sie unter [Ändern mehrerer Benutzerzuweisungen in einer Aufgabenliste](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Je nachdem, welches Feld in der Ansicht sichtbar ist, können Sie der Aufgabe die folgenden Entitäten zuweisen:

| Feld | Zugewiesene Einheiten |
|---|---|
| **Zuweisen zu** | Einen Benutzer zuweisen |
| **Zugewiesen** | Einen Benutzer zuweisen |
| **Arbeitsaufträge** | Zuweisen von Benutzern, Aufgabengebieten oder Teams |

So weisen Sie Aufgaben in einer Liste zu:

1. Navigieren Sie zu einer Liste von Aufgaben, die die Felder Zugewiesen an, Zugewiesen oder Zuweisungen in der Ansicht enthält.
1. (Optional) Klicken Sie auf **Dropdown-Menü** Automatisches Speichern“ und wählen Sie aus den folgenden Optionen:

   | Option | Beschreibung der Optionen |
   |---|---|
   | Automatisch speichern | Änderungen an den Aufgaben werden automatisch gespeichert und können nicht rückgängig gemacht werden |
   | Manuell speichern | Sie müssen Ihre Änderungen manuell speichern. Sie können Ihre Änderungen vor dem Speichern rückgängig machen. |
   | Timeline-Planung | Sie müssen Ihre Änderungen manuell speichern. Sie können Ihre Änderungen vor dem Speichern rückgängig machen. Das Speichern Ihrer Änderungen und aller Projektabhängigkeiten ist schneller als bei der Auswahl von „Manuelles Speichern“. |

   Weitere Informationen zum Speichern von Aufgaben während der Bearbeitung in einer Liste finden Sie unter [Bearbeiten von Aufgaben in einer Liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. Führen Sie einen der folgenden Schritte aus, um Aufgaben zuzuweisen:

   * Klicken Sie in die Felder **Zugewiesen an** oder **Zugewiesen** und geben Sie den Namen eines aktiven Benutzers ein, den Sie der Aufgabe zuweisen möchten. Klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.
   * Klicken Sie in das **Arbeitsaufträge** und geben Sie den Namen eines aktiven Benutzers, eines Aufgabengebiets oder Teams ein, den/das Sie der Aufgabe zuweisen möchten. Klicken Sie dann auf den Namen, wenn er/sie in der Liste angezeigt wird.

     >[!TIP]
     >
     >Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.
     >
     >Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)

     <!--<span class="preview">When adding a job role assignment, you can search for the job role or location. Select a Job role to use the default billing rate for the assignment, or select a Rate Card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. (Bedingt) Klicken Sie im Feld Arbeitsaufträge **Erweitert** am unteren Rand der Liste oder auf das **Personen-Symbol** ![Personen-Symbol](assets/teams.png) in der oberen rechten Ecke des Arbeitsauftragsfelds, um das Feld **Erweiterte Arbeitsaufträge** zu öffnen und erweiterte Arbeitsaufträge zu erstellen.

   Weitere Informationen finden Sie unter [Erstellen erweiterter Zuweisungen](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Erweiterte Zuweisungen können nicht über die Felder Zugewiesen an oder Zugewiesen an vorgenommen werden.

1. Nachdem Sie Ihre Beauftragten zur Aufgabe hinzugefügt haben, drücken Sie die Eingabetaste oder klicken Sie auf eine beliebige Stelle auf der Seite, um Ihre Änderungen zu speichern, wenn Sie „Automatisch speichern“ ausgewählt haben. Klicken Sie andernfalls auf **Speichern**.

## Massenweise Zuweisung mehrerer Aufgaben aus einer Liste

Die Massenzuweisung mehrerer Aufgaben aus einer Liste unterscheidet sich je nach ausgewählter Umgebung.

### Massenweise Zuweisung mehrerer Aufgaben aus einer Liste in der Produktionsumgebung

1. Navigieren Sie zu einer Liste von Aufgaben, die Sie stapelweise zuweisen möchten.
1. (Bedingt) Stellen Sie sicher, dass die Option **Automatisches Speichern** ausgewählt ist, wenn Sie sich in einer Liste von Aufgaben unter einem Projekt befinden.

   >[!IMPORTANT]
   >
   >Beim manuellen Speichern von Aufgaben für ein Projekt können Sie keine Aufgaben stapelweise bearbeiten.

1. Mehrere Aufgaben in der Aufgabenliste auswählen.
1. Klicken Sie auf **Bearbeiten**.

   Das **Aufgaben bearbeiten** wird in der neuen -Version geöffnet.

1. Weisen Sie weitere Aufgaben mithilfe der neuen -Version zu.

   Weitere Informationen finden Sie im Abschnitt [Massenzuweisung mehrerer Aufgaben aus einer Liste in der neuen -](#assign-multiple-tasks-in-bulk-from-a-list-in-the-new-experience) in diesem Artikel.

1. (Optional) Klicken Sie **Zurück zum alten Erlebnis wechseln** unten im Feld **Aufgaben bearbeiten**, um das alte Erlebnis zu öffnen.

1. (Bedingt) Wählen Sie unter Verwendung des alten Erlebnisses im Bereich **Arbeitsaufträge** das Feld **Verantwortlicher** aus und geben Sie dann den Namen eines Benutzers, eines Aufgabengebiets oder Teams ein, den/das Sie allen Aufgaben zuweisen möchten.

   >[!IMPORTANT]
   >
   >Wenn eine der Aufgaben bereits zugewiesen ist, werden die hier angegebenen Ressourcen zu den Vorgängen hinzugefügt, anstatt die vorhandenen Ressourcen in den Vorgängen zu ersetzen.

1. (Optional) Wählen Sie das Optionsfeld in der Spalte **Aufgabenbesitzer** aus, um anzugeben, welche Ressource der primäre Zugewiesene oder der Eigentümer der Aufgabe ist, wenn Sie der Aufgabe mehr als eine Ressource zuweisen. Dies ist nicht für Teams verfügbar.
1. (Bedingt) Geben Sie **Zuordnung %** für jede Ressource an, die dem Vorgang zugewiesen ist, wenn alle ausgewählten Vorgänge den Dauertyp „Leistungsgesteuert“ oder „Berechnete Zuordnung“ aufweisen. Dies gibt an, wie viel Zeit diese Ressourcen für die Durchführung der Aufgabe aufwenden sollten. Dies ist nur für Benutzer und Aufgabengebiete verfügbar.

   ODER

   Geben Sie den **(Stunden** für jede Ressource an, die dem Vorgang zugewiesen ist, wenn alle ausgewählten Vorgänge den Dauertyp „Einfach“ aufweisen. Die Summe aller Stunden für alle Ressourcen sollte der Anzahl der geplanten Stunden für die Aufgabe entsprechen.

   >[!IMPORTANT]
   >
   >Sie können den Zuordnungsprozentsatz oder die Anzahl der Stunden pro Ressource nicht angeben, wenn die ausgewählten Vorgänge unterschiedliche Dauertypen haben oder wenn die ausgewählten Vorgänge unterschiedliche Dauertypen haben.

   Informationen zum Dauertyp für Aufgaben finden Sie unter [Übersicht über die Aufgabendauer und den &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)&quot;

1. (Optional) Wählen Sie aus dem Dropdown-Menü **Rolle auswählen** in der Spalte „Rolle des **&quot; eine Rolle aus, die der Benutzer bei der Aufgabe erfüllen soll** wenn Sie Benutzer Aufgaben zuweisen. Wenn Sie keine Rolle auswählen, wählt Workfront automatisch die Primäre Rolle des Benutzers aus.

1. (Optional) Wenn Sie vorhandene Zugewiesene aus allen Aufgaben entfernen möchten, führen Sie einen der folgenden Schritte aus:

   1. Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein, den/das Sie aus der Aufgabe entfernen möchten, wählen Sie ihn/sie aus, wenn er/sie in der Liste angezeigt wird, und klicken Sie auf **Verantwortlichen entfernen** um weitere Verantwortliche zu entfernen.
   1. Klicken Sie **Alle vorhandenen Zugewiesenen entfernen**, um alle Zugewiesenen aus allen ausgewählten Aufgaben zu entfernen.

1. Klicken Sie auf **Änderungen speichern**.
1. (Optional und bedingt) Wenn die Felder Zugewiesen an oder Zuweisungen in Ihrer Aufgabenliste angezeigt werden, klicken Sie in eine dieser Spalten für eine Aufgabe und dann auf das Symbol **X** neben dem Namen eines Verantwortlichen, um sie aus der Aufgabe zu entfernen.


### Massenzuweisung mehrerer Aufgaben aus einer Liste in der neuen -Version

1. Navigieren Sie zu einer Liste von Aufgaben, die Sie stapelweise zuweisen möchten.
1. (Bedingt) Stellen Sie sicher, dass die Option **Automatisches Speichern** ausgewählt ist, wenn Sie sich in einer Liste von Aufgaben unter einem Projekt befinden.

   >[!IMPORTANT]
   >
   >Beim manuellen Speichern von Aufgaben für ein Projekt können Sie keine Aufgaben stapelweise bearbeiten.

1. Mehrere Aufgaben in der Aufgabenliste auswählen.
1. Klicken Sie auf **Bearbeiten**.

   Das **Aufgaben bearbeiten** wird geöffnet.

1. Beginnen Sie im Bereich **Arbeitsaufträge** mit der Eingabe des Namens der Benutzer, Teams oder Rollen in das bereitgestellte Feld **Personen, Rollen oder Teams suchen** und klicken Sie dann auf sie, wenn sie in der Liste angezeigt werden

   ODER

   Klicken Sie auf **Mir zuweisen**, um es sich selbst zuzuweisen.

   >[!IMPORTANT]
   >
   >Wenn eine der Aufgaben bereits zugewiesen ist, werden die hier angegebenen Ressourcen zu den Vorgängen hinzugefügt, anstatt die vorhandenen Ressourcen in den Vorgängen zu ersetzen.

1. Klicken Sie in das **Dauertyp** und wählen Sie einen Dauertyp aus.

   Informationen zum Dauertyp für Aufgaben finden Sie unter [Übersicht über die Aufgabendauer und den &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)&quot;

1. (Bedingt) Aktualisieren Sie je nach **von** ausgewählten „Dauertyp“ die folgenden Felder:

   * Dauer
   * Geplante Stunden

     Weitere Informationen finden Sie unter [Aufgaben bearbeiten](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Optional) Wenn Sie vorhandene Verantwortliche aus allen Aufgaben entfernen möchten, klicken Sie auf das **x** neben ihrem Namen im Feld **Personen, Rollen oder Teams suchen**.

1. Klicken Sie auf **Speichern**.
1. (Optional und bedingt) Wenn die Felder **Zugewiesen an** oder **Zuweisungen** in Ihrer Aufgabenliste angezeigt werden, klicken Sie in eine dieser Spalten für eine Aufgabe und dann auf das **X-Symbol** neben dem Namen eines Verantwortlichen, um sie aus der Aufgabe zu entfernen.

<div class="preview">

### Massenweise Zuweisung mehrerer Aufgaben aus einer Liste in der Vorschau-Umgebung

1. Navigieren Sie zu einer Liste von Aufgaben, die Sie stapelweise zuweisen möchten.
1. (Bedingt) Stellen Sie sicher, dass die Option **Automatisches Speichern** ausgewählt ist, wenn Sie sich in einer Liste von Aufgaben unter einem Projekt befinden.

   >[!IMPORTANT]
   >
   >Beim manuellen Speichern von Aufgaben für ein Projekt können Sie keine Aufgaben stapelweise bearbeiten.

1. Mehrere Aufgaben in der Aufgabenliste auswählen.
1. Klicken Sie auf **Bearbeiten**.

   Das **Aufgaben bearbeiten** wird geöffnet.

1. Beginnen Sie im Bereich **Arbeitsaufträge** mit der Eingabe des Namens der Benutzer, Teams oder Rollen in das bereitgestellte Feld **Personen, Rollen oder Teams suchen** und klicken Sie dann auf sie, wenn sie in der Liste angezeigt werden

   >[!IMPORTANT]
   >
   >Wenn eine der Aufgaben bereits zugewiesen ist, werden die hier angegebenen Ressourcen zu den Vorgängen hinzugefügt, anstatt die vorhandenen Ressourcen in den Vorgängen zu ersetzen.

1. Geben Sie die folgenden Felder für die ausgewählten Aufgaben an:

   * Bewegen Sie den Mauszeiger über den Zuweisungsnamen und klicken Sie dann auf **Primär machen**, um anzugeben, welcher Verantwortliche der Eigentümer der Aufgabe ist.
   * **Dauertyp**

     Informationen zum Dauertyp für Aufgaben finden Sie unter [Übersicht über die Aufgabendauer und den &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)&quot;

   * **Dauer**
   * **Geplante Stunden**

     Weitere Informationen finden Sie unter [Aufgaben bearbeiten](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Optional) Wenn Sie vorhandene Verantwortliche aus allen Aufgaben entfernen möchten, klicken Sie auf das **x** neben ihrem Namen im Feld **Personen, Rollen oder Teams suchen**.

1. Klicken Sie auf **Speichern**.
1. (Optional und bedingt) Wenn die Felder **Zugewiesen an** oder **Zuweisungen** in Ihrer Aufgabenliste angezeigt werden, klicken Sie in eine dieser Spalten für eine Aufgabe und dann auf das **X-Symbol** neben dem Namen eines Verantwortlichen, um sie aus der Aufgabe zu entfernen.

</div>

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


