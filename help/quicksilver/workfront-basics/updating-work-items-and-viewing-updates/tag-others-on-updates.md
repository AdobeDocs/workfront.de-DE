---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Tagging anderer Benutzer auf Updates
description: Wenn Sie Aktualisierungskommentare für ein Adobe Workfront-Objekt bereitstellen, können alle Benutzer des Projekts die übermittelten Informationen sehen. Es kann jedoch vorkommen, dass Benutzer, die nicht am Projekt teilnehmen, von der Anzeige dieser Informationen profitieren. Anstatt diese Benutzer in das Projekt aufzunehmen, können Sie sie in der Aktualisierung mit Tags versehen, um sie für sie freizugeben. Mit Tags versehene Benutzer erhalten eine Ereignisbenachrichtigung.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 4c17466705873b06e7ea7bb08bb78a7e68078f8b
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# Tagging anderer Benutzer auf Updates

<!--Audited: April, 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

Sie können Benutzer taggen, wenn Sie ein Objekt aktualisieren, wenn Sie deren Aufmerksamkeit auf ein Objekt lenken möchten, dem sie andernfalls möglicherweise nicht folgen.

Anstatt diese Benutzer in das Objekt einzuschließen, indem Sie sie ihm zuweisen oder sie dazu zwingen, es zu abonnieren, können Sie sie auf der Aktualisierung mit Tags versehen, um sie für sie freizugeben. Mit Tags versehene Benutzer erhalten eine Workfront-Benachrichtigung über die von Ihnen eingegebene Aktualisierung. Abhängig von den Benachrichtigungseinstellungen erhalten sie auch eine E-Mail über die von Ihnen eingegebene Aktualisierung.

## Überlegungen zum Tagging von Benutzern in Updates

* Benutzer, die in Updates getaggt wurden, müssen in ihrem Profil eine persönliche Benachrichtigung aktivieren, damit sie die E-Mail-Benachrichtigung erhalten. Weitere Informationen finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Informationen zum Hinzufügen von Aktualisierungen zu Workfront-Objekten finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Wenn ein Problem in ein Projekt oder eine Aufgabe konvertiert wird, werden die Aktualisierungen in das neue Projekt oder die neue Aufgabe kopiert, die getaggten Benutzer jedoch nicht. Um das Gespräch fortzusetzen, müssen Sie die Teilnehmer erneut taggen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Abo</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Neu: Mitarbeiter oder höher für Probleme und Dokumente; leicht oder höher für alle anderen Objekte</p>
   <p>Aktuell: Anfrage oder höher für Probleme und Dokumente; Überprüfung oder höher für alle anderen Objekte</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfiguration der Zugriffsebene</strong></td> 
   <td> <p>Zugriff auf die Objekte anzeigen, für die Sie die Antwort posten möchten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigung</strong></td> 
   <td> <p>Anzeigen oder höherer Berechtigungen für die Objekte, in denen Sie die Antwort posten möchten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen für die Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Tagging anderer Benutzer auf Updates

Sie können andere auf Aktualisierungen wie folgt taggen:

* **Automatisch**: Wenn ein Benutzer einen Thread startet, einen Kommentar hinzufügt oder eine Antwort hinzufügt, wird er automatisch mit Tags versehen und zum Bereich Personen oder Teams des Kommentarfelds hinzugefügt.

  >[!TIP]
  >
  >   Benutzer können nicht automatisch getaggt werden, wenn Sie einen Kommentar zu einer Iteration hinzufügen.  Weitere Informationen finden Sie unter [Iterationskommentare verwalten](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md). \
  >Benutzer können nicht automatisch getaggt werden, wenn Sie einen Kommentar aus anderen Anwendungen hinzufügen.


* **Manuell**: Wenn Sie einen Benutzer manuell zum Bereich Personen taggen des Kommentarfelds hinzufügen.

Sie können auch Benutzer entfernen, die versehentlich mit Tags versehen wurden, wenn Sie einen Kommentar bearbeiten oder darauf antworten.

1. Beginnen Sie mit der Aktualisierung eines Arbeitselements, wie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Als Eigentümer des Kommentars werden Sie automatisch mit Tags versehen und dem Bereich Personen oder Teams des Kommentarfelds hinzugefügt.

   >[!TIP]
   >
   >Der Eigentümer des Kommentars kann seinen eigenen Namen nicht im Bereich &quot;Personen taggen&quot;oder &quot;Teams&quot;des Kommentarfelds sehen.

