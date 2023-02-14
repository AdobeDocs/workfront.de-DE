---
title: Benutzerprofil bearbeiten
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator können Sie neue Benutzer erstellen und die Profile bestehender Benutzer verwalten.
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '2557'
ht-degree: 0%

---

# Benutzerprofil bearbeiten

<!--drafted for Work Time field: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

In the table below, under Resource Planning, add the "Work Time" field and update the "FTE" field:

<b><span class="preview">Work Time</span></b>: <span class="preview">Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.</span> 

<span class="preview">The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.</span>  

<span class="preview">The system uses this number to calculate the availability of the user for actual, project-related work.</span> 

<span class="preview">For more information about creating schedules in Workfront, see Create a schedule.</span>

<span class="preview">Schedule exceptions and time off might also affect the user capacity. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)


***UPDATED FTE FIELD***

FTE: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. The FTE indicates the amount of time that the user can spend at work. This includes overhead, and  time that is not spent on project work, but on other type of work. For example, time that is spent in meetings, or training is also included in the FTE. 

The FTE must be a decimal number up to 1, and it cannot be 0. 
The field's default is 1.

For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

Schedule exceptions, time off might, <span class="preview">and the value of Work Time</span> may affect the amount of available hours or the FTE. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)

If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

For more information about creating schedules in Workfront, see Create a schedule. (*****INSERT LINK*****)
-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Anweisungen zum Bearbeiten eines Benutzerprofils in der Adobe Admin Console finden Sie im Abschnitt &quot;Benutzerdetails bearbeiten&quot;im Artikel [Benutzer einzeln verwalten](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) oder wenden Sie sich an Ihren Adobe Admin Console-Administrator.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-Administrator können Sie neue Benutzer erstellen und die Profile bestehender Benutzer verwalten. Informationen zum Erstellen von Benutzern finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Benutzer mit einer Planungslizenz können auch Benutzer erstellen und verwalten. Informationen über den für die Bearbeitung von Benutzern benötigten Zugriff finden Sie unter [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsstufe konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens eines der beiden <b>Benutzer-Admin</b> Optionen aktiviert unter <b>Einstellungen anpassen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie ein Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> <p>Weitere Informationen zum <b>Benutzer</b> auf einer Zugriffsebene festzulegen, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Bearbeiten von Benutzerprofilen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).
1. Wählen Sie den Benutzer aus und klicken Sie auf das Symbol Bearbeiten . ![](assets/edit-icon.png).

