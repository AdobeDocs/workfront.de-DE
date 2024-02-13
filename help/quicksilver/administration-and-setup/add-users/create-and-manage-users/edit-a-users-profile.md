---
title: Profil eines Benutzers bearbeiten
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator können Sie neue Benutzer erstellen und die Profile bestehender Benutzer verwalten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 1949a0bb213553f1f1f252c4382a90514fcd0b5b
workflow-type: tm+mt
source-wordcount: '3279'
ht-degree: 0%

---

# Profil eines Benutzers bearbeiten

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Als Adobe Workfront-Administrator können Sie Benutzer erstellen und die Profile vorhandener Benutzer verwalten. Informationen zum Erstellen von Benutzern finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

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
   <td> <p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p>Die <b>Benutzer</b> -Objekt in Ihrer Zugriffsstufe, die für <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden folgenden <b>Benutzeradministrator</b> Optionen aktiviert unter <b>Optimieren Ihrer Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> Benutzeradmin. (Alle Benutzer)</li>
     <li>Benutzeradmin. (Gruppenbenutzer)</li></ul>
     <p>Wenn  <b>Benutzerverwaltung (Gruppenbenutzer)</b> aktiviert ist, müssen Sie ein Gruppenadministrator für eine Gruppe sein, in der der Benutzer Mitglied ist, um den Benutzer bearbeiten zu können.</p> 
     <p>Weitere Informationen zum <b>Benutzer</b> auf einer Zugriffsebene festzulegen, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table> 
*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Benutzerprofil bearbeiten

{{step-1-to-users}}

1. Wählen Sie den Benutzer aus und klicken Sie dann auf das **Bearbeiten** icon ![](assets/edit-icon.png).

   Das Feld Benutzer bearbeiten wird angezeigt.