1. Im **Personen oder Teams taggen** eingeben, den Namen des Benutzers oder Teams eingeben, den Sie einbeziehen möchten, und auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   Oder

   Geben Sie das @-Symbol in die **Kommentar schreiben** eingeben, den Namen des Benutzers oder Teams eingeben, den Sie in die Aktualisierung aufnehmen möchten, und dann auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   > 
   >Um den richtigen Benutzer zu identifizieren, wenn es Benutzer mit ähnlichen oder identischen Namen gibt, beachten Sie den Avatar, die Primäre Rolle des Benutzers oder dessen E-Mail-Adresse.
   > 
   >Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Taggen in einer Aktualisierung angezeigt werden können.
   > 
   >Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Benutzern Zugriff gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![Benutzer taggen](assets/tag-others-unified-commenting-with-all-tab.png)

1. (Optional) Um die Aktualisierung privat zu machen, aktivieren Sie **Privatperson in meinem Unternehmen** in der rechten unteren Ecke des Aktualisierungsfelds. Dadurch wird die Aktualisierung nur für Benutzer in Ihrem Unternehmen sichtbar. Die **Privatperson in meinem Unternehmen** ist nur verfügbar, wenn in Ihrem Workfront-Profil ein Unternehmen angegeben ist.

   >[!NOTE]
   >
   >* Diese Option wird nur angezeigt, wenn der Benutzer mit einem Unternehmen verknüpft ist.
   >* Mit Tags versehene Benutzer außerhalb des Unternehmens können weiterhin eine In-App-Benachrichtigung oder E-Mail erhalten, auch wenn sie die privaten Kommentare nicht auf der Registerkarte Updates sehen. Es wird empfohlen, keine externen Benutzer bei einer Aktualisierung zu taggen, wenn Sie die Informationen nicht für sie freigeben möchten.

1. (Optional) Wiederholen Sie Schritt 2, um mehrere Benutzer und Teams hinzuzufügen. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Alle im Feld &quot;Personen oder Teams taggen&quot;aufgelisteten Benutzer und Teammitglieder erhalten eine In-App-Benachrichtigung zu der Aktualisierung und erhalten je nach Konfiguration ihrer E-Mail-Benachrichtigungseinstellungen eine E-Mail. Benutzer, die sich in einem Kommentar oder einer Antwort taggen, erhalten eine Benachrichtigung zu diesem Kommentar oder dieser Antwort und können ihren Namen für den Rest des Threads als Mitglied des Threads in der Liste sehen. Sie erhalten jedoch keine weitere Benachrichtigung, es sei denn, sie taggen sich selbst. Weitere Informationen finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) und [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klicks **Einsenden**.\
   Benutzer, die in der Aktualisierung enthalten sind, erhalten automatisch die Berechtigung zum Anzeigen des Objekts und können Aktualisierungen anzeigen und auf diese reagieren.

   Die Namen der getaggten Entitäten werden neben ihren Avataren bis zu zwei Entitäten angezeigt. Wenn mehr als zwei Entitäten mit Tags versehen sind, wird neben einer Reihe weiterer Entitäten der Name der ersten angezeigt.

   ![](assets/members-icons-expanded-unshimmed.png)

   Wenn Sie im Kommentartext mit Tags versehen sind, wird Ihr Name in diesen Kommentaren hervorgehoben.

   Informationen zu den zusätzlichen Funktionen, die beim Aktualisieren eines Arbeitselements verfügbar sind, finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Optional) Klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) in der oberen rechten Ecke des Kommentars klicken Sie auf **Bearbeiten**. Entfernen Sie alle getaggten Benutzer und klicken Sie auf **Einsenden**.

   >[!IMPORTANT]
   >
   >Sie können einen Kommentar nur innerhalb von 15 Minuten nach seiner Eingabe bearbeiten. Sie können nur die hinzugefügten Kommentare bearbeiten.


<!--
   >[!TIP]
   >
   >When using the legacy commenting experience to add comments and replies, comment owners that were not specifically tagged cannot be manually removed by people who use the new commenting experience.
-->

<!--
### Tag others on updates in the legacy Updates section

You can manually tag users in the legacy Updates section. 

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Notify** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list.

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. 
   >
   >Users must be associated with at least one job role to view it as you tag them in an update. 
   >
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company. The **Private to my company** option is available only when a Company is specified in your Workfront profile. 

   >[!NOTE]
   >
   >Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them.  

1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the Notify field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in the Notify field for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Update**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply at the top of the update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.

   ![](assets/tagging-transparency-350x192.png)
-->

Informationen zu den zusätzlichen Funktionen, die beim Aktualisieren eines Arbeitselements verfügbar sind, finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