1. Im **Benutzer bearbeiten** ändern Sie die folgenden Informationen und klicken Sie auf **Änderungen speichern**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Persönliche Info </td> 
      <td> 
       <ul> 
        <li><b>Vorname</b>, <b>Nachname</b></li> 
        <li> <p><b>E-Mail-Adresse:</b> Die E-Mail-Adresse eines Benutzers ist auch sein Benutzername in Workfront. Bei diesem Feld wird zwischen Groß- und Kleinschreibung unterschieden und es muss eindeutig sein. Wenn ein Benutzer innerhalb eines 10-minütigen Fensters dreimal versucht, eine nicht eindeutige E-Mail-Adresse hinzuzufügen, wird eine reCAPTCHA-Antwort angezeigt.</p> <p>Wenn Sie die E-Mail-Zulassungsliste verwenden und eine E-Mail-Domäne eingeben, die nicht in der Liste enthalten ist, erhält der Benutzer keine E-Mail-Benachrichtigungen. Weitere Informationen zur Zulassungsliste finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Konfigurieren der E-Mail-Zulassungsliste</a>.</p> </li> 
        <li> <p><b>Kennwort zurücksetzen</b>: Klicken Sie auf diesen Link, um das Kennwort des Benutzers zurückzusetzen. Sie werden nach Ihrem eigenen Kennwort gefragt, bevor Sie das Kennwort eines Benutzers zurücksetzen können.</p> <p>Um das Kennwort eines anderen Benutzers zurückzusetzen, müssen Sie Workfront-Administrator oder Gruppenadministrator sein.</p> <p><b>NOTIZ</b>:  
          <ul> 
           <li> <p>Wenn Sie Gruppenadministrator sind, können Sie Kennwörter nur für Benutzer in den Gruppen zurücksetzen, in denen Sie als solche benannt sind. Außerdem muss die Berechtigung "Benutzeradministrator (Gruppenbenutzer)"in Ihrer Zugriffsebene aktiviert sein:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Diese Einstellung ist standardmäßig deaktiviert. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </li> 
           <li> <p>Sie können das Kennwort eines Workfront-Administrators nicht zurücksetzen.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Benutzername</b>: Wenn Ihr Workfront-Administrator eine SSO-Integration mit Workfront aktiviert hat, wird in diesem Feld der SSO-Benutzername angezeigt. In diesem Feld wird der Typ der für Ihre Workfront-Instanz aktivierten SSO-Konfiguration angezeigt. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Authentifizierung</b>: Wenn Ihr Workfront-Administrator eine SSO-Integration in Workfront aktiviert und alle Benutzer für die einmalige Anmeldung aktualisiert hat, ist dieses Feld standardmäßig ausgewählt. In diesem Feld wird der Typ der für Ihre Workfront-Instanz aktivierten SSO-Konfiguration angezeigt.</p> <p>Wenn dieses Feld ausgewählt ist, muss sich der Benutzer mit seinen SSO-Anmeldeinformationen bei Workfront anmelden. Wenn Sie diese Option deaktivieren, können sich die Benutzer mit ihren Workfront-Anmeldeinformationen bei Workfront anmelden.</p> <p>Weitere Informationen zum Konfigurieren von Workfront mit einer SSO-Lösung finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Überblick über Single Sign-on in Adobe Workfront</a></p> <p>Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Benutzer für Single Sign-on aktualisieren</a>.</p> <p><b>NOTE</b>: Wenn Sie Gruppenadministrator sind, können Sie die &lt;sso configuration=""&gt; -Felder nur für Benutzer in den Gruppen, in denen Sie als solche benannt sind. Außerdem muss die Berechtigung "Benutzeradministrator (Gruppenbenutzer)"in Ihrer Zugriffsebene aktiviert sein.
        <p>Wenn Sie Gruppenadministrator sind und die Berechtigung "Benutzeradministrator (Alle Benutzer)"in Ihrer Zugriffsebene aktiviert ist, können Sie die &lt;sso configuration=""&gt; -Felder für alle Benutzer.</p> </li> 
        <li><b>Auftragsinformationen:</b> Informationen über den Auftrag, wie die Berufsbezeichnung, und für welchen Fachbereich der Benutzer verantwortlich ist.</li> 
        <li><p><b>Kontaktangaben</b>: Die Telefonnummer und -adresse des Benutzers.</p>
        <p>Wenn der Benutzer für Unified User Management (UUM) oder Adobe Identity Management System (IMS) aktiviert ist, wird die <b>Land</b> im Abschnitt Kontaktinformationen nur Ländercodewerte akzeptiert (z. B. US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einstellungen </td> 
      <td> 
       <ul> 
        <li> <p><b>Zeitzone:</b> Die Zeitzone des Benutzers.</p> <p>Informationen dazu, wie Sie Benutzer in Workfront bei der zeitzonenübergreifenden Zusammenarbeit unterstützen, finden Sie unter <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Arbeiten über Zeitzonen hinweg</a>.</p> </li> 
        <li><b>Gebietsschema der E-Mail</b>: Das bevorzugte E-Mail-Gebietsschema des Benutzers. Dies wirkt sich auf das Zahlenformat und das Datumsformat der aus Workfront stammenden E-Mails aus.</li> 
        <li><b>Prozentualer Abschluss der Aktualisierung anzeigen</b>: Aktivieren Sie diese Option, wenn Sie eine prozentuale Abschlussleiste im Bereich Aktualisieren der Aufgaben dieses Benutzers anzeigen möchten.</li> 
        <li><b>Versand der Arbeit, die ich mir auf die Registerkarte "Arbeit an"zuweise</b>: Aktivieren Sie diese Option, wenn alles, was der Benutzer sich selbst zuweist, direkt auf der Registerkarte "Arbeiten am"angezeigt werden soll. Standardmäßig werden alle einem Benutzer zugewiesenen Elemente auf der Registerkarte "Arbeitsanforderung"aufgelistet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benachrichtigungen</td> 
      <td> <p>Wählen Sie die E-Mail-Benachrichtigungen aus, die für den neuen Benutzer aktiviert werden sollen.</p> <p>Sie können sowohl die sofortige als auch die tägliche Digest-Benachrichtigung auswählen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zugriff</td> 
      <td> 
       <ul> 
        <li><b>Ist aktiv:</b> Aktivieren Sie dieses Kontrollkästchen, um anzugeben, dass der Benutzer aktiv ist. Aktive Benutzer verwenden eine Workfront-Lizenz. Wenn Sie das Feld löschen, wird der Benutzer deaktiviert.</li> 
        <li> <p><b>Zugriffsebene:</b> Wählen Sie die Zugriffsebene aus, die diesem Benutzer zugewiesen werden soll.</p> 
        <p>Wenn Sie einem Benutzer eine Zugriffsebene zuweisen, können Sie eine Ebene zuweisen, die Ihrer eigenen Zugriffsebene entspricht oder darunter liegt. (Wenn Ihre Zugriffsebene beispielsweise "Planer"lautet, können Sie die Zugriffsebene "Administrator"nicht zuweisen.) Sie können jedoch keine Zugriffsstufe zuweisen, die standardmäßig kleiner als Ihre eigene Zugriffsstufe ist, wenn der Workfront-Administrator nicht standardmäßige Zugriffsberechtigungen für die Zugriffsebene aktiviert hat, die nicht auch in Ihrer eigenen Zugriffsstufe aktiviert sind (über die Einstellungen für die Feinabstimmung, wie hier beschrieben: <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>). </p> 
        <p>Weitere Informationen zu Zugriffsebenen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Zugriff auf Adobe Workfront konfigurieren</a>.</p> </li> 
        <li> <p><b>Layout-Vorlage</b>: Wählen Sie eine Layoutvorlage für den Benutzer aus. Diese Layout-Vorlage hat Vorrang vor jeder Layout-Vorlage, die der Startseite, dem Startseiten-Team oder der primären Auftragsrolle des Benutzers zugewiesen ist. Weitere Informationen zur Zuweisungspriorität von Layout-Vorlagen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layoutvorlagen</a>.</p> <p><b>NOTIZ</b>:  <p>Die Liste der in diesem Feld verfügbaren Vorlagen hängt von Ihrem Zugriff ab:</p> 
          <ul> 
           <li>Als Workfront-Administrator können Sie alle Layout-Vorlagen auf Systemebene und Gruppenebene sehen.</li> 
           <li>Als Gruppenadministrator können Sie die Layout-Vorlage auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Vorlagen sehen.</li> 
           <li>Als Benutzer mit einer Planungslizenz und Zugriff zur Bearbeitung von Benutzern können Sie nur Layoutvorlagen auf Systemebene sehen.</li> 
          </ul> <p>Weitere Informationen zu Layout-Vorlagen auf Gruppenebene finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layoutvorlagen</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation </td> 
      <td> 
       <ul> 
      <li><b>Firma</b>: Das Unternehmen des Benutzers. Benutzer können nur mit einem Unternehmen verknüpft werden. Sie müssen ein Unternehmen erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive Unternehmen angezeigt. Informationen zum Erstellen von Unternehmen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Erstellen und Bearbeiten von Unternehmen</a>.</li> 
      <li><b>Berichte an:</b> Wenn Sie ein Unternehmen für den Benutzer angegeben haben, können Sie in diesem Feld auch den direkten Manager des Benutzers angeben. Ein Benutzer kann nur einen Manager haben.</li> 
      <li><b>Direkte Berichte:</b> Wenn Sie ein Unternehmen für den Benutzer angegeben haben, können Sie auch die direkten Berichte des Benutzers angeben. Ein Benutzer kann über mehrere direkte Berichte verfügen.</li> 
      <li><b>Startseite</b>: Geben Sie das Startseiten-Team für den Benutzer an. Benutzer können nur ein Home-Team haben.</li> 
      <li><b>Sonstige Teams</b>: Benutzer können mehreren Teams angehören.</li> 
      <li> <p><b>Startseite:</b> Wählen Sie eine entsprechende Gruppe aus, um den Benutzer zuzuweisen. Dadurch erhält der Benutzer die Möglichkeit, auf Objekte zuzugreifen, die für die Gruppe freigegeben sind.</p> <p>Dies ist ein Pflichtfeld. Jeder Benutzer muss einer Startseite zugeordnet sein. Wenn Sie keine auswählen, wird Ihre Gruppe als Startseite des neuen Benutzers zugewiesen.</p> <p><b>NOTE</b>: Sie können einem Benutzer nur dann eine Gruppe zuweisen, wenn Sie Workfront-Administrator sind, der Gruppenadministrator sind oder die Gruppe öffentlich ist.</p> </li> 
      <li> <p><b>Andere Gruppen</b>: Benutzer können mehreren Gruppen angehören. Sie können einem Benutzer nur dann eine Gruppe zuweisen, wenn Sie Workfront-Administrator sind, der Gruppenadministrator sind oder die Gruppe öffentlich ist.</p> <p><b>WICHTIG</b>: Das Hinzufügen eines Benutzers zu mehr als 100 Gruppen kann Leistungsprobleme in allen Bereichen von Workfront verursachen, die die Gruppenliste laden.</p> <p>Weitere Informationen zu öffentlichen Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Gruppe erstellen</a>.</p> <p>Weitere Informationen zu Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppenübersicht</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ressourcenplanung </td> 
      <td> 
       <ul>
       <li><b>Deaktivierung planen</b>: Aktivieren Sie dieses Kontrollkästchen, wenn Sie planen möchten, dass dieser Benutzer nach einem bestimmten Zeitraum deaktiviert wird. </li> 
       <li><b>Geplantes Deaktivierungsdatum</b>: Das Datum, nach dem der Benutzer deaktiviert wird. Weitere Informationen zum Planen der Deaktivierung von Benutzern finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planen von Benutzern für die Deaktivierung</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Benutzer deaktivieren oder reaktivieren</a>.</li> 
       <li> <p><b>Primäre Rolle</b>: Dies ist die primäre Aufgabenrolle, die der Benutzer in Workfront erfüllen kann. Jede Aufgabe und jedes Problem, der der Benutzer zugewiesen ist, wird ebenfalls dieser Auftragsrolle zugewiesen. Arbeitsplatzrollen sind im Ressourcenmanagement von entscheidender Bedeutung. Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planungslizenz mit Administratorzugriff verfügen oder wenn Sie Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> <p>In der Liste werden nur aktive Vorgangsrollen angezeigt. </p> </li> 
       <li>Wenn Sie eine <b>Primäre Rolle</b>, die <b>Prozentsatz der VZÄ-Verfügbarkeit</b> angezeigt. Geben Sie an, welcher Prozentsatz der Zeit des Zeitplans des Benutzers dieser Auftragsrolle zugeordnet ist. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die Primäre Rolle beträgt 100 %. </li> 
       <li> <p><b>Sonstige Rollen</b>: Ein Benutzer kann in Workfront über mehrere Vorgangsrollen verfügen. Arbeitsplatzrollen sind im Ressourcenmanagement von entscheidender Bedeutung. Es gibt keine Beschränkung dafür, wie viele Jobrollen ein Benutzer erfüllen kann. Es wird jedoch empfohlen, keinen Benutzer einer zu großen Anzahl von Vorgängen zuzuweisen, da die Ressourcenverwaltung für diese Benutzer zu komplex werden kann.<p>In der Liste werden nur aktive Vorgangsrollen angezeigt. Weitere Informationen zu Auftragsrollen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Vorgangsrollen</a>.</p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planungslizenz mit Administratorzugriff verfügen oder wenn Sie Workfront-Administrator sind. <br>Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
       <li> <p>(Bedingt) Wenn Sie eine oder mehrere <b>Sonstige Rollen</b>, die <b>Prozentsatz der VZÄ-Verfügbarkeit</b> für jede Rolle angezeigt. Geben Sie an, welcher Prozentsatz der Zeit des Benutzerzeitplans den einzelnen Auftragsrollen zugeordnet wird. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die anderen Rollen beträgt 0 %.</p> <p><b>NOTE</b>: Wenn "Andere Rollen"eine FTE-Verfügbarkeit von 0 % haben, werden sie nicht im Ressourcen-Planer angezeigt, es sei denn, die Benutzer sind Aufgaben in diesen Rollen zugewiesen.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTIZ</b>: <p>Die Summe aller <b>Prozentsatz der VZÄ-Verfügbarkeit</b> für alle Rollen muss 100 % entsprechen. Jeder Prozentsatz der FTE-Verfügbarkeit berechnet die verfügbaren Stunden für jede Rolle pro Benutzer im Resource Planer. Die verfügbaren Stunden für jede Rolle pro Benutzer hängen von der verfügbaren Zeit des Benutzers ab.</p> <p>Die verfügbare Zeit für den Benutzer wird von Workfront entsprechend der Methode berechnet, die der Workfront-Administrator unter "Voreinstellungen für die Ressourcenverwaltung"zur Berechnung der FTE ausgewählt hat.</p> <p>Informationen zur Berechnung der Verfügbarkeit für den Benutzer finden Sie unter <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer</a>.</p> <p>Weitere Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.</p> </p> </li> 
       <li> <p><b>Zeitplan</b>: Verknüpfen Sie einen Zeitplan mit dem Benutzer. Der Zeitplan des Benutzers berechnet die Zeitleiste der Aufgaben, denen der Benutzer zugewiesen ist.</p> <p>Sie müssen einen Zeitplan erstellen, bevor Sie ihn mit einem Benutzer verknüpfen können. Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a>.</p> <p><b>NOTE</b>: Es wird empfohlen, dass der Zeitplan, den Sie mit dem Benutzer verknüpfen, mit der Zeitzone des Benutzers übereinstimmt.</p> </li> 
       <li> <p><b>Datenblatt-Profil</b>: Verknüpfen Sie ein Timesheet-Profil mit dem Benutzer, um sicherzustellen, dass Timesheets automatisch für den Benutzer generiert werden.</p> <p><b>NOTE</b>: Die Liste der in diesem Feld verfügbaren Profile hängt von Ihrem Zugriff ab:
       <ul>
       <li>Als Workfront-Administrator können Sie alle Timesheet-Profile auf Systemebene und auf Gruppenebene anzeigen.</li>
       <li>Als Gruppenadministrator können Sie auf Systemebene die Profile des Datenblatts sowie die mit den von Ihnen verwalteten Gruppen verknüpften Profile sehen.</li>
       <li>Als Benutzer mit einer Planungslizenz und Zugriff zur Bearbeitung von Benutzern können Sie nur Timesheet-Profile auf Systemebene sehen. Weitere Informationen zu Timesheet-Profilen auf Gruppenebene finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen</a>.</li>
      </ul></p> </li> 
       <li><b>Standardstündentyp</b>: Wählen Sie den Standardstundentyp für den Benutzer aus. Dies ist der Stundentyp, der standardmäßig verwendet wird, wenn der Benutzer die Zeit protokolliert.</li> 
       <li><b>Verfügbare Stundentypen</b>: Wählen Sie die für den Benutzer verfügbaren Stundentypen aus. Diese Stundentypen sind überall in Workfront sichtbar, wo der Benutzer die Zeit protokollieren kann. Ein Benutzer kann nur die Stunden-Typen sehen, die auf Projektebene und auf Benutzerebene aktiviert sind. Weitere Informationen darüber, welche Stundentypen Benutzern zur Verfügung stehen, finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Festlegen von Stundentypen und Verfügbarkeit für Timesheets</a>.</li> 
       <li><b>Log Time in:</b> Wählen Sie aus, ob der Benutzer die Zeit für Arbeitselemente in Stunden oder Tagen protokollieren soll. Weitere Informationen finden Sie unter <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird</a>.</li> 
       <li> <p><b>FTE</b>: Das System verwendet diese Zahl, um die Verfügbarkeit des Benutzers anhand des Standardzeitplans nur zu berechnen, wenn die Voreinstellungen für die Ressourcenverwaltung auf Systemebene auf <b>Standardzeitplan</b>. Der Wert muss <i>0</i> oder zwischen <i>.1</i> und <i>1</i>.</p> <p>Wenn der FTE-Wert beispielsweise 0,5 beträgt und der Standardzeitplan 40 Stunden beträgt, kann der Benutzer 20 Stunden pro Woche arbeiten.</p> <p>Wenn die Voreinstellungen für die Ressourcenverwaltung auf Systemebene auf <b>Zeitplan des Benutzers</b>festgelegt ist, wird der hier angegebene Wert ignoriert und der Benutzer wird gemäß den Angaben in seinem Zeitplan als verfügbar betrachtet. In diesem Fall wird die FTE des Benutzers für den Resource Planer anhand der folgenden Formel berechnet:</p> <p ><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><em><br></em> </p> <p>Weitere Informationen zur Berechnung der VZÄ des Nutzers finden Sie unter <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer</a>.<br>Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a>.</p> <p>Eine zeitliche Abrechnung von Ausnahmen und Zeitüberschreitungen kann sich auf die geplante Stundenzahl oder die VZÄ auswirken. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>. </p> </li> 
        <li><b>Ressourcen-Pools</b>: Verknüpfen Sie den Benutzer mit Ressourcen-Pools. Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Verknüpfen von Ressourcen-Pools mit Benutzern </a>.</li> 
        <li><b>Kosten pro Stunde</b>: Die Kosten pro Stunde für den Benutzer. </li> 
        <li><b>Abrechnung pro Stunde</b>: Die Höhe der Abrechnung pro Stunde für den Benutzer.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td>Verknüpfen Sie diesem Benutzer ein benutzerdefiniertes Benutzerformular. Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kommentar</td> 
      <td> <p>Geben Sie den Kommentar ein, den Sie den Benutzern und dem Bereich Updates ihrer Benutzerprofile senden möchten.</p> </td> 
     </tr> 
    </tbody> 
   </table>
