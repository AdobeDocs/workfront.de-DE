---
product-area: setup
navigation-topic: notifications
keywords: modify,email,notification,settings
title: Ihre eigenen E-Mail-Benachrichtigungen ändern
description: In diesem Artikel wird beschrieben, wie Sie Ihre E-Mail-Benachrichtigungen in Ihrem Benutzerprofil verwalten können.
author: Lisa
feature: Get Started with Workfront
exl-id: 3d1f877e-6bb4-494e-b08e-c18ec87dd001
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Ihre eigenen E-Mail-Benachrichtigungen ändern

<!-- Audited: 1/2024 -->

Ihre Adobe [!DNL Workfront] Der Administrator konfiguriert, welche E-Mail-Benachrichtigungen Benutzer erhalten, wenn Ereignisse in Workfront auftreten (siehe [[!UICONTROL Ereignis konfigurieren] Benachrichtigungen für alle im System](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)).

Ihr Gruppenadministrator kann auch konfigurieren, welche Benachrichtigungen für Sie und die Benutzer in Ihrer [!UICONTROL Startseite]. Wenn [!UICONTROL Startseite] eine Untergruppe ist, erhalten Sie die Benachrichtigungen, die für die Gruppe der obersten Ebene über Ihrer Gruppe aktiviert wurden.

Sie können dies weiter anpassen, indem Sie konfigurieren, welche Benachrichtigungen Sie erhalten. Sie können auch auswählen, ob Sie Benachrichtigungen bei Ereignissen oder eine tägliche Digest-E-Mail erhalten möchten.

Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie unter [[!DNL Adobe Workfront] Benachrichtigungen](../../workfront-basics/using-notifications/wf-notifications.md).

>[!NOTE]
>
>* Wenn Sie einen Benachrichtigungstyp aktivieren und dann feststellen, dass Sie keine Benachrichtigungen dieses Typs erhalten, liegt dies möglicherweise daran, dass dieser Typ nicht für Ihre Rolle gilt.
>* Die [!DNL Workfront] Administrator oder Gruppenadministrator kann keine Benachrichtigungen für [!DNL Workfront Goals]. Weitere Informationen zu den Benachrichtigungen finden Sie unter [!DNL Workfront] Administratoren können konfigurieren, siehe [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). Informationen zum Konfigurieren von einzelnen Benachrichtigungen für [!DNL Workfront Goals] lesen Sie diesen Artikel weiter.
>

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz</strong></td> 
   <td>  <p>Neu:</p> 
   <ul><li>Mitwirkende oder höher</li></ul>
   <p>Aktuell:</p>
   <ul><li>Anfrage oder höher</li></ul>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## E-Mail-Benachrichtigungseinstellungen anzeigen und ändern

{{step1-click-profile-pic}}

1. Klicken Sie auf **[!UICONTROL Mehr]** icon ![](assets/more-icon.png) neben Ihrem Namen klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

1. Im **[!UICONTROL Person bearbeiten]** das angezeigt wird, wechseln Sie zum **[!UICONTROL Benachrichtigungen]** Abschnitt.

1. Klicken Sie auf eine Kategorie, um die Benachrichtigungseinstellungen für diese Kategorie anzuzeigen.

   ![](assets/my-profile-notifications.png)

1. Aktivieren oder deaktivieren Sie die Kontrollkästchen auf der rechten Seite, um anzugeben, ob Sie Benachrichtigungen täglich, sofort oder beides empfangen möchten.

   Sie können auch die Kontrollkästchen für eine Kategorie verwenden, um alle Benachrichtigungen in dieser Kategorie zu aktivieren oder zu deaktivieren.

   >[!NOTE]
   >
   >Wenn Sie Teammitglied eines Projekts sind, erhalten Sie weiterhin E-Mail-Benachrichtigungen dafür, bis Sie aus dem Team entfernt werden, auch wenn Sie keinen Zugriff mehr auf das Projekt haben. Anweisungen zum Entfernen von Benutzern aus einem Team finden Sie unter [Entfernen von Benutzern aus Projekten](../../manage-work/projects/manage-projects/remove-users-from-projects.md).

   Für **[!UICONTROL Kommunikation]** -Kategorie, können Sie einzelne Benachrichtigungen nur für den sofortigen Versand auswählen. Damit Benachrichtigungen täglich versendet werden können, müssen Sie alle Benachrichtigungen auswählen.

   Wenn alle E-Mail-Benachrichtigungen für eine bestimmte Kategorie aktiviert sind, wird das Feld im Kategorientitel wie ausgewählt angezeigt. Wenn alle E-Mail-Benachrichtigungen einer bestimmten Kategorie deaktiviert sind, wird das Kontrollkästchen deaktiviert. Wenn einige Benachrichtigungen aktiviert und andere deaktiviert sind, wird das Kategorieprüffeld als gerade Zeile angezeigt.\
   Wenn Sie eine Benachrichtigungseinstellung ändern, wird der Titel **[!UICONTROL Bearbeitet]** für diese Benachrichtigungseinstellung angezeigt, um Sie darüber zu informieren, dass diese Benachrichtigungseinstellung geändert wurde.

1. Wenn Sie Benachrichtigungen ausgewählt haben, die als tägliche Zusammenfassung gesendet werden sollen, wählen Sie oben im **[!UICONTROL Benachrichtigungen]** im Abschnitt **[!UICONTROL Email Daily Digest nach]** Menü.

   ![](assets/digest-time-stamp-my-settings-350x78.png)

   Die tägliche Zusammenfassung enthält Ereignisse, die die Kriterien der Benachrichtigungen 24 Stunden vor dem ausgewählten Zeitpunkt erfüllen. Sie erhalten für jeden Benachrichtigungstyp eine tägliche Digest-E-Mail.\
   Der tägliche Digest kann nach der von Ihnen ausgewählten Zeit eintreffen, je nachdem, wie viele E-Mails in die Warteschlange für den Versand im System gestellt werden. Die angegebene Uhrzeit entspricht der Ortszeit, die Sie in den Browsereinstellungen angegeben haben.

1. (Bedingt und optional) Aktivieren Sie beim Ändern der Einstellungen für E-Mail-Benachrichtigungen in der Vorschau-Umgebung die Option **[!UICONTROL Empfangen von E-Mails aus dieser Testumgebung]** für den Empfang von E-Mails festlegen. E-Mails werden nicht automatisch aus der Vorschau-Umgebung generiert.

   ![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

1. Klicks **[!UICONTROL Änderungen speichern]**.
