---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Datum bestätigen - Übersicht
description: Das Datum der Veröffentlichung ist das Datum, bis zu dem ein Benutzer, der einer Aufgabe zugewiesen ist, oder ein Problem verpflichtet, die Aufgabe oder das Problem abzuschließen. Dies unterscheidet sich vom geplanten Abschlussdatum, da es eine realistischere Schätzung des Abschlussdatums darstellt, das der Benutzer, der direkt für die Arbeit verantwortlich ist, angegeben hat.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# Datum bestätigen - Übersicht

<!--Audited: 07/2024-->

<!-- <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Das Datum der Veröffentlichung ist das Datum, bis zu dem ein Benutzer, der einer Aufgabe zugewiesen ist, oder ein Problem verpflichtet, die Aufgabe oder das Problem abzuschließen.

Dies unterscheidet sich vom geplanten Abschlussdatum einer Aufgabe oder eines Problems, da es eine realistischere Schätzung des Abschlussdatums ist, das nur vom für die Arbeit verantwortlichen Benutzer angegeben wird.

Weitere Informationen zum geplanten Abschlussdatum finden Sie unter [Übersicht über das geplante Abschlussdatum der Aufgabe](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Datum bestätigen - Übersicht

Beachten Sie beim Arbeiten mit Commit-Daten Folgendes:

* Nur Aufgaben und Probleme haben ein &quot;Commit Date&quot;.
* Commit-Daten werden von Adobe Workfront nicht automatisch festgelegt.\
  Wenn Sie eine Aufgabe oder ein Problem erstellen, wird der Aufgabe oder dem Problem kein Commit-Datum zugewiesen.
* Wenn Sie einer Aufgabe oder einem Problem zugewiesen sind, können Sie das Veröffentlichungsdatum wie folgt festlegen:

   * Lassen Sie Workfront das Datum für die Übermittlung so festlegen, dass es dem bereits geplanten Abschlussdatum der Aufgabe oder des Problems entspricht, indem Sie auf &quot;Bearbeiten&quot;, &quot;Problem starten&quot;oder &quot;Aufgabe starten&quot;für die Aufgabe oder das Problem klicken. Weitere Informationen zum Ersetzen der Schaltfläche &quot;Work On It&quot;durch eine Schaltfläche &quot;Start&quot;finden Sie unter [Ersetzen der Schaltfläche &quot;Work On It&quot;durch eine Schaltfläche &quot;Start&quot;](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Legen Sie das Datum für die Übermittlung manuell fest, abhängig davon, wann Sie glauben, dass die Aufgabe oder das Problem möglicherweise abgeschlossen ist. Dies ist Ihre Schätzung und Zusage als Verantwortlicher für den Projektmanager, dass die Aufgabe oder das Problem bis zu einem bestimmten Datum abgeschlossen sein wird.
Weitere Informationen finden Sie unter [Aktualisierungsdaten für Aufgaben und Probleme aktualisieren](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

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
>Weitere Informationen zum Aufgabeneigentümer finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Suchen Sie nach dem Datum des Versands der Aufgaben und Probleme

Das Datum der Übermittlung an Aufgaben und Probleme finden Sie in den folgenden Bereichen von Workfront:

* Die Detailseite
* Nachdem ein Workfront- oder Gruppenadministrator sie Ihrer Layoutvorlage hinzugefügt hat, wird sie im Bereich &quot;Zusammenfassung&quot;angezeigt. Weitere Informationen finden Sie unter [Anpassen des Zusammenfassungsbereichs mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Die Kopfzeile einer Aufgabe oder eines Problems, nachdem ein Workfront- oder Gruppenadministrator sie zu Ihrer Layoutvorlage hinzugefügt hat. Weitere Informationen finden Sie unter [Anpassen von Objektüberschriften mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Durch Änderung des Zusagedatums ausgelöste Benachrichtigungen und Aktualisierungen {#notifications-and-updates-triggered-by-changing-the-commit-date}

Wenn ein Aufgaben- oder Problemverantwortlicher ein Veröffentlichungsdatum manuell in ein Datum ändert, das sich vom geplanten Abschlussdatum unterscheidet, das vom Projekteigentümer festgelegt wurde, gibt es eine Reihe von Benachrichtigungen und Aktualisierungen, die den Projektinhaber und andere Benutzer auf diese Änderung hinweisen.

>[!NOTE]
>
>Änderungen am Datum der Übermittlung ändern nicht automatisch die geplanten Daten, und Änderungen an den geplanten Daten ändern nicht automatisch das Datum der Veröffentlichung.

Durch manuelles Festlegen des Veröffentlichungsdatums für eine Aufgabe oder ein Problem werden die folgenden Trigger geändert:

* Die Änderung &quot;Datum der Übermittlung&quot;wird in der Systemaktivität und auf den Registerkarten Alle im Abschnitt Aktualisieren der Aufgabe oder des Problems angezeigt.

  ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  Die Änderung des Veröffentlichungsdatums wird im Bereich Updates der Aufgabe bzw. des Problems angezeigt, wenn der Workfront-Administrator diese Aktualisierung im Bereich Updates-Feeds unter Einrichtung aktiviert. Weitere Informationen finden Sie unter [Vom System getrackte Updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

  Wenn ein Projekteigentümer die Änderung nicht akzeptieren möchte, empfehlen wir ihm, dem Benutzer, der über die Registerkarte Kommentare im Abschnitt Aktualisierungen ein neues Datum vorschlägt, einen Kommentar abzugeben, ihn aufzufordern, das Veröffentlichungsdatum zurück zum ursprünglichen geplanten Datum zu ändern, oder ein neues Datum auszuwählen.

  Wenn ein Projekteigentümer die Änderung akzeptiert, kann er das geplante Abschlussdatum manuell so anpassen, dass es mit dem vom dem Artikel zugewiesenen Benutzer angegebenen Zustimmungsdatum übereinstimmt, indem er die Aufgabe oder das Problem bearbeitet.

  Sie müssen Zugriff haben, um die Aufgabe oder das Problem zu verwalten und sie zu bearbeiten.

  >[!TIP]
  >
  >Sie können Ihren System- oder Gruppenadministrator bitten, das Feld &quot;Commit Date&quot;Ihrem Zusammenfassungsbereich oder Ihrer Kopfzeile hinzuzufügen, um die Aktualisierung zu vereinfachen.
  >
  >Weitere Informationen finden Sie in den folgenden Artikeln:
  >
  >* [Überblick über die Zusammenfassung](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [Anpassen des Zusammenfassungsbereichs mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [Anpassen von Objektüberschriften mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* Das geplante Abschlussdatum der Aufgabe oder des Problems ist auf das gleiche Datum festgelegt, da die Aufgabe jetzt genauer angibt, wann sie wahrscheinlich abgeschlossen sein wird.

  Weitere Informationen zum geplanten Abschlussdatum finden Sie unter [Überblick über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* Der Projekteigentümer wird im Bereich Benachrichtigungen darüber benachrichtigt, dass sich das Datum der Übertragung einer Aufgabe oder eines Problems geändert hat.

  ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >Die Benachrichtigung, dass das Veröffentlichungsdatum geändert wurde, wird nur dann an den Projekteigentümer gesendet, wenn der Workfront-Administrator die Anzeige des Bestätigungsdatums im Bereich &quot;Aktualisierungen-Feeds&quot;im Setup-Bereich aktiviert. Weitere Informationen finden Sie unter [Vom System getrackte Updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Informationen zu den zusätzlichen Funktionen, die beim Aktualisieren eines Arbeitselements verfügbar sind, finden Sie unter [Arbeit aktualisieren](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Informationen zum Aktualisieren der Daten für die Veröffentlichung für Aufgaben und Probleme finden Sie unter [Aktualisierungsdaten für Aufgaben und Probleme aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
