---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront mit SAML 2.0 konfigurieren
description: Als Adobe Workfront-Administrator können Sie die Web- und mobilen Anwendungen von Workfront so konfigurieren, dass sie mit einer SAML 2.0-Lösung (Security Assertion Markup Language) für einmaliges Anmelden (SSO) integriert werden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 93f4c1691210d88531fcc269bd40ee7ed8633309
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 8%

---

# Adobe Workfront mit SAML 2.0 konfigurieren

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->



>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Adobe Admin Console integriert haben.
>
>Informationen zum Zuordnen von Benutzerattributen in Organisationen, die in Adobe Admin Console integriert wurden, finden Sie unter [Zuordnen von Benutzerattributen im einheitlichen Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) im Artikel Zuordnen von Benutzerattributen.

Als Adobe Workfront-Administrator können Sie die Web- und mobilen Anwendungen von Workfront so konfigurieren, dass sie mit einer SAML 2.0-Lösung (Security Assertion Markup Language) für einmaliges Anmelden (SSO) integriert werden.

Nachdem Sie SAML 2.0 in Workfront konfiguriert haben, wie in den folgenden Abschnitten beschrieben, können Sie die Konfiguration beibehalten, wie in [Aktualisieren von SAML 2.0-Metadaten in Ihrem Identitätsanbieter](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md) beschrieben.

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
   <td><p>Neu: Standard </p>
       <p>oder</p> 
       <p>Aktuell: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktivieren der Authentifizierung für Workfront mit SAML 2.0

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Single Sign-On (SSO).**

1. Wählen Sie in **Dropdown** Liste „Typ“ **SAML 2.0.**

1. Klicken Sie oben in den angezeigten Optionen auf **SAML 2.0-Metadaten herunterladen**, um die Datei auf Ihren Computer herunterzuladen.

   Ihr SAML 2.0-Identitätsanbieter erfordert eine XML-Datei mit Informationen, die in Ihrer Workfront-Instanz generiert wurden. Nach dem Herunterladen der Datei müssen Sie auf Ihren SAML 2.0 Identity Provider-Server zugreifen und die XML-Metadatendatei für Workfront SAML 2.0 dort hochladen.

