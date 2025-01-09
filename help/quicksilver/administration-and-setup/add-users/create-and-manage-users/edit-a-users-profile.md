---
title: Benutzerprofil bearbeiten
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Admin können Sie neue Benutzende erstellen und die Profile vorhandener Benutzender verwalten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 532a7badf236d0d9568bc6c632b7badf3576cce3
workflow-type: tm+mt
source-wordcount: '3273'
ht-degree: 0%

---

# Benutzerprofil bearbeiten

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

Als Adobe Workfront-Administrator können Sie Benutzende erstellen und die Profile bestehender Profile verwalten. Informationen zum Erstellen von Benutzern finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Informationen dazu, wie Benutzer ihre eigenen Profile aktualisieren, finden Sie unter [Konfigurieren meiner Einstellungen](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

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
   <td><p>Neu: Standard</p><p>Oder</p><p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bearbeiten eines Benutzerprofils

{{step-1-to-users}}

1. Wählen Sie den Benutzer aus und klicken Sie dann auf das **Bearbeiten**-Symbol ![](assets/edit-icon.png).

   Das Feld Benutzer bearbeiten wird angezeigt.

1. Ändern Sie **Feld****Benutzer bearbeiten“ eine der folgenden Informationen und klicken Sie** auf „Änderungen speichern“:

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
        <li> <p><b>E-Mail-Adresse</b> Die E-Mail-Adresse für einen Benutzer ist auch dessen Benutzername in Workfront. Bei diesem Feld wird zwischen Groß- und Kleinschreibung unterschieden und es muss eindeutig sein. Wenn ein(e) Benutzende(r) versucht, innerhalb eines 10-minütigen Fensters dreimal eine nicht eindeutige E-Mail-Adresse hinzuzufügen, wird eine reCAPTCHA-Antwort angezeigt.</p> <p> Wählen Sie die Einstellung <b>Ich bin kein Roboter</b> aus, bevor Sie fortfahren können.</p><p>Wenn Sie die E-Mail-Zulassungsliste verwenden und eine E-Mail-Domain eingeben, die nicht auf der Liste steht, erhält der/die Benutzende keine E-Mail-Benachrichtigungen. Weitere Informationen über die Zulassungsliste auf die Zulassungsliste setzte finden Sie unter <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Konfigurieren Ihrer E-Mail</a>.</p> </li> 
        <li> <p><b>Kennwort zurücksetzen</b>: Klicken Sie auf diesen Link, um das Kennwort des Benutzers zurückzusetzen. Sie müssen Ihr eigenes Kennwort eingeben, bevor Sie das Kennwort eines anderen Benutzers zurücksetzen können.</p> <p>Zum Zurücksetzen des Kennworts eines anderen Benutzers müssen Sie ein Workfront-Administrator oder ein Gruppenadministrator sein.</p> <p><b>HINWEIS</b>:  
          <ul> 
           <li> <p>Wenn Sie Gruppenadministrator sind, können Sie Kennwörter nur für Benutzer in den Gruppen zurücksetzen, in denen Sie als Administrator festgelegt sind. Außerdem muss in Ihrer Zugriffsebene die Berechtigung Benutzeradmin (Gruppenbenutzer) aktiviert sein:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Diese Einstellung ist standardmäßig deaktiviert. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </li> 
           <li> <p>Das Kennwort eines Workfront-Administrators kann nicht zurückgesetzt werden.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO-Konfiguration&gt; Benutzername</b>: Wenn Ihr Workfront-Administrator eine SSO-Integration mit Workfront aktiviert hat, wird der SSO-Benutzername in diesem Feld angezeigt. Der Typ der für Ihre Workfront-Instanz aktivierten SSO-Konfiguration wird in diesem Feld angezeigt. </li> 
        <li> <p><b>Nur &lt;SSO-Konfiguration&gt; Authentifizierung zulassen</b>: Wenn der Workfront-Administrator eine SSO-Integration mit Workfront aktiviert hat und alle Benutzer für SSO aktualisiert hat, ist dieses Feld standardmäßig ausgewählt. Der Typ der für Ihre Workfront-Instanz aktivierten SSO-Konfiguration wird in diesem Feld angezeigt.</p> <p>Wenn dieses Feld ausgewählt ist, muss sich der Benutzer mit seinen SSO-Anmeldeinformationen bei Workfront anmelden. Wenn Sie diese Option deaktivieren, können sich Benutzer mit ihren Workfront-Anmeldeinformationen bei Workfront anmelden.</p> <p>Weitere Informationen zum Konfigurieren von Workfront mit einer SSO-Lösung finden Sie <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Übersicht über Single Sign-on in Adobe Workfront</a></p> <p>Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Aktualisieren von Benutzern für einmaliges Anmelden</a>.</p> 
        <p><b>HINWEIS</b>:</p> 
        <p> Wenn Sie Gruppenadministrator sind, können Sie die Felder &lt;SSO Configuration&gt; nur für Benutzer in den Gruppen bearbeiten, in denen Sie als solcher angegeben sind. Außerdem muss in Ihrer Zugriffsebene die Berechtigung Benutzeradmin (Gruppenbenutzer) aktiviert sein.
        <p>Wenn Sie Gruppenadministrator sind und für Ihre Zugriffsebene die Berechtigung Benutzeradministration (alle Benutzer) aktiviert haben, können Sie die Felder &lt;SSO-Konfiguration&gt; für alle Benutzer bearbeiten.</p> </li> 
        <li><b>Jobinfo:</b> Informationen über den Job, wie z. B. die Jobbezeichnung (im <b>Titel</b>-Feld) und welchen Fachbereich der Benutzer verantwortet (im <b>Sprechen Sie mit mir über</b>).</li> 
        <li><p><b>Kontaktinformationen</b>: Die Telefonnummer des Benutzers (in der <b>Telefonnummer, Durchwahl.</b> und <b>Mobiltelefonnummer</b>) und Adresse (in den Feldern <b>Adresse, Stadt, Bundesland, Postleitzahl, </b> ).</p>
        <p>Wenn die Benutzerin bzw. der Benutzer für Unified User Management (UUM) oder Adobe Identity Management System (IMS) aktiviert ist, akzeptiert das Feld <b>Country</b> im Abschnitt Kontaktinformationen nur Ländercodewerte (z. B. US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einstellungen </td> 
      <td> 
       <ul> 
      <li> <p><b>Zeitzone</b>: Die Zeitzone des Benutzers.</p> <p>Informationen zur Unterstützung von Benutzern bei der Zusammenarbeit in Workfront über Zeitzonen hinweg finden Sie <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Arbeiten über Zeitzonen hinweg</a>.</p> </li>

   <li><p><b>E-Mail</b>Gebietsschema: Das bevorzugte E-Mail-Gebietsschema des Benutzers. Dies wirkt sich auf das Format der Zahlen und Daten in den E-Mails aus, die von Workfront an diesen Benutzer gesendet werden.</p>
      <p><b>HINWEIS:</b> Wenn Ihr Unternehmen das einheitliche Adobe-Erlebnis verwendet, werden die Spracheinstellungen des Benutzers in seinem Adobe-Profil gespeichert und das E-Mail-Gebietsschema wird nicht verwendet. Weitere Informationen zum Zugriff auf diese Voreinstellungen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></li>

   <li><b>E-Mails von dieser Testumgebung empfangen</b>: Aktivieren Sie diese Option, wenn Sie E-Mail-Benachrichtigungen von der Umgebung erhalten möchten, in der Sie derzeit angemeldet sind.
      <p><b>NOTIZ</b></p>
      <p>Diese Option ist nur in der Vorschau- und Sandbox-Umgebung verfügbar. E-Mail-Benachrichtigungen sind standardmäßig in der Produktionsumgebung aktiviert. </p>
      </li>

   </li> 
       <li><b>Arbeit, die ich mir selbst zuweise, an meine Registerkarte „Arbeiten an“ senden</b>: Diese Einstellung bezieht sich auf eine veraltete Funktion, die aus Workfront entfernt wurde.</li> 
       <li><b>Beim Hochladen von Dokumenten automatisch Korrekturabzüge generieren</b>: Aktivieren Sie diese Option, wenn die Dokumente, die der Benutzer hochlädt, sofort einen Korrekturabzug generieren sollen. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benachrichtigungen</td> 
      <td> <p>Wählen Sie die E-Mail-Benachrichtigungen aus, die für den neuen Benutzer aktiviert werden sollen.</p> <p>Sie können sowohl sofortige als auch tägliche Digest-Benachrichtigungen auswählen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zugriff</td> 
      <td> 
       <ul> 
      <li><b>Ist Aktiv</b> Aktivieren Sie dieses Kontrollkästchen, um anzugeben, dass der Benutzer aktiv ist. Aktive Benutzende verwenden eine Workfront-Lizenz. Wenn Sie das Kästchen entfernen, wird der Benutzer deaktiviert und daran gehindert, sich bei Workfront anzumelden.</li> 
       <li> <p><b>Zugriffsebene:</b> Wählen Sie die Zugriffsebene aus, die Sie diesem Benutzer zuweisen möchten.</p> 
       <p>Wenn Sie einem Benutzer eine Zugriffsebene zuweisen, können Sie eine Zugriffsebene zuweisen, die Ihrer eigenen Zugriffsebene entspricht oder niedriger ist.</p>
       <p>Wenn Ihre Zugriffsebene beispielsweise „Plan“ lautet, können Sie keine Administrator-Zugriffsebene zuweisen. Sie können jedoch keine Zugriffsebene zuweisen, die standardmäßig niedriger ist als Ihre eigene Zugriffsebene, wenn der Workfront-Administrator nicht standardmäßige Berechtigungen auf der Zugriffsebene aktiviert hat, die nicht auch in Ihrer eigenen Zugriffsebene aktiviert sind. </p>
       <p>Wenn Sie beispielsweise über eine Planlizenz ohne Zugriff zum Löschen von Aufgaben verfügen, können Sie niemandem eine Arbeitslizenz mit Zugriff zum Löschen von Aufgaben zuweisen, obwohl die Arbeitslizenz niedriger als die Planlizenz ist. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>. </p> 
       <p>Weitere Informationen zu Zugriffsebenen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Zugriff auf Adobe Workfront konfigurieren</a>.</p>
       <p> <b>HINWEIS:</b></p> 
       <p> Wenn Ihr Unternehmen das neue Zugriffsmodell (Standard/Light/Contributor) verwendet, können Sie einen Standard- oder Light-Benutzer nicht einer Contributor-Zugriffsebene zuweisen, wenn dieser Benutzer bereits das Entscheidungslimit für den Monat erreicht hat. </p><p>Weitere Informationen zum neuen Zugriffsmodell finden Sie unter <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Übersicht über neue Zugriffsebenen</a>. </p><p>Informationen zu Entscheidungsbeschränkungen finden Sie unter <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Eingeschränktes Dokument und Korrekturabzugsentscheidung für nicht bezahlte Benutzer - Übersicht</a>.</p></li> 
       <li> <p><b>Layout-</b>: Wählen Sie eine Layout-Vorlage für den Benutzer aus. Diese Layout-Vorlage hat Vorrang vor jeder Layout-Vorlage, die der Hauptgruppe, dem Hauptteam oder der Primären Rolle des Benutzers zugewiesen ist. Weitere Informationen zur Zuweisungspriorität von Layout-Vorlagen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layout-Vorlagen</a>.</p> <p><b>HINWEIS</b>:  <p>In der folgenden Liste wird beschrieben, wie die Liste der Vorlagen, die Sie in diesem Feld haben, von Ihrem Zugriff abhängt:</p> 
       <ul> 
       <li>Als Workfront-Administrator können Sie alle Layoutvorlagen auf Systemebene und Gruppenebene sehen.</li> 
       <li>Als Gruppenadministrator bzw. -administratorin können Sie die Layoutvorlagen auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Vorlagen sehen.</li> 
       <li>Benutzende mit einer Planlizenz und dem Zugriff auf die Bearbeitung von Benutzenden können nur Layoutvorlagen auf Systemebene sehen.</li> 
       </ul> <p>Weitere Informationen zu Layout-Vorlagen auf Gruppenebene finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layout-Vorlagen</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation </td> 
      <td> 
       <ul> 
      <li><b>Unternehmen</b>: Das Unternehmen des Benutzers. Benutzende können nur mit einer Firma verknüpft werden. Sie müssen eine Firma erstellen, bevor Sie sie mit einem Benutzer verknüpfen können. In der Liste werden nur aktive Unternehmen angezeigt. Informationen zum Erstellen von Unternehmen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Erstellen und Bearbeiten von Unternehmen</a>.</li> 
      <li><b>Berichte an:</b> Wenn Sie ein Unternehmen für den Benutzer angegeben haben, können Sie in diesem Feld auch den direkten Manager des Benutzers angeben. Ein Benutzer kann nur über einen Manager verfügen. Dieses Feld wird nicht angezeigt, wenn der/die Benutzende nicht zuerst einer Firma zugeordnet ist. </li> 
      <li><b>Direktberichte:</b> Sie ein Unternehmen für den Benutzer angegeben haben, können Sie auch die Direktberichte des Benutzers angeben. Ein Benutzer kann über mehrere Direktberichte verfügen. Dieses Feld wird nicht angezeigt, wenn der/die Benutzende nicht zuerst einer Firma zugeordnet ist.</li> 
      <li><b>Home-</b>: Geben Sie das Home-Team für den Benutzer an. Benutzer können nur über ein Home-Team verfügen. Das Haupt-Team ist beim Zuweisen einer Layout-Vorlage oder beim Definieren der Schaltfläche Bearbeiten für die dem Benutzer zugewiesenen Aufgaben und Probleme wichtig. </li> 
      <li><b>Andere Teams</b>: Benutzer können mehreren Teams angehören. Ein(e) Benutzende(r) kann Arbeitselemente anzeigen, die einem seiner Teams in seinem/ihrem Home-Bereich zugewiesen sind. </li> 
      <li> <p><b>Hauptgruppe: </b> Sie eine geeignete Gruppe aus, um den Benutzer zuzuweisen. Dadurch kann der Benutzer auf Objekte zugreifen, die für die Gruppe freigegeben sind. Sie können Layout-Vorlagen auch für die Hauptgruppe der Benutzenden freigeben.</p> <p>Dies ist ein Pflichtfeld. Jeder Benutzer muss einer Hauptgruppe zugeordnet sein. Wenn Sie keine Hauptgruppe auswählen, wird diese der Hauptgruppe des neuen Benutzers zugewiesen.</p> <p><b>HINWEIS</b>:</p> 
      <p> Sie können eine Gruppe nur dann einem Benutzer zuweisen, wenn einer der folgenden Punkte zutrifft:</p>
      <ul><li>Sie sind ein Workfront-Administrator</li>
      <li>Sie sind der Administrator der Gruppe</li>
      <li>Die Gruppe ist öffentlich.</li></ul> 
      <li> <p><b>Andere Gruppen</b>: Benutzer können mehreren Gruppen angehören. Eine Gruppe kann einem Benutzer nur zugewiesen werden, wenn Sie Workfront-Administrator sind, Administrator der Gruppe sind oder die Gruppe öffentlich ist.</p> <p><b>WICHTIG</b>:</p> 
      <p>Das Hinzufügen eines Benutzers zu mehr als 100 Gruppen kann in jedem Bereich von Workfront, der die Liste der Gruppen lädt, zu Leistungsproblemen führen.</p> <p>Weitere Informationen zu öffentlichen Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Erstellen einer Gruppe</a>.</p> <p>Weitere Informationen zu Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppen - Übersicht</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ressourcenplanung </td> 
      <td> 
       <ul>
       <li>
       <b>Arbeitszeit</b>: Gibt den Prozentsatz der Vollzeitäquivalenzzeit (VZÄ) an, die der Benutzer für die tatsächliche Arbeit zur Verfügung hat, ohne Gemeinkosten. Arbeitszeit muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. So würde beispielsweise eine Verfügbarkeit von 20 % für die tatsächliche Arbeit 0,2 betragen.

   Der Standardwert des Feldes ist 1. Dies bedeutet, dass ein Benutzer sein gesamtes FTE für die tatsächliche, projektbezogene Arbeit verwendet.

   Anhand dieser Zahl berechnet das System die Verfügbarkeit des Nutzers für die tatsächliche, projektbezogene Arbeit.

   Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>.

   Zeitplanausnahmen und Ausfallzeiten können sich ebenfalls auf die Kapazität des Benutzers auswirken.

   Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich. Weitere Informationen finden Sie unter <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.

   <b>TIPP</b>

   Legen Sie den Wert für Arbeitszeit auf 1 fest, um anzugeben, dass der Benutzer für projektbezogene Arbeit bis zum gesamten Vollzeitäquivalent verfügbar ist.
   </li> 
      <li> <b>Deaktivierung planen</b>: Aktivieren Sie dieses Kontrollkästchen, wenn Sie möchten, dass dieser Benutzer an einem bestimmten Datum und zu einer bestimmten Uhrzeit deaktiviert wird. </li> 
       <li><b>Geplantes Deaktivierungsdatum</b>: Datum und Uhrzeit der Deaktivierung des Benutzers. Informationen zum Planen von Benutzern für die Deaktivierung finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planen von Benutzern für die </a>) in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren von Benutzern</a>.</li> 
       <li> <p><b>Primäre Rolle</b>: Dies ist das primäre Aufgabengebiet, das Benutzende in Workfront erfüllen können. Jede Aufgabe und jedes Problem, der bzw. dem der Benutzer zugewiesen ist, wird ebenfalls diesem Aufgabengebiet zugewiesen. Aufgabengebiete sind im Ressourcen-Management von entscheidender Bedeutung. Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planlizenz mit administrativem Benutzerzugriff verfügen oder wenn Sie ein Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit administrativem Benutzerzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> <p>In der Liste werden nur aktive Aufgabengebiete angezeigt. </p> </li> 
       <li>Wenn Sie eine <b>Primäre Rolle ausgewählt haben</b> wird das Feld <b>Prozentsatz der FTE-Verfügbarkeit</b> angezeigt. Geben Sie an, wie viel Prozent der Zeit im Zeitplan des Benutzers diesem Aufgabengebiet zugewiesen ist. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die Primäre Funktion ist 100 %. </li> 
       <li> <p><b>Andere Rollen</b>: Ein Benutzer kann über mehrere Aufgabengebiete in Workfront verfügen. Aufgabengebiete sind im Ressourcen-Management von entscheidender Bedeutung. Es gibt keine Begrenzung dafür, wie viele Aufgabengebiete ein Benutzer erfüllen kann. Wir empfehlen jedoch, einer zu großen Anzahl von Aufgabengebieten nicht einen Benutzer zuzuweisen, da die Ressourcenverwaltung für diese Benutzer möglicherweise zu komplex wird.<p>In der Liste werden nur aktive Aufgabengebiete angezeigt. Weitere Informationen zu Aufgabengebieten finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planlizenz mit administrativem Benutzerzugriff verfügen oder wenn Sie ein Workfront-Administrator sind. <br>Weitere Informationen zum Einrichten von Benutzern mit administrativem Benutzerzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Benutzerzugriffs</a>.</p> </li> 
       <li> <p>(Bedingt) Wenn Sie eine oder mehrere Rollen <b>Sonstige Rollen</b> ausgewählt haben, wird für </b> jeweilige Rolle das Feld <b>Prozentsatz der FTE-Verfügbarkeit“ angezeigt. Geben Sie an, welcher Prozentsatz des Zeitplans des Benutzers den einzelnen Aufgabengebieten zugewiesen wird. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die anderen Funktionen ist 0 %.</p> <p><b>HINWEIS</b>: Wenn andere Funktionen eine FTE-Verfügbarkeit von 0 % aufweisen, werden sie nicht im Ressourcenplaner angezeigt, es sei denn, die Benutzer sind Aufgaben in diesen Rollen zugewiesen.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>HINWEIS</b>: <p>Die Summe aller <b>Prozentsätze der FTE-Verfügbarkeit</b> für alle Rollen muss 100 % betragen. Jeder Prozentsatz der FTE-Verfügbarkeit berechnet die verfügbaren Stunden für jede Rolle pro Benutzer im Ressourcenplaner. Die verfügbaren Stunden für jede Rolle pro Benutzer hängen von der verfügbaren Zeit für den Benutzer ab.</p> <p>Die verfügbare Zeit für den Benutzer wird von Workfront abhängig von der Methode berechnet, die vom Workfront-Administrator zur Berechnung des FTE in den Voreinstellungen für das Ressourcenmanagement ausgewählt wurde.</p> <p>Informationen zur Berechnung der Verfügbarkeit für den Benutzer finden Sie unter <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung von Stunden und VZÄ für Benutzer und Funktionen im Ressourcenplaner</a>.</p> <p>Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurieren der Voreinstellungen für die </a>).</p> </p>
       <span class="preview"><p>(Optional) Datumsbasierte Zuweisungen für Aufgabengebiete werden in Finanzberechnungen verwendet, wenn sich das Aufgabengebiet des/r Benutzenden während eines Projekts ändert.</p><p>Klicken Sie auf <b>Rollen nach Datum definieren</b>, wählen Sie die <b>Primäre Rolle</b> und <b>Andere Rollen</b> aus und geben Sie den Zuordnungsprozentsatz für jede Rolle ein. Die Rollen können mit den vorhandenen Rollen übereinstimmen (mit unterschiedlichen Prozentsätzen) oder neue Rollen sein. Wählen Sie das <b>Startdatum</b> aus, an dem diese Rollen aktiv werden. Dies kann ein Datum in der Zukunft sein. Wenn die neuesten Rollen aktiv werden, können Sie auf <b>Vorherige Rollen anzeigen</b> klicken, um die vorherigen, inaktiven Rollen anzuzeigen.</p> </li></span>
       <li> <p><b>Zeitplan</b>: Verknüpfen Sie einen Zeitplan mit dem Benutzer. Der Zeitplan des Benutzers berechnet die Zeitleiste der Aufgaben, denen der Benutzer zugewiesen ist.</p> <p>Sie müssen einen Zeitplan erstellen, bevor Sie ihn einem Benutzer zuordnen können. Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Erstellen eines Zeitplans</a>.</p> <p><b>HINWEIS</b>: Es wird empfohlen, dass der Zeitplan, den Sie mit dem Benutzer verknüpfen, mit der Zeitzone des Benutzers übereinstimmt.</p> </li> 
       <li> <p><b>Arbeitszeittabellen-</b>: Verknüpfen Sie ein Arbeitszeittabellen-Profil mit dem Benutzer, um sicherzustellen, dass Arbeitszeittabellen automatisch für den Benutzer generiert werden.</p> <p><b>HINWEIS</b>: Die Liste der Profile, die in diesem Feld verfügbar sind, hängt von Ihrem Zugriff ab:
       <ul>
       <li>Als Workfront-Administrator können Sie alle Arbeitszeittabellen-Profile auf Systemebene und Gruppenebene anzeigen.</li>
       <li>Als Gruppenadministrator können Sie Arbeitszeittabellen-Profile auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Profile anzeigen.</li>
       <li>Benutzende mit Plan-Lizenz, die Zugriff auf die Bearbeitung von Benutzenden haben, können nur Arbeitszeittabellen-Profile auf Systemebene anzeigen. Weitere Informationen zu Arbeitszeittabellen-Profilen auf Gruppenebene finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen</a>.</li>
      </ul></p> </li> 
       <li><b>Standardstundentyp</b>: Wählen Sie den Standardstundentyp für den Benutzer aus. Dies ist der Stundentyp, der standardmäßig verwendet wird, wenn Benutzende die Zeit protokollieren.</li> 
       <li><b>Verfügbare Stundentypen</b>: Wählen Sie die Stundentypen aus, die für den Benutzer verfügbar sein sollen. Diese Stundentypen sind überall in Workfront sichtbar, wo Benutzende die Zeit protokollieren können. Ein Benutzer kann nur die Stundentypen sehen, die sowohl auf Projekt- als auch auf Benutzerebene aktiviert sind. Weitere Informationen dazu, welche Stundentypen Benutzern zur Verfügung stehen, finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Festlegen von Stundentypen und Verfügbarkeit</a>.</li> 
       <li><b>Zeit eintragen:</b> Wählen Sie aus, ob die Zeit in Arbeitselementen in Stunden oder Tagen protokolliert werden soll. Weitere Informationen finden Sie unter <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird</a>.</li>

   <li> <b>FTE</b>: Dies ist das Vollzeitäquivalent des Benutzers. Workfront verwendet diese Zahl, um die Verfügbarkeit der Benutzerin bzw. des Benutzers auf der Grundlage des Standardzeitplans nur dann zu berechnen, wenn die Ressourcenverwaltungseinstellungen auf Systemebene auf den Standardzeitplan eingestellt sind.

   <p>Das FTE gibt an, wie viel Zeit der Benutzer bei der Arbeit verbringen kann. Dazu gehören Gemeinkosten sowie die Zeit, die mit der Projektarbeit verbracht wird. Beispielsweise wird die Zeit, die in Meetings oder Schulungen verbracht wird, ebenfalls in das VZÄ einbezogen.</p>

   Der FTE muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. Wenn beispielsweise der FTE-Wert 0,5 beträgt und der Standardzeitplan in Workfront 40 Stunden beträgt, ist die Benutzerin bzw. der Benutzer 20 Stunden pro Woche verfügbar.

   Der Standardwert des Felds ist 1.

   Zeitplanausnahmen, Ausfallzeiten und der Wert der Arbeitszeit können sich auf die Verfügbarkeit der Benutzenden auswirken.

   Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich.

   Wenn die Voreinstellungen für das Ressourcen-Management auf Systemebene auf den Zeitplan des Benutzers festgelegt sind, wird der hier angegebene Wert ignoriert und der Benutzer wird gemäß den Angaben in seinem Zeitplan als verfügbar betrachtet.

   Weitere Informationen finden Sie unter <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.

   Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>.
   </li>

   <li><b>Ressourcenpools</b>: Verknüpfen Sie den Benutzer mit Ressourcenpools. Weitere Informationen finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Zuordnen von Ressourcenpools zu Benutzern </a>.</li>

   <li><b>Kostensatz</b>: Der Betrag der Kosten pro Stunde für den Benutzer.
      <p>Klicken Sie für gültige Datumssätze auf "<strong> hinzufügen</strong>. Geben Sie den Wert des Kostensatzes für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Kostensatz 1 hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.</p><p>Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Kostensatz 1 kein Enddatum hat und Sie Kostensatz 2 mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem Kostensatz 1 das Enddatum 30. April 2023 hinzugefügt, sodass keine Lücken entstehen.</p></li>

   <li><b>Abrechnungssatz</b>: Der Abrechnungsbetrag pro Stunde für den Benutzer.
      <p>Klicken Sie für Abrechnungssätze mit Gültigkeitsdatum auf <strong>Abrechnungssatz hinzufügen</strong>. Geben Sie den Wert des Abrechnungssatzes für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Abrechnungssatz 1 hat kein Startdatum und der letzte Abrechnungssatz hat kein Enddatum.</p> <p>Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungssatz 1 kein Enddatum hat und Sie eine Sekunde mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem Abrechnungssatz 1 ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.</p><p> <img alt="Benutzerkosten und Abrechnungssätze" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Formulare</td> 
      <td><p>Verknüpfen Sie ein benutzerdefiniertes Formular eines vorhandenen Benutzers mit diesem Benutzer. Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Felder, auf die Sie keinen Zugriff haben, werden nicht in einem einzelnen benutzerdefinierten Formular angezeigt.</p> <p><strong>Hinweis</strong> Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind nur verfügbar, wenn Sie den Benutzerdatensatz auf der Detailseite öffnen, nicht im Dialogfeld „Benutzer bearbeiten“. (Klicken Sie in der Benutzerliste auf den Benutzernamen, um die Details zu öffnen.)</p> <p>Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Erstellen eines benutzerdefinierten Formulars</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kommentar</td> 
      <td>Geben Sie den Kommentar ein, den Sie den Benutzern und dem Bereich Aktualisierungen ihrer Benutzerprofile senden möchten.</td> 
     </tr> 
    </tbody> 
   </table>
