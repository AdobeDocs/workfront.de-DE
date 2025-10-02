---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Arbeitszeittabellen-Profile erstellen, bearbeiten und zuweisen
description: Sie können Arbeitszeittabellen-Profile erstellen, bearbeiten und zuweisen, die ohne weiteres Eingreifen von Ihnen wiederkehrende Arbeitszeittabellen für Ihre Benutzer generieren. Dies spart Ihnen Zeit und sorgt für Konsistenz zwischen den Benutzern.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 611c3c947855610cf86cdcbf96d1e9d847e34f38
workflow-type: tm+mt
source-wordcount: '1668'
ht-degree: 2%

---

# Arbeitszeittabellen-Profile erstellen, bearbeiten und zuweisen

<!--Audited: 06/2025-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau -Umgebung verfügbar und wird in einem schrittweisen Rollout in die Produktion veröffentlicht.</span>

Sie können Arbeitszeittabellen-Profile erstellen, bearbeiten und zuweisen, die ohne weiteres Eingreifen von Ihnen wiederkehrende Arbeitszeittabellen für Ihre Benutzer generieren. Dies spart Zeit und stellt sicher, dass Folgendes zwischen den Benutzern konsistent ist:

* Arbeitszeittabellen-Zeitrahmen
* Genehmigende Personen
* Allgemeine Stundentypen

