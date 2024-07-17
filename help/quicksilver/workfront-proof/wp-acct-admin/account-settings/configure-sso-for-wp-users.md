---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Single Sign-On für [!DNL Workfront Proof] Benutzer konfigurieren
description: Wenn Sie über einen Select- oder Premium-Plan verfügen, können Sie eine Single Sign-On (SSO)-Funktion bereitstellen, mit der Sie den Benutzernamen und das Kennwort Ihres bestehenden Unternehmens für den Zugriff auf Ihr [!DNL Workfront Proof] Konto verwenden können.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 007a603ef1df2a02959d7fb623ac784bf5b9cb80
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# Single Sign-On für [!DNL Workfront Proof] Benutzer konfigurieren

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie über einen Select- oder Premium-Plan verfügen, können Sie eine Single Sign-On (SSO)-Funktion bereitstellen, mit der Sie den Benutzernamen und das Kennwort Ihres bestehenden Unternehmens für den Zugriff auf Ihr [!DNL Workfront Proof]-Konto verwenden können.

Dies bedeutet, dass Sie sich bei Ihrem eigenen Anmeldesystem authentifizieren, nicht bei der Anmeldeseite von [!DNL Workfront Proof].

>[!NOTE]
>
>Sie müssen eine benutzerdefinierte Subdomäne oder Domäne für Ihr [!DNL Workfront Proof]-Konto einrichten, um SAML zu aktivieren. Benutzerdefinierte Subdomains können kostenlos eingerichtet werden. Weitere Informationen finden Sie unter [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding). Weitere Informationen zu vollständig angepassten Domänen finden Sie in unserer [Marke der  [!DNL Workfront Proof] Site - erweitert](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Aktivieren der einmaligen Anmeldung innerhalb von [!DNL Workfront Proof]

Die Single-Sign-On-Funktion kann auf der Registerkarte [!UICONTROL Single-Sign-on] Ihrer [!UICONTROL Kontoeinstellungen] aktiviert werden. Sie gilt für alle Benutzer in Ihrem [!DNL Workfront Proof]-Konto. Weitere Informationen finden Sie unter [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) .

## Entity ID

Als Dienstleister haben wir unsere Entitäts-ID hier veröffentlicht:

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (wobei &quot;Ihre Subdomain&quot;die Subdomäne Ihres Kontos ist)

[!DNL Workfront Proof] erfordert die E-Mail-Adresse des Benutzers als eindeutige Kennung, die als eines der folgenden Attribute übergeben werden kann:

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* mail
* email
* emailAddress

So konfigurieren Sie SSO:

1. Öffnen Sie die Registerkarte **[!UICONTROL Single Sign-On]** (1).
1. Geben Sie die **SSO-URL** (2) ein.
Dies ist der Link zu Ihrem SSO-Server (z. B. **https://sso.mycompany.com/opensso**).

1. Geben Sie die **Anmelde-URL** (3) ein.
Dies ist die URL, die aufgerufen wird, um die Benutzer an Ihren Identitätsanbieter umzuleiten.

1. Dies ist keine tatsächliche URL, die Sie im Browser eingeben, sondern ein Endpunkt, der die von uns gesendeten Informationen verarbeitet, um den Anmeldebildschirm darzustellen.

Geben Sie die **Abmelde-URL** (4) ein.
Dies ist die URL, an die Sie nach dem Abmelden zurückgegeben werden, z. B.

**https://www.yourcompany.com/services/logout.asp**

1. Geben Sie den **Zertifikatfingerabdruck** (5) ein.
1. Der SHA1-Fingerabdruck des SAML-Zertifikats, das von Ihrem SAML-Identitätsanbieter bereitgestellt wird.
1. Stellen Sie sicher, dass Sie die Schlüsselinformationen einschließen, indem Sie diese in Ihrem Identitäts-Provider festlegen.
1. Wechseln Sie **SSO** zu **[!UICONTROL Aktiviert]** (6).
Sobald SSO aktiviert ist, melden Sie sich mit anderen Benutzern in Ihrem Konto mit Ihrem eigenen Authentifizierungsmechanismus an. Das bedeutet, dass Benutzer, die auf den Anmeldebildschirm Ihres [!DNL Workfront Proof]-Kontos zugreifen (z. B. **yourcompany.proofhq.com/login**), mit dem Übertragungsfenster zur eigenen Anmeldeseite für die Authentifizierung aufgefordert werden.

1. (Optional) Aktivieren Sie **Benutzer automatisch bereitstellen** (7).
Sobald diese Option aktiviert ist, werden die Benutzerkonten automatisch für Personen erstellt, die nicht über eigene [!DNL Workfront Proof] -Profile verfügen, aber mit ihren Single-Sign-On-Anmeldedaten auf Ihr [!DNL Workfront Proof] -Konto zugreifen. Diese Aktion wird nur ausgeführt, wenn das Benutzerlimit in Ihrem Konto noch nicht erreicht ist.

1. Neue bereitgestellte Benutzer erhalten standardmäßig die Profilberechtigungen Manager . Weitere Informationen finden Sie unter [Profile für Testberechtigungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Aktivieren der einmaligen Anmeldung für Satellitenkonten

Wenn Sie über Satellitenkonten verfügen, die mit Ihrem Hub-Konto verbunden sind, können Sie diese auf der Hub-Kontoebene verwalten.

Single Sign-On ist eine Select- und Premium-Funktion, sodass Single Sign-On nur für Satelliten aktiviert werden kann, die sich auf Select- und Premium-Pläne befinden.

1. Klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** (1).

1. Klicken Sie auf das Satellitenkonto im Dropdown-Menü (2).
1. Öffnen Sie die Registerkarte **[!UICONTROL Single Sign-On]** (3).
1. Bearbeiten Sie die SSO-Konfiguration (4).
1. ![Aktivieren_SSO_-_satellite_account.png](assets/enabling-sso---satellite-account-350x266.png)
Hier finden Sie zwei Konfigurationsmethoden (5):

1. **Vererbt:** SSO mit der Konfiguration, die von Ihrem Hub-Konto übernommen wurde.
Wenn ein Benutzer über die Standardanmeldeseite **https://www.proofhq.com/login](https://www.proofhq.com/login) auf [!DNL Workfront Proof] zugreift, gibt es** zwei Berechtigungsebenen **: Zunächst wird ein Benutzer aufgefordert, sich mit [!DNL Workfront Proof] Zugangsdaten anzumelden (E-Mail und Kennwort), dann wird der Benutzer über ein SSO-Fenster auf die SSO-Anmeldeseite übertragen.**[
Wenn der SSO-Dienst aktiviert ist, empfehlen wir daher, sich über Ihre eigene [!DNL Workfront Proof]-Subdomäne/Domäne anzumelden.

   >[!NOTE]
   >
   >Wenn derzeit Single Sign-On für Ihr [!DNL Workfront Proof] -Konto aktiviert ist, können Sie sich mit diesen Anmeldedaten nicht bei der iPhone-App anmelden.

   1. **Manuell** (Standard): SSO mit einer anderen Konfiguration (z. B. Verweis auf einen anderen Identitätsanbieter).

      >[!NOTE]
      >
      >Wenn das Satellitenkonto die SSO-Konfiguration vom Hub-Konto übernimmt, ist der Anmeldebildschirm der des Hub-Kontos. Wenn der Benutzer des Satellitenkontos seine SSO-Anmeldedaten auf dieser Seite eingibt, wird er zum Satellitenkonto zurückgeleitet.

      ![Aktivieren_SSO_-_satellite_account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Klicken Sie auf **[!UICONTROL Speichern]** (6).

## Von einem Hub-Konto übernommene SSO-Einstellungen

Wenn Sie die Einstellungen von Ihrem Hub-Konto übernehmen möchten, werden Sie feststellen, dass alle Felder jetzt mit den Daten aus Ihrem Hub-Konto (7) ausgefüllt sind und dass Single Sign-On automatisch aktiviert/deaktiviert (8) ist, wie in Ihrem Hauptkonto. Es gibt auch keine Bearbeitungslinks mehr in den Feldern, da die gesamte SSO-Konfiguration für das Satellitenkonto jetzt über Ihr Hub-Konto festgelegt und verwaltet wird.

![satellite_account_-_inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

In Ihrem Hub-Konto (9) zeigt das Feld [!UICONTROL SSO-Nutzung] an, dass diese Konfiguration von Satellitenkonten verwendet wird (10).\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## Manuell konfigurierte SSO

Wenn für ein Satellitenkonto (1) die manuelle SSO-Konfiguration ausgewählt wurde, müssen Sie die Daten für das Single-Sign-On manuell eingeben.

1. Klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** (1).

1. Öffnen Sie die Registerkarte **[!UICONTROL Single Sign-on]** .
1. Klicken Sie auf **[!UICONTROL Bearbeiten],** füllen Sie das Feld aus und klicken Sie dann auf **[!UICONTROL Speichern]** (2).

1. Klicken Sie in der Zeile **[!UICONTROL SSO]** auf **[!UICONTROL Aktiviert]** (3).

![satellite_account_-_manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## SSO-Anmeldung

1. Klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** (1).

1. Öffnen Sie die Registerkarte **[!UICONTROL Single Sign-on]** .
1. Stellen Sie sicher, dass Ihre [!DNL Workfront Proof]-Domäne/Subdomäne (1) eingerichtet ist und dass Ihre Benutzer über diese benutzerdefinierte Domäne/Subdomäne auf Ihr [!DNL Workfront Proof]-Konto zugreifen.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Wenn Sie Single Sign-On aktiviert haben, zeigt Ihre Sub-Domain-Anmelde-URL (z. B. yourcompany.proofhq.com/login) einen Übertragungsbildschirm (2) an, der Sie direkt zur SSO-Anmeldeseite führt.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Wenn ein Benutzer über die Standardanmeldeseite **([https://www.proofhq.com/login](https://www.proofhq.com/login)) auf [!DNL Workfront Proof] zugreift, gibt es** zwei Berechtigungsebenen **.** Zunächst wird ein Benutzer aufgefordert, sich mit [!DNL Workfront Proof] Zugangsdaten (E-Mail und Passwort) anzumelden. Anschließend wird der Benutzer über ein SSO-Fenster (2) zur SSO-Anmeldeseite weitergeleitet.\
   Wenn der SSO-Dienst aktiviert ist, empfehlen wir daher, sich über Ihre eigene [!DNL Workfront Proof]-Subdomäne/Domäne anzumelden.

1. Wenn derzeit Single Sign-On für Ihr Workfront Proof-Konto aktiviert ist, können Sie sich mit diesen Anmeldedaten nicht bei der iPhone-App anmelden.

## Über das Hinzufügen eines neuen Benutzers

Wenn die Single-Sign-On-Funktion in Ihrem [!DNL Workfront Proof]-Konto aktiviert ist, erhalten neue Benutzer keine Bestätigungs-E-Mails, da ihre Konten automatisch aktiviert und einsatzbereit sind.

Auf Ihrer [!DNL Workfront Proof] -Anmeldeseite werden Benutzer nach dem Klicken auf die Schaltfläche [!UICONTROL Anmelden] zu Ihrer SSO-Anmeldeseite geleitet und aufgefordert, Ihre Single Sign-On-Anmeldedaten einzugeben.

>[!IMPORTANT]
>
>Benutzer werden während des Authentifizierungsprozesses über eine E-Mail-Adresse identifiziert. Das bedeutet, dass das für Ihre SSO-Anmeldung verwendete E-Mail-Konto die E-Mail-Adresse des in Ihrem Konto registrierten Benutzers sein muss.

## Active Directory Federation Services (AD FS)

Die Active Directory Federation Services (AD FS) ist eine [!DNL Microsoft] -Softwarekomponente, die auf Windows Server-Betriebssystemen installiert werden kann, um Benutzern einen Single-Sign-On-Zugriff auf Systeme und Anwendungen zu ermöglichen, die sich über Unternehmensgrenzen hinweg befinden. Weitere Informationen finden Sie unter &quot;Active Directory Federation Services&quot;auf der Microsoft Developer Network-Website.

Das System [!DNL Workfront Proof] unterstützt SAML 2.0 und ist nur mit AD FS Version 2.0 oder höher kompatibel.

Detaillierte Anweisungen finden Sie unter [Single Sign-On in [!DNL Workfront Proof]: AD FS-Konfiguration](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) .
