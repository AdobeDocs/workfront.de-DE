---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern
description: Bei der Verwaltung von Aufgabenzuweisungen können Sie sie gleichzeitig für mehrere Aufgaben ändern, indem Sie die Massenbearbeitung in einer Aufgabenliste verwenden.
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 7b0da61c301fe8f1f24aa27a469952fbd46987c5
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern

<!--Audited: 07/2024-->

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Bei der Verwaltung von Aufgabenzuweisungen können Sie sie gleichzeitig für mehrere Aufgaben ändern, indem Sie die Massenbearbeitung in einer Aufgabenliste verwenden.

Dieser Artikel bezieht sich auf das Ändern mehrerer Benutzerzuweisungen für mehrere Aufgaben in einer Aufgabenliste. Lesen Sie auch die folgenden Artikel zum Ändern von Zuweisungen für mehrere Aufgaben in anderen Bereichen:

* Informationen zum Zuweisen von Aufgaben mithilfe des Lastenausgleichs finden Sie unter [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Informationen zum Zuweisen einer Aufgabe zu einer Ressource in einer Liste finden Sie unter [Aufgaben zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Zugriffsanforderungen

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
   <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Benutzer</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute oder höhere Berechtigungen für Aufgaben</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Ändern von Zuweisungen für mehrere Aufgaben

1. Markieren Sie die Liste mit den Aufgaben, für die Sie Zuweisungen ändern möchten.
1. (Optional) Erstellen Sie einen Filter, um nur die Aufgaben anzuzeigen, die dem Empfänger zugewiesen sind, den Sie ändern möchten.

   Wenn Ihr Projekt beispielsweise eine bestimmte Rolle als Standardverantwortlicher für mehrere Aufgaben enthält, können Sie einen Filter erstellen, um nur Aufgaben mit dieser Rolle als Verantwortlicher anzuzeigen. Anschließend können Sie die Rolle durch einen bestimmten Benutzer ersetzen.

   Informationen zum Erstellen eines Filters finden Sie unter [Filter erstellen oder bearbeiten](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Um nach einer Rolle zu filtern, wählen Sie **Zuweisungsrollen** und klicken Sie dann auf **ID**.

   >[!TIP]
   >
   >Verwenden Sie nicht das Feld **Zugeordnet zu** . Dadurch wird nur der Primäre Eigentümer der Aufgabe anstelle der Rollen gefunden, die ihm zugewiesen werden könnten.

   Oder

   Um nach einem Benutzer zu filtern, wählen Sie **Zuweisungsbenutzer** und klicken Sie dann auf **ID**.

   >[!TIP]
   >
   >Verwenden Sie nicht das Feld **Zugeordnet zu** . Dadurch wird nur der Primäre Eigentümer der Aufgabe anstelle der Benutzer gefunden, die ihnen zugewiesen werden könnten.

1. Wählen Sie die Aufgaben aus, für die Sie Zuweisungen ändern möchten, und klicken Sie dann auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

   Die Seite &quot;Aufgaben bearbeiten&quot;wird angezeigt. Die von Ihnen bearbeiteten Elemente werden in der oberen linken Ecke der Seite angezeigt.

1. Wechseln Sie zum Abschnitt **Zuweisungen** .
1. Führen Sie einen der folgenden Schritte aus, um Bevollmächtigte hinzuzufügen oder zu entfernen:

   >[!IMPORTANT]
   >
   >Das Entfernen von Zuweisungen kann sich auf die Aufgabenzeiten und Zuordnungsprozentsätze auswirken. Weitere Informationen finden Sie im Abschnitt [Wie sich das Entfernen von Bevollmächtigten auf die Aufgabenzeiten und Zuordnungsprozentsätze auswirkt](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in diesem Artikel.

   * So fügen Sie einen neuen Bevollmächtigten hinzu:

      1. Wählen Sie im Abschnitt **Zuweisungen** die Option **Bevollmächtigter** aus.

         Informationen, die für alle ausgewählten Aufgaben gelten, werden angezeigt. Wenn beispielsweise derselbe Benutzer allen Aufgaben zugewiesen ist, wird dieser Benutzer in der Spalte **Zuweisung** angezeigt. Wenn Informationen nicht für alle ausgewählten Aufgaben gelten, werden keine Informationen angezeigt.

      1. Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Die Zuweisung wird hinzugefügt und ersetzt nicht die aktuellen Zuweisungen für die ausgewählten Aufgaben.


     >[!TIP]
     >
     > * Sie können mehrere Benutzer, Auftragsrollen oder Teams zuweisen. Sie können nur aktive Benutzer, Stellenrollen und Teams zuweisen.
     >   
     > * Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können. Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Wenn ein Benutzer, eine Rolle oder ein Team zugewiesen wurde, bevor sie deaktiviert wurden, bleiben sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
     >   
     >     * Weisen Sie das Arbeitselement aktiven Ressourcen erneut zu.
     >     * Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team erneut zu.


   * So entfernen Sie einzelne Bevollmächtigte:

      1. Klicken Sie auf das Symbol **X** neben dem Namen des Empfängers, den Sie entfernen möchten, wenn der Verantwortliche in der Liste Zuweisungen angezeigt wird.

         Oder

         (Bedingt) Wenn der zu entfernende Bevollmächtigte nicht im Abschnitt &quot;Zuweisungen&quot;angezeigt wird, da der Bevollmächtigte nur bestimmten von Ihnen ausgewählten Aufgaben zugewiesen ist, klicken Sie auf **Bevollmächtigten entfernen** und beginnen Sie mit der Eingabe des Namens des Bevollmächtigten, den Sie entfernen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.

   * So entfernen Sie alle vorhandenen Bevollmächtigten:

      1. Klicken Sie auf **Alle vorhandenen Zuweisungen entfernen** und dann auf **Ja, alle Zuweisungen löschen**.

         Dadurch werden nicht nur häufig verwendete Bevollmächtigte (Bevollmächtigte, die im Dialogfeld &quot;Bearbeiten&quot;angezeigt werden), sondern auch alle Bevollmächtigten für alle ausgewählten Aufgaben entfernt.

     Das Entfernen von Benutzern aus Aufgaben kann sich auf die Aufgabenzeiten und Zuordnungsprozentsätze auswirken.

     Weitere Informationen finden Sie unter [Übersicht über das Ändern von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Optional) Ändern Sie eine der folgenden Optionen für Bevollmächtigte:

   * (Bedingt) **Zuordnung % oder Stunden**: Geben Sie einen neuen Zuordnungsprozentsatz oder neue Zuordnungsstunden an.

     >[!NOTE]
     >
     >Diese Option kann nur geändert werden, wenn der Dauer-Typ für alle in Bearbeitung befindlichen Aufgaben identisch ist. Wenn der Typ Dauer berechnet wird, können Sie den Zuordnungsprozentsatz aktualisieren. Wenn der Typ Dauer einfach ist, können Sie die Stunden aktualisieren. Weitere Informationen zum Dauer-Typ finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     >Wenn das Feld leer ist, bedeutet dies, dass der Wert von Aufgabe zu Aufgabe unterschiedlich ist. Sie können ihn jedoch trotzdem ändern.

   * **Aufgabenbesitzer**: Wählen Sie diese Option, um den Verantwortlichen für alle in Bearbeitung befindlichen Aufgaben zum Eigentümer der Aufgabe zu machen.
   * **Rolle des Bevollmächtigten**: Wählen Sie eine Rolle aus der Dropdownliste aus. Wenn die Option nicht ausgewählt ist, wählt Adobe Workfront automatisch die Primäre Rolle des Benutzers aus.

1. Klicken Sie auf **Änderungen speichern.**
