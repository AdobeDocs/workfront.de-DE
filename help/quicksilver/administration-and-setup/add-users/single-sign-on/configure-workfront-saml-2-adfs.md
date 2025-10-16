---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS
description: Sie können die Authentifizierung für Workfront mit SAML 2.0 aktivieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 1%

---

# Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Workfront mit einer SAML 2.0-Lösung (Security Assertion Markup Language) für einmaliges Anmelden integrieren, während Sie Active Directory Federation Services (ADFS) verwenden.

In diesem Handbuch wird das Einrichten von ADFS ohne automatische Bereitstellung oder Attributzuordnungen beschrieben. Es wird empfohlen, die Einrichtung abzuschließen und zu testen, bevor Sie eine automatische Bereitstellung einrichten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktivieren der Authentifizierung für Workfront mit SAML 2.0

Um die Authentifizierung für die Workfront-Web-Anwendung und die Workfront-Mobile-App mit SAML 2.0 zu aktivieren, füllen Sie die folgenden Abschnitte aus:

* [Abrufen der Workfront SSO-Metadatendatei](#retrieve-the-workfront-sso-metadata-file)
* [Konfigurieren von Vertrauensstellungen vertrauender Parteien](#configure-relying-party-trusts)
* [Anspruchsregeln konfigurieren](#configure-claim-rules)
* [Hochladen der Metadatendatei und Testen der Verbindung](#upload-the-metadata-file-and-test-the-connection)

### Abrufen der Workfront SSO-Metadatendatei {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **System** > **Single Sign-On (SSO)**.
1. Klicken Sie **Dropdown-** „Typ“ auf **SAML 2.0**, um zusätzliche Informationen und Optionen anzuzeigen.
1. Kopieren Sie die URL, die nach **Metadaten-URL** angezeigt wird.
1. Fahren Sie mit dem folgenden Abschnitt fort[&#x200B; „Konfigurieren von Vertrauensstellungen vertrauender Parteien](#configure-relying-party-trusts).

### Konfigurieren von Vertrauensstellungen vertrauender Parteien {#configure-relying-party-trusts}

1. Öffnen Sie **ADFS-Manager** mithilfe von Windows Server 2008 R2 (Version kann abweichen).
1. Gehe zu **Start.**
1. Klicken Sie auf **Administration-Tools.**
1. Klicken Sie auf **ADFS 2.0-Verwaltung.**
1. Wählen Sie **ADFS** aus und erweitern Sie **Vertrauensstellungen**.
1. Klicken Sie mit **rechten Maustaste auf Vertrauensstellungen für vertrauende** und wählen Sie **Vertrauensstellung für vertrauende Parteien hinzufügen**, um den Assistenten zum Hinzufügen vertrauender Parteien zu starten.
1. Wählen Sie auf der **Begrüßungsseite** die Option **Starten** aus.
1. Fügen **im Abschnitt „Select Date Source** die Metadaten-URL aus Workfront ein.
1. Klicken Sie auf **Weiter**.
1. Klicken Sie **OK**, um die Warnmeldung zu bestätigen.
1. Fügen Sie im Abschnitt **Anzeigenamen angeben** einen **Anzeigenamen** und **Hinweise** hinzu, um die Vertrauensstellung zu unterscheiden, und klicken Sie dann auf **Weiter**.
1. Wählen Sie **Zugriff aller Benutzer auf diese vertrauende Seite zulassen** (oder **Keine**, wenn Sie dies später konfigurieren möchten) aus.
1. Klicken Sie auf **Weiter**.

   Dadurch gelangen Sie zum Abschnitt **Bereit zum Hinzufügen von**&quot;.

1. Fahren Sie mit dem folgenden Abschnitt [Konfigurieren von &#x200B;](#configure-claim-rules) fort.

### Anspruchsregeln konfigurieren {#configure-claim-rules}

1. Klicken Sie **Abschnitt** Bereit zum Hinzufügen der **) auf „Weiter** und stellen Sie sicher, dass die Option **Öffnen des Dialogfelds „Anspruchsregeln bearbeiten** ausgewählt ist.

   Auf diese Weise können Sie in einem zukünftigen Schritt Anspruchsregeln bearbeiten.

1. Klicken Sie auf **Schließen**.
1. Klicken Sie **Regel hinzufügen.**
1. Wählen Sie **LDAP-Attribut als Ansprüche senden** aus.
1. Klicken Sie **Weiter**, um den Schritt **Anspruchsregel konfigurieren** anzuzeigen.
1. Geben Sie die folgenden Mindestanforderungen an, um die Anspruchsregel zu konfigurieren: (Diese wird bei der Benutzereinrichtung in der **Federation ID** angegeben und wird verwendet, um zu unterscheiden, wer sich anmeldet.)


   <table >                
      <tbody>
            <tr>
               <td>Name der Anforderungsregel
               </td>
               <td>Geben Sie einen Namen für die Anspruchsregel an. Beispiel: "Workfront.“</td>
            </tr>
            <tr>
               <td>Attributspeicher</td>
               <td >Wählen <b>Active Directory</b> aus dem Dropdown-Menü aus.</td>
            </tr>
            <tr>
               <td>LDAP-Attribut</td>
               <td>Dies kann jeder Attributtyp sein. Es wird empfohlen<b> für dieses Attribut "</b>-account-name“ zu verwenden.</td>
            </tr>
            <tr>
               <td>Ausgehender Anspruchtyp</td>
               <td>Sie müssen <b>Name ID</b> als Typ des ausgehenden Anspruchs auswählen</td>
            </tr>
      </tbody>
   </table>

1. (Optional) Um die automatische Bereitstellung einzurichten, fügen Sie die folgenden zusätzlichen Ansprüche sowohl im LDAP-Attribut als auch im Typ Ausgehender Anspruch hinzu:

   * Vorname
   * Nachname
   * E-Mail-Adresse

1. Klicken Sie **Beenden** und klicken Sie dann **nächsten Bildschirm auf** OK“.
1. Klicken Sie mit der rechten Maustaste auf die neue **Vertrauensstellung der vertrauenden Seite** und wählen Sie dann **Eigenschaften** aus.
1. Wählen Sie die **Erweitert**. Wählen Sie unter **Sicherer Hash-** die Option SHA-1 oder SHA-256 aus.

   >[!NOTE]
   >
   >Die Option, die Sie unter „Sicherer Hash-Algorithmus“ auswählen, muss mit dem Feld „Sicherer Hash-Algorithmus“ in Workfront unter „Setup“ > „System“ > „Single Sign-On (SSO)“ übereinstimmen.

1. Fahren Sie mit dem folgenden Abschnitt fort [Hochladen der Metadatendatei und Testen der Verbindung](#upload-the-metadata-file-and-test-the-connection).

### Hochladen der Metadatendatei und Testen der Verbindung {#upload-the-metadata-file-and-test-the-connection}

1. Öffnen Sie einen Browser und navigieren Sie zu `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Dadurch sollte eine Metadatendatei „FederationMetadata.xml“ heruntergeladen werden.

1. Klicken Sie **Datei auswählen** unter **Felder aus Identity Provider-Metadaten** und wählen Sie die Datei **FederationMetadata.xml** aus.

1. (Optional) Wenn die Zertifikatsinformationen nicht in die Metadatendatei eingefügt wurden, können Sie eine Datei separat hochladen. Wählen Sie **Abschnitt** Zertifikat **aus**.

1. Klicken Sie **Verbindung testen**. Wenn dies korrekt eingerichtet ist, sollte eine Seite ähnlich der unten gezeigten angezeigt werden:

   ![SAML 2-Erfolgsmeldung](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Wenn Sie die Attributzuordnung einrichten möchten, stellen Sie sicher, dass Sie die Attribute aus der Testverbindung in das Verzeichnisattribut kopieren. Weitere Informationen finden Sie unter Zuordnen von Benutzerattributen .

1. Wählen Sie **Admin-Ausnahme** aus, damit sich Workfront-Administratoren mit den Workfront-Anmeldeinformationen und der Umgehungs-URL anmelden können.

   Lesezeichen, die auf `<yourdomain>`.my.workfront.com/login verweisen, umgehen die Umleitung.

1. Aktivieren Sie das **Aktivieren**, um die Konfiguration zu aktivieren.
1. Klicken Sie auf **Speichern**.

## Informationen zum Aktualisieren von Benutzern für SSO

Nach diesem Handbuch ist der **SSO-Benutzername** der **Active Directory-Benutzername**.

Als Workfront-Administrator können Sie Benutzer für SSO per Massenaktualisierung aktualisieren. Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter [Aktualisieren von Benutzern für einmaliges Anmelden](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Als Workfront-Administrator können Sie auch manuell eine Federation ID zuweisen, indem Sie das Benutzerprofil bearbeiten und das Feld Federation ID ausfüllen. Weitere Informationen zum Bearbeiten eines Benutzers finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Wenn Sie beim Bearbeiten von Benutzerprofilen eine Federation ID angeben und **Nur SAML 2.0-Authentifizierung zulassen** wird die Möglichkeit entfernt, sich über die Umgehungs-URL (`<yourdomain>`.my.workfront.com/login) bei Workfront anzumelden.
