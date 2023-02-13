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
source-wordcount: '870'
ht-degree: 0%

---

# Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Workfront mit einer SAML (Security Assertion Markup Language) 2.0-Lösung für Single Sign-on integrieren, während Sie Active Directory Federation Services (ADFS) verwenden.

Dieses Handbuch konzentriert sich auf die Einrichtung von ADFS ohne automatische Bereitstellung oder Attributzuordnungen. Es wird empfohlen, das Setup abzuschließen und vor der Einrichtung einer automatischen Bereitstellung zu testen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aktivieren der Authentifizierung für Workfront mit SAML 2.0

Um die Authentifizierung für die Workfront-Webanwendung und die Workfront-Mobile App mit SAML 2.0 zu aktivieren, führen Sie die folgenden Abschnitte aus:

* [Abrufen der Workfront SSO-Metadatendatei](#retrieve-the-workfront-sso-metadata-file)
* [Konfigurieren von Vertrauenswürdigkeit-Partei-Trusts](#configure-relying-party-trusts)
* [Anforderungsregeln konfigurieren](#configure-claim-rules)
* [Hochladen der Metadatendatei und Testen der Verbindung](#upload-the-metadata-file-and-test-the-connection)

### Abrufen der Workfront SSO-Metadatendatei {#retrieve-the-workfront-sso-metadata-file}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).
1. Klicken Sie im linken Bereich auf **System** > **Single Sign-On (SSO)**.
1. Im **Typ** Dropdown-Menü, klicken Sie auf **SAML 2.0** um zusätzliche Informationen und Optionen anzuzeigen.
1. Kopieren Sie die URL, die nach **Metadaten-URL**.
1. Fahren Sie mit dem folgenden Abschnitt fort: [Konfigurieren von Vertrauenswürdigkeit-Partei-Trusts](#configure-relying-party-trusts).

### Konfigurieren von Vertrauenswürdigkeit-Partei-Trusts {#configure-relying-party-trusts}

1. Öffnen Sie die **ADFS Manager** Verwendung des Windows-Servers 2008 R2 (Version kann variieren).
1. Navigieren Sie zu **Starten Sie.**
1. Klicken **Administrationstools.**
1. Klicken **ADFS 2.0-Verwaltung.**
1. Auswählen **ADFS** und erweitern **Vertrauensbeziehungen**.
1. Rechtsklick **Vertrauen in Partei**, wählen Sie **Vertrauenswürdigen Parteien-Vertrauen hinzufügen** , um den Assistenten zum Hinzufügen des Vertrauenswürdigen Partei-Vertrauensassistenten zu starten.
1. Aus dem **Begrüßungsseite** auswählen **Starten**.
1. Im **Datenquelle auswählen** Fügen Sie die Metadaten-URL aus Workfront ein.
1. Klicken **Nächste**.
1. Klicken **OK** um die Warnmeldung zu bestätigen.
1. Im **Anzeigename angeben** -Abschnitt, fügen Sie eine **Anzeigename** und **Hinweise** um den Trust zu unterscheiden, klicken Sie auf **Nächste**.
1. Auswählen **Erlauben Sie allen Benutzern den Zugriff auf diese vertrauende Partei** (Oder **Keines** , wenn Sie dies später konfigurieren möchten).
1. Klicken **Nächste**.

   Dadurch gelangen Sie zum **Bereit zum Hinzufügen von Vertrauen** Abschnitt.

1. Fahren Sie mit dem folgenden Abschnitt fort [Anforderungsregeln konfigurieren](#configure-claim-rules).

### Anforderungsregeln konfigurieren {#configure-claim-rules}

1. Klicken **Nächste** im **Bereit zum Hinzufügen von Vertrauen** und stellen Sie sicher, dass die **Öffnen Sie das Dialogfeld Anforderungsregeln bearbeiten .** ausgewählt ist.

   Auf diese Weise können Sie Anforderungsregeln in einem künftigen Schritt bearbeiten.

1. Klicken Sie auf **Schließen**.
1. Klicken **Regel hinzufügen.**
1. Auswählen **LDAP-Attribut als Ansprüche senden**.
1. Klicken **Nächste** , um **Anforderungsregel konfigurieren** Schritt.
1. Geben Sie die folgenden Mindestanforderungen an, um die Schadensregel zu konfigurieren: (Dies wird im Abschnitt **Federation ID** in der Benutzereinrichtung und wird verwendet, um zu unterscheiden, wer sich anmeldet.)


   <table >                
      <tbody>
            <tr>
               <td>Name der Regel
               </td>
               <td>Geben Sie einen Namen für die Schadensregel an. Beispiel: "Workfront".</td>
            </tr>
            <tr>
               <td>Attributspeicher</td>
               <td >Auswählen <b>Active Directory</b> aus dem Dropdown-Menü.</td>
            </tr>
            <tr>
               <td>LDAP-Attribut</td>
               <td>Dies kann ein beliebiger Attributtyp sein. Wir empfehlen, <b>SAM-Account-Name</b> für dieses Attribut.</td>
            </tr>
            <tr>
               <td>Ausgehender Anforderungstyp</td>
               <td>Sie müssen <b>Name: ID</b> als Typ der ausgehenden Forderung</td>
            </tr>
      </tbody>
   </table>

1. (Optional) Um die automatische Bereitstellung einzurichten, fügen Sie die folgenden zusätzlichen Ansprüche sowohl im LDAP-Attribut als auch im ausgehenden Anforderungstyp hinzu:

   * Vorname
   * Nachname
   * E-Mail-Adresse

1. Klicken **Beenden** Klicken Sie auf **OK** auf dem nächsten Bildschirm.
1. Klicken Sie mit der rechten Maustaste auf das neue **Vertrauen von Parteien**, wählen Sie **Eigenschaften**.
1. Wählen Sie die **Erweiterte Registerkarte**. Und unter **Sicherer Hash-Algorithmus** Wählen Sie SHA-1 oder SHA-256 aus.

   >[!NOTE]
   >
   >Die Option, die Sie unter &quot;Sicherer Hash-Algorithmus&quot;auswählen, muss mit dem Feld &quot;Sicherer Hash-Algorithmus&quot;in Workfront unter &quot;Setup&quot;> &quot;System&quot;> &quot;Single Sign-ON (SSO) übereinstimmen.

1. Fahren Sie mit dem folgenden Abschnitt fort [Hochladen der Metadatendatei und Testen der Verbindung](#upload-the-metadata-file-and-test-the-connection).

### Hochladen der Metadatendatei und Testen der Verbindung {#upload-the-metadata-file-and-test-the-connection}

1. Öffnen Sie einen Browser und navigieren Sie zu `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Dadurch sollte eine Metadatendatei der Datei FederationMetadata.xml heruntergeladen werden.

1. Klicken **Datei auswählen** under **Füllen von Feldern aus Identity Provider-Metadaten** und wählen Sie die **FederationMetadata.xml** -Datei.

1. (Optional) Wenn die Zertifikatinformationen nicht mit der Metadatendatei gefüllt wurden, können Sie eine Datei separat hochladen. Auswählen **Datei auswählen** im **Zertifikat** Abschnitt.

1. Klicken **Verbindung testen**. Bei korrekter Einrichtung sollte eine Seite ähnlich der folgenden angezeigt werden:

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Wenn Sie die Attributzuordnung einrichten möchten, stellen Sie sicher, dass Sie die Attribute aus der Testverbindung in das Verzeichnisattribut kopieren. Weitere Informationen finden Sie unter Zuordnen von Benutzerattributen .

1. Auswählen **Admin-Ausnahme** , damit sich Workfront-Administratoren mit Workfront-Anmeldeinformationen mit der Umgehungs-URL anmelden können.

   Lesezeichen mit Verweis auf `<yourdomain>`.my.workfront.com/login umgehen.

1. Wählen Sie die **Aktivieren** aktivieren, um die Konfiguration zu aktivieren.
1. Klicken Sie auf **Speichern**.

## Informationen zum Aktualisieren von Benutzern für SSO

In diesem Handbuch wird die Variable **SSO-Benutzername** werden **Active Directory-Benutzername**.

Als Workfront-Administrator können Sie Benutzer für die einmalige Anmeldung stapelweise aktualisieren. Weitere Informationen zum Aktualisieren von Benutzern für SSO finden Sie unter [Benutzer für Single Sign-on aktualisieren](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Als Workfront-Administrator können Sie auch manuell eine Verband-ID zuweisen, mit der das Benutzerprofil bearbeitet und das Feld &quot;Verband-ID&quot;ausgefüllt wird. Weitere Informationen zum Bearbeiten eines Benutzers finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Wenn Sie Benutzerprofile bearbeiten, um eine Verband-ID einzuschließen, wählen Sie **Nur SAML 2.0-Authentifizierung zulassen** entfernt die Möglichkeit, sich mit der Umgehungs-URL (`<yourdomain>`.my.workfront.com/login).
