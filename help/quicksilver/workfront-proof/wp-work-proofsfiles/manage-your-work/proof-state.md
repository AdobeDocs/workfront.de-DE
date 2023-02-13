---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Grundlegendes zum Testversandstatus in Workfront Testversand
description: In [!DNL Workfront Proof], existieren Testsendungen in verschiedenen Status. Diese Status bestimmen, welche Aktionen Sie für den Testversand ausführen können, z. B. Kommentare oder Entscheidungen treffen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Grundlegendes zum Testversandstatus in Workfront Testversand

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

In [!DNL Workfront Proof], existieren Testsendungen in verschiedenen Status. Diese Status bestimmen, welche Aktionen Sie für den Testversand ausführen können, z. B. Kommentare oder Entscheidungen treffen.

## Grundlagen zum Teststatus

Die vier Status lauten wie folgt:

* [Aktiv](#active)
* [Gesperrt](#locked)
* [Entwurf (nur Dropzone)](#draft-dropzone-only)
* [Gesendet (nur Dropzone)](#submitted-dropzone-only)

### Aktiv {#active}

Testsendungen, die in hochgeladen werden [!DNL Workfront Proof] über die Seite Neuer Testversand oder die Dropzone wird nach der Verarbeitung als aktiv angezeigt. Wenn ein Testversand aktiv ist, können Benutzer den Testversand überprüfen, kommentieren und Entscheidungen treffen.

>[!NOTE]
>
>Testsendungen, die über die Dropzone hochgeladen werden, werden nur dann als aktiv angezeigt, wenn die Option Testversand bei Übermittlung aktivieren aktiviert ist. Wenn die Option nicht aktiviert ist, müssen Sie den Testversand manuell aktivieren.

Weitere Informationen zu Dropzone-Einstellungen finden Sie unter [Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### Gesperrt {#locked}

Sie können einen Testversand sperren, wenn Sie die Überprüfung abgeschlossen haben. Das Sperren eines Testversands bedeutet, dass keine weiteren Kommentare oder Entscheidungen zum Testversand getroffen werden können, der Testversand jedoch trotzdem geöffnet werden kann.

Alle Benutzer mit Bearbeitungsrechten für den Testversand können ihn entsperren.

Weitere Informationen zu Berechtigungen finden Sie unter [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>E-Mail-Benachrichtigungen werden beim Sperren eines Testversands nicht mehr gesendet. Wenn beispielsweise ein Testversand vor Ablauf der Frist gesperrt wird, wird bei Erreichen der entsprechenden Frist keine Benachrichtigungs-E-Mail gesendet.

### Entwurf (nur Dropzone) {#draft-dropzone-only}

Wenn Sie einen Testversand über die Dropzone senden, wird er in den Status Entwurf versetzt, bevor der Administrator ihn aktiviert. Wenn es sich im Entwurfsbereich befindet, können Sie keine Aktionen für den Testversand durchführen.

### Gesendet (nur Dropzone) {#submitted-dropzone-only}

Nachdem ein Entwurf vom Administrator aktiviert wurde, wird Ihr Testversand als Gesendet in der Dropzone angezeigt. Nach der Übermittlung können Sie den Testversand bearbeiten.

## Anzeigen und Ändern des Teststatus

Informationen zum Anzeigen einer Liste aller Testsendungen in einem bestimmten Status, z. B. zum Anzeigen aller aktiven oder gesperrten Testsendungen, finden Sie unter [Elemente auf der Seite &quot;Ansichten&quot;verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) im Artikel [Elemente auf der Seite &quot;Ansichten&quot;verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Zugriff auf [!DNL Workfront Proof] Dashboard.

   Weitere Informationen finden Sie unter [Zugriff [!DNL Workfront Proof] von Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. Im **[!UICONTROL Dashboard]**, klicken Sie auf die **[!UICONTROL Erweitern]** neben dem Testversand, den Sie anzeigen oder ändern möchten.

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   Die **[!UICONTROL Workflow-Prozess]** angezeigt.

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. Anzeigen der **[!UICONTROL state]** im **[!UICONTROL Workflow-Prozess]**.

1. (Optional) Um den Status zu ändern, bewegen Sie den Mauszeiger über den aktuellen **[!UICONTROL state]** und klicken Sie auf das Dropdown-Menü und wählen Sie einen neuen Status aus.

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
