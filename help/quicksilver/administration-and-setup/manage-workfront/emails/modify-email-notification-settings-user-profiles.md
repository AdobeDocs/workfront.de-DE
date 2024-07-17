---
user-type: administrator
product-area: system-administration
keywords: modify,email,notification,settings,bulk,bulk,edit,configure,multiple,users
navigation-topic: emails-administration
title: E-Mail-Benachrichtigungseinstellungen mehrerer Benutzer ändern
description: Dieser Artikel enthält Informationen für Workfront- oder Gruppenadministratoren darüber, wie sie die E-Mail-Benachrichtigungen anderer Benutzer aktualisieren können.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# E-Mail-Benachrichtigungseinstellungen mehrerer Benutzer ändern

<!-- Audited: 12/2023 -->

Wenn Sie Adobe Workfront-Administrator sind oder über die Zugriffsebene &quot;Planer&quot;verfügen, mit der Sie die Einstellungen anderer Benutzer bearbeiten können, können Sie die Benachrichtigungseinstellungen für mehrere Benutzer gleichzeitig konfigurieren. Dazu gehört auch die Angabe, ob Benutzer Benachrichtigungen bei Ereignissen erhalten oder in einer täglichen Digest-E-Mail, wie in [Adobe Workfront-Benachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md) beschrieben. Weitere Informationen zur Zugriffsstufe, die zum Bearbeiten von Benutzern erforderlich ist, finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Sie können auch E-Mail-Benachrichtigungen für jeweils einen Benutzer konfigurieren, einschließlich Ihres eigenen Profils. Weitere Informationen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neuer Plan: Standard </p>
 <p>oder</p> 
<p>Aktueller Plan: Plan </p> 
</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## E-Mail-Benachrichtigungseinstellungen für mehrere Benutzer ändern

Wenn Sie die Benachrichtigungseinstellungen stapelweise konfigurieren, können Sie nur die Einstellungen ändern, die den ausgewählten Benutzern gemeinsam sind.

Wenn Sie eine Benachrichtigungseinstellung ändern, wird für diese Benachrichtigungseinstellung die Bezeichnung **Bearbeitet** angezeigt, um Sie darüber zu informieren, dass diese Benachrichtigungseinstellung geändert wurde.

So ändern Sie die E-Mail-Benachrichtigungseinstellungen für mehrere Benutzer:

{{step-1-to-users}}

1. Wählen Sie die Benutzer aus und klicken Sie dann auf **Bearbeiten**.
1. Klicken Sie im angezeigten Feld **Person bearbeiten** auf **Benachrichtigungen**.

1. Erweitern Sie eine Kategorie, um Benachrichtigungseinstellungen zu dieser Kategorie anzuzeigen.

   Wenn mindestens ein Benutzer ausgewählt ist, bei dem die Benachrichtigungen nicht mit den Benachrichtigungen der anderen ausgewählten Benutzer übereinstimmen, enthält das Kategorieprüffeld für diese Benachrichtigung eine horizontale Zeile ![](assets/straight-line-instead-of-checkmark.jpg) anstelle eines Kontrollkästchens.


1. Klicken Sie auf alle Benachrichtigungen, die die Benutzer täglich oder sofort erhalten sollen, oder löschen Sie alle Benachrichtigungen, die sie nicht mehr erhalten sollen.

   >[!NOTE]
   >
   >   In der Kategorie **Kommunikation** können Sie einzelne Benachrichtigungen nur für den sofortigen Versand auswählen. Sie müssen alle Benachrichtigungen auswählen, die täglich versendet werden sollen.


1. Wenn Sie Benachrichtigungen als täglichen Digest ausgewählt haben, wählen Sie oben im Abschnitt **Benachrichtigungen** im Menü **Tägliche Digest per E-Mail nach** die Uhrzeit aus, zu der die Digest-Versendung durchgeführt werden soll.

   ![](assets/daily-digest-time.png)

   Die tägliche Zusammenfassung enthält Ereignisse, die die Kriterien der Benachrichtigungen 24 Stunden vor dem ausgewählten Zeitpunkt erfüllen. Benutzer erhalten für jeden Benachrichtigungstyp eine tägliche Digest-E-Mail.

   Der tägliche Digest kann nach der von Ihnen ausgewählten Zeit eintreffen, je nachdem, wie viele E-Mails in die Warteschlange für den Versand im System gestellt werden. Die angegebene Uhrzeit entspricht der Ortszeit, die Sie in den Browsereinstellungen angegeben haben.
