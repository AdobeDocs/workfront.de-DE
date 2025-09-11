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
source-git-commit: de7432c66d9d71a4c1b0b4b6c43b306d0fae9fef
workflow-type: tm+mt
source-wordcount: '3425'
ht-degree: 0%

---

# Benutzerprofil bearbeiten

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/de/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Als Adobe Workfront-Administrator können Sie Benutzende erstellen und die Profile bestehender Profile verwalten. Informationen zum Erstellen von Benutzern finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Informationen dazu, wie Benutzer ihre eigenen Profile aktualisieren, finden Sie unter [Konfigurieren meiner Einstellungen](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

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

1. Wählen Sie den Benutzer aus und klicken Sie dann auf **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).

   Das Feld Benutzer bearbeiten wird angezeigt.

1. Ändern Sie im Feld **Benutzer bearbeiten** die Informationen in einem der Abschnitte und klicken Sie **auf** Speichern“.

### Persönliche Info

* **Vorname**
* **Nachname**

  >[!NOTE]
  >
  >Beim Bearbeiten des Benutzernamens in Workfront wird der Benutzername in der Adobe Admin Console nicht bearbeitet.

* **E-Mail** Adresse: Die E-Mail-Adresse für einen Benutzer ist auch dessen Benutzername in Workfront. Bei diesem Feld wird zwischen Groß- und Kleinschreibung unterschieden und es muss eindeutig sein. Wenn ein(e) Benutzende(r) versucht, innerhalb eines 10-minütigen Fensters dreimal eine nicht eindeutige E-Mail-Adresse hinzuzufügen, wird eine reCAPTCHA-Antwort angezeigt.

  Wählen Sie die Einstellung **Ich bin kein Roboter** aus, bevor Sie fortfahren können.

  Wenn Sie die E-Mail-Zulassungsliste verwenden und eine E-Mail-Domain eingeben, die nicht auf der Liste steht, erhält der/die Benutzende keine E-Mail-Benachrichtigungen. Weitere Informationen über die Zulassungsliste auf die Zulassungsliste setzte finden Sie unter [Konfigurieren Ihrer E-Mail](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

  Wenn Ihre Organisation in die Adobe Admin Console migriert wurde, können Sie die E-Mail-Adresse von Benutzenden in Workfront nicht bearbeiten. Die E-Mail-Adresse des Benutzers ist in der Adobe Admin Console festgelegt.

* **Kennwort ändern**: Klicken Sie auf diese Schaltfläche, um das Kennwort des Benutzers zurückzusetzen. Sie müssen Ihr eigenes Kennwort eingeben, bevor Sie das Kennwort eines anderen Benutzers zurücksetzen können.

  Zum Zurücksetzen des Kennworts eines anderen Benutzers müssen Sie ein Workfront-Administrator oder ein Gruppenadministrator sein.

  Wenn Sie Gruppenadministrator sind, können Sie Kennwörter nur für Benutzer in den Gruppen zurücksetzen, in denen Sie als Administrator festgelegt sind. Außerdem muss in Ihrer Zugriffsebene die Berechtigung Benutzeradmin (Gruppenbenutzer) aktiviert sein:

  ![Zugriffsebenen-Einstellung für Administrator des Benutzers](assets/group-admin-user.png)

  Diese Einstellung ist standardmäßig deaktiviert. Weitere Informationen finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Das Kennwort eines Workfront-Administrators kann nicht zurückgesetzt werden.

* **&lt;SSO-Konfiguration> Benutzername**: Wenn Ihr Workfront-Administrator eine SSO-Integration mit Workfront aktiviert hat, wird der SSO-Benutzername in diesem Feld angezeigt. Der Typ der für Ihre Workfront-Instanz aktivierten SSO-Konfiguration wird in diesem Feld angezeigt.
* **Nur &lt;SSO-Konfiguration> Authentifizierung zulassen**: Wenn der Workfront-Administrator eine SSO-Integration mit Workfront aktiviert hat und alle Benutzer für SSO aktualisiert hat, ist dieses Feld standardmäßig ausgewählt. Der Typ der für Ihre Workfront-Instanz aktivierten SSO-Konfiguration wird in diesem Feld angezeigt.

  Wenn dieses Feld ausgewählt ist, muss sich der Benutzer mit seinen SSO-Anmeldeinformationen bei Workfront anmelden. Wenn Sie diese Option deaktivieren, können sich Benutzer mit ihren Workfront-Anmeldeinformationen bei Workfront anmelden.

  Weitere Informationen zum Konfigurieren von Workfront mit einer SSO-Lösung finden Sie [Übersicht über Single Sign-on in Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

  Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter [Aktualisieren von Benutzern für einmaliges Anmelden](/help/quicksilver/administration-and-setup/add-users/single-sign-on/update-users-sso.md).

  >[!NOTE]
  >
  >Wenn Sie Gruppenadministrator sind, können Sie die Felder &lt;SSO Configuration> nur für Benutzer in den Gruppen bearbeiten, in denen Sie als solcher angegeben sind. Außerdem muss in Ihrer Zugriffsebene die Berechtigung Benutzeradmin (Gruppenbenutzer) aktiviert sein.
  >
  >Wenn Sie Gruppenadministrator sind und für Ihre Zugriffsebene die Berechtigung Benutzeradministration (alle Benutzer) aktiviert haben, können Sie die Felder &lt;SSO-Konfiguration> für alle Benutzer bearbeiten.

* **Profilfoto**: Klicken Sie auf **Neu hochladen**, um das Profilbild des Benutzers zu laden. Sie können eine JPG-, GIF- oder PNG-Datei hochladen. Die Dateigrößenbeschränkung beträgt 4 MB.

  Das Profilbild wird zum Avatar der Benutzerin oder des Benutzers und ist im gesamten Workfront-System sichtbar, unabhängig davon, wo der Name der Person angezeigt wird.

* **Jobinfo**: Informationen über den Auftrag, wie z. B. die Stellenbezeichnung (im **Titel**-Feld) und den Fachbereich, für den der Benutzer verantwortlich ist (im **Sprechen Sie mit mir über**).
* **Kontaktinformationen**: Die Telefonnummer des Benutzers (in der **Telefonnummer**, **Durchwahl.** und **Mobiltelefonnummer**) und Adresse (in den Feldern **Adresse**, **Stadt**, **Staat**, **Postleitzahl** und **Land**).

  Wenn die Benutzerin bzw. der Benutzer für Unified User Management (UUM) oder Adobe Identity Management System (IMS) aktiviert ist, akzeptiert das Feld **Country** im Abschnitt Kontaktinformationen nur Ländercodewerte (z. B. US, GB, IN).

### Einstellungen

* **Zeitzone**: Die Zeitzone des Benutzers.

  Informationen zur Unterstützung von Benutzern bei der Zusammenarbeit in Workfront über Zeitzonen hinweg finden Sie [Arbeiten über Zeitzonen hinweg](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **E-Mail** Gebietsschema: Das bevorzugte E-Mail-Gebietsschema des Benutzers. Dies wirkt sich auf das Format der Zahlen und Daten in den E-Mails aus, die von Workfront an diesen Benutzer gesendet werden.

  >[!NOTE]
  >
  >Wenn Ihr Unternehmen Adobe Unified Experience nutzt, werden die Spracheinstellungen des Benutzers in seinem Adobe-Profil gespeichert und das E-Mail-Gebietsschema wird nicht verwendet. Informationen zum Zugriff auf diese Voreinstellungen finden Sie unter [Einheitliches Adobe-Erlebnis für Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* **E-Mails von dieser Testumgebung empfangen**: Aktivieren Sie diese Option, wenn Sie E-Mail-Benachrichtigungen von der Umgebung erhalten möchten, in der Sie derzeit angemeldet sind.

  >[!NOTE]
  >
  >Diese Option ist nur in der Vorschau- und Sandbox-Umgebung verfügbar. E-Mail-Benachrichtigungen sind standardmäßig in der Produktionsumgebung aktiviert.

<!--* **Automatically set the task status to In Progress when tasks are self-assigned**: When this option is selected, work that the user self-assigns is automatically set to In Progress status instead of New.-->

* **Arbeit, die ich mir selbst zuweise, an meine Registerkarte „Arbeiten an“ senden**: Wenn diese Option aktiviert ist, wird Arbeit, die der/die Benutzende sich selbst zuweist, automatisch auf den Status „In Bearbeitung“ anstelle von „Neu“ gesetzt. <!--This setting refers to a deprecated feature that has been removed from Workfront.-->

* **Beim Hochladen von Dokumenten automatisch Korrekturabzüge generieren**: Aktivieren Sie diese Option, wenn die Dokumente, die der Benutzer hochlädt, sofort einen Korrekturabzug generieren sollen.

### Benachrichtigungen

Wählen Sie die E-Mail-Benachrichtigungen aus, die für den neuen Benutzer aktiviert werden sollen.

Sie können sowohl sofortige als auch tägliche Digest-Benachrichtigungen auswählen.

Weitere Informationen finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

### Zugriff

* **Benutzer ist aktiv**: Aktivieren Sie diese Option, um anzugeben, dass der Benutzer aktiv ist. Aktive Benutzende verwenden eine Workfront-Lizenz. Durch Deaktivieren des Felds wird der Benutzer deaktiviert und daran gehindert, sich bei Workfront anzumelden.

* **Zugriffsebene**: Wählen Sie die Zugriffsebene aus, die Sie diesem Benutzer zuweisen möchten.

  Wenn Sie einem Benutzer eine Zugriffsebene zuweisen, können Sie eine Zugriffsebene zuweisen, die Ihrer eigenen Zugriffsebene entspricht oder niedriger ist. (Wenn Ihre Zugriffsebene beispielsweise „Standard“ ist, können Sie keine Administratorzugriffsebene zuweisen.)

  Sie können jedoch keine Zugriffsebene zuweisen, die standardmäßig niedriger ist als Ihre eigene Zugriffsebene, wenn der Workfront-Administrator nicht standardmäßige Berechtigungen auf der Zugriffsebene aktiviert hat, die nicht auch in Ihrer eigenen Zugriffsebene aktiviert sind.

  Wenn Sie beispielsweise über eine Standardlizenz ohne Zugriff auf das Löschen von Aufgaben verfügen, können Sie niemandem eine Light-Lizenz mit Zugriff auf das Löschen von Aufgaben zuweisen, obwohl die Light-Lizenz niedriger als die Standard-Lizenz ist. Weitere Informationen finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Weitere Informationen zu Zugriffsebenen finden Sie unter [Zugriff auf Adobe Workfront konfigurieren](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  >[!NOTE]
  >
  >Wenn Ihr Unternehmen das neue Zugriffsmodell (Standard/Light/Contributor) verwendet, können Sie einen Standard- oder Light-Benutzer nicht einer Contributor-Zugriffsebene zuweisen, wenn dieser Benutzer bereits das Entscheidungslimit für den Monat erreicht hat.
  >
  >Weitere Informationen zum neuen Zugriffsmodell finden Sie unter [Übersicht über neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >Informationen zu Entscheidungsbeschränkungen finden Sie unter [Eingeschränktes Dokument und Korrekturabzugsentscheidung für nicht bezahlte Benutzer - Übersicht](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Layout-**: Wählen Sie eine Layout-Vorlage für den Benutzer aus. Diese Layout-Vorlage hat Vorrang vor jeder Layout-Vorlage, die der Hauptgruppe, dem Hauptteam oder der Primären Rolle des Benutzers zugewiesen ist. Weitere Informationen zur Zuweisungspriorität von Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

  In der folgenden Liste wird beschrieben, wie die Liste der Vorlagen, die Sie in diesem Feld haben, von Ihrem Zugriff abhängt:

   * Als Workfront-Administrator können Sie alle Layoutvorlagen auf Systemebene und Gruppenebene sehen.
   * Als Gruppenadministrator bzw. -administratorin können Sie die Layoutvorlagen auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Vorlagen sehen.
   * Benutzende mit einer Standard- oder Plan-Lizenz, die Zugriff auf die Bearbeitung von Benutzenden haben, können nur Layoutvorlagen auf Systemebene sehen.

     Weitere Informationen zu Layout-Vorlagen auf Gruppenebene finden Sie unter [Erstellen und Ändern der Layout-Vorlagen einer Gruppe](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organisation

* **Unternehmen**: Das Unternehmen des Benutzers. Benutzende können nur mit einer Firma verknüpft werden. Sie müssen eine Firma erstellen, bevor Sie sie mit einem Benutzer verknüpfen können. In der Liste werden nur aktive Unternehmen angezeigt. Informationen zum Erstellen von Unternehmen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* **Berichte an**: Wenn Sie ein Unternehmen für den Benutzer angegeben haben, können Sie in diesem Feld auch den direkten Manager des Benutzers angeben. Ein Benutzer kann nur über einen Manager verfügen. Dieses Feld wird nicht angezeigt, wenn der/die Benutzende nicht zuerst einer Firma zugeordnet ist.
* **Direktberichte**: Wenn Sie ein Unternehmen für den Benutzer angegeben haben, können Sie auch die Direktberichte des Benutzers angeben. Ein Benutzer kann über mehrere Direktberichte verfügen. Dieses Feld wird nicht angezeigt, wenn der/die Benutzende nicht zuerst einer Firma zugeordnet ist.
* **Home-**: Geben Sie das Home-Team für den Benutzer an. Benutzer können nur über ein Home-Team verfügen. Das Haupt-Team ist beim Zuweisen einer Layout-Vorlage oder beim Definieren der Schaltfläche Bearbeiten für die dem Benutzer zugewiesenen Aufgaben und Probleme wichtig.
* **Andere Teams**: Benutzer können mehreren Teams angehören. Ein(e) Benutzende(r) kann Arbeitselemente anzeigen, die einem seiner Teams in seinem/ihrem Home-Bereich zugewiesen sind.
* **Aktuelle Hauptgruppe**: Wählen Sie eine geeignete Gruppe aus, um den Benutzer zuzuweisen. Dadurch kann der Benutzer auf Objekte zugreifen, die für die Gruppe freigegeben sind. Sie können Layout-Vorlagen auch für die Hauptgruppe der Benutzenden freigeben.

  Dies ist ein Pflichtfeld. Jeder Benutzer muss einer Hauptgruppe zugeordnet sein. Wenn Sie keine Hauptgruppe auswählen, wird diese der Hauptgruppe des neuen Benutzers zugewiesen.

  Sie können eine Gruppe nur dann einem Benutzer zuweisen, wenn einer der folgenden Punkte zutrifft:

   * Sie sind ein Workfront-Administrator
   * Sie sind der Administrator der Gruppe
   * Die Gruppe ist öffentlich

* **Andere Gruppen**: Benutzer können mehreren Gruppen angehören. Eine Gruppe kann einem Benutzer nur zugewiesen werden, wenn Sie Workfront-Administrator sind, Administrator der Gruppe sind oder die Gruppe öffentlich ist.

  >[!IMPORTANT]
  >
  >Das Hinzufügen eines Benutzers zu mehr als 100 Gruppen kann in jedem Bereich von Workfront, der die Liste der Gruppen lädt, zu Leistungsproblemen führen.

  Weitere Informationen zu öffentlichen Gruppen finden Sie unter [Erstellen einer Gruppe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

  Weitere Informationen zu Gruppen finden Sie unter [Gruppen - Übersicht](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Ressourcenplanung

* **Arbeitszeit**: Gibt den Prozentsatz der Vollzeitäquivalenzzeit (VZÄ) an, die der Benutzer für die tatsächliche Arbeit zur Verfügung hat, ohne Gemeinkosten. Arbeitszeit muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. So würde beispielsweise eine Verfügbarkeit von 20 % für die tatsächliche Arbeit 0,2 betragen.

  Der Standardwert des Feldes ist 1. Dies bedeutet, dass ein Benutzer sein gesamtes FTE für die tatsächliche, projektbezogene Arbeit verwendet.

  Anhand dieser Zahl berechnet das System die Verfügbarkeit des Nutzers für die tatsächliche, projektbezogene Arbeit.

  Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter [Erstellen eines Zeitplans](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Zeitplanausnahmen und Ausfallzeiten können sich ebenfalls auf die Kapazität des Benutzers auswirken.

  Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich. Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  >[!TIP]
  >
  >Legen Sie den Wert für Arbeitszeit auf 1 fest, um anzugeben, dass der Benutzer für projektbezogene Arbeit bis zum gesamten Vollzeitäquivalent verfügbar ist.

* **Deaktivierungsdatum festlegen** Klicken Sie auf diese Schaltfläche, um die Deaktivierung dieses Benutzers zu einem bestimmten Datum und zu einer bestimmten Uhrzeit zu planen.
* **Deaktivierungsdatum**: Datum und Uhrzeit der Deaktivierung des Benutzers. Informationen zum Planen von Benutzern für die Deaktivierung finden Sie unter [Planen von Benutzern für die ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation)) in [Deaktivieren oder Reaktivieren von Benutzern](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
* **Primäre Rolle**: Dies ist das primäre Aufgabengebiet, das Benutzende in Workfront erfüllen können. Jede Aufgabe und jedes Problem, der bzw. dem der Benutzer zugewiesen ist, wird ebenfalls diesem Aufgabengebiet zugewiesen. Aufgabengebiete sind im Ressourcen-Management von entscheidender Bedeutung. Sie können dieses Feld nur aktualisieren, wenn Sie über eine Standard- oder Planlizenz mit administrativem Benutzerzugriff verfügen oder wenn Sie ein Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit administrativem Benutzerzugriff finden Sie unter [Gewähren des Zugriffs für Benutzer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  In der Liste werden nur aktive Aufgabengebiete angezeigt.

* (Bedingt) Wenn Sie eine **Primäre Rolle ausgewählt haben** wird das Feld **Prozentsatz der FTE-Verfügbarkeit** angezeigt. Geben Sie an, wie viel Prozent der Zeit im Zeitplan des Benutzers diesem Aufgabengebiet zugewiesen ist. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die Primäre Funktion ist 100 %.
* **Andere Rollen**: Ein Benutzer kann über mehrere Aufgabengebiete in Workfront verfügen. Aufgabengebiete sind im Ressourcen-Management von entscheidender Bedeutung. Es gibt keine Begrenzung dafür, wie viele Aufgabengebiete ein Benutzer erfüllen kann. Wir empfehlen jedoch, einer zu großen Anzahl von Aufgabengebieten nicht einen Benutzer zuzuweisen, da die Ressourcenverwaltung für diese Benutzer möglicherweise zu komplex wird.

  In der Liste werden nur aktive Aufgabengebiete angezeigt. Weitere Informationen zu Aufgabengebieten finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

  Sie können dieses Feld nur aktualisieren, wenn Sie über eine Standard- oder Planlizenz mit administrativem Benutzerzugriff verfügen oder wenn Sie ein Workfront-Administrator sind.

  Weitere Informationen zum Einrichten von Benutzern mit administrativem Benutzerzugriff finden Sie unter [Gewähren des Zugriffs für Benutzer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Bedingt) Wenn Sie eine oder mehrere Rollen **Sonstige Rollen** ausgewählt haben, wird für **jeweilige Rolle das Feld** Prozentsatz der FTE-Verfügbarkeit“ angezeigt. Geben Sie an, welcher Prozentsatz des Zeitplans des Benutzers den einzelnen Aufgabengebieten zugewiesen wird. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die anderen Funktionen ist 0 %.

  Wenn für andere Funktionen eine FTE-Verfügbarkeit von 0 % verfügbar ist, werden sie nicht im Ressourcenplaner angezeigt, es sei denn, die Benutzer sind Aufgaben in diesen Rollen zugewiesen.

  ![Benutzerrollen und FTE](assets/user-roles-fte-2025.png)

  Die Summe aller **Prozentsätze der FTE-Verfügbarkeit** für alle Rollen muss 100 % betragen. Jeder Prozentsatz der FTE-Verfügbarkeit berechnet die verfügbaren Stunden für jede Rolle pro Benutzer im Ressourcenplaner. Die verfügbaren Stunden für jede Rolle pro Benutzer hängen von der verfügbaren Zeit für den Benutzer ab.

  Die verfügbare Zeit für den Benutzer wird von Workfront abhängig von der Methode berechnet, die vom Workfront-Administrator zur Berechnung des FTE in den Voreinstellungen für das Ressourcenmanagement ausgewählt wurde.

  Informationen zur Berechnung der Verfügbarkeit für den Benutzer finden Sie unter [Übersicht über die Berechnung von Stunden und VZÄ für Benutzer und Funktionen im Ressourcenplaner](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung finden Sie [Konfigurieren der Voreinstellungen für die ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)).

  <span class="preview">(Optional) Datumsbasierte Zuweisungen für Aufgabengebiete werden in Finanzberechnungen verwendet, wenn sich das Aufgabengebiet des/r Benutzenden während eines Projekts ändert.</span>

  <span class="preview">Klicken Sie auf **Rollen nach Datum definieren**, wählen Sie die **Primäre Funktion** und **Andere Funktionen** aus und geben Sie den Zuordnungsprozentsatz für jede Funktion ein. Die Rollen können mit den vorhandenen Rollen übereinstimmen (mit unterschiedlichen Prozentsätzen) oder neue Rollen sein. Wählen Sie das Startdatum aus, an dem diese Rollen aktiv werden. Dies kann ein Datum in der Zukunft sein. Wenn die neuesten Rollen aktiv werden, können Sie auf **Vorherige Rollen anzeigen** klicken, um die vorherigen, inaktiven Rollen anzuzeigen.</span>

* **Zeitplan**: Verknüpfen Sie einen Zeitplan mit dem Benutzer. Der Zeitplan des Benutzers berechnet die Zeitleiste der Aufgaben, denen der Benutzer zugewiesen ist.

  Sie müssen einen Zeitplan erstellen, bevor Sie ihn einem Benutzer zuordnen können. Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter [Erstellen eines Zeitplans](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  >[!NOTE]
  >
  >Es wird empfohlen, dass der mit dem Benutzer verknüpfte Zeitplan mit der Zeitzone des Benutzers übereinstimmt.

  >[!IMPORTANT]
  >
  >Workfront verwendet den Zeitplan eines Benutzers nur, wenn die Einstellung **Ressourcenverfügbarkeit berechnen mit** auf &quot;**des Benutzers“** ist. Weitere Informationen darüber, wie sich diese Einstellung auf den für die Ressourcenverwaltung verwendeten Zeitplan auswirkt, finden Sie [Konfigurieren der Voreinstellungen für die ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)&quot;.

* **Arbeitszeittabellen-**: Verknüpfen Sie ein Arbeitszeittabellen-Profil mit dem Benutzer, um sicherzustellen, dass Arbeitszeittabellen automatisch für den Benutzer generiert werden.

  Die Liste der Profile, die in diesem Feld verfügbar sind, hängt von Ihrem Zugriff ab:

   * Als Workfront-Administrator können Sie alle Arbeitszeittabellen-Profile auf Systemebene und Gruppenebene anzeigen.
   * Als Gruppenadministrator können Sie Arbeitszeittabellen-Profile auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Profile anzeigen.
   * Benutzende mit einer Standard- oder Plan-Lizenz, die Zugriff haben, um Benutzende zu bearbeiten, können nur Arbeitszeittabellen-Profile auf Systemebene sehen. Weitere Informationen zu Arbeitszeittabellen-Profilen auf Gruppenebene finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Standardstundentyp**: Wählen Sie den Standardstundentyp für den Benutzer aus. Dies ist der Stundentyp, der standardmäßig verwendet wird, wenn Benutzende die Zeit protokollieren.
* **Verfügbare Stundentypen**: Wählen Sie die Stundentypen aus, die für den Benutzer verfügbar sein sollen. Diese Stundentypen sind überall in Workfront sichtbar, wo Benutzende die Zeit protokollieren können. Ein Benutzer kann nur die Stundentypen sehen, die sowohl auf Projekt- als auch auf Benutzerebene aktiviert sind. Weitere Informationen dazu, welche Stundentypen Benutzern zur Verfügung stehen, finden Sie unter [Festlegen von Stundentypen und Verfügbarkeit](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **Zeit eintragen**: Wählen Sie aus, ob die Zeit in Arbeitselementen in Stunden oder Tagen protokolliert werden soll. Weitere Informationen finden Sie unter [Konfigurieren, ob die Zeit in Stunden oder Tagen protokolliert wird](/help/quicksilver/timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).
* **FTE**: Dies ist das Vollzeitäquivalent des Benutzers. Workfront verwendet diese Zahl, um die Verfügbarkeit der Benutzerin bzw. des Benutzers auf der Grundlage des Standardzeitplans nur dann zu berechnen, wenn die Ressourcenverwaltungseinstellungen auf Systemebene auf den Standardzeitplan eingestellt sind.

  Das FTE gibt an, wie viel Zeit der Benutzer bei der Arbeit verbringen kann. Dazu gehören Gemeinkosten sowie die Zeit, die mit der Projektarbeit verbracht wird. Beispielsweise wird die Zeit, die in Meetings oder Schulungen verbracht wird, ebenfalls in das VZÄ einbezogen.

  Der FTE muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. Wenn beispielsweise der FTE-Wert 0,5 beträgt und der Standardzeitplan in Workfront 40 Stunden beträgt, ist die Benutzerin bzw. der Benutzer 20 Stunden pro Woche verfügbar.

  Der Standardwert des Felds ist 1.

  Zeitplanausnahmen, Ausfallzeiten und der Wert der Arbeitszeit können sich auf die Verfügbarkeit der Benutzenden auswirken.

  Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich.

  Wenn die Voreinstellungen für das Ressourcen-Management auf Systemebene auf den Zeitplan des Benutzers festgelegt sind, wird der hier angegebene Wert ignoriert und der Benutzer wird gemäß den Angaben in seinem Zeitplan als verfügbar betrachtet.

  Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter [Erstellen eines Zeitplans](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Ressourcenpools**: Verknüpfen Sie den Benutzer mit Ressourcenpools. Weitere Informationen finden Sie unter [Zuordnen von Ressourcenpools zu Benutzern](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).
* **Kostensatz**: Der Betrag der Kosten pro Stunde für den Benutzer.

  Klicken Sie für gültige Datumssätze auf &quot;**hinzufügen**. Geben Sie den Wert des Kostensatzes für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Kostensatz 1 hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.

  Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Kostensatz 1 kein Enddatum hat und Sie Kostensatz 2 mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem Kostensatz 1 das Enddatum 30. April 2023 hinzugefügt, sodass keine Lücken entstehen.

* **Abrechnungssatz**: Der Abrechnungsbetrag pro Stunde für den Benutzer.

  Klicken Sie für Abrechnungssätze mit Gültigkeitsdatum auf **Abrechnungssatz hinzufügen**. Geben Sie den Wert des Abrechnungssatzes für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Abrechnungssatz 1 hat kein Startdatum und der letzte Abrechnungssatz hat kein Enddatum.

  Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungssatz 1 kein Enddatum hat und Sie eine Sekunde mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem Abrechnungssatz 1 ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.

  ![Benutzerkosten und Abrechnungssätze](assets/user-cost-billing-rates-2025.png)

### Benutzerdefinierte Formulare

Verknüpfen Sie ein benutzerdefiniertes Formular eines vorhandenen Benutzers mit diesem Benutzer. Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Felder, auf die Sie keinen Zugriff haben, werden nicht in einem einzelnen benutzerdefinierten Formular angezeigt.

>[!NOTE]
>
>Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind nur verfügbar, wenn Sie den Benutzerdatensatz auf der Detailseite öffnen, nicht im Dialogfeld „Benutzer bearbeiten“. (Klicken Sie in der Benutzerliste auf den Benutzernamen, um die Details zu öffnen.)

Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Kommentar

Geben Sie den Kommentar ein, den Sie an die Benutzerin bzw. den Benutzer senden möchten, und gehen Sie zum Bereich Aktualisierungen ihres Benutzerprofils.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personal Info </td> 
      <td> 
       <ul> 
        <li><p><b>First Name</b></p></li>
        <li><p><b>Last Name</b></p><p><b>NOTE:</b></p><p>Editing a user's name in Workfront does not edit the user's name in the Adobe Admin Console.</p></li> 
        <li> <p><b>Email Address:</b> The email address for a user is also their username in Workfront. This field is case-sensitive and must be unique. If any user attempts to add a non-unique email address 3 times within a 10-minute window, a reCAPTCHA response appears.</p> <p> Select the <b>I am not a robot</b> setting before you can proceed.</p><p>If you use the email allowlist and enter an email domain not on the list, the user will not receive email notifications. For more information about the allowlist, see <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configure your email allowlist</a>.</p><p>If your organization has been migrated to the Adobe Admin Console, you cannot edit a user's email address in Workfront. The user's email address is set in the Adobe Admin Console. </li> 
        <li> <p><b>Reset Password</b>: Click this link to reset the user's password. You must enter your own password before you can reset another user's password.</p> <p>To reset another user's password, you must be a Workfront administrator, or a group administrator.</p> <p><b>NOTE</b>:  
          <ul> 
           <li> <p>If you are a group administrator, you can reset passwords only for users in the groups where you are designated as an administrator. Also, the User Admin (Group Users) permission must be enabled in your access level:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>This setting is disabled by default. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
           <li> <p>You cannot reset the password of a Workfront administrator.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO Configuration&gt; Username</b>: If your Workfront administrator enabled an SSO integration with Workfront, the SSO Username displays in this field. The type of SSO configuration enabled for your Workfront instance is visible in this field. </li> 
        <li> <p><b>OnlyAllow &lt;SSO Configuration&gt; Authentication</b>: If your Workfront administrator enabled an SSO integration with Workfront and has updated all users for SSO, this field is selected by default. The type of SSO configuration enabled for your Workfront instance is visible in this field.</p> <p>When this field is selected, the user is required to log into Workfront with their SSO credentials. Unchecking it will allow them to log in to Workfront with their Workfront credentials.</p> <p>For more information about configuring Workfront with an SSO solution, see <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Overview of single sign-on in Adobe Workfront</a></p> <p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p> 
        <p><b>NOTE</b>:</p> 
        <p> If you are a group administrator, you can edit the &lt;SSO Configuration&gt; fields only for users in the groups where you are designated as such. Also, the User Admin (Group Users) permission must be enabled in your access level.
        <p>If you are a group administrator and you have the User Admin (All Users) permission enabled in your access level, you can edit the &lt;SSO Configuration&gt; fields for all users.</p> </li> 
        <li><b>Job Info:</b> Information about the job, like the job title (in the <b>Title</b> field), and what area of expertise the user is responsible for (in the <b>Talk to Me About</b> field).</li> 
        <li><p><b>Contact Info</b>: The user's phone number (in the <b>Phone number, Ext.</b>, and <b>Mobile number</b> fields) and address (in the <b>Address, City, State, Postal Code, Country</b> fields ).</p>
        <p>If the user is enabled for Unified User Management (UUM) or Adobe Identity Management System (IMS), the <b>Country</b> field in the Contact Info section only accepts country code values (for example, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferences </td> 
      <td> 
       <ul> 
      <li> <p><b>Time Zone:</b> The user's time zone.</p> <p>For information about helping users collaborate in Workfront across time zones, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Working across time zones</a>.</p> </li>

      <li><p><b>Email Locale</b>: The user's preferred email locale. This affects the format of numbers and dates in the emails that come from Workfront to this user.</p>
      <p><b>NOTE:</b> When your organization is on the Adobe Unified Experience, the user's language preferences are stored in their Adobe profile and the email locale is not used. For information about accessing these preferences, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></li> 
      
      <li><b>Receive emails from this test environment</b>: Check this option if you want to receive email notifications from the environment that you are currently logged in.
      <p><b>NOTE</b></p>
      <p>This option is available only in the Preview and Sandbox environments. Email notifications are enabled in the Production environment by default. </p>
      </li> 
      
      </li> 
       <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       <li><b>Automatically generate proofs when uploading documents</b>: Check this option if you want the documents that the user uploads to immediately generate a proof. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td> <p>Select the email notifications which should be enabled for the new user.</p> <p>You can select instant as well as daily digest notifications.</p> <p>For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
      <li><b>Is Active:</b> Select this box to indicate that the user is active. Active users use a Workfront license. Clearing the box deactivates the user and prevents them from logging in to Workfront.</li> 
       <li> <p><b>Access Level:</b> Select the access level to assign to this user.</p> 
       <p>When you assign an access level to a user, you can assign a level equal to or lower than your own access level.</p>
       <p>For example, if your access level is Plan, you cannot assign the Administrator access level. However, you cannot assign an access level that by default is lower than your own access level if the Workfront administrator has enabled non-default permissions on the access level that are not also enabled in your own access level. </p>
       <p>For example, if you have a Plan license with no access to delete tasks, you cannot assign someone a Work license with access to delete tasks, although the Work license is lower than the Plan license. For more information, see  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> 
       <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p>
       <p> <b>NOTE:</b></p> 
       <p> If your organization uses the new access model (Standard/Light/Contributor), you cannot reassign a Standard or Light user to a Contributor access level if that user has already reached their decision limit for the month. </p><p>For more information on the new access model, see <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">New access levels overview</a>. </p><p>For information on decision limits, see <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Limited document and proof decision for non-paid users overview</a>.</p></li> 
       <li> <p><b>Layout Template</b>: Choose a Layout Template for the user. This Layout Template takes precedence over any Layout Template assigned to the user's Home Group, Home Team or Primary Role. For more information about the assignment priority of Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> <p><b>NOTE</b>:  <p>The following list describes how the list of templates you have available in this field depends on your access:</p> 
       <ul> 
       <li>As a Workfront administrator, you can see all system-level and group-level Layout Templates.</li> 
       <li>As a group administrator, you can see system-level layout template, as well as those associated with the groups that you manage.</li> 
       <li>As a user with a Plan license and access to edit users, you can see only system-level Layout Templates.</li> 
       </ul> <p>For more information about group-level Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization </td> 
      <td> 
       <ul> 
      <li><b>Company</b>: The company of the user. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Create and edit companies</a>.</li> 
      <li><b>Reports to:</b> If you specified a company for the user, you can also specify the direct manager of the user in this field. A user can have only one manager. This field does not display if the user is not associated with a company first. </li> 
      <li><b>Direct Reports:</b> If you specified a company for the user, you can also specify the direct reports of the user. A user can have multiple direct reports. This field does not display if the user is not associated with a company first.</li> 
      <li><b>Home Team</b>: Specify the home team for the user. Users can only have one home team. The Home Team is important when assigning a layout template or when defining the Work On It button for the tasks and issues assigned to the user. </li> 
      <li><b>Other Teams</b>: Users can belong to multiple teams. A user can view work items assigned to any of their teams in their Home area. </li> 
      <li> <p><b>Home Group:</b> Select an appropriate group to assign the user. This gives the user the ability to access objects that are shared with the group. You can also share layout templates with the user's Home Group.</p> <p>This is a required field. Every user must be associated with a home group. If you don't select one, your Home Group is assigned as the new user's Home Group.</p> <p><b>NOTE</b>:</p> 
      <p> You can assign a group to a user only if one of the following is true:</p>
      <ul><li>you are a Workfront administrator</li>
      <li>you are the administrator of the group</li>
      <li>the group is public.</li></ul> 
      <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only if you are a Workfront administrator, you are the administrator of the group, or the group is public.</p> <p><b>IMPORTANT</b>:</p> 
      <p>Adding a user to more than 100 groups may cause performance issues in any area of Workfront that loads the list of groups.</p> <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning </td> 
      <td> 
       <ul>
       <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.  

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user's capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to 1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 
      <li> <b>Schedule Deactivation</b>: Check this box if you want to schedule this user to be deactivated on a certain date and at a certain time. </li> 
       <li><b>Scheduled Deactivation Date</b>: The date and time on which the user becomes deactivated. For information about scheduling users for deactivation, see the <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that the user can fulfill in Workfront. Every task and issue that the user is assigned to is also assigned to this job role. Job roles are essential in resource management. You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> <p>Only active job roles display in the list. </p> </li> 
       <li>If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the user's schedule is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%. </li> 
       <li> <p><b>Other Roles</b>: A user can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.<p>Only active job roles display in the list. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. <br>For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the user's schedule is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTE</b>: <p>The sum of all <b>Percentages of FTE Availability</b> for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </p>
       <span class="preview"><p>(Optional) Date effective job role assignments are used in financial calculations if the user's job role changes during a project.</p><p>Click <b>Define roles by date</b>, select the <b>Primary Role</b> and <b>Other Roles</b>, and enter the allocation percentage for each role. The roles could be the same as the existing roles (using different percentages), or new roles. Select the <b>Start date</b> when these roles become active. This can be a future date. When the newest roles become active, you can click <b>Show previous roles</b> to see the previous, inactive roles.</p> </li></span>
       <li> <p><b>Schedule</b>: Associate a schedule with the user. The schedule of the user calculates the timeline of the tasks the user is assigned to.</p> <p>You must create a schedule before you can associate it with a user. For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>NOTE</b>: We recommend that the schedule you associate with the user matches the user's Time Zone.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the user to ensure that timesheets generate automatically for the user.</p> <p><b>NOTE</b>:  The list of profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and all group-level Timesheet Profiles.</li>
       <li>As a group administrator, you can see system-level Timesheet Profiles, as well as those associated with the groups that you manage.</li>
       <li>As a user with a Plan license and access to edit users, you can see only system-level Timesheet Profiles. For more information about group-level Timesheet Profiles, see <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Create, edit, and assign timesheet profiles</a>.</li>
      </ul></p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the user. This is the hour type that is used by default when the user logs time.</li> 
       <li><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the user can log time. A user can only see the hour types that are enabled at the project level as well as the user level. For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</li> 
       <li><b>Log Time in:</b> Select whether the user should log time on work items in hours or days. For more information, see <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configure whether time is logged in hours or days</a>.</li>
       
      <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
      
      <li><b>Resource Pools</b>: Associate the user with Resource Pools. For more information, see <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a>.</li> 
      
      <li><b>Cost Rate</b>: The amount of cost per hour for the user.
      <p>For date effective cost rates, click <strong>Add Rate</strong>. Enter the value of the cost rate for the time period, and assign a Start Date and End Date as needed. Cost Rate 1 will not have a start date and the last cost rate will not have an end date.</p><p>Some dates are added automatically. For example, if Cost Rate 1 does not have an end date, and you add Cost Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Cost Rate 1 so that no gaps exist.</p></li> 
      
      <li><b>Billing Rate</b>: The amount of billing per hour for the user.
      <p>For date effective billing rates, click <strong>Add Rate</strong>. Enter the value of the billing rate for the time period, and assign a Start Date and End Date as needed. Billing Rate 1 will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.</p><p> <img alt="User cost and billing rates" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td><p>Associate an existing user custom form with this user. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. Fields you do not have access to edit are not displayed in an individual custom form.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the user record on the details page, not on the Edit User dialog. (From the list of users, click the user name to open the details.)</p> <p>For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Create a custom form</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comment</td> 
      <td>Type the comment you want to send to the users and to the Updates area of their user profiles.</td> 
     </tr> 
    </tbody> 
   </table>
-->
