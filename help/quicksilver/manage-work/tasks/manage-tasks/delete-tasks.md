---
product-area: projects
navigation-topic: manage-tasks
title: Aufgaben löschen
description: Sie können Aufgaben löschen, die möglicherweise dupliziert oder fehlerhaft erstellt wurden.
author: Alina
feature: Work Management
exl-id: aee5c293-e5fa-413e-9d9b-c62528941be7
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 1%

---

# Aufgaben löschen

Sie können Aufgaben löschen, die möglicherweise dupliziert oder fehlerhaft erstellt wurden.

Für Aufgaben mit Verlaufsinformationen (Aktualisierungen, Änderungen des Zeitplans, Status oder andere Felder) empfehlen wir, diese zu schließen oder sie als &quot;Dead&quot;zu kennzeichnen, anstatt sie zu löschen. Auf diese Weise können Sie die historischen Informationen für Ihre Projekte speichern.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte mit Zugriff auf "Löschen"bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Aufgaben finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Zugriff auf Aufgaben gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute-Berechtigungen für das Projekt mit der Möglichkeit, Aufgaben hinzuzufügen oder höher</p> <p>Wenn Sie eine Aufgabe erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für die Aufgabe</p> <p> Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Aufgabe freigeben </a>. </p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Vorgehensweise beim Löschen von Aufgaben

