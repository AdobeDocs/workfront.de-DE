---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Grundlegendes zum Teststatus in Workfront Proof
description: In  [!DNL Workfront Proof] gibt es Korrekturabzüge in verschiedenen Status. Diese Zustände bestimmen, welche Aktionen Sie für den Korrekturabzug durchführen können, z. B. Kommentare oder Entscheidungen treffen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Grundlegendes zum Teststatus in Workfront Proof

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

In [!DNL Workfront Proof] gibt es Korrekturabzüge in verschiedenen Status. Diese Zustände bestimmen, welche Aktionen Sie für den Korrekturabzug durchführen können, z. B. Kommentare oder Entscheidungen treffen.

## Grundlagen zum Teststatus

Die vier Status lauten wie folgt:

* [Aktiv](#active)
* [Gesperrt](#locked)
* [Entwurf (nur Ablagebereich)](#draft-dropzone-only)
* [Gesendet (nur Dropzone)](#submitted-dropzone-only)

### Aktiv {#active}

Korrekturabzüge, die über die Seite Neuer Korrekturabzug oder die Dropzone in [!DNL Workfront Proof] hochgeladen werden, werden nach der Verarbeitung als aktiv angezeigt. Wenn ein Korrekturabzug aktiv ist, können Benutzende ihn überprüfen, Kommentare abgeben und Entscheidungen über den Korrekturabzug treffen.

>[!NOTE]
>
>Korrekturabzüge, die über den Ablagebereich hochgeladen werden, werden nur dann als aktiv angezeigt, wenn die Option Korrekturabzug bei Übermittlung aktivieren aktiviert ist. Wenn die Option nicht aktiviert ist, müssen Sie den Korrekturabzug manuell aktivieren.

Weitere Informationen zu Dropzone-Einstellungen finden Sie unter [Konfigurieren der Dropzone in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Gesperrt {#locked}

Sie können einen Korrekturabzug sperren, wenn Sie mit der Überprüfung fertig sind. Das Sperren eines Korrekturabzugs bedeutet, dass keine Kommentare oder Entscheidungen mehr zum Korrekturabzug getroffen werden können, aber der Korrekturabzug kann weiterhin geöffnet werden.

Alle Benutzer mit Bearbeitungsrechten für den Korrekturabzug können ihn entsperren.

Weitere Informationen zu Berechtigungen finden Sie unter [Korrekturabzugsberechtigungsprofile in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>E-Mail-Benachrichtigungen werden nicht mehr gesendet, wenn ein Korrekturabzug gesperrt ist. Wenn beispielsweise ein Korrekturabzug vor Ablauf der Frist gesperrt wird, wird beim Erreichen der Frist keine Benachrichtigungs-E-Mail gesendet.

### Entwurf (nur Ablagebereich) {#draft-dropzone-only}

Wenn Sie einen Korrekturabzug über die Ablagefläche senden, wechselt er in den Status Entwurf , bevor ihn der Administrator aktiviert. Wenn er sich im Entwurfsbereich befindet, können Sie keine Aktionen für den Korrekturabzug durchführen.

### Gesendet (nur Dropzone) {#submitted-dropzone-only}

Nachdem ein Entwurf vom Administrator aktiviert wurde, wird Ihr Korrekturabzug als „Gesendet“ im Ablagebereich angezeigt. Nachdem er übermittelt wurde, können Sie Aktionen für den Korrekturabzug durchführen.

## Anzeigen und Ändern des Status des Korrekturabzugs

Informationen zum Anzeigen einer Liste aller Korrekturabzüge in einem bestimmten Status, z. B. aller aktiven oder gesperrten Korrekturabzüge, finden Sie unter [Verwalten von Elementen auf der Seite &quot; [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)&quot; im Artikel [Verwalten von Elementen auf der Seite „Ansichten“ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Greifen Sie auf Ihr [!DNL Workfront Proof] Dashboard zu.

   Weitere Informationen finden Sie unter [Zugriff [!DNL Workfront Proof]  von Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. Klicken Sie **[!UICONTROL Dashboard]** auf den Pfeil **[!UICONTROL Erweitern]** neben dem Korrekturabzug, dessen Status Sie anzeigen oder ändern möchten.

   ![Erweitern](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   Der **[!UICONTROL Workflow-Prozess]** wird angezeigt.

   ![Workflow-](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Zeigen Sie den **[!UICONTROL Status]** im **[!UICONTROL Workflow-Prozess]** an.

1. (Optional) Um den Status zu ändern, bewegen Sie den Mauszeiger über **[!UICONTROL aktuellen Status]** klicken Sie auf das Dropdown-Menü und wählen Sie dann einen neuen Status aus.

   ![Neuer Status](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
