---
product-area: projects
navigation-topic: manage-tasks
title: Aufgaben löschen
description: Sie können Aufgaben löschen, die möglicherweise dupliziert sind oder fehlerhaft erstellt wurden.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 463fc65db6adb5cae6ecffb2e165155c89a63d6d
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---

# Aufgaben löschen

Sie können Aufgaben löschen, die möglicherweise dupliziert sind oder fehlerhaft erstellt wurden.

Für Aufgaben mit historischen Informationen (Aktualisierungen, Änderungen des Zeitplans, Status oder andere Felder) empfehlen wir, sie zu schließen oder als Eingestellt zu markieren, anstatt sie zu löschen. Auf diese Weise können Sie die historischen Informationen für Ihre Projekte aufbewahren.

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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte mit Zugriff auf „Löschen“ bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen zum Zugriff auf Aufgaben finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Zugriff auf Aufgaben gewähren</a>. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute-Berechtigungen für das Projekt mit der Möglichkeit, Aufgaben oder höher hinzuzufügen</p> <p>Wenn Sie eine Aufgabe erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für die Aufgabe</p> <p> Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Freigeben einer </a>. </p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriff auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Verstehen des Prozesses zum Löschen von Aufgaben

* [Einschränkungen beim Löschen von Aufgaben](#limitations-for-deleting-tasks)
* [Auswirkungen des Löschens von Aufgaben](#the-impact-of-deleting-tasks)

### Einschränkungen beim Löschen von Aufgaben  {#limitations-for-deleting-tasks}

* Wenn ein Projekt den Status „Abgeschlossen“ hat, können Sie Aufgaben nur löschen, wenn dies von Ihrem Workfront-Administrator oder einem Gruppenadministrator im Bereich „Projektvoreinstellungen“ zugelassen wurde. Informationen zum Einrichten von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Wenn für die Aufgabe Stunden protokolliert wurden, muss der Workfront- oder Gruppenadministrator das Löschen dieser Aufgaben zulassen, indem er die Voreinstellungen für Aufgaben und Probleme in der Workfront-Instanz konfiguriert. Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, in denen Aufgaben mit Stunden protokolliert sind.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Weitere Informationen zum Aktivieren des Löschens von Aufgaben, bei denen Stunden protokolliert werden, finden Sie im Abschnitt „Löschen“ in [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Auswirkungen des Löschens von Aufgaben {#the-impact-of-deleting-tasks}

Wenn Sie eine Aufgabe löschen, wirkt sich dies auf andere mit der Aufgabe verknüpfte Objekte aus.

Die folgenden mit einer Aufgabe verbundenen Objekte werden ebenfalls gelöscht, wenn Sie eine Aufgabe löschen:

* Dokumente

  Sie können eine Aufgabe, an die ein ausgechecktes Dokument angehängt ist, nicht löschen. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Auschecken von Dokumenten](../../../documents/managing-documents/check-out-documents.md).

* Probleme
* Teilaufgaben
* Notizen
* Genehmigungen

Je nachdem, wie Ihr Workfront-Administrator die Einstellungen für die Projekt-, Aufgaben- oder Problemlöschung in den Arbeitszeittabellen- und Stundeneinstellungen Ihrer Workfront-Instanz konfiguriert, werden die für die Aufgaben protokollierten Stunden beim Löschen einer Aufgabe auf eine der folgenden Arten gehandhabt:

* Verschieben Sie in das Projekt und wird bei der Aufgabe nicht wiederhergestellt, wenn die Aufgabe später wiederhergestellt wird.
* werden gelöscht und für die Aufgabe wiederhergestellt, wenn die Aufgabe später wiederhergestellt wird.

  Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, in denen Aufgaben mit Stunden protokolliert sind.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  Weitere Informationen zum Konfigurieren der Löschvoreinstellungen für Stunden, die bei Problemen protokolliert sind, finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundenvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Kosten für die Aufgabe werden in das Projekt verschoben.

* Die Benutzer, die der Aufgabe oder der Aufgabengenehmigung zugewiesen sind, bleiben im Projektteam.

  Weitere Informationen zu Projektteams finden Sie unter [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Aufgaben löschen

* [Gleichzeitiges Löschen mehrerer Aufgaben in einem Projekt](#delete-multiple-tasks-in-a-project-simultaneously)
* [Eine einzelne Aufgabe löschen](#delete-a-single-task)

### Gleichzeitiges Löschen mehrerer Aufgaben in einem Projekt  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken Sie auf **Projekte**.
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
      1. Klicken Sie **Löschen**.
      1. (Optional) Klicken Sie auf **Rückgängig**, um Ihre Änderung rückgängig zu machen und die Aufgaben nicht zu löschen.
      1. Klicken Sie **Wiederholen**, wenn Sie die Änderung beibehalten und die Aufgabe löschen möchten.
      1. Klicken Sie auf **Speichern**, um die Aufgaben zu löschen.

         Aufgaben werden erst gelöscht, nachdem Sie Ihre Änderungen gespeichert haben.

### Eine einzelne Aufgabe löschen {#delete-a-single-task}

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken Sie auf **Projekte**.
1. Klicken Sie auf den Projektnamen, der die Aufgabe enthält, die Sie löschen möchten.
1. Klicken Sie **linken** auf „Aufgaben“.
1. Klicken Sie auf den Namen der Aufgabe, die Sie löschen möchten.
1. Klicken Sie auf **Mehr**-Symbol ![](assets/qs-more-menu.png)in der oberen rechten Ecke.

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Klicken Sie **Aufgabe löschen**.
1. Wenn der Löschvorgang zulässig ist, klicken Sie auf **Löschen**.

   Ihr Workfront-Administrator oder Gruppenadministrator erlaubt möglicherweise nicht das Löschen von Aufgaben, bei denen Stunden protokolliert werden.

   Weitere Informationen zu den Zugriffsrechten und Berechtigungen, die zum Löschen einer Aufgabe erforderlich sind, finden Sie im Abschnitt [Einschränkungen beim Löschen von Aufgaben](#limitations-for-deleting-tasks) in diesem Artikel.

## Gelöschte Aufgaben wiederherstellen

Ein Workfront- oder Gruppen-Administrator kann Aufgaben innerhalb von 30 Tagen nach ihrem Löschen wiederherstellen, wie unter [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) beschrieben.
