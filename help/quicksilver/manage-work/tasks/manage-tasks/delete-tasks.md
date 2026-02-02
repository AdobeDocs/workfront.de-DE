---
product-area: projects
navigation-topic: manage-tasks
title: Aufgaben löschen
description: Sie können Aufgaben löschen, die möglicherweise dupliziert sind oder fehlerhaft erstellt wurden.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 5%

---

# Aufgaben löschen

Sie können Aufgaben löschen, die möglicherweise dupliziert sind oder fehlerhaft erstellt wurden.

Für Aufgaben mit historischen Informationen (Aktualisierungen, Änderungen des Zeitplans, Status oder andere Felder) empfehlen wir, sie zu schließen oder als Eingestellt zu markieren, anstatt sie zu löschen. Auf diese Weise können Sie die historischen Informationen für Ihre Projekte aufbewahren.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> 
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte mit Zugriff auf „Löschen“ bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt mit der Möglichkeit zum Hinzufügen von Aufgaben oder höher hinzufügen</p> <p>Wenn Sie eine Aufgabe erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für die Aufgabe</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects with access to Delete</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Verstehen des Prozesses zum Löschen von Aufgaben

* [Einschränkungen beim Löschen von Aufgaben](#limitations-for-deleting-tasks)
* [Auswirkungen des Löschens von Aufgaben](#the-impact-of-deleting-tasks)

### Einschränkungen beim Löschen von Aufgaben  {#limitations-for-deleting-tasks}

* Wenn ein Projekt den Status „Abgeschlossen“ hat, können Sie Aufgaben nur löschen, wenn dies von Ihrem Workfront-Administrator oder einem Gruppenadministrator im Bereich „Projektvoreinstellungen“ zugelassen wurde. Informationen zum Einrichten von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Wenn für die Aufgabe Stunden protokolliert wurden, muss der Workfront- oder Gruppenadministrator das Löschen dieser Aufgaben zulassen, indem er die Voreinstellungen für Aufgaben und Probleme in der Workfront-Instanz konfiguriert. Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, in denen Aufgaben mit Stunden protokolliert sind.

  <!--
  (NOTE: the last statement is NWE only; not possible in classic)
  -->

  Weitere Informationen zum Aktivieren des Löschens von Aufgaben, bei denen Stunden protokolliert werden, finden Sie im Abschnitt „Löschen“ in [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Auswirkungen des Löschens von Aufgaben {#the-impact-of-deleting-tasks}

Wenn Sie eine Aufgabe löschen, wirkt sich dies auf andere mit der Aufgabe verknüpfte Objekte aus.

Beachten Sie Folgendes:

* Die folgenden mit einer Aufgabe verbundenen Objekte werden ebenfalls gelöscht, wenn Sie eine Aufgabe löschen:

   * Dokumente

  Sie können eine Aufgabe, an die ein ausgechecktes Dokument angehängt ist, nicht löschen. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Auschecken von Dokumenten](../../../documents/managing-documents/check-out-documents.md).

   * Probleme
   * Teilaufgaben
   * Anmerkungen
   * Genehmigungen

* Je nachdem, wie Ihr Workfront-Administrator die Einstellungen für die Projekt-, Aufgaben- oder Problemlöschung in den Arbeitszeittabellen- und Stundeneinstellungen Ihrer Workfront-Instanz konfiguriert, werden die für die Aufgaben protokollierten Stunden beim Löschen einer Aufgabe auf eine der folgenden Arten gehandhabt:

   * Verschieben Sie in das Projekt und wird bei der Aufgabe nicht wiederhergestellt, wenn die Aufgabe später wiederhergestellt wird.
   * werden gelöscht und für die Aufgabe wiederhergestellt, wenn die Aufgabe später wiederhergestellt wird.

  Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, in denen Aufgaben mit Stunden protokolliert sind.

  Weitere Informationen zum Konfigurieren der Löschvoreinstellungen für Stunden, die bei Problemen protokolliert sind, finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundenvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
   * Kosten für die Aufgabe werden in das Projekt verschoben.

   * Die Benutzer, die der Aufgabe oder der Aufgabengenehmigung zugewiesen sind, bleiben im Projektteam.

  Weitere Informationen zu Projektteams finden Sie unter [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

* Wenn Sie eine untergeordnete Aufgabe löschen und ihre übergeordnete Aufgabe in ein anderes Projekt verschieben und dann die gelöschte untergeordnete Aufgabe wiederherstellen, wird die Aufgabe im ursprünglichen Projekt als Hauptaufgabe wieder hinzugefügt.

<!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

## Aufgaben löschen

* [Gleichzeitiges Löschen mehrerer Aufgaben in einem Projekt](#delete-multiple-tasks-in-a-project-simultaneously)
* [Eine einzelne Aufgabe löschen](#delete-a-single-task)

### Gleichzeitiges Löschen mehrerer Aufgaben in einem Projekt  {#delete-multiple-tasks-in-a-project-simultaneously}

{{step1-to-projects}}

1. Klicken Sie auf den Projektnamen, der die Aufgaben enthält, die Sie löschen möchten.
1. Klicken Sie **linken** auf „Aufgaben“.
1. Führen Sie einen der folgenden Schritte aus:

   1. (Bedingt) Wenn der Umschalter **Automatisches Speichern** aktiviert ist:

      1. Wählen Sie die Aufgaben aus, die Sie löschen möchten, und klicken Sie dann auf **Mehr**
      1. Klicken Sie auf **Löschen** und dann auf **Löschen**, um den Löschvorgang zu bestätigen.

         Die Aufgaben werden gelöscht.

   1. (Bedingt) Klicken Sie auf das Symbol **Planmodus** und wählen Sie **Manuelles Speichern** aus, wenn Sie die Änderungen an der Aufgabenliste rückgängig machen möchten.

      ![Wählen Sie Manuelles Speichern](assets/manual-save-option.png)

      Gehen Sie folgendermaßen vor:

      1. Wählen Sie die Aufgaben aus, die Sie löschen möchten.
      1. Klicken Sie auf **Löschen**.
      1. (Optional) Klicken Sie auf **Rückgängig**, um Ihre Änderung rückgängig zu machen und die Aufgaben nicht zu löschen.
      1. Klicken Sie **Wiederholen**, wenn Sie die Änderung beibehalten und die Aufgabe löschen möchten.
      1. Klicken Sie auf **Speichern**, um die Aufgaben zu löschen.

         Aufgaben werden erst gelöscht, nachdem Sie Ihre Änderungen gespeichert haben.

### Eine einzelne Aufgabe löschen {#delete-a-single-task}

{{step1-to-projects}}

1. Klicken Sie auf den Projektnamen, der die Aufgabe enthält, die Sie löschen möchten.
1. Klicken Sie **linken** auf „Aufgaben“.
1. Klicken Sie auf den Namen der Aufgabe, die Sie löschen möchten.
1. Klicken Sie auf das **Mehr**-Symbol ![Mehr Menü](assets/qs-more-menu.png) in der oberen rechten Ecke.

   ![Aufgaben auf Aufgabenebene löschen](assets/delete-tasks-task-level-nwe-350x225.png)

1. Klicken Sie **Aufgabe löschen**.
1. Wenn der Löschvorgang zulässig ist, klicken Sie auf **Löschen**.

   Ihr Workfront-Administrator oder Gruppenadministrator erlaubt möglicherweise nicht das Löschen von Aufgaben, bei denen Stunden protokolliert werden.

   Weitere Informationen zu den Zugriffsrechten und Berechtigungen, die zum Löschen einer Aufgabe erforderlich sind, finden Sie im Abschnitt [Einschränkungen beim Löschen von Aufgaben](#limitations-for-deleting-tasks) in diesem Artikel.

## Gelöschte Aufgaben wiederherstellen

Ein Workfront- oder Gruppen-Administrator kann Aufgaben innerhalb von 30 Tagen nach ihrem Löschen wiederherstellen, wie unter [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) beschrieben.
