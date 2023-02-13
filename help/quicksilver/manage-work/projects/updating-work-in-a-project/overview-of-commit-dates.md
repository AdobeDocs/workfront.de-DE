---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Datum bestätigen - Übersicht
description: Das Datum der Veröffentlichung ist das Datum, bis zu dem ein Benutzer, der einer Aufgabe zugewiesen ist, oder ein Problem verpflichtet, die Aufgabe oder das Problem abzuschließen. Dies unterscheidet sich vom geplanten Abschlussdatum, da es eine realistischere Schätzung des Abschlussdatums darstellt, das nur vom für die Arbeit verantwortlichen Benutzer angegeben wird. Informationen zum geplanten Abschlussdatum finden Sie unter Übersicht über die geplante Aufgabe mit dem geplanten Abschlussdatum.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Datum bestätigen - Übersicht

Das Datum der Veröffentlichung ist das Datum, bis zu dem ein Benutzer, der einer Aufgabe zugewiesen ist, oder ein Problem verpflichtet, die Aufgabe oder das Problem abzuschließen. Dies unterscheidet sich vom geplanten Abschlussdatum, da es eine realistischere Schätzung des Abschlussdatums darstellt, das nur vom für die Arbeit verantwortlichen Benutzer angegeben wird. Weitere Informationen zum geplanten Abschlussdatum finden Sie unter [Übersicht über die geplante Aufgabe - Abschlussdatum](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Datum bestätigen - Übersicht

Beachten Sie beim Arbeiten mit Commit-Daten Folgendes:

* Nur Aufgaben und Probleme haben ein &quot;Commit Date&quot;.
* Commit-Daten werden von Adobe Workfront nicht automatisch festgelegt.\
   Wenn Sie eine Aufgabe oder ein Problem erstellen, wird der Aufgabe oder dem Problem kein Commit-Datum zugewiesen.
* Wenn Sie einer Aufgabe oder einem Problem zugewiesen sind, können Sie das Veröffentlichungsdatum wie folgt festlegen:

   * Lassen Sie Workfront das Datum für die Übermittlung so festlegen, dass es dem bereits geplanten Abschlussdatum der Aufgabe oder des Problems entspricht, indem Sie auf &quot;Bearbeiten&quot;, &quot;Problem starten&quot;oder &quot;Aufgabe starten&quot;für die Aufgabe oder das Problem klicken. Weitere Informationen zum Ersetzen der Schaltfläche &quot;Work On It&quot;durch eine Schaltfläche &quot;Start&quot;finden Sie unter  [Ersetzen der Schaltfläche &quot;Work On It&quot;durch die Schaltfläche Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Legen Sie das Datum für die Übermittlung manuell fest, abhängig davon, wann Sie glauben, dass die Aufgabe oder das Problem möglicherweise abgeschlossen ist. Dies ist Ihre Schätzung und Zusage als Verantwortlicher für den Projektmanager, dass die Aufgabe oder das Problem bis zu einem bestimmten Datum abgeschlossen sein wird.

>[!NOTE]
>
>Sie müssen der Aufgabenbesitzer einer Aufgabe sein, um das Veröffentlichungsdatum zu ändern. Die folgenden Benutzer können das &quot;Commit Date&quot;einer Aufgabe nicht ändern:
>
>* Projektbesitzer
>* Projektsponsor
>* Ressourcenmanager
>* Systemadministrator
>* Jeder andere Verantwortliche für die Aufgabe
>* Jeder andere Benutzer mit Berechtigungen für die Aufgabe.
>
>Weitere Informationen zum Aufgabeneigentümer finden Sie im Abschnitt [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Durch Änderung des Zusagedatums ausgelöste Benachrichtigungen und Aktualisierungen {#notifications-and-updates-triggered-by-changing-the-commit-date}

Wenn eine Aufgabe oder ein Problemverantwortlicher ein Komprimierungsdatum auswählt, das sich vom geplanten Abschlussdatum unterscheidet, das vom Projekteigentümer festgelegt wurde, gibt es eine Reihe von Benachrichtigungen und Aktualisierungen, die den Projekteigentümer und andere Benutzer auf diese Änderung hinweisen.

>[!NOTE]
>
>Änderungen am Datum der Übermittlung ändern nicht automatisch die geplanten Daten, und Änderungen an den geplanten Daten ändern nicht automatisch das Datum der Veröffentlichung. 

Durch das Festlegen des Veröffentlichungsdatums für eine Aufgabe oder ein Problem werden die folgenden Trigger :

* Das Datum der Veröffentlichung wird im Aktualisierungsstream der Aufgabe oder des Problems angegeben.

   ![](assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png)

   Die Änderung des Veröffentlichungsdatums wird im Bereich Updates der Aufgabe bzw. des Problems angezeigt, wenn der Workfront-Administrator diese Aktualisierung im Bereich Updates-Feeds unter Einrichtung aktiviert. Weitere Informationen finden Sie unter [Vom System verfolgte Aktualisierungen](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* Das geplante Abschlussdatum der Aufgabe oder des Problems ist auf das gleiche Datum festgelegt, da die Aufgabe jetzt genauer angibt, wann sie wahrscheinlich abgeschlossen sein wird.

   Weitere Informationen zum geplanten Abschlussdatum finden Sie unter [Übersicht über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

   ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* Der Projekteigentümer wird im Benachrichtigungsbereich und im Tab Updates der Aufgabe darüber benachrichtigt, ob diese Änderung sich auf die Projektzeitleiste auswirkt.

   ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

   >[!TIP]
   Die Benachrichtigung, dass das Veröffentlichungsdatum geändert wurde, wird nur dann an den Projekteigentümer gesendet, wenn der Workfront-Administrator die Anzeige des Bestätigungsdatums im Bereich &quot;Aktualisierungen-Feeds&quot;im Setup-Bereich aktiviert. Weitere Informationen finden Sie unter [Vom System verfolgte Aktualisierungen](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

   Wenn ein Projekteigentümer die Änderung nicht akzeptieren möchte, empfehlen wir ihm, dem Benutzer, der ein neues Datum vorschlägt, einen Kommentar abzugeben, um ihn aufzufordern, das Veröffentlichungsdatum zurück zum ursprünglichen geplanten Datum zu ändern, oder ein neues Datum auszuwählen. Wenn ein Projekteigentümer die Änderung akzeptiert, kann er das geplante Abschlussdatum manuell so anpassen, dass es mit dem vom dem Artikel zugewiesenen Benutzer angebotenen Zustimmungsdatum übereinstimmt.

   Der Projekteigentümer kann das Datum des Versands verwenden, um das geplante Abschlussdatum zurückzusetzen. Wählen Sie dazu im Tab Aktualisierungen der Aufgabe die Option Geplantes Datum einstellen auf aus. Sie müssen Zugriff haben, um die Aufgabe und das Projekt zu verwalten und diese Änderung zu akzeptieren.

   >[!NOTE]
   Wenn Sie sehen möchten, wie sich die Timeline des Projekts auswirkt, indem Sie das geplante Abschlussdatum der Aufgabe ändern, klicken Sie auf **Projekt-Timeline**. Dadurch wird das Gantt-Diagramm geöffnet, in dem Sie die Datumsänderungen bewerten können.
   ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >

Informationen zu den zusätzlichen Funktionen, die beim Aktualisieren eines Arbeitselements verfügbar sind, finden Sie unter  [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

Informationen zum Aktualisieren der Zusagedaten für Aufgaben und Probleme finden Sie unter [Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE:&nbsp;moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On&nbsp;It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click&nbsp;<strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
