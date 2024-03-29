---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern
description: Bei der Verwaltung von Aufgabenzuweisungen können Sie sie gleichzeitig für mehrere Aufgaben ändern, indem Sie die Massenbearbeitung in einer Aufgabenliste verwenden.
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

Bei der Verwaltung von Aufgabenzuweisungen können Sie sie gleichzeitig für mehrere Aufgaben ändern, indem Sie die Massenbearbeitung in einer Aufgabenliste verwenden.

Dieser Artikel bezieht sich auf das Ändern mehrerer Benutzerzuweisungen für mehrere Aufgaben in einer Aufgabenliste. Lesen Sie auch die folgenden Artikel zum Ändern von Zuweisungen für mehrere Aufgaben in anderen Bereichen:

* Informationen zum Zuweisen von Aufgaben mithilfe des Lastenausgleichs finden Sie unter [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Informationen zum Zuweisen einer Aufgabe zu einer Ressource in einer Liste finden Sie unter [Aufgaben zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

## Zugriffsanforderungen

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
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Benutzer</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen oder höhere Berechtigungen zu Aufgaben</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
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
1. (Optional) Erstellen Sie einen Filter, um nur die dem Empfänger zugewiesenen Aufgaben anzuzeigen, die Sie ändern möchten.

   Wenn Ihr Projekt beispielsweise eine bestimmte Rolle als Standardverantwortlicher für mehrere Aufgaben enthält, können Sie einen Filter erstellen, um nur Aufgaben mit dieser Rolle als Verantwortlicher anzuzeigen. Anschließend können Sie die Rolle durch einen bestimmten Benutzer ersetzen.

   Informationen zum Erstellen eines Filters finden Sie unter [Filter erstellen oder bearbeiten](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. Um nach einer Rolle zu filtern, wählen Sie **Zuweisungsrollen** Klicken Sie auf **ID**.

   >[!TIP]
   >
   >Verwenden Sie nicht das **Zugeordnet zu** -Feld. Dadurch wird nur der Primäre Eigentümer der Aufgabe anstelle der Rollen gefunden, die ihm zugewiesen werden könnten.

   Oder

   Um nach einem Benutzer zu filtern, wählen Sie **Zuweisung von Benutzern,** Klicken Sie dann auf **Kennung.**

   >[!TIP]
   >
   >Verwenden Sie nicht das **Zugeordnet zu** -Feld. Dadurch wird nur der Primäre Eigentümer der Aufgabe anstelle der Benutzer gefunden, die ihnen zugewiesen werden könnten.

1. Wählen Sie die Aufgaben aus, für die Sie Zuweisungen ändern möchten, und klicken Sie dann auf die **Bearbeiten** icon ![](assets/edit-icon.png).

   Die Seite &quot;Aufgaben bearbeiten&quot;wird angezeigt. Die von Ihnen bearbeiteten Elemente werden in der oberen linken Ecke der Seite angezeigt.

1. Navigieren Sie zu **Zuweisungen** Abschnitt.
1. Führen Sie einen der folgenden Schritte aus, um Bevollmächtigte hinzuzufügen oder zu entfernen:

   >[!IMPORTANT]
   >
   >Das Entfernen von Zuweisungen kann sich auf die Aufgabenzeiten und Zuordnungsprozentsätze auswirken. Weitere Informationen finden Sie im Abschnitt . [Wie sich das Entfernen von Bevollmächtigten auf die Aufgabenzeiten und Zuordnungsprozentsätze auswirkt](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in diesem Artikel.

   * So fügen Sie einen neuen Bevollmächtigten hinzu:

      1. Im **Zuweisungen** Bereich, wählen Sie **Bevollmächtigter**.

         Informationen, die für alle ausgewählten Aufgaben gelten, werden angezeigt. Wenn beispielsweise derselbe Benutzer allen Aufgaben zugewiesen ist, wird dieser Benutzer im **Bevollmächtigter** Spalte. Wenn Informationen nicht für alle ausgewählten Aufgaben gelten, werden keine Informationen angezeigt.

      1. Geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Die Zuweisung wird hinzugefügt und ersetzt nicht die aktuellen Zuweisungen für die ausgewählten Aufgaben.


     >[!TIP]
     >
     > * Sie können mehrere Benutzer, Auftragsrollen oder Teams zuweisen. Sie können nur aktive Benutzer, Stellenrollen und Teams zuweisen.
     >   
     > * Beachten Sie beim Hinzufügen einer Benutzerzuweisung den Avatar, die Primäre Rolle des Benutzers oder seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können. Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   Wenn ein Benutzer, eine Rolle oder ein Team zugewiesen wurde, bevor sie deaktiviert wurden, bleiben sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
     >   
     >     * Weisen Sie das Arbeitselement aktiven Ressourcen erneut zu.
     >     * Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team erneut zu.


   * So entfernen Sie einzelne Bevollmächtigte:

      1. Klicken Sie auf **X-Symbol** neben dem Namen des Bevollmächtigten, den Sie entfernen möchten, wenn der Bevollmächtigte in der Liste &quot;Zuweisungen&quot;angezeigt wird.

         Oder

         (Bedingt) Wenn der zu entfernende Bevollmächtigte nicht im Abschnitt Zuweisungen angezeigt wird, da der Bevollmächtigte nur einigen der von Ihnen ausgewählten Aufgaben zugewiesen ist, klicken Sie auf **Zuweisung entfernen** Geben Sie den Namen des Empfängers ein, den Sie entfernen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   * So entfernen Sie alle vorhandenen Bevollmächtigten:

      1. Klicken **Alle vorhandenen Zuweisung entfernen** Klicken Sie auf **Ja, alle Zuweisung löschen**.

         Dadurch werden nicht nur häufig verwendete Bevollmächtigte (Bevollmächtigte, die im Dialogfeld &quot;Bearbeiten&quot;angezeigt werden), sondern auch alle Bevollmächtigten für alle ausgewählten Aufgaben entfernt.

     Das Entfernen von Benutzern aus Aufgaben kann sich auf die Aufgabenzeiten und Zuordnungsprozentsätze auswirken.

     Weitere Informationen finden Sie unter [Übersicht über das Ändern von Aufgabenzuweisungen](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. (Optional) Ändern Sie eine der folgenden Optionen für Bevollmächtigte:

   * (Bedingt) **Zuteilung in % oder Stunden**: Geben Sie einen neuen Zuordnungsprozentwert oder neue Stunden an.

     >[!NOTE]
     >
     >Diese Option kann nur geändert werden, wenn der Dauer-Typ für alle in Bearbeitung befindlichen Aufgaben identisch ist. Wenn der Typ Dauer berechnet wird, können Sie den Zuordnungsprozentsatz aktualisieren. Wenn der Typ Dauer einfach ist, können Sie die Stunden aktualisieren. Weitere Informationen zum Typ der Dauer finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     Wenn das Feld leer ist, bedeutet dies, dass sich der Wert von Aufgabe zu Aufgabe unterscheidet. Sie können sie jedoch noch ändern.

   * **Aufgabeneigentümer**: Wählen Sie diese Option aus, um den Verantwortlichen für alle in Bearbeitung befindlichen Aufgaben zum Eigentümer der Aufgabe zu machen.
   * **Rolle des Bevollmächtigten**: Wählen Sie eine Rolle aus der Dropdownliste aus. Wenn die Option nicht ausgewählt ist, wählt Adobe Workfront automatisch die Primäre Rolle des Benutzers aus.

1. Klicken **Speichern Sie die Änderungen.**
