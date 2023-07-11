---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Tagging anderer Benutzer auf Updates
description: Wenn Sie Aktualisierungskommentare für ein Adobe Workfront-Objekt bereitstellen, können alle Benutzer des Projekts die übermittelten Informationen sehen. Es kann jedoch vorkommen, dass Benutzer, die nicht am Projekt teilnehmen, von der Anzeige dieser Informationen profitieren. Anstatt diese Benutzer in das Projekt aufzunehmen, können Sie sie in der Aktualisierung mit Tags versehen, um sie für sie freizugeben. Tagging-Benutzer erhalten eine Ereignisbenachrichtigung.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 4116cd1610cc5b8de0407a96a4bc67532d78a25e
workflow-type: tm+mt
source-wordcount: '1485'
ht-degree: 0%

---

# Tagging anderer Benutzer auf Updates

<!--take "Beta" references out when we remove the beta-->


<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung verfügbar.

>[!NOTE]
>
>Die Kommentarerfahrung in Adobe Workfront wird derzeit umgestaltet.
>
>Weitere Informationen zum neuen Kommentierungserlebnis finden Sie unter [Neues Kommentierungserlebnis](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Für die folgenden Objekte können Sie auf das neue Erlebnis zugreifen:
> * Probleme, <span class="preview">Projekte, Aufgaben und Dokumente</span>.
>
>     Dies ist verfügbar, wenn Sie das Beta-Kommentar-Erlebnis aktivieren.
>
>     Diese Funktion ist nur für den Abschnitt Updates verfügbar und nicht für die folgenden Bereiche:
>
>     * Startseite
>     * Zusammenfassungsbereich in Listen
>     * Zusammenfassungsbereich in Timesheets
>
> * Ziele, Karten im Bereich der Foren
>
>   Das neue Kommentarerlebnis ist das einzige Erlebnis für Ziele und Karten. Sie benötigen eine zusätzliche Lizenz für den Zugriff auf Workfront Goals. Weitere Informationen finden Sie unter [Anforderungen für die Verwendung von Workfront-Zielen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     Sie können Karten im Bereich &quot;Pinnwände&quot;um Aktualisierungen ergänzen und anzeigen, wenn Sie die Abschnitte &quot;Kommentare&quot;und &quot;Systemaktivität&quot;auf einer Karte aktivieren. Weitere Informationen finden Sie unter [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](../../agile/get-started-with-boards/add-card-to-board.md).


Sie können Benutzer taggen, wenn Sie ein Objekt aktualisieren, wenn Sie deren Aufmerksamkeit auf ein Objekt lenken möchten, dem sie andernfalls möglicherweise nicht folgen.
Anstatt diese Benutzer in das Objekt einzuschließen, indem Sie sie ihm zuweisen oder sie dazu zwingen, es zu abonnieren, können Sie sie auf der Aktualisierung mit Tags versehen, um sie für sie freizugeben. Mit Tags versehene Benutzer erhalten eine Benachrichtigung über die von Ihnen eingegebene Aktualisierung.

>[!NOTE]
>
>Der Benutzer muss eine persönliche Benachrichtigung in seinem Profil aktivieren, damit er die E-Mail-Benachrichtigung erhält. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>

Informationen zum Hinzufügen von Aktualisierungen zu Workfront-Objekten finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Wenn ein Problem in ein Projekt oder eine Aufgabe konvertiert wird, werden die Aktualisierungen in das neue Projekt oder die neue Aufgabe kopiert, die getaggten Benutzer jedoch nicht. Um das Gespräch fortzusetzen, müssen Sie die Teilnehmer erneut taggen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Anfrage oder höher für Probleme und Dokumente; Überprüfen oder höher für alle anderen Objekte</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Anforderer oder höher für Probleme und Dokumente; Für alle anderen Objekte validieren oder höher</p> 
   <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf das Objekt anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Tagging anderer Benutzer auf Updates

Das Tagging anderer Benutzer in einer Aktualisierung hängt davon ab, welches Erlebnis und welches Objekt Sie auswählen.

### Taggen Sie andere auf Updates im Abschnitt &quot;Aktuelle Updates&quot;.

Sie können Benutzer im Abschnitt &quot;Aktuelle Updates&quot;manuell taggen.

1. Aktualisieren Sie ein Arbeitselement, wie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Im **Benachrichtigen** eingeben, den Namen des Benutzers oder Teams eingeben, den Sie einbeziehen möchten, und auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   Oder

   Geben Sie das @-Symbol in die **Neue Aktualisierung starten** eingeben, den Namen des Benutzers oder Teams eingeben, den Sie in die Aktualisierung aufnehmen möchten, und dann auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Um den richtigen Benutzer zu identifizieren, wenn es Benutzer mit ähnlichen oder identischen Namen gibt, beachten Sie den Avatar, die Primäre Rolle des Benutzers oder dessen E-Mail-Adresse. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Taggen in einer Aktualisierung angezeigt werden können.

   ![](assets/tag-users-in-update.png)

1. (Optional) Um die Aktualisierung privat zu machen, aktivieren Sie **Privatperson in meinem Unternehmen** in der rechten unteren Ecke des Aktualisierungsfelds. Dadurch wird die Aktualisierung nur für Benutzer in Ihrem Unternehmen sichtbar. Die **Privatperson in meinem Unternehmen** ist nur verfügbar, wenn in Ihrem Workfront-Profil ein Unternehmen angegeben ist.

   >[!NOTE]
   >
   >Mit Tags versehene Benutzer außerhalb des Unternehmens können weiterhin eine In-App-Benachrichtigung oder E-Mail erhalten, auch wenn sie die privaten Kommentare nicht auf der Registerkarte Updates sehen. Es wird empfohlen, keine externen Benutzer bei einer Aktualisierung zu taggen, wenn Sie die Informationen nicht für sie freigeben möchten.

1. (Optional) Wiederholen Sie Schritt 2, um mehrere Benutzer und Teams hinzuzufügen.

   >[!NOTE]
   >
   >Alle im Feld Benachrichtigung aufgeführten Benutzer und Teammitglieder erhalten eine In-App-Benachrichtigung zu der Aktualisierung und erhalten je nach Konfiguration ihrer E-Mail-Benachrichtigungseinstellungen eine E-Mail. Benutzer, die sich in einem Kommentar oder einer Antwort mit Tags versehen, erhalten eine Benachrichtigung zu diesem Kommentar oder dieser Antwort und können ihren Namen für den Rest des Threads im Feld Benachrichtigen anzeigen. Sie erhalten jedoch keine weitere Benachrichtigung, es sei denn, sie taggen sich selbst. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) und [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klicken **Aktualisieren**.\
   Benutzer, die in der Aktualisierung enthalten sind, erhalten automatisch die Berechtigung zum Anzeigen des Objekts und können Aktualisierungen anzeigen und auf diese reagieren.

   Oben im Aktualisierungs-Thread können Sie sehen, wer in jeder Antwort getaggt wurde. Diese Benutzer erhalten zusammen mit allen Benutzern, die das Objekt abonniert haben, eine Benachrichtigung, sobald ein Objekt aktualisiert oder beantwortet wird.

   ![](assets/tagging-transparency-350x192.png)

   Informationen zu den zusätzlichen Funktionen, die beim Aktualisieren eines Arbeitselements verfügbar sind, finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### Tagging anderer Benutzer über Aktualisierungen im Beta-Kommentarerlebnis

<!--replace the first paragraph in this section with the commented out piece when this releases to preview - July 13, 2023??

You can tag others on updates in the new commenting experience in the following ways:

* <span class="preview"> **Automatically**: When a user adds a comment or a reply, they are automatically tagged and added to the Tag people or teams area of the commenting box. </span>
* **Manually**: When you manually add a user to the Tag people area of the commenting box.

You can also remove users who are tagged by mistake when you edit or reply to a comment.-->


Sie können anderen manuell Tags für Aktualisierungen im Beta-Kommentar-Erlebnis zuweisen. Sie können auch Benutzer entfernen, die versehentlich mit Tags versehen wurden, wenn Sie einen Kommentar bearbeiten oder darauf antworten.

1. Aktualisieren Sie ein Arbeitselement, wie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). <!--<span class="preview">As the comment owner, you are automatically tagged and added to the Tag people or teams area of the commenting box. </span> -->
1. Im **Personen oder Teams taggen** eingeben, den Namen des Benutzers oder Teams eingeben, den Sie einbeziehen möchten, und auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   Oder

   Geben Sie das @-Symbol in die **Kommentar schreiben** eingeben, den Namen des Benutzers oder Teams eingeben, den Sie in die Aktualisierung aufnehmen möchten, und dann auf den Namen klicken, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Um den richtigen Benutzer zu identifizieren, wenn es Benutzer mit ähnlichen oder identischen Namen gibt, beachten Sie den Avatar, die Primäre Rolle des Benutzers oder dessen E-Mail-Adresse. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Taggen in einer Aktualisierung angezeigt werden können.

   ![](assets/tag-others-unified-commenting.png)

1. (Optional) Um die Aktualisierung privat zu machen, aktivieren Sie **Privatperson in meinem Unternehmen** in der rechten unteren Ecke des Aktualisierungsfelds. Dadurch wird die Aktualisierung nur für Benutzer in Ihrem Unternehmen sichtbar. Die **Privatperson in meinem Unternehmen** ist nur verfügbar, wenn in Ihrem Workfront-Profil ein Unternehmen angegeben ist.

   >[!NOTE]
   >
   >* Diese Option wird nur angezeigt, wenn der Benutzer mit einem Unternehmen verknüpft ist.
   >* Mit Tags versehene Benutzer außerhalb des Unternehmens können weiterhin eine In-App-Benachrichtigung oder E-Mail erhalten, auch wenn sie die privaten Kommentare nicht auf der Registerkarte Updates sehen. Es wird empfohlen, keine externen Benutzer bei einer Aktualisierung zu taggen, wenn Sie die Informationen nicht für sie freigeben möchten.

1. (Optional) Wiederholen Sie Schritt 2, um mehrere Benutzer und Teams hinzuzufügen. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Alle im Feld &quot;Personen oder Teams taggen&quot;aufgelisteten Benutzer und Teammitglieder erhalten eine In-App-Benachrichtigung zu der Aktualisierung und erhalten je nach Konfiguration ihrer E-Mail-Benachrichtigungseinstellungen eine E-Mail. Benutzer, die sich in einem Kommentar oder einer Antwort taggen, erhalten eine Benachrichtigung zu diesem Kommentar oder dieser Antwort und können ihren Namen für den Rest des Threads als Mitglied des Threads in der Liste sehen. Sie erhalten jedoch keine weitere Benachrichtigung, es sei denn, sie taggen sich selbst. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) und [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klicken **Einsenden**.\
   Benutzer, die in der Aktualisierung enthalten sind, erhalten automatisch die Berechtigung zum Anzeigen des Objekts und können Aktualisierungen anzeigen und auf diese reagieren.

   Sie können sehen, wer in jeder Antwort unter dem Text der Aktualisierung getaggt wurde, im Bereich Mitglieder . Diese Benutzer erhalten zusammen mit allen Benutzern, die das Objekt abonniert haben, eine Benachrichtigung, sobald ein Objekt aktualisiert oder beantwortet wird.
1. (Optional) Klicken Sie auf die Anzahl der **Mitglieder** in das Update aufgenommen wurde, um eine Liste von Entitäten anzuzeigen, für die die von Ihnen eingegebene Aktualisierung freigegeben wurde.

   ![](assets/members-icons-expanded-unshimmed.png)

   Informationen zu den zusätzlichen Funktionen, die beim Aktualisieren eines Arbeitselements verfügbar sind, finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Optional) Klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Symbol &quot;Gefällt mir&quot;und klicken Sie dann auf **Bearbeiten**. Entfernen Sie alle getaggten Benutzer und klicken Sie auf **Einsenden**. Sie können einen Kommentar nur innerhalb von 15 Minuten nach seiner Eingabe bearbeiten. Sie können nur die Kommentare bearbeiten, die Sie hinzugefügt haben.