1. Im **Benutzer bearbeiten** ändern Sie die folgenden Informationen und klicken Sie auf **Änderungen speichern** jederzeit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Persönliche Info </td> 
      <td> 
       <ul> 
        <li><p><b>Vorname</b></p></li>
        <li><p><b>Nachname</b></p></li> 
        <li> <p><b>Email Address:</b> Die E-Mail-Adresse eines Benutzers ist auch sein Benutzername in Workfront. Bei diesem Feld wird zwischen Groß- und Kleinschreibung unterschieden und es muss eindeutig sein. Wenn ein Benutzer innerhalb eines 10-minütigen Fensters dreimal versucht, eine nicht eindeutige E-Mail-Adresse hinzuzufügen, wird eine reCAPTCHA-Antwort angezeigt.</p> <p> Wählen Sie die <b>Ich bin kein Roboter</b> -Einstellung, bevor Sie fortfahren können.</p><p>Wenn Sie die E-Mail-Zulassungsliste verwenden und eine E-Mail-Domäne eingeben, die nicht in der Liste enthalten ist, erhält der Benutzer keine E-Mail-Benachrichtigungen. Weitere Informationen zur Zulassungsliste finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Konfigurieren der E-Mail-Zulassungsliste</a>.</p> </li> 
        <li> <p><b>Kennwort zurücksetzen</b>: Klicken Sie auf diesen Link, um das Kennwort des Benutzers zurückzusetzen. Sie müssen Ihr eigenes Kennwort eingeben, bevor Sie das Kennwort eines anderen Benutzers zurücksetzen können.</p> <p>Um das Kennwort eines anderen Benutzers zurückzusetzen, müssen Sie Workfront-Administrator oder Gruppenadministrator sein.</p> <p><b>NOTE</b>:  
          <ul> 
           <li> <p>Wenn Sie Gruppenadministrator sind, können Sie Kennwörter nur für Benutzer in den Gruppen zurücksetzen, in denen Sie als Administrator benannt sind. Außerdem muss die Berechtigung "Benutzeradministrator (Gruppenbenutzer)"in Ihrer Zugriffsebene aktiviert sein:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Diese Einstellung ist standardmäßig deaktiviert. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </li> 
           <li> <p>Sie können das Kennwort eines Workfront-Administrators nicht zurücksetzen.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Benutzername</b>: Wenn Ihr Workfront-Administrator eine SSO-Integration in Workfront aktiviert hat, wird in diesem Feld der SSO-Benutzername angezeigt. In diesem Feld wird der Typ der für Ihre Workfront-Instanz aktivierten SSO-Konfiguration angezeigt. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Authentifizierung</b>: Wenn Ihr Workfront-Administrator eine SSO-Integration in Workfront aktiviert und alle Benutzer für die einmalige Anmeldung aktualisiert hat, ist dieses Feld standardmäßig ausgewählt. In diesem Feld wird der Typ der für Ihre Workfront-Instanz aktivierten SSO-Konfiguration angezeigt.</p> <p>Wenn dieses Feld ausgewählt ist, muss sich der Benutzer mit seinen SSO-Anmeldeinformationen bei Workfront anmelden. Wenn Sie diese Option deaktivieren, können sich die Benutzer mit ihren Workfront-Anmeldeinformationen bei Workfront anmelden.</p> <p>Weitere Informationen zum Konfigurieren von Workfront mit einer SSO-Lösung finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Überblick über Single Sign-on in Adobe Workfront</a></p> <p>Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Benutzer für Single Sign-on aktualisieren</a>.</p> 
        <p><b>NOTE</b>:</p> 
        <p> Als Gruppenadministrator können Sie die &lt;sso configuration=""&gt; -Felder nur für Benutzer in den Gruppen, in denen Sie als solche benannt sind. Außerdem muss die Berechtigung "Benutzeradministrator (Gruppenbenutzer)"in Ihrer Zugriffsebene aktiviert sein.
        <p>Wenn Sie Gruppenadministrator sind und die Berechtigung "Benutzeradministrator (Alle Benutzer)"in Ihrer Zugriffsebene aktiviert ist, können Sie die &lt;sso configuration=""&gt; -Felder für alle Benutzer.</p> </li> 
        <li><b>Auftragsinformationen:</b> Informationen zum Auftrag, z. B. die Berufsbezeichnung (im <b>Titel</b> und für welchen Bereich des Know-hows der Benutzer verantwortlich ist (im Bereich <b>Sprechen Sie mit mir über</b> -Feld).</li> 
        <li><p><b>Kontaktangaben</b>: Die Telefonnummer des Benutzers (im <b>Telefonnummer, Ausg.</b>, und <b>Mobiltelefonnummer</b> -Felder und -Adressen (im <b>Adresse, Ort, Bundesland, Postleitzahl, Land</b> -Felder ).</p>
        <p>Wenn der Benutzer für Unified User Management (UUM) oder Adobe Identity Management System (IMS) aktiviert ist, wird die <b>Land</b> im Abschnitt Kontaktinformationen nur Ländercodewerte akzeptiert (z. B. US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einstellungen </td> 
      <td> 
       <ul> 
      <li> <p><b>Zeitzone:</b> Die Zeitzone des Benutzers.</p> <p>Informationen dazu, wie Sie Benutzer in Workfront bei der zeitzonenübergreifenden Zusammenarbeit unterstützen, finden Sie unter <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Arbeiten über Zeitzonen hinweg</a>.</p> </li> 
       <li><b>Gebietsschema der E-Mail</b>: Das bevorzugte E-Mail-Gebietsschema des Benutzers. Dies wirkt sich auf das Zahlenformat und das Datumsformat der E-Mails aus, die von Workfront an diesen Benutzer gesendet werden.</li>

   <li><b>Empfangen von E-Mails aus dieser Testumgebung</b>: Aktivieren Sie diese Option, wenn Sie E-Mail-Benachrichtigungen von der Umgebung erhalten möchten, in der Sie derzeit angemeldet sind.
      <p><b>NOTIZ</b></p>
      <p>Diese Option ist nur in den Umgebungen Vorschau und Sandbox verfügbar. E-Mail-Benachrichtigungen sind in der Produktionsumgebung standardmäßig aktiviert. </p>
      </li>

   <li><b>Prozentualer Abschluss der Aktualisierung anzeigen</b>: Aktivieren Sie diese Option, wenn Sie bei Verwendung des bisherigen Kommentierungserlebnisses im Bereich Aktualisieren der Aufgaben dieses Benutzers eine prozentuale Leiste zum Abschluss anzeigen möchten. Weitere Informationen finden Sie unter <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">Neues Kommentierungserlebnis</a>.</li> 
       <li><b>Versand der Arbeit, die ich mir auf die Registerkarte "Arbeit an"zuweise</b>: Aktivieren Sie diese Option, wenn alles, was der Benutzer sich selbst zuweist, direkt in der Liste "Arbeiten auf"im Bereich "Startseite"angezeigt werden soll. Standardmäßig werden alle Elemente aufgelistet, die einem Benutzer in den Listen "Bereit zum Start"oder "Nicht bereit"im Bereich "Startseite"zugewiesen sind.</li> 
       <li><b>Automatische Erstellung von Testsendungen beim Hochladen von Dokumenten</b>: Aktivieren Sie diese Option, wenn die vom Benutzer hochgeladenen Dokumente sofort einen Testversand erzeugen sollen. </li>
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
      <li><b>Ist aktiv:</b> Aktivieren Sie dieses Kontrollkästchen, um anzugeben, dass der Benutzer aktiv ist. Aktive Benutzer verwenden eine Workfront-Lizenz. Wenn Sie das Feld löschen, wird der Benutzer deaktiviert und verhindert, dass er sich bei Workfront anmeldet.</li> 
       <li> <p><b>Zugriffsebene:</b> Wählen Sie die Zugriffsebene aus, die diesem Benutzer zugewiesen werden soll.</p> 
       <p>Wenn Sie einem Benutzer eine Zugriffsebene zuweisen, können Sie eine Ebene zuweisen, die Ihrer eigenen Zugriffsebene entspricht oder darunter liegt.</p>
       <p>Wenn Ihre Zugriffsebene beispielsweise Plan lautet, können Sie die Zugriffsebene "Administrator"nicht zuweisen. Sie können jedoch keine Zugriffsstufe zuweisen, die standardmäßig niedriger ist als Ihre eigene Zugriffsstufe, wenn der Workfront-Administrator nicht standardmäßige Zugriffsberechtigungen für die Zugriffsstufe aktiviert hat, die nicht auch in Ihrer eigenen Zugriffsstufe aktiviert sind. </p>
       <p>Wenn Sie beispielsweise über eine Planlizenz ohne Zugriff auf Löschaufgaben verfügen, können Sie niemandem eine Work-Lizenz mit Zugriff auf Löschaufgaben zuweisen, obwohl die Work-Lizenz niedriger als die Plan-Lizenz ist. Weitere Informationen finden Sie unter  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> 
       <p>Weitere Informationen zu Zugriffsebenen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Zugriff auf Adobe Workfront konfigurieren</a>.</p>
       <p> <b>NOTE:</b></p> 
       <p> Wenn Ihr Unternehmen das neue Zugriffsmodell (Standard/Light/Contributor) verwendet, können Sie einen Standard- oder Light-Benutzer nicht einer Contributor-Zugriffsstufe zuweisen, wenn dieser Benutzer seine Entscheidungsgrenze für den Monat bereits erreicht hat. </p><p>Weitere Informationen zum neuen Zugriffsmodell finden Sie unter <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Übersicht über die neuen Zugriffsebenen</a>. </p><p>Informationen zu Entscheidungsgrenzen finden Sie unter <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Begrenzte Dokument- und Testentscheidung für nicht bezahlte Benutzer - Überblick</a>.</p></li> 
       <li> <p><b>Layout-Vorlage</b>: Wählen Sie eine Layoutvorlage für den Benutzer aus. Diese Layout-Vorlage hat Vorrang vor jeder Layout-Vorlage, die der Startseite, dem Startseiten-Team oder der Primären Rolle des Benutzers zugewiesen ist. Weitere Informationen zur Zuweisungspriorität von Layout-Vorlagen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layoutvorlagen</a>.</p> <p><b>NOTE</b>:  <p>In der folgenden Liste wird beschrieben, wie die Liste der Vorlagen, die in diesem Feld verfügbar sind, von Ihrem Zugriff abhängt:</p> 
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
      <li><b>Berichte an:</b> Wenn Sie ein Unternehmen für den Benutzer angegeben haben, können Sie in diesem Feld auch den direkten Manager des Benutzers angeben. Ein Benutzer kann nur einen Manager haben. Dieses Feld wird nicht angezeigt, wenn der Benutzer nicht zuerst einem Unternehmen zugeordnet ist. </li> 
      <li><b>Direkte Berichte:</b> Wenn Sie ein Unternehmen für den Benutzer angegeben haben, können Sie auch die direkten Berichte des Benutzers angeben. Ein Benutzer kann über mehrere direkte Berichte verfügen. Dieses Feld wird nicht angezeigt, wenn der Benutzer nicht zuerst einem Unternehmen zugeordnet ist.</li> 
      <li><b>Startseite</b>: Geben Sie das Startseiten-Team für den Benutzer an. Benutzer können nur ein Home-Team haben. Das Home Team ist wichtig, wenn es eine Layoutvorlage zuweist oder wenn es die Schaltfläche Work On It für die dem Benutzer zugewiesenen Aufgaben und Probleme definiert. </li> 
      <li><b>Sonstige Teams</b>: Benutzer können mehreren Teams angehören. Ein Benutzer kann die einem seiner Teams zugewiesenen Arbeitselemente in seinem Heimbereich anzeigen. </li> 
      <li> <p><b>Startseite:</b> Wählen Sie eine entsprechende Gruppe aus, um den Benutzer zuzuweisen. Dadurch erhält der Benutzer die Möglichkeit, auf Objekte zuzugreifen, die für die Gruppe freigegeben sind. Sie können Layoutvorlagen auch für die Startseite des Benutzers freigeben.</p> <p>Dies ist ein erforderliches Feld. Jeder Benutzer muss einer Startseite zugeordnet sein. Wenn Sie keine auswählen, wird Ihre Gruppe als Startseite des neuen Benutzers zugewiesen.</p> <p><b>NOTE</b>:</p> 
      <p> Sie können einem Benutzer nur dann eine Gruppe zuweisen, wenn einer der folgenden Punkte zutrifft:</p>
      <ul><li>Sie sind Workfront-Administrator</li>
      <li>Sie sind der Administrator der Gruppe</li>
      <li>die Gruppe öffentlich ist.</li></ul> 
      <li> <p><b>Andere Gruppen</b>: Benutzer können mehreren Gruppen angehören. Sie können einem Benutzer nur dann eine Gruppe zuweisen, wenn Sie Workfront-Administrator sind, der Gruppenadministrator sind oder die Gruppe öffentlich ist.</p> <p><b>WICHTIG</b>:</p> 
      <p>Das Hinzufügen eines Benutzers zu mehr als 100 Gruppen kann Leistungsprobleme in allen Bereichen von Workfront verursachen, die die Gruppenliste laden.</p> <p>Weitere Informationen zu öffentlichen Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Gruppe erstellen</a>.</p> <p>Weitere Informationen zu Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppenübersicht</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ressourcenplanung </td> 
      <td> 
       <ul>
       <li>
       <b>Arbeitszeit</b>: Stellt den Prozentsatz der Vollzeitäquivalenzzeit (FTE) dar, zu dem der Benutzer für die tatsächliche Arbeit verfügbar ist, ohne dass der Overhead eingeschlossen ist. Die Arbeitszeit muss eine Dezimalzahl von bis zu 1 sein, und sie darf nicht 0 sein. Eine Verfügbarkeit von 20 % für tatsächliche Arbeit wäre beispielsweise 0,2.

   Der Standardwert des Felds ist 1, was bedeutet, dass ein Benutzer seine gesamte FTE für tatsächliche, projektbezogene Arbeiten ausgibt.

   Das System verwendet diese Zahl, um die Verfügbarkeit des Benutzers für tatsächliche, projektbezogene Arbeiten zu berechnen.

   Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Zeitplan erstellen</a>.

   Eine Planung von Ausnahmen und Zeitüberschreitungen kann sich auch auf die Kapazität des Benutzers auswirken.

   Workfront berechnet die Verfügbarkeit eines Benutzers entsprechend den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich. Weitere Informationen finden Sie unter <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.

   <b>TIPP</b>

   Setzen Sie den Wert für die Arbeitszeit auf 1, um anzugeben, dass der Benutzer für projektbezogene Arbeiten in seiner gesamten Vollzeitäquivalenz verfügbar ist.
   </li> 
      <li> <b>Deaktivierung planen</b>: Aktivieren Sie dieses Kontrollkästchen, wenn Sie planen möchten, dass dieser Benutzer zu einem bestimmten Datum und zu einem bestimmten Zeitpunkt deaktiviert wird. </li> 
       <li><b>Geplantes Deaktivierungsdatum</b>: Datum und Uhrzeit der Deaktivierung des Benutzers. Weitere Informationen zum Planen der Deaktivierung von Benutzern finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planen von Benutzern für die Deaktivierung</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Benutzer deaktivieren oder reaktivieren</a>.</li> 
       <li> <p><b>Primäre Rolle</b>: Dies ist die primäre Aufgabenrolle, die der Benutzer in Workfront erfüllen kann. Jede Aufgabe und jedes Problem, der der Benutzer zugewiesen ist, wird ebenfalls dieser Auftragsrolle zugewiesen. Arbeitsplatzrollen sind im Ressourcenmanagement von entscheidender Bedeutung. Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planungslizenz mit Administratorzugriff verfügen oder wenn Sie Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> <p>In der Liste werden nur aktive Vorgangsrollen angezeigt. </p> </li> 
       <li>Wenn Sie eine <b>Primäre Rolle</b>, die <b>Prozentsatz der VZÄ-Verfügbarkeit</b> angezeigt. Geben Sie an, welcher Prozentsatz der Zeit des Zeitplans des Benutzers dieser Auftragsrolle zugeordnet ist. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die Primäre Rolle beträgt 100 %. </li> 
       <li> <p><b>Sonstige Rollen</b>: Ein Benutzer kann in Workfront über mehrere Vorgangsrollen verfügen. Arbeitsplatzrollen sind im Ressourcenmanagement von entscheidender Bedeutung. Es gibt keine Beschränkung dafür, wie viele Jobrollen ein Benutzer erfüllen kann. Es wird jedoch empfohlen, keinen Benutzer einer zu großen Anzahl von Vorgängen zuzuweisen, da die Ressourcenverwaltung für diese Benutzer zu komplex werden kann.<p>In der Liste werden nur aktive Vorgangsrollen angezeigt. Weitere Informationen zu Auftragsrollen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Vorgangsrollen</a>.</p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planungslizenz mit Administratorzugriff verfügen oder wenn Sie Workfront-Administrator sind. <br>Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
       <li> <p>(Bedingt) Wenn Sie eine oder mehrere <b>Sonstige Rollen</b>, die <b>Prozentsatz der VZÄ-Verfügbarkeit</b> für jede Rolle angezeigt. Geben Sie an, welcher Prozentsatz der Zeit des Benutzerzeitplans den einzelnen Auftragsrollen zugeordnet wird. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die anderen Rollen beträgt 0 %.</p> <p><b>NOTE</b>: Wenn für andere Rollen eine FTE-Verfügbarkeit von 0 % vorliegt, werden sie nicht im Ressourcen-Planer angezeigt, es sei denn, die Benutzer sind Aufgaben in diesen Rollen zugewiesen.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTE</b>: <p>Die Summe aller <b>Prozentsatz der VZÄ-Verfügbarkeit</b> für alle Rollen muss 100 % entsprechen. Jeder Prozentsatz der FTE-Verfügbarkeit berechnet die verfügbaren Stunden für jede Rolle pro Benutzer im Resource Planer. Die verfügbaren Stunden für jede Rolle pro Benutzer hängen von der verfügbaren Zeit des Benutzers ab.</p> <p>Die verfügbare Zeit für den Benutzer wird von Workfront entsprechend der Methode berechnet, die der Workfront-Administrator unter "Voreinstellungen für die Ressourcenverwaltung"zur Berechnung der FTE ausgewählt hat.</p> <p>Informationen zur Berechnung der Verfügbarkeit für den Benutzer finden Sie unter <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer</a>.</p> <p>Weitere Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.</p> </p>
       <span class="preview"><p>(Optional) Das Datum, an dem effektive Aufgabenrollenzuweisungen in Finanzberechnungen verwendet werden, wenn sich die Rolle des Benutzers im Arbeitsbereich eines Projekts ändert.</p><p>Klicks <b>Rollen nach Datum definieren</b>, wählen Sie die <b>Primäre Rolle</b> und <b>Sonstige Rollen</b>und geben Sie den Zuordnungsprozentsatz für jede Rolle an. Die Rollen können mit den vorhandenen Rollen (mit unterschiedlichen Prozentsätzen) oder neuen Rollen identisch sein. Wählen Sie die <b>Startdatum</b> wenn diese Rollen aktiv werden. Dies kann ein zukünftiges Datum sein. Wenn die neuesten Rollen aktiv werden, können Sie auf <b>Vorherige Rollen anzeigen</b> um die vorherigen, inaktiven Rollen anzuzeigen.</p> </li></span>
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

   <li> <b>FTE</b>: Dies ist das Vollzeitäquivalent des Benutzers. Workfront verwendet diese Zahl, um die Verfügbarkeit des Benutzers anhand des Standardzeitplans nur zu berechnen, wenn die Voreinstellungen für die Ressourcenverwaltung auf Systemebene auf den Standardzeitplan gesetzt sind.

   <p>Die FTE gibt die Zeit an, die der Benutzer bei der Arbeit verbringen kann. Dazu gehören Gemeinkosten sowie die Zeit, die für die Projektarbeit benötigt wird. Beispielsweise wird auch die in Sitzungen verbrachte Zeit oder Schulungen in die VZÄ einbezogen.</p>

   Die VZÄ muss eine Dezimalzahl von bis zu 1 haben und darf nicht 0 sein. Wenn der FTE-Wert beispielsweise 0,5 beträgt und der Standardzeitplan in Workfront 40 Stunden beträgt, ist der Benutzer 20 Stunden pro Woche verfügbar.

   Der Standardwert des Felds ist 1.

   Planen Sie Ausnahmen, eine Zeitüberschreitung und den Wert der Arbeitszeit können sich auf die Verfügbarkeit des Benutzers auswirken.

   Workfront berechnet die Verfügbarkeit eines Benutzers entsprechend den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich.

   Wenn die Voreinstellungen für die Ressourcenverwaltung auf Systemebene auf den Zeitplan des Benutzers gesetzt sind, wird der hier angegebene Wert ignoriert und der Benutzer gilt als gemäß den Angaben in seinem Zeitplan verfügbar.

   Weitere Informationen finden Sie unter <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.

   Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Zeitplan erstellen</a>.
   </li>

   <li><b>Ressourcenpools</b>: Verknüpfen Sie den Benutzer mit Ressourcen-Pools. Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Verknüpfen von Ressourcen-Pools mit Benutzern </a>.</li>

   <li><b>Kostensatz</b>: Die Kosten pro Stunde für den Benutzer.
      <p>Klicken Sie für datumswirksame Kostensätze auf <strong>Rate hinzufügen</strong>. Geben Sie den Wert der Kostensätze für den Zeitraum ein und weisen Sie nach Bedarf ein Startdatum und ein Enddatum zu. Kostenstelle 1 hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.</p><p>Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Kostensatz 1 kein Enddatum hat und Sie Kostensatz 2 mit einem Startdatum vom 1. Mai 2023 hinzufügen, wird das Enddatum 30. April 2023 zu Kostensatz 1 hinzugefügt, sodass keine Lücken bestehen.</p></li>

   <li><b>Abrechnungsrate</b>: Die Höhe der Abrechnung pro Stunde für den Benutzer.
      <p>Klicken Sie für datumswirksame Abrechnungsraten auf <strong>Rate hinzufügen</strong>. Geben Sie den Wert der Abrechnungsrate für den Zeitraum ein und weisen Sie nach Bedarf ein Startdatum und ein Enddatum zu. Der Abrechnungskurs 1 hat kein Startdatum und der letzte Abrechnungskurs hat kein Enddatum.</p> <p>Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungsrate 1 kein Enddatum hat und Sie eine zweite mit dem Startdatum 1. Mai 2023 hinzufügen, wird das Enddatum 30. April 2023 zum Abrechnungskurs 1 hinzugefügt, sodass keine Lücken bestehen.</p><p> <img alt="Benutzerkosten und Abrechnungssätze" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td><p>Verknüpfen Sie diesem Benutzer ein benutzerdefiniertes Benutzerformular. Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Felder, auf die Sie keinen Zugriff haben, werden nicht in einem benutzerdefinierten Formular angezeigt.</p> <p>Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kommentar</td> 
      <td>Geben Sie den Kommentar ein, den Sie den Benutzern und dem Bereich Updates ihrer Benutzerprofile senden möchten.</td> 
     </tr> 
    </tbody> 
   </table>