Weitere Informationen zum manuellen Erstellen einer Arbeitszeittabelle finden Sie unter [Erstellen einer Arbeitszeittabelle zur einmaligen Verwendung](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen administrativen Zugriff auf Arbeitszeittabellen haben. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeitszeittabellen-Profil erstellen oder bearbeiten

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Um Arbeitszeittabellen-Profiländerungen in aktuellen Arbeitszeittabellen zu aktivieren, müssen Sie zunächst die vorhandenen Arbeitszeittabellen löschen, bevor Sie die Änderungen an den Arbeitszeittabellen-Profilen vornehmen, und dann neue Arbeitszeittabellen erstellen. Anweisungen finden Sie unter [Arbeitszeittabellen in Adobe Workfront löschen](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) und [Arbeitszeittabellen manuell generieren](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Wenn Sie ein Arbeitszeittabellen-Profil zur Verwendung im gesamten System erstellen oder bearbeiten, klicken Sie auf **Arbeitszeittabelle und Stunden**.

   Oder

   Wenn Sie ein Arbeitszeittabellen-Profil für eine Gruppe erstellen oder bearbeiten, klicken Sie auf **Gruppen** und dann auf den Namen der Gruppe.

1. Klicken Sie **Arbeitszeittabellen-Profile**.
1. Um ein Arbeitszeittabellen-Profil zu erstellen, klicken Sie auf **Neues Profil**.

   Oder

   Um ein vorhandenes Arbeitszeittabellen-Profil zu bearbeiten, wählen Sie das zu bearbeitende Arbeitszeittabellen-Profil aus und klicken Sie dann auf **Bearbeiten**.

   Die Seite mit dem neuen oder vorhandenen Arbeitszeittabellen-Profil wird angezeigt.

1. Aktualisieren Sie die folgenden Informationen:

   * **Name**: Fügen Sie einen Namen für das Arbeitszeittabellen-Profil hinzu. Dabei kann es sich um den Namen eines Teams oder einer Gruppe handeln, dessen Personen für ihre Arbeitszeittabellen denselben Zeitrahmen verwenden. Dies ist ein Pflichtfeld.
   * **Beschreibung**: Fügen Sie weitere Informationen zum Arbeitszeittabellen-Profil hinzu.
   * **Mit Administratorzugriff gruppieren**: Wenn Sie ein Arbeitszeittabellen-Profil auf Systemebene erstellen, lassen Sie dieses Feld leer.

     Jeder Benutzer, der Benutzerkonten bearbeiten kann, kann anderen Benutzern eine Arbeitszeittabelle auf Systemebene anhängen.

     Nur ein Workfront-Administrator kann ein Arbeitszeittabellen-Profil auf Systemebene bearbeiten.

     Wenn Sie ein Arbeitszeittabellen-Profil für eine von Ihnen verwaltete Gruppe erstellen, identifizieren Sie die Gruppe hier.

     Dadurch wird das Arbeitszeittabellen-Profil nicht den Benutzenden in der Gruppe zugewiesen, sondern nur den Gruppenadministratoren, das Arbeitszeittabellen-Profil zu ändern. Sie weisen das Profil in Schritt 6 Benutzern zu.

     >[!NOTE]
     >
     >Wenn Benutzende außerhalb der Gruppe Arbeitszeittabellen-Profile an andere Benutzende anhängen, können sie dieses Arbeitszeittabellen-Profil nicht anzeigen oder anhängen.

   * **Arbeitszeittabellen erstellen**: Geben Sie an, wann das Arbeitszeittabellenprofil die Arbeitszeittabellen generieren soll. Eine Arbeitszeittabelle kann so eingerichtet werden, dass sie automatisch auf wöchentlicher, zweiwöchentlicher, halbmonatlicher oder monatlicher Basis generiert wird. Wählen Sie den Wochentag aus, an dem die Arbeitszeittabelle erstellt werden soll.

     Eine wöchentliche Arbeitszeittabelle beginnt mit dem Datum ihrer Erstellung. Wenn Sie beispielsweise wöchentliche Arbeitszeittabellen jeden Donnerstag erstellen, ist der erste Wochentag auf der Arbeitszeittabelle Donnerstag.

     >[!NOTE]
     >
     >Workfront erstellt immer zwei Arbeitszeittabellen gleichzeitig: Die erste Arbeitszeittabelle enthält immer das aktuelle Datum, und die zweite Arbeitszeittabelle beginnt, wenn der Zeitrahmen der ersten endet.

   * **Genehmiger**: Genehmigende Personen sind Benutzer, die die Arbeitszeittabelle für die mit der Arbeitszeittabelle verknüpften Benutzer genehmigen. Sie können bis zu 7 Benutzer in einer Arbeitszeittabelle als genehmigende Personen angeben. Die Identifizierung mehrerer Benutzer ist nützlich, um sicherzustellen, dass eine genehmigende Person verfügbar ist, wenn jemand abwesend ist. Alle genehmigenden Personen werden benachrichtigt, wenn ein Benutzer die Arbeitszeittabelle zur Genehmigung einreicht. Nur ein Benutzer muss die Arbeitszeittabelle genehmigen, damit sie genehmigt werden kann.

     Nur Benutzer mit Verwaltungsrechten für Arbeitszeittabellen können als genehmigende Personen festgelegt werden. Weitere Informationen zu Arbeitszeittabellen-Administratorrechten finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Wählen Sie im Dropdown-Menü die genehmigende Person für die Arbeitszeittabelle aus (wenn eine genehmigende Person erforderlich ist). Sie können aus den folgenden Optionen auswählen:

      * **Keine**: Die Arbeitszeittabelle muss nicht genehmigt werden.
      * **Ihr Manager**: Dies ist die vom System festgelegte standardmäßige genehmigende Person. In diesem Fall genehmigt der als Manager benannte Benutzer die Arbeitszeittabelle, wenn sie zur Genehmigung eingereicht wird.
      * **Spezifische Personen**: Sie können bestimmte Benutzer bzw. Benutzerinnen nach Namen als Arbeitszeittabellen-Genehmiger bzw. -Genehmigerinnen bestimmen. Eine Arbeitszeittabelle kann mehrere genehmigende Personen enthalten. Wenn eine der genehmigenden Personen die Arbeitszeittabelle genehmigt hat, wird diese als &quot;**&quot;** und verschwindet aus der Liste der Arbeitszeittabellen-Genehmigungen aller verbleibenden genehmigenden Personen.

   * **Kann die Zeit bearbeiten**: Wählen Sie diese Option aus, damit die genehmigenden Personen Stunden auf der Arbeitszeittabelle bearbeiten können.

     Diese Option funktioniert zusammen mit der Einstellung **Bearbeitung von Arbeitszeittabellen auf Inhaber und Administratoren beschränken** im Bereich Setup > Arbeitszeittabellen und Stunden > Voreinstellungen. Weitere Informationen finden Sie unter [Arbeitszeittabelle und Stundenvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     Die folgenden Szenarien sind vorhanden:

     Wenn die **Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken** aktiviert ist:

      * Genehmigende Personen können Arbeitszeittabellen nur genehmigen und ablehnen, unabhängig davon, ob die Option Zeit bearbeiten aktiviert ist oder nicht.
      * Die Manager der Arbeitszeittabellen-Besitzer können nur die Arbeitszeittabellen ihrer direkt unterstellten Mitarbeiter anzeigen.

     Wenn die **Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken** deaktiviert ist:

      * Wenn **Kann die Zeit bearbeiten** aktiviert ist, können die genehmigenden Personen die Arbeitszeittabelle senden, erneut öffnen oder schließen und die Zeit bearbeiten.
      * Wenn **Kann die Zeit bearbeiten** deaktiviert ist, können die genehmigenden Personen die Arbeitszeittabelle nicht senden, erneut öffnen oder schließen und auch die Zeit nicht bearbeiten. Genehmigende Personen können die Arbeitszeittabelle nur genehmigen oder ablehnen.
      * Die Manager von Arbeitszeittabellen-Besitzern können die Arbeitszeittabellen ihrer direkt unterstellten Mitarbeiter senden, zurückrufen, erneut öffnen und bearbeiten.

     >[!NOTE]
     >
     >Nachdem Sie eine Arbeitszeittabelle zur Genehmigung eingereicht haben, können Sie die Stunden nicht mehr bearbeiten. Um eine übermittelte Arbeitszeittabelle in den bearbeitbaren Status zurückzuversetzen, rufen Sie die Arbeitszeittabelle zurück oder bitten Sie die genehmigende Person, die Arbeitszeittabelle abzulehnen. Weitere Informationen finden Sie unter [Arbeitszeittabelle zur Genehmigung einreichen](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) und [Arbeitszeittabelle genehmigen](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md).

   * **Überstunden**: Sie können das Feld „Überstunden“ in den Arbeitszeittabellen ausblenden. Standardmäßig ist diese Option deaktiviert.
   * **Verfügbare Stundentypen**: Diese Einstellung bezieht sich nur auf allgemeine Stundentypen und nicht auf projektspezifische Stundentypen.

     Standardmäßig sehen Benutzer alle allgemeinen Stunden auf einer Arbeitszeittabelle. Wenn Ihr Unternehmen jedoch möchte, dass nur bestimmte allgemeine Stunden für eine bestimmte Benutzergruppe angezeigt werden, können Sie die allgemeinen Stunden auswählen, die in den Arbeitszeittabellen angezeigt werden sollen, indem Sie sie in diesem Feld in ihrem Arbeitszeittabellen-Profil auswählen. Wenn Sie alle allgemeinen Stunden deaktivieren möchten, heben Sie die Auswahl aller Stundentypen auf, um die Arbeitszeittabelle ohne Abschnitt für allgemeine Stunden zu erstellen.

   * **Erinnerungsnachrichten**: Fügen Sie eine Erinnerungsnachricht hinzu. Workfront sendet Benutzern Erinnerungen, damit diese ihre Arbeitszeittabellen ausfüllen oder genehmigen können. Sie müssen Erinnerungsnachrichten erstellen, bevor Sie sie mit einem Arbeitszeittabellen-Profil verknüpfen können.

1. Klicken Sie beim Erstellen von Arbeitszeittabellen-Profilen auf Gruppenebene in der Produktionsumgebung auf die Registerkarte **Personen zuweisen**, um das Arbeitszeittabellen-Profil bestimmten Benutzenden, Gruppen oder (wenn Sie Workfront-Administrator sind) Teams zuzuordnen. <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   <span class="preview">Scrollen Sie beim Erstellen von Arbeitszeittabellen-Profilen auf Gruppenebene in der Vorschau zum unteren Seitenrand und suchen Sie den Abschnitt **Personen zuweisen**.</span>

   Scrollen Sie beim Erstellen von Arbeitszeittabellen-Profilen für das System nach unten auf der Seite und suchen Sie den Abschnitt **Personen zuweisen**.

   Beginnen Sie mit der Eingabe des Namens des Benutzers, der Gruppe oder des Teams und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   Wenn Sie Gruppenadministrator sind, können Sie das Arbeitszeittabellen-Profil Gruppen zuweisen, die Sie verwalten, jedoch nicht Teams. Weitere Informationen finden Sie unter [&#x200B; für einen Gruppenadministrator beim Zuweisen eines Arbeitszeittabellen-Profils &#x200B;](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) diesem Artikel.

   >[!NOTE]
   >
   >* Sie können einen Benutzer auch mit einem Arbeitszeittabellen-Profil verknüpfen, indem Sie das Benutzerprofil bearbeiten. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Wenn Sie eine Gruppe hinzufügen, wird nur der Gruppenname auf der Registerkarte Personen zuweisen angezeigt, nicht die Liste der Gruppenmitglieder. Wenn Sie die hier aufgeführten Gruppenmitglieder sehen möchten, klicken Sie auf Änderungen speichern und dann auf den Namen des soeben erstellten Arbeitszeittabellen-Profils.
   >* Wenn Sie diese Schritte abgeschlossen haben, generiert das Arbeitszeittabellen-Profil Arbeitszeittabellen nur für die zugewiesenen Benutzer oder Gruppenmitglieder, die für den aktuellen Zeitraum keine Arbeitszeittabellen haben.

1. Klicken Sie auf **Speichern**.

1. Klicken Sie oben in der Arbeitszeittabellen-Profilliste auf das Symbol **Mehr** (![-Symbol](assets/more-icon.png) und dann auf **Arbeitszeittabellen erstellen**.

   Unten im Bildschirm wird eine Bestätigung angezeigt, dass Arbeitszeittabellen erfolgreich generiert wurden. Neue Arbeitszeittabellen werden auf der Grundlage der von Ihnen erstellten neuen Profile generiert.

   Weitere Informationen finden Sie unter [Arbeitszeittabellen manuell generieren](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   Wenn das Arbeitszeittabellen-Profil zum ersten Mal Arbeitszeittabellen generiert, werden für jeden Benutzer zwei Arbeitszeittabellen erstellt, und zwar sowohl für den Zeitrahmen, der die aktuelle Zeit enthält, als auch für den folgenden Zeitrahmen.

   Danach wird jedes Mal, wenn neue Arbeitszeittabellen erstellt werden, eine Arbeitszeittabelle pro Benutzer erstellt.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Einschränkungen für die Zuweisung eines Arbeitszeittabellen-Profils durch einen Gruppenadministrator {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Wenn Sie Gruppenadministrator sind und die Zugriffsoption „Arbeitszeittabellen und Stunden“ auf Ihrer Zugriffsebene deaktiviert ist, können Sie Arbeitszeittabellen-Profile erstellen, diese jedoch nur folgenden Benutzern zuweisen:

* Von Ihnen verwaltete Gruppen
* Einzelne Benutzende, die Sie bearbeiten können und die sich in einer von Ihnen verwalteten Gruppe befinden

Für diese Gruppen und Benutzer haben Sie keinen Zugriff auf die Arbeitszeittabellen, die das Arbeitszeittabellen-Profil generiert.

Wenn außerdem die Option Benutzerverwaltung (Gruppenbenutzer) auf Ihrer Zugriffsebene deaktiviert ist, können Sie das Arbeitszeittabellen-Profil einer von Ihnen verwalteten Gruppe zuweisen, dies wirkt sich jedoch nur auf die Benutzer in der Gruppe aus, auf die Sie Zugriff haben, um es zu bearbeiten. Wenn die Gruppe Benutzer enthält, auf die Sie keinen Zugriff haben, um sie zu bearbeiten, wird ihnen das Arbeitszeittabellen-Profil nicht zusammen mit dem Rest der Gruppe zugewiesen.

Informationen zur Option Arbeitszeittabellen und Stunden in Ihrer Zugriffsebene finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Informationen zur Option Benutzeradmin. (Gruppenbenutzer) in Ihrer Zugriffsebene finden Sie unter [Gewähren des Zugriffs für Benutzer](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Mehrere wiederkehrende Arbeitszeittabellen-Profile

Sie können über mehr als ein Arbeitszeittabellen-Profil für Ihre Organisation verfügen, wenn Folgendes zutrifft:

* Eindeutige Zahlungszeiträume für verschiedene Benutzergruppen
* Eindeutige genehmigende Personen für verschiedene Benutzergruppen
* Eindeutige allgemeine Stundenanforderungen für verschiedene Benutzergruppen

Ein Benutzer kann nicht gleichzeitig mit mehr als einem Arbeitszeittabellen-Profil verknüpft werden.

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->