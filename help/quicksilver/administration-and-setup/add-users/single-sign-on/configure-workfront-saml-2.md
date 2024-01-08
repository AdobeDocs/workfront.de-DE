---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Konfigurieren von Adobe Workfront mit SAML 2.0
description: Als Adobe Workfront-Administrator können Sie die Web- und Mobile-Apps von Workfront so konfigurieren, dass sie in eine SAML (Security Assertion Markup Language) 2.0-Lösung für Single Sign-on (SSO) integriert werden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 7%

---

# Konfigurieren von Adobe Workfront mit SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie die Web- und Mobile-Apps von Workfront so konfigurieren, dass sie in eine SAML (Security Assertion Markup Language) 2.0-Lösung für Single Sign-on (SSO) integriert werden.

Nachdem Sie SAML 2.0 in Workfront wie in den folgenden Abschnitten beschrieben konfiguriert haben, können Sie die Konfiguration wie in [SAML 2.0-Metadaten in Ihrem Identitäts-Provider aktualisieren](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

## Zugriffsanforderungen

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
   <td><p>Neu: Standard </p>
       <p>oder</p> 
       <p>Aktuell: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Aktivieren der Authentifizierung für Workfront mit SAML 2.0

{{step-1-to-setup}}

1. Klicks **System** > **Single Sign-On (SSO).**

1. Im **Typ** Dropdown-Liste auswählen **SAML 2.0.**

1. Klicken Sie oben in den angezeigten Optionen auf **SAML 2.0-Metadaten herunterladen** , um die Datei auf Ihren Computer herunterzuladen.

   Ihr SAML 2.0 Identity Provider benötigt eine XML-Datei mit Informationen, die in Ihrer Workfront-Instanz generiert werden. Nach dem Herunterladen der Datei müssen Sie auf Ihren SAML 2.0 Identity Provider-Server zugreifen und dort die Workfront SAML 2.0-Metadaten-XML-Datei hochladen.

1. Geben Sie die folgenden Informationen in Workfront an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Service Provider-ID </td>
      <td> Diese URL, die bereits für Sie ausgefüllt wurde, identifiziert Workfront für Ihren Identitäts-Provider. Beispiel: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td>
     </tr>
     <tr>
      <td role="rowheader">Bindungstyp</span> </td>
      <td> <p>Wählen Sie die von Ihrem IDP-Server unterstützte Methode zum Senden von Authentifizierungsinformationen aus:</p>
       <ul>
       <li>POST</li>
       <li>REDIRECT</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">Füllen der Felder aus den Metadaten des Identitätsanbieters </td> 
      <td>Exportieren Sie in Ihrer SAML 2.0 Identity Provider-Lösung eine XML-Datei für Service Provider-Metadaten und speichern Sie sie an einem temporären Speicherort auf Ihrem Computer. Auswählen <strong>Datei auswählen</strong>, suchen und wählen Sie die gespeicherte Datei aus, um sie Ihrer Workfront-Konfiguration hinzuzufügen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anmeldungsportal-URL</span> </td> 
      <td>Geben Sie das allgemeine Anmeldeportal Ihres Unternehmens ein. Dies ist die URL, unter der sich Benutzer anmelden, um auf Workfront und alle anderen in SAML 2.0 integrierten Anwendungen zuzugreifen.</td> 
     </tr>
     <tr>
      <td role="rowheader">Abmelde-URL</span> </td> 
      <td> <p>Geben Sie die Abmelde-URL für den IDP-Server ein. Workfront sendet eine HTTP-Anforderung an diese URL, bevor es sich von Workfront abmeldet. Dadurch wird die Benutzersitzung auf dem Remote-Server geschlossen, wenn die Workfront-Sitzung geschlossen wird.</p> <p><b>NOTE</b>: Sie werden nur dann zur Abmelde-URL weitergeleitet, wenn Sie über die Option verfügen. <strong>Nur SAML 2.0-Authentifizierung zulassen</strong> in Ihrem Benutzerprofil aktiviert wurde.</p> </td>
     </tr>
     <tr>
      <td role="rowheader">Kennwortänderungs-URL </td> 
      <td> <p> Geben Sie die URL an, zu der Benutzer umgeleitet werden, um ihr Passwort zu ändern. </p> <p>Da die SAML 2.0-Anmeldeinformationen für den Zugriff auf Workfront verwendet werden, müssen Benutzer zu einer Seite weitergeleitet werden, auf der sie ihr SAML 2.0-Kennwort ändern können, anstatt diese Aktivität über Workfront abzuschließen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sicherer Hash-Algorithmus </td> 
      <td> <p>Wählen Sie den SHA-Algorithmus (Secure Hash Algorithm) aus, den Ihr IDP unterstützt:</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer automatisch bereitstellen</span> </td> 
      <td> <p>Mit dieser Option wird automatisch ein Benutzer im System erstellt, wenn ein neuer Benutzer mit einem Ordnernamen "username"und "password"zum ersten Mal versucht, sich bei Workfront anzumelden.</p> <p>Um Benutzer in Workfront zu erstellen, müssen Sie Workfront-Datenattribute den folgenden Benutzerdatenattributen in Ihrem Ordneranbieter zuordnen:</p> 
       <ul> 
       <li>Vorname</li> 
       <li>Nachname</li> 
       <li>E-Mail-Adresse</li> 
       </ul> 
       <p>Wenn Sie das Kontrollkästchen aktivieren, werden die folgenden Optionen angezeigt:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Wählen Sie aus der Dropdownliste das Workfront-Benutzerattribut aus, das Sie zuordnen möchten, und geben Sie dann das entsprechende Ordnerattribut im Benutzerverzeichnis an.</p> 
       <p>Die <strong>Verzeichnisattribut</strong> sollte den Verzeichnisattributnamen aus der Benutzerattribut-Tabelle enthalten, die Sie beim erfolgreichen Testen Ihrer SAML 2.0-Konfiguration gespeichert haben.</p> 
       <p>Sie können den Workfront-Standardwert im <strong>Standardwert</strong> -Feld. Sie können Regeln auch auf Grundlage der Werte Ihres SAML 2.0 Identity Providers festlegen.</p> 
       <p><b>WARNUNG</b>: Workfront versucht, die unten aufgeführten Attribute jedes Mal zuzuordnen, wenn sich ein Benutzer beim System anmeldet. Aus diesem Grund empfehlen wir keine Zuordnung von Zugriffsebenen. Wenn ein Attribut falsch zugeordnet ist, können Sie den Administratorzugriff einfach entfernen. Klicks <strong>Zuordnung hinzufügen</strong> , um zusätzliche Regeln hinzuzufügen.
       </p> 
       <p>Sie können die folgenden Workfront-Attribute zuordnen:</p> 
      <ul> 
      <li> <p>Zugriffsebene</p> </li> 
      <li> <p>Adresse</p> </li> 
      <li> <p>Adresse2</p> </li> 
      <li> <p>Abrechnung pro Stunde</p> </li> 
      <li> <p>Stadt</p> </li> 
      <li> <p>Firma</p> </li> 
      <li> <p>Kosten pro Stunde</p> </li> 
      <li> <p>E-Mail-Adresse</p> </li> 
      <li> <p>Erweiterung</p> </li> 
      <li> <p>Vorname</p> </li> 
      <li> <p>Hauptgruppe</p> </li> 
      <li> <p>Home-Team</p> </li> 
      <li> <p>Aufgabengebiet</p> </li> 
      <li> <p>Nachname</p> </li> 
      <li> <p>Layoutvorlage</p> </li> 
      <li> <p>Managerin bzw. Manager</p> </li> 
      <li> <p>Mobiltelefon</p> </li> 
      <li> <p>Telefonnummer</p> </li> 
      <li> <p>Postleitzahl</p> </li> 
      <li> <p>Zeitplan</p> </li> 
      <li> <p>Status</p> </li> 
      <li> <p>Arbeitszeittabellen-Profil</p> </li> 
      <li> <p>Titel</p> </li> 
      </ul>
      <p>Klicks <strong>Speichern</strong> wenn Sie die Zuordnung von Benutzerattributen abgeschlossen haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zertifikat </td> 
      <td> <p>Laden Sie ein gültiges SSL-Zertifikat hoch, um eine sichere Verbindung zwischen dem Authentifizierungsdienst und Workfront sicherzustellen. Für OnDemand-Konten ist immer ein Zertifikat erforderlich. Sie können dieses Zertifikat von Ihrem SAML 2.0-Systemadministrator abrufen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Admin-Ausnahme </td> 
      <td> <p>Ermöglicht Workfront-Administratoren den Zugriff auf Workfront mithilfe ihrer Workfront-Anmeldung. Wenn diese Option nicht aktiviert ist, müssen Workfront-Administratoren ihren SAML 2.0-Benutzernamen und ihr Kennwort verwenden.</p> 
      <p>Workfront versucht zunächst, sich über SAML 2.0 bei Workfront für Benutzer mit der Zugriffsstufe "Workfront-Systemadministrator"anzumelden. Wenn die SAML 2.0-Authentifizierung fehlschlägt, verwendet Workfront die lokale Authentifizierung für Workfront-Administratoren.</p> 
      <p>Es wird empfohlen, diese Option immer auszuwählen, damit sich Ihr Workfront-Administrator bei Workfront anmelden kann, wenn Ihr SAML 2.0-Provider vorübergehend nicht verfügbar ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivieren </td> 
      <td> <p>Aktiviert SSO auf dem Workfront-System. Stellen Sie sicher, dass Sie Ihren Benutzern Anleitungen zur Anmeldung übermittelt haben.</p> <p>Nachdem Sie Ihre SSO-Konfiguration in Workfront aktiviert haben, müssen Sie die <strong>Nur SAML 2.0-Authentifizierung zulassen</strong> für alle Benutzer festgelegt, damit sie SSO verwenden können.</p> <p>Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Benutzer für Single Sign-on aktualisieren</a>.</p> <p>Weitere Informationen zu Benutzereinstellungen finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Konfiguration bestätigen </td> 
      <td> 
      <p>Klicks <strong>Verbindung testen</strong> , um zu überprüfen, ob Workfront und der SAML 2.0 Identity Provider miteinander kommunizieren können. Diese Verbindung ist nur erfolgreich, wenn Sie die XML-Dateien ausgetauscht haben.
      </p> 
      <p>Nachdem Sie die Verknüpfung zwischen Ihrem SAML 2.0 Identity Provider und Workfront erfolgreich getestet haben, wird ein Bildschirm ähnlich dem folgenden angezeigt.</p>
      <p><b>NOTE</b>: Dieser Bildschirm wird in einem Browser-Popup angezeigt, sodass Sie Popup-Blocker in Ihrem Browser deaktivieren.</p>
      <p>Speichern Sie die in der Tabelle angezeigten Informationen zur späteren Verwendung.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **Speichern** , um die SAML 2.0-Konfiguration zu speichern.
