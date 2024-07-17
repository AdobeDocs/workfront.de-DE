---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS
description: Sie können die Authentifizierung für Workfront mit SAML 2.0 aktivieren.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Workfront mit einer SAML (Security Assertion Markup Language) 2.0-Lösung für Single Sign-on integrieren, während Sie Active Directory Federation Services (ADFS) verwenden.

Dieses Handbuch konzentriert sich auf die Einrichtung von ADFS ohne automatische Bereitstellung oder Attributzuordnungen. Wir empfehlen Ihnen, das Setup abzuschließen und es zu testen, bevor Sie eine automatische Bereitstellung einrichten.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aktivieren der Authentifizierung für Workfront mit SAML 2.0

Um die Authentifizierung für die Workfront-Webanwendung und die Workfront-Mobile App mit SAML 2.0 zu aktivieren, führen Sie die folgenden Abschnitte aus:

* [Rufen Sie die Workfront SSO-Metadatendatei ab](#retrieve-the-workfront-sso-metadata-file)
* [Konfigurieren von vertrauenswürdigen Vertrauenden Parteien](#configure-relying-party-trusts)
* [Konfigurieren von Anforderungsregeln](#configure-claim-rules)
* [Hochladen der Metadatendatei und Testen der Verbindung](#upload-the-metadata-file-and-test-the-connection)

### Abrufen der Workfront SSO-Metadatendatei {#retrieve-the-workfront-sso-metadata-file}

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)
1. Klicken Sie im linken Bereich auf **System** > **Single Sign-On (SSO)**.
1. Klicken Sie im Dropdownmenü **Typ** auf **SAML 2.0** , um weitere Informationen und Optionen anzuzeigen.
1. Kopieren Sie die URL, die nach **Metadaten-URL** angezeigt wird.
1. Fahren Sie mit dem folgenden Abschnitt fort: [Vertrauenswürdige GruppenTrusts konfigurieren](#configure-relying-party-trusts).

### Konfigurieren von Vertrauenswürdigkeit-Partei-Trusts {#configure-relying-party-trusts}

1. Öffnen Sie den **ADFS Manager** unter Verwendung des Windows-Servers 2008 R2 (Version kann variieren).
1. Wechseln Sie zu **Start.**
1. Klicken Sie auf **Administrationstools.**
1. Klicken Sie auf **ADFS 2.0-Verwaltung.**
1. Wählen Sie **ADFS** aus und erweitern Sie **Vertrauensbeziehungen**.
1. Klicken Sie mit der rechten Maustaste auf **Vertrauenswürdige GruppenTrusts vertrauen** und wählen Sie dann **Vertrauenswürdigen Parteivertrauen hinzufügen** aus, um den Assistenten zum Hinzufügen von Vertrauenspartenvertrauen zu starten.
1. Wählen Sie auf der **Begrüßungsseite** **Start** aus.
1. Fügen Sie im Abschnitt **Datum Source auswählen** die Metadaten-URL aus Workfront ein.
1. Klicken Sie auf **Weiter**.
1. Klicken Sie auf **OK** , um die Warnmeldung zu bestätigen.
1. Fügen Sie im Abschnitt **Anzeigename angeben** einen **Anzeigenamen** und einen **Notizen** hinzu, um den Trust zu unterscheiden, und klicken Sie dann auf **Weiter**.
1. Wählen Sie **Erlauben Sie allen Benutzern, auf diese vertrauende Partei zuzugreifen** (oder **Keine** , wenn Sie dies später konfigurieren möchten).
1. Klicken Sie auf **Weiter**.

   Dadurch gelangen Sie zum Abschnitt &quot;**Bereit zum Hinzufügen von Trust**&quot;.

1. Fahren Sie mit dem folgenden Abschnitt [Anforderungsregeln konfigurieren](#configure-claim-rules) fort.

### Anforderungsregeln konfigurieren {#configure-claim-rules}

1. Klicken Sie im Abschnitt &quot;**Bereit zum Hinzufügen von Trust**&quot;auf &quot;**Weiter**&quot;und stellen Sie sicher, dass die Option &quot;**Öffnen Sie das Dialogfeld &quot;Anforderungsregeln bearbeiten&quot;**&quot;ausgewählt ist.

   Auf diese Weise können Sie Anforderungsregeln in einem künftigen Schritt bearbeiten.

1. Klicken Sie auf **Schließen**.
1. Klicken Sie auf **Regel hinzufügen**.
1. Wählen Sie **LDAP-Attribut als Ansprüche senden** aus.
1. Klicken Sie auf **Weiter** , um den Schritt **Anforderungsregel konfigurieren** anzuzeigen.
1. Geben Sie die folgenden Mindestanforderungen an, um die Schadensregel zu konfigurieren: (Dies wird in der **Föderations-ID** des Benutzer-Setups angezeigt und wird verwendet, um zu unterscheiden, wer sich anmeldet.)


   <table >                
      <tbody>
            <tr>
               <td>Name der Regel
               </td>
               <td>Geben Sie einen Namen für die Schadensregel an. Beispiel: "Workfront".</td>
            </tr>
            <tr>
               <td>Attributspeicher</td>
               <td >Wählen Sie <b>Active Directory</b> aus dem Dropdownmenü aus.</td>
            </tr>
            <tr>
               <td>LDAP-Attribut</td>
               <td>Dies kann ein beliebiger Attributtyp sein. Es wird empfohlen, für dieses Attribut <b>SAM-Account-Name</b> zu verwenden.</td>
            </tr>
            <tr>
               <td>Ausgehender Anforderungstyp</td>
               <td>Sie müssen <b>Name ID</b> als ausgehenden Forderungstyp auswählen</td>
            </tr>
      </tbody>
   </table>

1. (Optional) Um die automatische Bereitstellung einzurichten, fügen Sie die folgenden zusätzlichen Ansprüche sowohl im LDAP-Attribut als auch im ausgehenden Anforderungstyp hinzu:

   * Vorname
   * Nachname
   * E-Mail-Adresse

1. Klicken Sie auf **Beenden** und dann im nächsten Bildschirm auf **OK** .
1. Klicken Sie mit der rechten Maustaste auf den neuen &quot;**Vertrauenswürdigen Parteien-Trust**&quot;, und wählen Sie dann &quot;**Eigenschaften**&quot;.
1. Wählen Sie die Registerkarte **Erweitert** aus. Wählen Sie unter **Sicherer Hash-Algorithmus** SHA-1 oder SHA-256 aus.

   >[!NOTE]
   >
   >Die Option, die Sie unter &quot;Sicherer Hash-Algorithmus&quot;auswählen, muss mit dem Feld &quot;Sicherer Hash-Algorithmus&quot;in Workfront unter &quot;Setup&quot;> &quot;System&quot;> &quot;Single Sign-ON (SSO) übereinstimmen.

1. Fahren Sie mit dem folgenden Abschnitt fort: [Laden Sie die Metadatendatei hoch und testen Sie die Verbindung](#upload-the-metadata-file-and-test-the-connection).

### Hochladen der Metadatendatei und Testen der Verbindung {#upload-the-metadata-file-and-test-the-connection}

1. Öffnen Sie einen Browser und navigieren Sie zu `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Dadurch sollte eine Metadatendatei der Datei FederationMetadata.xml heruntergeladen werden.

1. Klicken Sie unter &quot;**Füllen der Felder aus den Identity Provider-Metadaten**&quot;auf &quot;**Datei auswählen**&quot;und wählen Sie die Datei &quot;**FederationMetadata.xml**&quot;.

1. (Optional) Wenn die Zertifikatinformationen nicht mit der Metadatendatei gefüllt wurden, können Sie eine Datei separat hochladen. Wählen Sie **Datei auswählen** im Abschnitt **Zertifikat** aus.

1. Klicken Sie auf **Verbindung testen**. Bei korrekter Einrichtung sollte eine Seite ähnlich der folgenden angezeigt werden:

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Wenn Sie die Attributzuordnung einrichten möchten, stellen Sie sicher, dass Sie die Attribute aus der Testverbindung in das Verzeichnisattribut kopieren. Weitere Informationen finden Sie unter Zuordnen von Benutzerattributen .

1. Wählen Sie **Admin Exemption** aus, damit sich Workfront-Administratoren mit Workfront-Anmeldeinformationen mit der Umgehungs-URL anmelden können.

   Lesezeichen, die auf `<yourdomain>`.my.workfront.com/login verweisen, umgehen die Umleitung.

1. Aktivieren Sie das Feld **Aktivieren** , um die Konfiguration zu aktivieren.
1. Klicken Sie auf **Speichern**.

## Informationen zum Aktualisieren von Benutzern für SSO

Nach diesem Handbuch ist der **SSO-Benutzername** ihr **Active Directory-Benutzername**.

Als Workfront-Administrator können Sie Benutzer für die einmalige Anmeldung stapelweise aktualisieren. Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter [Aktualisieren von Benutzern für Single Sign-on](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Als Workfront-Administrator können Sie auch manuell eine Verband-ID zuweisen, mit der das Benutzerprofil bearbeitet und das Feld &quot;Verband-ID&quot;ausgefüllt wird. Weitere Informationen zum Bearbeiten eines Benutzers finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Wenn Sie Benutzerprofile so bearbeiten, dass sie eine Verband-ID enthalten, können Sie sich mit der Auswahl von **Nur SAML 2.0-Authentifizierung zulassen** nicht mehr mit der Umgehungs-URL (`<yourdomain>`.my.workfront.com/login) bei Workfront anmelden.
