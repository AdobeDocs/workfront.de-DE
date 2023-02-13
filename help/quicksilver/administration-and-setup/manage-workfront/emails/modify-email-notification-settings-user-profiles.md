---
user-type: administrator
product-area: system-administration
keywords: modify,email,notification,settings,bulk,bulk,edit,configure,multiple,users
navigation-topic: emails-administration
title: E-Mail-Benachrichtigungseinstellungen in Benutzerprofilen ändern
description: Wenn Sie Adobe Workfront-Administrator sind oder über die Zugriffsebene "Planer"verfügen, mit der Sie die Einstellungen anderer Benutzer bearbeiten können, können Sie die Benachrichtigungseinstellungen für mehrere Benutzer gleichzeitig konfigurieren. Dazu gehört auch die Angabe, ob Benutzer Benachrichtigungen bei Ereignissen erhalten oder in einer täglichen Digest-E-Mail, wie in Adobe Workfront-Benachrichtigungen beschrieben. Informationen zu der für die Bearbeitung von Benutzern erforderlichen Zugriffsebene finden Sie unter Gewähren von Zugriff für Benutzer.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# E-Mail-Benachrichtigungseinstellungen in Benutzerprofilen ändern

Wenn Sie Adobe Workfront-Administrator sind oder über die Zugriffsebene &quot;Planer&quot;verfügen, mit der Sie die Einstellungen anderer Benutzer bearbeiten können, können Sie die Benachrichtigungseinstellungen für mehrere Benutzer gleichzeitig konfigurieren. Dazu gehört auch die Angabe, ob Benutzer Benachrichtigungen im Fall von Ereignissen erhalten oder in einer täglichen Digest-E-Mail, wie hier beschrieben: [Adobe Workfront-Benachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md). Informationen zur Zugriffsstufe, die zum Bearbeiten von Benutzern erforderlich ist, finden Sie unter [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Wenn Sie die Benachrichtigungseinstellungen stapelweise konfigurieren, können Sie nur die Einstellungen ändern, die den ausgewählten Benutzern gemeinsam sind.

Sie können auch E-Mail-Benachrichtigungen für jeweils einen Benutzer konfigurieren. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben.

## Die E-Mail-Benachrichtigungseinstellungen für mehrere Benutzer stapelweise ändern

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png). Wählen Sie die Benutzer aus und klicken Sie auf **Bearbeiten**.
1. Im **Person bearbeiten** wird angezeigt, klicken Sie auf **Benachrichtigungen**.

1. Erweitern Sie eine Kategorie, um die mit dieser Kategorie verbundenen Benachrichtigungseinstellungen anzuzeigen.

   Wenn mindestens ein Benutzer ausgewählt ist, bei dem die Benachrichtigungen nicht mit den Benachrichtigungen der anderen ausgewählten Benutzer übereinstimmen, enthält das Kategorieprüffeld für diese Benachrichtigung eine horizontale Zeile ![](assets/straight-line-instead-of-checkmark.jpg) anstelle eines Häkchen.

1. Klicken Sie auf alle Benachrichtigungen, die die Benutzer täglich oder sofort erhalten sollen, oder löschen Sie alle Benachrichtigungen, die sie nicht mehr erhalten sollen.

   Für **Kommunikation** -Kategorie, können Sie einzelne Benachrichtigungen nur für den sofortigen Versand auswählen. Sie müssen alle Benachrichtigungen auswählen, die täglich versendet werden sollen.

   Wenn Sie eine Benachrichtigungseinstellung ändern, wird der Titel **Bearbeitet** für diese Benachrichtigungseinstellung angezeigt, um Sie darüber zu informieren, dass diese Benachrichtigungseinstellung geändert wurde.

1. Wenn Sie Benachrichtigungen als täglichen Digest ausgewählt haben, wählen Sie oben in der **Benachrichtigungen** im Abschnitt **Email Daily Digest nach** Menü.

   Nach Auswahl der Versandzeit wird die **Email Daily Digest nach** wird mit einem orangefarbenen Rahmen angezeigt, um anzugeben, dass die Versandzeit bearbeitet wurde.

   Die tägliche Zusammenfassung enthält Ereignisse, die die Kriterien der Benachrichtigungen 24 Stunden vor dem ausgewählten Zeitpunkt erfüllen. Benutzer erhalten für jeden Benachrichtigungstyp eine tägliche Digest-E-Mail.

   Der tägliche Digest kann nach der von Ihnen ausgewählten Zeit eintreffen, je nachdem, wie viele E-Mails in die Warteschlange für den Versand im System gestellt werden. Die angegebene Uhrzeit entspricht der Ortszeit, die Sie in den Browsereinstellungen angegeben haben.