* [Einschränkungen zum Löschen von Aufgaben](#limitations-for-deleting-tasks)
* [Auswirkungen des Löschens von Aufgaben](#the-impact-of-deleting-tasks)

### Einschränkungen beim Löschen von Aufgaben  {#limitations-for-deleting-tasks}

* Wenn ein Projekt den Status Abgeschlossen aufweist, können Sie Aufgaben nur löschen, wenn dies Ihr Workfront-Administrator oder ein Gruppenadministrator im Bereich &quot;Projekteinstellungen&quot;zugelassen hat. Weitere Informationen zum Einrichten von Projektvoreinstellungen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Wenn die Aufgabe Stunden protokolliert hat, muss der Workfront- oder Gruppenadministrator das Löschen dieser Aufgaben zulassen, indem er die Voreinstellungen für Aufgaben und Probleme in Ihrer Workfront-Instanz konfiguriert. Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, bei denen Aufgaben mit aufgezeichneten Stunden ausgeführt werden.

  <!--
  (NOTE: the last statement is NWE&nbsp;only; not possible in classic)
  -->

  Weitere Informationen zum Aktivieren des Löschens von Aufgaben, bei denen Stunden protokolliert werden, finden Sie im Abschnitt &quot;Löschung&quot;unter [Systemweite Aufgabe konfigurieren und Ausgabevoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Auswirkungen des Löschens von Aufgaben {#the-impact-of-deleting-tasks}

Wenn Sie eine Aufgabe löschen, wirkt sich dies auf andere Objekte aus, die mit der Aufgabe verknüpft sind.

Die folgenden Objekte, die an eine Aufgabe angehängt sind, werden auch beim Löschen einer Aufgabe gelöscht:

* Dokumente

  Sie können eine Aufgabe nicht löschen, der ein ausgechecktes Dokument angehängt ist. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Dokumente auschecken](../../../documents/managing-documents/check-out-documents.md).

* Probleme
* Teilaufgaben
* Notizen
* Genehmigungen

Je nachdem, wie Ihr Workfront-Administrator die Voreinstellungen zum Projekt, zur Aufgabe oder zum Löschen von Problemen in den Voreinstellungen für das Arbeitsblatt und die Stunde Ihrer Workfront-Instanz konfiguriert, werden die für die Aufgaben protokollierten Stunden beim Löschen einer Aufgabe auf eine der folgenden Arten verarbeitet:

* Wechseln Sie zum Projekt und werden nicht in der Aufgabe wiederhergestellt, wenn die Aufgabe später wiederhergestellt wird.
* werden gelöscht und für die Aufgabe wiederhergestellt, wenn die Aufgabe später wiederhergestellt wird.

  Dies gilt auch, wenn Sie versuchen, Projekte zu löschen, bei denen Aufgaben mit aufgezeichneten Stunden ausgeführt werden.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this stays NWE; not possible in classic;)
  </MadCap:conditionalText>
  -->

  Weitere Informationen zum Konfigurieren der Löschvoreinstellungen für Stunden, die bei Problemen protokolliert werden, finden Sie unter [Konfigurieren von Voreinstellungen für Zeitblätter und Stunden](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Die Ausgaben für die Aufgabe werden in das Projekt verschoben.

* Die der Aufgabe oder der Aufgabenvalidierung zugewiesenen Benutzer verbleiben im Projektteam.

  Weitere Informationen zu Projektteams finden Sie unter [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Aufgaben löschen

* [Mehrere Aufgaben in einem Projekt gleichzeitig löschen](#delete-multiple-tasks-in-a-project-simultaneously)
* [Löschen einer einzelnen Aufgabe](#delete-a-single-task)

### Mehrere Aufgaben gleichzeitig in einem Projekt löschen  {#delete-multiple-tasks-in-a-project-simultaneously}

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Projekte**.
1. Klicken Sie auf den Projektnamen, der die Aufgaben enthält, die Sie löschen möchten.
1. Klicken Sie im linken Bereich auf **Aufgaben** .
1. Führen Sie einen der folgenden Schritte aus:

   1. (Bedingt) Wenn der Umschalter **Autosave** aktiviert ist:

      1. Wählen Sie die Aufgaben aus, die Sie löschen möchten, und klicken Sie dann auf **Mehr**
      1. Klicken Sie auf **Löschen** und dann auf **Ja, löschen Sie es**, um den Löschvorgang zu bestätigen.

         Die Aufgaben werden gelöscht.

   1. (Bedingt) Klicken Sie auf das Symbol **Planmodus** und wählen Sie **Manuelles Speichern** aus, wenn Sie die an der Aufgabenliste vorgenommenen Änderungen rückgängig machen möchten.

      ![Manuelles Speichern auswählen](assets/manual-save-option.png)

      Gehen Sie wie folgt vor:

      1. Wählen Sie die Aufgaben aus, die Sie löschen möchten.
      1. Klicken Sie auf **Löschen**.
      1. (Optional) Klicken Sie auf **Rückgängig** , um Ihre Änderung rückgängig zu machen und die Aufgaben nicht zu löschen.
      1. Klicken Sie auf **Wiederholen** , wenn Sie die Änderung beibehalten und die Aufgabe löschen möchten.
      1. Klicken Sie auf **Speichern** , um die Aufgaben zu löschen.

         Aufgaben werden erst gelöscht, nachdem Sie Ihre Änderungen gespeichert haben.

### Löschen einer einzelnen Aufgabe {#delete-a-single-task}

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Projekte**.
1. Klicken Sie auf den Projektnamen, der die Aufgabe enthält, die Sie löschen möchten.
1. Klicken Sie im linken Bereich auf **Aufgaben** .
1. Klicken Sie auf den Namen der Aufgabe, die Sie löschen möchten.
1. Klicken Sie oben rechts auf das Symbol **Mehr** ![](assets/qs-more-menu.png).

   ![](assets/delete-tasks-task-level-nwe-350x225.png)

1. Klicken Sie auf **Aufgabe löschen**.
1. Wenn der Löschvorgang zulässig ist, klicken Sie auf **Ja, löschen Sie ihn**.

   Möglicherweise lässt Ihr Workfront-Administrator oder Gruppenadministrator das Löschen von Aufgaben, bei denen Stunden protokolliert werden, nicht zu.

   Weitere Informationen zu Zugriff und Berechtigungen, die zum Löschen einer Aufgabe erforderlich sind, finden Sie im Abschnitt [Einschränkungen zum Löschen von Aufgaben](#limitations-for-deleting-tasks) in diesem Artikel.

## Gelöschte Aufgaben wiederherstellen

Ein Workfront- oder Gruppenadministrator kann Aufgaben innerhalb von 30 Tagen nach dem Löschen wiederherstellen, wie unter [Gelöschte Elemente wiederherstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) beschrieben.