1. Geben Sie die folgenden Informationen in Workfront an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Service Provider-ID </td>
      <td> Diese bereits für Sie ausgefüllte URL identifiziert Workfront gegenüber Ihrem Identitätsanbieter. Beispiel: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td>
     </tr>
     <tr>
      <td role="rowheader">Bindungstyp</span> </td>
      <td> <p>Wählen Sie die von Ihrem IDP-Server unterstützte Methode zum Senden von Authentifizierungsinformationen aus:</p>
       <ul>
       <li>POST</li>
       <li>UMLEITUNG</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">Füllen der Felder aus den Metadaten des Identitätsanbieters </td> 
      <td>Exportieren Sie in Ihrer SAML 2.0 Identity Provider-Lösung eine XML-Datei mit den Metadaten des Dienstleisters und speichern Sie sie an einem temporären Speicherort auf Ihrem Computer. Wählen Sie <strong>Datei auswählen</strong> und suchen Sie dann die gespeicherte Datei, um sie zu Ihrer Workfront-Konfiguration hinzuzufügen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anmeldeportal-URL</span> </td> 
      <td>Geben Sie das gemeinsame Anmeldeportal Ihres Unternehmens ein. Dies ist die URL, unter der sich Benutzer anmelden, um auf Workfront und alle anderen in SAML 2.0 integrierten Anwendungen zuzugreifen.</td> 
     </tr>
     <tr>
      <td role="rowheader">Abmeldungs-URL</span> </td> 
      <td> <p>Geben Sie die Abmelde-URL für den IDP-Server ein. Workfront sendet eine HTTP-Anfrage an diese URL, bevor es sich von Workfront abmeldet. Dadurch wird die Benutzersitzung auf dem Remoteserver geschlossen, wenn die Workfront-Sitzung geschlossen wird.</p> <p><b>HINWEIS</b>: Sie werden nur dann zur Abmelde-URL weitergeleitet, wenn Sie in Ihrem Benutzerprofil die Option <strong>Nur SAML 2.0-</strong> zulassen) aktiviert haben.</p> </td>
     </tr>
     <tr>
      <td role="rowheader">Kennwortänderungs-URL </td> 
      <td> <p> Geben Sie die URL an, zu der Benutzer weitergeleitet werden, um ihre Passwörter zu ändern. </p> <p>Da die SAML 2.0-Anmeldeinformationen für den Zugriff auf Workfront verwendet werden, müssen Benutzende zu einer Seite umgeleitet werden, auf der sie ihr SAML 2.0-Kennwort ändern können, anstatt diese Aktivität über Workfront abzuschließen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sicherer Hash-Algorithmus </td> 
      <td> <p>Wählen Sie den von Ihrem IDP unterstützten Secure Hash Algorithm (SHA) aus:</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer automatisch bereitstellen</span> </td> 
      <td> <p>Mit dieser Option wird automatisch ein Benutzer im System erstellt, wenn ein neuer Benutzer mit einem Verzeichnis-Benutzernamen und -Kennwort versucht, sich zum ersten Mal bei Workfront anzumelden.</p> <p>Um Benutzende in Workfront zu erstellen, müssen Sie Workfront-Datenattribute den folgenden Benutzerdatenattributen in Ihrem Ordneranbieter zuordnen:</p> 
       <ul> 
       <li>Vorname</li> 
       <li>Nachname</li> 
       <li>E-Mail-Adresse</li> 
       </ul> 
       <p>Wenn Sie das Kontrollkästchen aktivieren, werden die folgenden Optionen angezeigt:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Wählen Sie in der Dropdown-Liste das Workfront-Benutzerattribut aus, das Sie zuordnen möchten, und geben Sie dann das entsprechende Verzeichnisattribut im Benutzerverzeichnis an.</p> 
       <p>Das Feld <strong>Verzeichnisattribut</strong> sollte den Verzeichnisattributnamen aus der Benutzerattributtabelle enthalten, die Sie beim erfolgreichen Testen Ihrer SAML 2.0-Konfiguration gespeichert haben.</p> 
       <p>Sie können im Feld „Standardwert“ einen <strong> Workfront-</strong> festlegen. Sie können auch Regeln basierend auf den Werten Ihres SAML 2.0-Identitätsanbieters festlegen.</p> 
       <p><b>WARNUNG</b>: Workfront versucht jedes Mal, wenn sich ein Benutzer beim System anmeldet, die unten aufgeführten Attribute zuzuordnen. Aus diesem Grund empfehlen wir nicht, Zugriffsebenen zuzuordnen. Sie können den administrativen Zugriff einfach entfernen, wenn ein Attribut falsch zugeordnet ist. Klicken Sie <strong>Zuordnung hinzufügen</strong>, um zusätzliche Regeln hinzuzufügen.
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
      <li> <p>Land</p> </li> 
      <li> <p>Arbeitszeittabellen-Profil</p> </li> 
      <li> <p>Titel</p> </li> 
      </ul>
      <p>Klicken Sie <strong>Speichern</strong> wenn Sie mit der Zuordnung der Benutzerattribute fertig sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zertifikat </td> 
      <td> <p>Laden Sie ein gültiges SSL-Zertifikat hoch, um eine sichere Verbindung zwischen dem Authentifizierungsdienst und Workfront zu gewährleisten. Für OnDemand-Konten ist immer ein Zertifikat erforderlich. Sie können dieses Zertifikat von Ihrem SAML 2.0-Systemadministrator erhalten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Admin-Ausnahme </td> 
      <td> <p>Ermöglicht Workfront-Administratoren den Zugriff auf Workfront über ihre Workfront-Anmeldung. Wenn diese Option nicht ausgewählt ist, müssen Workfront-Administratoren ihren SAML 2.0-Benutzernamen und ihr Kennwort verwenden.</p> 
      <p>Workfront versucht zunächst, sich für Benutzende mit Workfront-Systemadministrator-Zugriffsebene über SAML 2.0 bei Workfront anzumelden. Wenn die SAML 2.0-Authentifizierung fehlschlägt, verwendet Workfront die lokale Authentifizierung für Workfront-Administratoren.</p> 
      <p>Es wird empfohlen, diese Option immer auszuwählen, damit sich Ihr Workfront-Administrator bei Workfront anmelden kann, falls Ihr SAML 2.0-Anbieter vorübergehend nicht verfügbar ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivieren </td> 
      <td> <p>Aktiviert SSO auf dem Workfront-System. Stellen Sie sicher, dass Sie Ihren Benutzern die Anmeldeanweisungen mitgeteilt haben.</p> <p>Nachdem Sie Ihre SSO-Konfiguration in Workfront aktiviert haben, müssen Sie die Einstellung <strong>Nur SAML 2.0-Authentifizierung zulassen</strong> für alle Benutzenden aktivieren, damit sie SSO verwenden können.</p> <p>Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Aktualisieren von Benutzern für einmaliges Anmelden</a>.</p> <p>Weitere Informationen zu Benutzereinstellungen finden Sie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Konfiguration bestätigen </td> 
      <td> 
      <p>Klicken Sie <strong>Verbindung testen</strong>, um zu überprüfen, ob Workfront und der SAML 2.0-Identitätsanbieter miteinander kommunizieren können. Diese Verbindung ist nur erfolgreich, wenn Sie die XML-Dateien ausgetauscht haben.
      </p> 
      <p>Nachdem Sie die Verknüpfung zwischen Ihrem SAML 2.0-Identitätsanbieter und Workfront erfolgreich getestet haben, wird ein Bildschirm ähnlich der folgenden Abbildung angezeigt.</p>
      <p><b>HINWEIS</b>: Dieser Bildschirm wird in einem Browser-Popup angezeigt. Stellen Sie daher sicher, dass Sie Popup-Blocker in Ihrem Browser deaktivieren.</p>
      <p>Speichern Sie die in der Tabelle angezeigten Informationen zur späteren Verwendung.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Speichern**, um die SAML 2.0-Konfiguration zu speichern.
