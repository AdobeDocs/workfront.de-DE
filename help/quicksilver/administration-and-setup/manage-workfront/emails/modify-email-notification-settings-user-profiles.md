---
user-type: administrator
product-area: system-administration
keywords: Ändern,E-Mail,Benachrichtigung,Einstellungen,Bulk,Bulk-Edit,Konfigurieren,Mehrere,Benutzer
navigation-topic: emails-administration
title: Ändern der E-Mail-Benachrichtigungseinstellungen mehrerer Benutzer
description: Dieser Artikel enthält Informationen für Workfront- oder Gruppenadministratoren darüber, wie sie die E-Mail-Benachrichtigungen anderer Benutzer aktualisieren können.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# Ändern der E-Mail-Benachrichtigungseinstellungen mehrerer Benutzer

<!-- Audited: 12/2023 -->

Wenn Sie Adobe Workfront-Administrator sind oder über eine Zugriffsebene für Planer verfügen, mit der Sie die Einstellungen anderer Benutzender bearbeiten können, können Sie die Benachrichtigungseinstellungen für mehrere Benutzende gleichzeitig konfigurieren. Dazu gehört auch die Angabe, ob Benutzer Benachrichtigungen erhalten, wenn Ereignisse eintreten, oder in einer täglichen Digest-E-Mail, wie in [Adobe Workfront-Benachrichtigungen](../../../workfront-basics/using-notifications/wf-notifications.md) beschrieben. Informationen zur Zugriffsebene, die zum Bearbeiten von Benutzern benötigt wird, finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Sie können auch E-Mail-Benachrichtigungen für jeweils einen Benutzer konfigurieren, einschließlich Ihres eigenen Profils. Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## E-Mail-Benachrichtigungseinstellungen für mehrere Benutzer ändern

Wenn Sie Benachrichtigungseinstellungen stapelweise konfigurieren, können Sie nur die Einstellungen ändern, die die ausgewählten Benutzer gemeinsam haben.

Wenn Sie eine Benachrichtigungseinstellung ändern, wird für diese Benachrichtigungseinstellung **Titel &quot;**&quot; angezeigt, um Sie darüber zu informieren, dass diese Benachrichtigungseinstellung geändert wurde.

So ändern Sie E-Mail-Benachrichtigungseinstellungen für mehrere Benutzer:

{{step-1-to-users}}

1. Wählen Sie die Benutzer aus und klicken Sie dann auf **Bearbeiten**.
1. Klicken Sie im **Person bearbeiten** auf **Benachrichtigungen**.

1. Erweitern Sie eine Kategorie, um Benachrichtigungseinstellungen anzuzeigen, die sich auf diese Kategorie beziehen.

   Wenn mindestens ein Benutzer aktiviert wurde und die Benachrichtigungen nicht mit den Benachrichtigungen der anderen ausgewählten Benutzer übereinstimmen, enthält das Kontrollkästchen Kategorie für diese Benachrichtigung eine horizontale Linie ![Linie anstelle &#x200B;](assets/straight-line-instead-of-checkmark.jpg) Kontrollkästchens.


1. Klicken Sie auf eine Benachrichtigung, die Benutzerinnen und Benutzer entweder täglich oder sofort erhalten sollen, oder löschen Sie alle Benachrichtigungen, die sie nicht mehr erhalten sollen.

   >[!NOTE]
   >
   >   Für die Kategorie **Kommunikation** können Sie einzelne Benachrichtigungen nur für den sofortigen Versand auswählen. Sie müssen alle Benachrichtigungen auswählen, die in einer täglichen Zusammenfassung zugestellt werden sollen.


1. Wenn Sie Benachrichtigungen als tägliche Zusammenfassung gesendet haben, wählen Sie die Tageszeit, zu der die Zusammenfassung zugestellt werden soll, oben im Abschnitt **Benachrichtigungen** im Menü **Tägliche Zusammenfassung nach** aus.

   ![Tägliche Digest-Zeit](assets/daily-digest-time.png)

   Die tägliche Zusammenfassung enthält Ereignisse, die den Kriterien der Benachrichtigungen 24 Stunden vor der ausgewählten Zeit entsprechen. Benutzende erhalten für jeden Benachrichtigungstyp eine tägliche Digest-E-Mail.

   Die tägliche Zusammenfassung kann nach der von Ihnen ausgewählten Zeit eintreffen, je nachdem, wie viele E-Mails im System für den Versand in die Warteschlange gestellt werden. Die aufgelistete Zeit ist die Ortszeit, die in Ihren Browser-Einstellungen angegeben ist.
