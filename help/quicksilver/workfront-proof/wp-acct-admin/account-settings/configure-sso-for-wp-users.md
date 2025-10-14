---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Konfigurieren von Single Sign-On für  [!DNL Workfront Proof] '
description: Wenn Sie über den Select- oder Premium-Plan verfügen, können Sie eine Single Sign-On (SSO)-Funktion bereitstellen, mit der Sie den Benutzernamen und das Kennwort Ihres bestehenden Unternehmens für den Zugriff auf Ihr - [!DNL Workfront Proof]  verwenden können.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# Konfigurieren von Single Sign-On für [!DNL Workfront Proof] Benutzer

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie über den Select- oder Premium-Plan verfügen, können Sie eine Single Sign-On (SSO)-Funktion bereitstellen, mit der Sie den Benutzernamen und das Kennwort Ihres bestehenden Unternehmens verwenden können, um auf Ihr [!DNL Workfront Proof]-Konto zuzugreifen.

Das bedeutet, dass Sie sich über Ihr eigenes Anmeldesystem authentifizieren, nicht über die [!DNL Workfront Proof] Anmeldeseite.

>[!NOTE]
>
>Sie müssen eine benutzerdefinierte Subdomain oder Domain in Ihrem [!DNL Workfront Proof] Konto eingerichtet haben, um SAML zu aktivieren. Benutzerdefinierte Subdomains können frei eingerichtet werden. Weitere Informationen finden Sie [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding). Weitere Informationen zu vollständig angepassten Domains finden Sie auf unserer [Marke der Website [!DNL Workfront Proof]  „Erweitert](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Aktivieren von SSO in [!DNL Workfront Proof]

Die Single Sign-On-Funktion kann auf der Registerkarte [!UICONTROL Single Sign-On] Ihrer [!UICONTROL Kontoeinstellungen] aktiviert werden und gilt für alle Benutzer in Ihrem [!DNL Workfront Proof]. Siehe [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) für weitere Informationen.

## Entitäts-ID

Als Dienstleister haben wir hier unsere Entitäts-ID veröffentlicht:

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (wobei „IhreSubdomain“ die Subdomain Ihres Kontos ist)

[!DNL Workfront Proof] erfordert die E-Mail-Adresse des Benutzers als eindeutige Kennung, die als eines der folgenden Attribute übergeben werden kann:

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* E-Mail
* E-Mail
* emailAddress

SSO konfigurieren:

1. Öffnen Sie die **[!UICONTROL Single Sign-On]**-Registerkarte (1).
1. Geben Sie die **SSO URL** ein (2).
Dies ist der Link zu Ihrem SSO-Server (z. B. **https://sso.mycompany.com/opensso**).

1. Geben Sie die **Anmelde-URL** ein (3).
Dies ist die URL, die aufgerufen wird, um die Benutzer an Ihren Identitätsanbieter weiterzuleiten.

   Dies ist keine tatsächliche URL, die Sie im Browser eingeben, sondern ein Endpunkt, der die Informationen verarbeitet, die wir senden, um den Anmeldebildschirm anzuzeigen.

1. Geben Sie die **Abmelde-URL** ein (4).
Dies ist die URL, zu der Sie nach dem Abmelden zurückgegeben werden, z. B.

   **https://www.yourcompany.com/services/logout.asp**

1. Geben Sie den **Zertifikatfingerabdruck** (5) ein.
1. Der SHA1-Fingerabdruck des SAML-Zertifikats, das von Ihrem SAML-Identitätsanbieter bereitgestellt wird.
1. Stellen Sie sicher, dass Sie die Schlüsselinformationen einschließen, indem Sie dies für Ihren Identitätsanbieter festlegen.
1. Wechseln **SSO** zu **[!UICONTROL Aktiviert]** (6).
Sobald SSO aktiviert ist, werden Sie und andere Benutzer in Ihrem Konto mit Ihrem eigenen Authentifizierungsmechanismus angemeldet. Das bedeutet, dass Benutzer, die auf den Anmeldebildschirm Ihres [!DNL Workfront Proof]-Kontos zugreifen (z. B. **yourcompany.proofhq.com/login**), über das Übertragungsfenster zur Anmeldeseite Ihrer eigenen Authentifizierung aufgefordert werden.

1. (Optional) Aktivieren Sie **Benutzer automatisch bereitstellen** (7).
Sobald diese Option aktiviert ist, werden die Benutzerkonten automatisch für Personen erstellt, die nicht über eigene [!DNL Workfront Proof] verfügen, aber über ihre Single-Sign-On-Anmeldeinformationen auf Ihr [!DNL Workfront Proof]-Konto zugreifen. Dies wird nur aktiv, wenn das Benutzerlimit für Ihr Konto noch nicht erreicht wurde.

1. Neu bereitgestellten Benutzern werden standardmäßig die Manager-Profilberechtigungen zugewiesen. Weitere Informationen finden Sie unter [Profile für Korrekturabzugsberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![enable_sso_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## SSO für Satellitenkonten aktivieren

Wenn Sie über Satellitenkonten verfügen, die mit Ihrem Hub-Konto verbunden sind, können Sie diese auf der Ebene des Hub-Kontos verwalten.

Single Sign-On ist eine Select- und Premium-Funktion, sodass Single Sign-On nur für Satelliten aktiviert werden kann, die einen Select- oder Premium-Plan besitzen.

1. Klicken Sie **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** (1).

1. Klicken Sie im Dropdown-Menü (2) auf das Satellitenkonto.
1. Öffnen Sie die **[!UICONTROL Single Sign-On]**-Registerkarte (3).
1. Bearbeiten Sie die SSO-Konfiguration (4).
1. ![enable_sso_-_satellite_account.png](assets/enabling-sso---satellite-account-350x266.png)
Hier gibt es zwei Konfigurationsmethoden (5):

1. **Vererbt:** SSO mit der Konfiguration, die von Ihrem Hub-Konto übernommen wird.
Wenn ein Benutzer über die **Standard-Anmeldeseite** ([https://business.adobe.com/products/workfront/proofing-approvals.html](https://business.adobe.com/products/workfront/proofing-approvals.html)) auf [!DNL Workfront Proof] zugreift, **zwei Berechtigungsebenen**: Zunächst wird ein Benutzer aufgefordert, sich mit [!DNL Workfront Proof] Zugriffsdaten (E-Mail und Passwort) anzumelden, dann wird der Benutzer über ein SSO-Fenster zur SSO-Anmeldeseite weitergeleitet.
Bei aktiviertem SSO-Service empfehlen wir daher, sich über Ihre eigene [!DNL Workfront Proof] Subdomain/Domain anzumelden.

   >[!NOTE]
   >
   >Wenn Single Sign-On in Ihrem [!DNL Workfront Proof]-Konto aktiviert ist, können Sie sich derzeit nicht mit diesen Anmeldeinformationen bei der iPhone-App anmelden.

   1. **Manuell** (Standard): SSO mit einer anderen Konfiguration (z. B. Verweisen auf einen anderen Identitätsanbieter).

      >[!NOTE]
      >
      >Wenn das Satellitenkonto die SSO-Konfiguration vom Hub-Konto übernimmt, ist der Anmeldebildschirm der des Hub-Kontos. Wenn der Benutzer des Satellitenkontos seine SSO-Anmeldedaten auf dieser Seite eingibt, wird er zurück zum Satellitenkonto weitergeleitet.

      ![enable_sso_-_satellite_account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Klicken Sie **[!UICONTROL Speichern]** (6).

## Von einem Hub-Konto geerbte SSO-Einstellungen

Wenn Sie die Einstellungen von Ihrem Hub-Konto übernehmen, werden Sie feststellen, dass alle Felder jetzt mit den Daten aus Ihrem Hub-Konto gefüllt sind (7) und dass Single Sign-On automatisch aktiviert/deaktiviert wird (8), wie bei Ihrem Hauptkonto. Es gibt auch keine Bearbeitungslinks mehr in den Feldern, da die gesamte SSO-Konfiguration für das Satellitenkonto nun von Ihrem Hub-Konto aus festgelegt und verwaltet wird.

![satellite_account_-_inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

In Ihrem Hub-Konto (9) zeigt das Feld [!UICONTROL SSO Usage] an, dass diese Konfiguration von Satellitenkonten verwendet wird (10).\
![Hub_Account_-_inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## SSO manuell konfiguriert

Wenn die manuelle SSO-Konfiguration für ein Satellitenkonto ausgewählt wurde (1), müssen Sie die Daten für das Single Sign-On manuell eingeben.

1. Klicken Sie **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** (1).

1. Öffnen Sie die **[!UICONTROL Single Sign-On]** .
1. Klicken Sie **[!UICONTROL Bearbeiten], füllen** das Feld aus und klicken Sie dann auf **[!UICONTROL Speichern]** (2).

1. Klicken Sie in der **[!UICONTROL SSO]**-Zeile auf **[!UICONTROL Aktiviert]** (3).

![satellite_account_-_manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## SSO-Anmeldung

1. Klicken Sie **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** (1).

1. Öffnen Sie die **[!UICONTROL Single Sign-On]** .
1. Stellen Sie sicher, dass Ihre [!DNL Workfront Proof] Domain/Subdomain (1) eingerichtet ist und dass Ihre Benutzer über diese benutzerdefinierte Domain/Subdomain auf Ihr [!DNL Workfront Proof]-Konto zugreifen.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Bei aktiviertem Single Sign-On zeigt Ihre Subdomain-Anmelde-URL (z. B. yourcompany.proofhq.com/login) einen Übertragungsbildschirm (2) an, über den Sie direkt zu Ihrer SSO-Anmeldeseite gelangen.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Wenn eine Benutzerin oder ein Benutzer über die **Standardanmeldeseite** ([https://business.adobe.com/products/workfront/proofing-approvals.html](https://business.adobe.com/products/workfront/proofing-approvals.html)) auf [!DNL Workfront Proof] zugreift, gibt es **zwei Autorisierungsebenen**. Zunächst wird ein Benutzer aufgefordert, sich mit [!DNL Workfront Proof] Zugangsdaten (E-Mail und Passwort) anzumelden. Anschließend wird der Benutzer über ein SSO-Fenster (2) auf die SSO-Anmeldeseite übertragen.\
   Bei aktiviertem SSO-Service empfehlen wir daher, sich über Ihre eigene [!DNL Workfront Proof] Subdomain/Domain anzumelden.

1. Wenn Single Sign-On in Ihrem Workfront Proof-Konto aktiviert ist, können Sie sich derzeit nicht mit diesen Anmeldeinformationen bei der iPhone-App anmelden.

## Informationen zum Hinzufügen neuer Benutzer

Wenn die Single Sign-On-Funktion in Ihrem [!DNL Workfront Proof]-Konto aktiviert ist, erhalten neue Benutzer keine Bestätigungs-E-Mails, da ihre Konten automatisch aktiviert werden und einsatzbereit sind.

Nachdem Sie auf Ihrer [!DNL Workfront Proof]-Anmeldeseite auf die Schaltfläche [!UICONTROL Anmelden] geklickt haben, werden Benutzer zu Ihrer SSO-Anmeldeseite weitergeleitet und aufgefordert, Ihre Single-Sign-On-Anmeldedaten einzugeben.

>[!IMPORTANT]
>
>Benutzer werden während des Authentifizierungsprozesses über eine E-Mail-Adresse identifiziert, was bedeutet, dass das für Ihre SSO-Anmeldung verwendete E-Mail-Konto die E-Mail-Adresse des in Ihrem Konto registrierten Benutzers sein muss.

## Active Directory-Verbunddienste (AD FS)

Active Directory Federation Services (AD FS) ist eine [!DNL Microsoft] Softwarekomponente, die auf Windows Server-Betriebssystemen installiert werden kann, um Benutzern Single Sign-On Zugriff auf Systeme und Anwendungen zu gewähren, die sich über Unternehmensgrenzen hinweg befinden. Weitere Informationen finden Sie unter „Active Directory Federation Services“ auf der Microsoft Developer Network-Website.

Das [!DNL Workfront Proof] unterstützt SAML 2.0 und ist nur mit AD FS Version 2.0 oder höher kompatibel.

Detaillierte Anweisungen finden [&#x200B; unter „Single Sign [!DNL Workfront Proof]On: AD FS](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md)Konfiguration“.
