---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen
description: Sie können Timesheet-Profile erstellen, bearbeiten und zuweisen, die wiederkehrende Timesheets für Ihre Benutzer generieren, ohne dass Sie weitere Eingriffe vornehmen müssen. Dadurch sparen Sie Zeit und stellen sicher, dass die folgenden Elemente zwischen Benutzern konsistent sind - BEARBEITEN SIE MICH.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 7e2a4b02277e8b82ac6ee92a7994250fcdebb0b0
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 1%

---

# Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen

Sie können Timesheet-Profile erstellen, bearbeiten und zuweisen, die wiederkehrende Timesheets für Ihre Benutzer generieren, ohne dass Sie weitere Eingriffe vornehmen müssen. Dadurch sparen Sie Zeit und stellen sicher, dass die folgenden Punkte für alle Benutzer einheitlich sind:

* Zeitrahmen des Zeitplans
* Genehmigende Personen
* Allgemeine Stundentypen

Weitere Informationen zum manuellen Erstellen eines Zeitblatts finden Sie unter [Erstellen eines Datenblatts für die einmalige Verwendung](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen über Administratorzugriff auf Timesheets verfügen. </p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p>  <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen oder Bearbeiten eines Zeitleistenprofils

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Um Profiländerungen in aktuellen Timesheets zu aktivieren, müssen Sie die vorhandenen Timesheets löschen und dann neue erstellen. Anweisungen finden Sie unter [Löschen von Timesheets in Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) und [Manuelles Generieren von Timesheets](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Wenn Sie ein Timesheet-Profil für die Verwendung im gesamten System erstellen oder bearbeiten, klicken Sie auf **Datenblatt und Stunden**.

   Oder

   Wenn Sie ein Timesheet-Profil für eine Gruppe erstellen oder bearbeiten, klicken Sie auf **Gruppen** und klicken Sie dann auf den Namen der Gruppe.

1. Klicken **Datenblatt-Profile**.
1. Um ein neues Zeitleistenprofil zu erstellen, klicken Sie auf **Neues Profil**.

   Oder

   Um ein vorhandenes Timesheet-Profil zu bearbeiten, wählen Sie das zu bearbeitende Timesheet-Profil aus und klicken Sie auf **Bearbeiten**.

   Das neue oder vorhandene Timesheet-Profil wird angezeigt.


1. Im **Details festlegen** tab, geben Sie eine **Name** und **Beschreibung** für das Timesheet-Profil und geben Sie folgende Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Gruppe mit Administratorzugriff</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Wenn Sie ein Timesheet-Profil auf Systemebene erstellen, lassen Sie dieses Feld leer.</p> <p>Jeder Benutzer, der Benutzerkonten bearbeiten kann, kann ein Timesheet auf Systemebene an andere Benutzer anhängen.</p> <p>Nur ein Workfront-Administrator kann ein Timesheet-Profil auf Systemebene bearbeiten.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Wenn Sie ein Timesheet-Profil für eine von Ihnen verwaltete Gruppe erstellen, identifizieren Sie die Gruppe hier.</p> <p>Dadurch wird den Benutzern in der Gruppe nicht das Timesheet-Profil zugewiesen. Sie ermöglicht es nur den Administratoren der Gruppe, das Timesheet-Profil zu ändern. Sie weisen das Profil den Benutzern in Schritt 6 zu.</p> <p><b>NOTIZ</b>

   Wenn Benutzer außerhalb der Gruppe Timesheet-Profile an andere Benutzer anhängen, können sie dieses Timesheet-Profil nicht sehen oder anhängen.</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Arbeitszeittabellen erstellen</strong> </td> 
      <td> <p> <p>Geben Sie an, wann das Timesheet-Profil die Timesheets generieren soll. Ein Zeitblatt kann so eingestellt werden, dass es automatisch wöchentlich, zweimal wöchentlich, halbmonatlich oder monatlich generiert wird. Wählen Sie den Wochentag aus, an dem das Datenblatt erstellt werden soll.</p> <p><b>NOTIZ</b>

   Wenn Sie ein Timesheet-Profil konfigurieren, um an einem Freitag Timesheets zu erstellen, können Benutzer für die aktuelle Woche keine Stunden am Freitag, Samstag und Sonntag aufzeichnen.</p> <p>Workfront erstellt immer zwei Timesheets auf einmal: Das erste Timesheet enthält immer das aktuelle Datum und das zweite Timesheet beginnt mit dem Ende des ersten Zeitrahmens.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Genehmigende Personen</strong></p> </td> 
      <td> <p> <p>Genehmiger sind Benutzer, die das Timesheet für die mit dem Timesheet verknüpften Benutzer validieren. Sie können bis zu 7 Benutzer als Genehmiger auf einem Zeitblatt identifizieren. Die Identifizierung mehrerer Benutzer ist nützlich, um sicherzustellen, dass ein Genehmiger verfügbar ist, wenn ein Benutzer nicht im Büro ist. Alle Genehmiger werden benachrichtigt, wenn ein Benutzer das Datenblatt zur Genehmigung einreicht. Nur ein Benutzer muss das Datenblatt validieren, damit es genehmigt werden kann.</p> <p>Als Genehmiger können nur Benutzer mit Zeitblatt-Administratorrechten festgelegt werden. Weitere Informationen zu den Verwaltungsrechten für Zeitblätter finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> <p>Wählen Sie im Dropdown-Menü den Genehmiger für das Zeitblatt aus (falls ein Genehmiger erforderlich ist). Sie können aus den folgenden Optionen auswählen:</p> 
      <ul> 
      <li><strong>Keines</strong>: Das Timesheet muss nicht genehmigt werden.</li> 
      <li><strong>Ihr Manager</strong>: Dies ist der standardmäßige Genehmiger, der vom System festgelegt wird. In diesem Fall genehmigt der Benutzer, der als Manager benannt wurde, das Datenblatt, wenn es zur Genehmigung eingereicht wird.</li> 
      <li><strong>Spezifische Personen:</strong> Sie können bestimmte Benutzer nach Namen als Timesheet-Genehmiger festlegen. Sie können mehrere Genehmiger auf einem Zeitblatt haben. In diesem Fall wird das Timesheet nach Genehmigung durch einen der Genehmiger als <strong>Geschlossen</strong> und wird aus der Liste der Zeitdatenblatt-Genehmigungen aller verbleibenden Genehmiger entfernt.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Kann Zeit bearbeiten </strong> </td> 
      <td> <p> <p>Wählen Sie diese Option aus, damit die Genehmiger Stunden auf dem Zeitblatt bearbeiten können.

   Diese Option funktioniert zusammen mit dem **Beschränken der Bearbeitung von Zeitblättern auf Eigentümer und Administratoren** im Bereich Einstellungen > Timesheet &amp; Stunden > Voreinstellungen . Weitere Informationen finden Sie unter <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Zeitblatt- und Stundenvoreinstellungen konfigurieren</a>.

   Die folgenden Szenarien existieren:

   <ul>
      <li>Wenn die <b>Beschränken der Bearbeitung von Zeitblättern auf Eigentümer und Administratoren</b> -Option aktiviert ist:</li>
      <ul><li>Die Genehmiger können das Timesheet nur genehmigen und ablehnen, unabhängig davon, ob die <b>Kann die Zeit bearbeiten</b> aktiviert ist oder nicht. </li>
      <li>Die Manager der Timesheet-Eigentümer können nur die Timesheets ihrer direkt unterstellten Mitarbeiter anzeigen.</li></ul>
      <li>Wenn die <b>Beschränken der Bearbeitung von Zeitblättern auf Eigentümer und Administratoren</b> ist deaktiviert:</li>
    <ul><li>Wenn die <b>Kann die Zeit bearbeiten</b> aktiviert ist, können Genehmiger das Timesheet senden, erneut öffnen oder schließen und die Zeit bearbeiten.</li>
      <li>Wenn die <b>Kann die Zeit bearbeiten</b> deaktiviert ist, können Genehmiger das Timesheet nicht senden, erneut öffnen oder schließen und können die Zeit nicht bearbeiten. Die Validierer können das Timesheet nur genehmigen oder ablehnen. </li>
      <li>Die Manager von Timesheet-Eigentümern können die Timesheets ihrer direkt unterstellten Mitarbeiter senden, abrufen, erneut öffnen und bearbeiten.</li></ul>
      </ul>

   <p><b>NOTIZ</b>

   Sobald Sie ein Zeitblatt zur Genehmigung eingereicht haben, können Sie die Stunden nicht mehr bearbeiten. Um ein gesendetes Timesheet in einen bearbeitbaren Zustand zurückzuversetzen, rufen Sie das Timesheet auf oder lassen Sie den Genehmiger das Timesheet zurückweisen. Weitere Informationen finden Sie unter <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Zeitblatt zur Genehmigung einreichen</a> und<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Timesheet genehmigen</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Verfügbare Stundentypen</strong> </td> 
      <td>Standardmäßig sehen Benutzer alle allgemeinen Stunden auf einem Timesheet. Wenn Ihre Organisation jedoch nur bestimmte allgemeine Stunden für eine bestimmte Benutzergruppe anzeigen möchte, können Sie die allgemeinen Stunden auswählen, die sie in ihren Timesheets sehen möchten, indem Sie sie in ihrem Timesheet-Profil in diesem Feld auswählen. Wenn Sie alle allgemeinen Stunden deaktivieren möchten, deaktivieren Sie alle Stundentypen, um das Timesheet ohne Abschnitt für allgemeine Stunden zu erstellen.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Überstunden</span> </td> 
      <td>Sie können das Feld "Overtime"in Timesheets ausblenden. Diese Option ist standardmäßig deaktiviert.</td> 
     </tr> 
    </tbody> 
    </table>

1. Klicken Sie auf **Personen zuweisen** , um das Timesheet-Profil bestimmten Benutzern, Gruppen oder (falls Sie Workfront-Administrator sind) Teams zuzuordnen. Beginnen Sie mit der Eingabe des Namens des Benutzers, der Gruppe oder des Teams und klicken Sie dann auf diesen, wenn er in der Dropdown-Liste angezeigt wird.

   Wenn Sie Gruppenadministrator sind, können Sie das Profil des Zeitblatts Gruppen zuweisen, die Sie verwalten, nicht aber Teams. Weitere Informationen finden Sie unter [Einschränkungen für einen Gruppenadministrator, der ein Timesheet-Profil zuweist](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) in diesem Artikel.

   >[!NOTE]
   >
   >* Sie können einen Benutzer auch mit einem Zeitblatt-Profil verknüpfen, indem Sie das Benutzerprofil bearbeiten. Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Wenn Sie eine Gruppe hinzufügen, wird nur der Gruppenname auf der Registerkarte &quot;Personen zuweisen&quot;angezeigt, nicht die Liste der Gruppenmitglieder. Wenn Sie die hier aufgelisteten Gruppenmitglieder sehen möchten, klicken Sie auf Änderungen speichern und dann auf den Namen des soeben erstellten Timesheet-Profils.
   >* Wenn Sie diese Schritte abschließen, generiert das Timesheet-Profil nur Timesheets für die zugewiesenen Benutzer oder Gruppenmitglieder, die keine Timesheets für den aktuellen Zeitraum haben.


1. Klicken **Änderungen speichern**.

   Wenn das Timesheet-Profil zum ersten Mal Timesheets generiert, werden für jeden Benutzer zwei Timesheets erstellt. Danach wird jedes Mal, wenn neue Timesheets erstellt werden, pro Benutzer ein Timesheet erstellt.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Einschränkungen für einen Gruppenadministrator, der ein Timesheet-Profil zuweist {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Wenn Sie Gruppenadministrator sind und die Option Timesheets &amp; hours für den administrativen Zugriff in Ihrer Zugriffsebene deaktiviert ist, können Sie Zeitleistenprofile erstellen, diese jedoch nur folgenden Benutzern zuweisen:

* Von Ihnen verwaltete Gruppen
* Einzelne Benutzer, auf die Sie Zugriff haben, um sie zu bearbeiten, die sich in einer Gruppe befinden, die Sie verwalten

Für diese Gruppen und Benutzer haben Sie keinen Zugriff auf die Timesheets, die vom Timesheet-Profil erstellt werden.

Wenn die Option &quot;Benutzeradministrator (Gruppenbenutzer)&quot;auch in Ihrer Zugriffsebene deaktiviert ist, können Sie das Timesheet-Profil einer von Ihnen verwalteten Gruppe zuweisen, es betrifft jedoch nur die Benutzer in der Gruppe, auf die Sie Zugriff haben. Wenn die Gruppe Benutzer enthält, auf die Sie keinen Zugriff haben, wird ihnen nicht das Timesheet-Profil und der Rest der Gruppe zugewiesen.

Informationen zur Option Timesheets und Stunden in Ihrer Zugriffsebene finden Sie unter [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Informationen zur Option &quot;Benutzeradministrator (Gruppenbenutzer)&quot;in Ihrer Zugriffsebene finden Sie unter [Benutzern Zugriff gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Mehrere wiederkehrende Timesheet-Profile

Sie können mehr als ein Timesheet-Profil für Ihre Organisation haben, wenn Folgendes vorhanden ist:

* Eindeutige Entgeltzeiträume für verschiedene Benutzergruppen
* Eindeutige Genehmiger für verschiedene Benutzergruppen
* Unique General Hours-Anforderungen für verschiedene Benutzergruppen

Ein Benutzer kann nicht mit mehr als einem Timesheet-Profil gleichzeitig verknüpft werden. 
