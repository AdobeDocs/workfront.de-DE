---
product-area: projects
navigation-topic: manage-tasks
title: Überblick über das Speichern gleichzeitiger Änderungen in einer Aufgabenliste
description: Wenn Sie Aufgaben in einer Liste bearbeiten, können Sie separate Speichereinstellungen verwenden, um anzugeben, ob Ihre Änderungen beim Bearbeiten von Aufgaben in einer Liste manuell gespeichert werden sollen.
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Überblick über das Speichern gleichzeitiger Änderungen in einer Aufgabenliste

Wenn Sie Aufgaben in einer Liste bearbeiten, können Sie separate Speichereinstellungen verwenden, um anzugeben, ob Ihre Änderungen beim Bearbeiten von Aufgaben in einer Liste manuell gespeichert werden sollen.

Informationen zum Bearbeiten von Aufgaben in einer Aufgabenliste finden Sie im Artikel [Bearbeiten von Aufgaben in einer Liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Manchmal können Konflikte auftreten, wenn zwei Benutzer Änderungen an denselben Aufgaben vornehmen.

Beachten Sie beim Bearbeiten von Aufgaben in einer Aufgabenliste Folgendes:

* Adobe Workfront speichert die Änderungen, die Sie an Aufgaben vornehmen, sofort, wenn Sie Ihre Änderungen automatisch speichern möchten, falls der Projektaktualisierungstyp „Automatisch“, „Automatisch“ oder „Bei Änderung“ ist. Informationen zum Projektaktualisierungstyp finden Sie unter [Auswahl des Projektaktualisierungstyps](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfront aktualisiert die Informationen auf der Liste, an der Sie arbeiten, minütlich mit Änderungen, die andere Benutzer an einer anderen Stelle im System vornehmen könnten. Dadurch wird sichergestellt, dass Sie immer die neuesten Informationen zu den Aufgaben erhalten.

Die folgenden Szenarien bestehen, wenn mehrere Benutzer dieselben Aufgaben bearbeiten:

* **Ein(e) Benutzende(r) speichert die Änderungen in einer Aufgabenliste automatisch und ein(e) andere(r) manuell**: Wenn ein(e) Benutzende(r) (Benutzer A) Änderungen manuell speichert, während Benutzer B dieselben Aufgaben bearbeitet, seine Änderungen jedoch automatisch speichert, werden die von Benutzer B vorgenommenen Live-Änderungen jede Minute in der Liste für Benutzer A aktualisiert. Wenn es Konflikte zwischen den Änderungen gibt, die von den beiden Benutzern vorgenommen wurden, wird beim manuellen Speichern (Benutzer A) eine Warnmeldung angezeigt, bevor die Änderungen gespeichert werden können. Die Warnmeldung zeigt die Elemente an, bei denen die Änderungen widersprüchlich sind. Zu diesem Zeitpunkt kann Benutzer A wählen, ob seine Änderungen beibehalten (wodurch die von Benutzer B vorgenommenen Änderungen überschrieben werden) oder verworfen werden sollen (wodurch die von Benutzer B vorgenommenen Änderungen beibehalten werden).

>[!NOTE]
>
>Wenn Sie die von Ihnen vorgenommenen Änderungen verwerfen, gilt dies für alle Änderungen und nicht nur für die Änderungen, die mit den von einem anderen Benutzer vorgenommenen Änderungen in Konflikt stehen.

* **Mehrere Benutzer speichern die Änderungen in einer Aufgabenliste manuell**: Wenn mehrere Benutzer, die Änderungen an Aufgaben in einer Liste vornehmen, gleichzeitig manuell speichern, speichert Workfront die Änderungen, die von dem Benutzer vorgenommen wurden, der zuerst speichert. Beim Speichern dieser Änderungen sollten keine Konflikte auftreten. Workfront vergleicht dann die von allen anderen Benutzern vorgenommenen Änderungen mit den bereits gespeicherten Informationen und zeigt eine Warnung zu den widersprüchlichen Änderungen an den anderen Benutzern an, bevor diese ihre Informationen speichern können.

>[!IMPORTANT]
>
>Wenn Sie auswählen, dass Ihre Änderungen über allen anderen Änderungen bleiben sollen, werden alle Ihre Änderungen gespeichert, es sei denn, die Aufgaben, an denen Sie Änderungen vorgenommen haben, wurden von einem anderen Benutzer gelöscht. In diesem Fall werden Sie durch die Warnmeldung darüber informiert, dass die von Ihnen an den gelöschten Aufgaben vorgenommenen Änderungen verloren gehen.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
