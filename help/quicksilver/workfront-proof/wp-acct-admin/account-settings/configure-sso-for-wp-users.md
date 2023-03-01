---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Single Sign-On konfigurieren für [!DNL Workfront Proof] Benutzer
description: Wenn Sie über einen Select- oder Premium-Plan verfügen, können Sie eine Single Sign-On-Funktion (SSO) bereitstellen, mit der Sie den Benutzernamen und das Kennwort Ihres bestehenden Unternehmens für den Zugriff auf Ihre [!DNL Workfront Proof] -Konto.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 007a603ef1df2a02959d7fb623ac784bf5b9cb80
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 0%

---

# Single Sign-On konfigurieren für [!DNL Workfront Proof] Benutzer

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie über einen Select- oder Premium-Plan verfügen, können Sie eine Single Sign-On-Funktion (SSO) bereitstellen, mit der Sie den Benutzernamen und das Kennwort Ihres bestehenden Unternehmens für den Zugriff auf Ihre [!DNL Workfront Proof] -Konto.

Dies bedeutet, dass Sie sich bei Ihrem eigenen Anmeldesystem authentifizieren, nicht bei der [!DNL Workfront Proof] Anmeldeseite.

>[!NOTE]
>
>Sie müssen eine benutzerdefinierte Sub-Domain oder Domäne für Ihre [!DNL Workfront Proof] -Konto, um SAML zu aktivieren. Benutzerdefinierte Subdomains können kostenlos eingerichtet werden. Siehe [Branding](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) Weitere Informationen finden Sie in unseren [Markieren Sie die [!DNL Workfront Proof] site - advanced](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Aktivieren von SSO in [!DNL Workfront Proof]

Die Single-Sign-On-Funktion kann auf der [!UICONTROL Single Sign-on] Registerkarte Ihres [!UICONTROL Kontoeinstellungen]und wird für alle Benutzer auf Ihrer [!DNL Workfront Proof] -Konto. Siehe [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) für weitere Informationen.

## Entitäts-ID

Als Dienstleister haben wir unsere Entitäts-ID hier veröffentlicht:

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (wobei &quot;Ihre Subdomäne&quot;die Subdomäne Ihres Kontos ist)

[!DNL Workfront Proof] erfordert die E-Mail-Adresse des Benutzers als eindeutige Kennung, die als eines der folgenden Attribute übergeben werden kann:

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0,9,2342,19200300,100,1,3
* http://axschema.org/contact/email
* openid.sreg.email
* mail
* email
* emailAddress

So konfigurieren Sie SSO:

1. Öffnen Sie die **[!UICONTROL Single Sign-on]** Registerkarte (1).
1. Geben Sie die **SSO-URL** Absatz 2.
Dies ist der Link zu Ihrem SSO-Server (z. B. **https://sso.mycompany.com/opensso**).

1. Geben Sie die **Anmelde-URL** Absatz 3.
Dies ist die URL, die aufgerufen wird, um die Benutzer an Ihren Identitätsanbieter umzuleiten.

1. Dies ist keine tatsächliche URL, die Sie im Browser eingeben, sondern ein Endpunkt, der die von uns gesendeten Informationen verarbeitet, um den Anmeldebildschirm darzustellen.

Geben Sie die **Abmelde-URL** 4.
Dies ist die URL, an die Sie nach dem Abmelden zurückgegeben werden, z. B.

**https://www.yourcompany.com/services/logout.asp**

1. Geben Sie die **Certificate fingerprint** Absatz 5.
1. Der SHA1-Fingerabdruck des SAML-Zertifikats, das von Ihrem SAML-Identitätsanbieter bereitgestellt wird.
1. Stellen Sie sicher, dass Sie die Schlüsselinformationen einschließen, indem Sie diese in Ihrem Identitäts-Provider festlegen.
1. Switch **SSO** nach **[!UICONTROL Aktiviert]** 6.
Sobald SSO aktiviert ist, melden Sie sich mit anderen Benutzern in Ihrem Konto mit Ihrem eigenen Authentifizierungsmechanismus an. Das bedeutet, dass Benutzer beim Zugriff auf Ihre [!DNL Workfront Proof] Bildschirm zur Kontoanmeldung (z. B. **yourcompany.proofhq.com/login**), werden sie mit dem Übertragungsfenster zu Ihrer eigenen Anmeldeseite für die Authentifizierung aufgefordert.

1. (Optional) Aktivieren Sie **Benutzer automatisch bereitstellen** 7.
Sobald diese Option aktiviert ist, werden die Benutzerkonten automatisch für Personen erstellt, die nicht über eigene [!DNL Workfront Proof] Profile, aber auf Ihre [!DNL Workfront Proof] -Konto mit ihren Single-Sign-On-Anmeldedaten verwenden. Diese Aktion wird nur ausgeführt, wenn das Benutzerlimit in Ihrem Konto noch nicht erreicht ist.

1. Neue bereitgestellte Benutzer erhalten standardmäßig die Profilberechtigungen Manager . Weitere Informationen finden Sie unter [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Aktivieren der einmaligen Anmeldung für Satellitenkonten

Wenn Sie über Satellitenkonten verfügen, die mit Ihrem Hub-Konto verbunden sind, können Sie diese auf der Hub-Kontoebene verwalten.

Single Sign-On ist eine Select- und Premium-Funktion, sodass Single Sign-On nur für Satelliten aktiviert werden kann, die sich auf Select- und Premium-Pläne befinden.

1. Klicken **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** Absatz 1.

1. Klicken Sie auf das Satellitenkonto im Dropdown-Menü (2).
1. Öffnen Sie die **[!UICONTROL Single Sign-on]** Registerkarte (3).
1. Bearbeiten Sie die SSO-Konfiguration (4).
1. ![enabling_SSO_-_satellite_account.png](assets/enabling-sso---satellite-account-350x266.png)
Hier finden Sie zwei Konfigurationsmethoden (5):

1. **Vererbt:** SSO mit der Konfiguration von Ihrem Hub-Konto aus.
Wenn ein Benutzer auf [!DNL Workfront Proof] durch **Standard-Anmeldeseite** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) wird **zwei Zulassungsstufen**: Zunächst wird ein Benutzer aufgefordert, sich mit [!DNL Workfront Proof] auf Daten zugreifen (E-Mail und Passwort); dann wird der Benutzer über ein SSO-Fenster auf die SSO-Anmeldeseite übertragen.
Daher empfehlen wir bei aktiviertem SSO-Dienst, sich über Ihre eigene [!DNL Workfront Proof] Subdomäne/Domäne.

   >[!NOTE]
   >
   >Wenn derzeit Single Sign-On in Ihrem [!DNL Workfront Proof] -Konto verwenden, können Sie sich nicht mit diesen Anmeldedaten bei der iPhone-App anmelden.

   1. **Manuell** (Standard): SSO mit einer anderen Konfiguration (z. B. Verweis auf einen anderen Identitäts-Provider).

      >[!NOTE]
      >
      >Wenn das Satellitenkonto die SSO-Konfiguration vom Hub-Konto übernimmt, ist der Anmeldebildschirm der des Hub-Kontos. Wenn der Benutzer des Satellitenkontos seine SSO-Anmeldedaten auf dieser Seite eingibt, wird er zum Satellitenkonto zurückgeleitet.

      ![Enable_SSO_-_satellite_account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Klicken **[!UICONTROL Speichern]** 6.

## Von einem Hub-Konto übernommene SSO-Einstellungen

Wenn Sie die Einstellungen von Ihrem Hub-Konto übernehmen möchten, werden Sie feststellen, dass alle Felder jetzt mit den Daten aus Ihrem Hub-Konto (7) ausgefüllt sind und dass Single Sign-On automatisch aktiviert/deaktiviert (8) ist, wie in Ihrem Hauptkonto. Es gibt auch keine Bearbeitungslinks mehr in den Feldern, da die gesamte SSO-Konfiguration für das Satellitenkonto jetzt über Ihr Hub-Konto festgelegt und verwaltet wird.

![satellite_account_-_inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

In Ihrem Hub-Konto (9) ist die [!UICONTROL SSO-Nutzung] zeigt an, dass diese Konfiguration von Satellitenkonten verwendet wird (10).\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## Manuell konfigurierte SSO

Wenn für ein Satellitenkonto (1) die manuelle SSO-Konfiguration ausgewählt wurde, müssen Sie die Daten für das Single-Sign-On manuell eingeben.

1. Klicken **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** Absatz 1.

1. Öffnen Sie die **[!UICONTROL Single Sign-on]** Registerkarte.
1. Klicken **[!UICONTROL Bearbeiten],** Füllen Sie das Feld aus und klicken Sie auf **[!UICONTROL Speichern]** Absatz 2.

1. Im **[!UICONTROL SSO]** Zeile, klicken Sie auf **[!UICONTROL Aktiviert]** Absatz 3.

![satellite_account_-_manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## SSO-Anmeldung

1. Klicken **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** Absatz 1.

1. Öffnen Sie die **[!UICONTROL Single Sign-on]** Registerkarte.
1. Stellen Sie sicher, dass Ihr [!DNL Workfront Proof] Domäne/Subdomäne (1) eingerichtet ist und dass Ihre Benutzer auf Ihre [!DNL Workfront Proof] über diese benutzerdefinierte Domäne/Subdomäne.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Wenn Sie Single Sign-On aktiviert haben, zeigt Ihre Sub-Domain-Anmelde-URL (z. B. yourcompany.proofhq.com/login) einen Übertragungsbildschirm (2) an, der Sie direkt zur SSO-Anmeldeseite führt.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Wenn ein Benutzer auf [!DNL Workfront Proof] durch **Standard-Anmeldeseite** ([https://www.proofhq.com/login](https://www.proofhq.com/login)) wird **zwei Zulassungsstufen**. Zunächst wird ein Benutzer aufgefordert, sich mit [!DNL Workfront Proof] auf Daten zugreifen (E-Mail und Passwort). Anschließend wird der Benutzer über ein SSO-Fenster (2) zur SSO-Anmeldeseite weitergeleitet.\
   Daher empfehlen wir bei aktiviertem SSO-Dienst, sich über Ihre eigene [!DNL Workfront Proof] Subdomäne/Domäne.

1. Wenn derzeit Single Sign-On für Ihr Workfront-Testkonto aktiviert ist, können Sie sich mit diesen Anmeldedaten nicht bei der iPhone-App anmelden.

## Über das Hinzufügen eines neuen Benutzers

Wenn die Single-Sign-On-Funktion in Ihrer [!DNL Workfront Proof] -Konto, erhalten neue Benutzer keine Bestätigungs-E-Mails, da ihre Konten automatisch aktiviert und einsatzbereit sind.

Von Ihrem [!DNL Workfront Proof] Anmeldeseite, nachdem Sie auf [!UICONTROL Anmelden] -Schaltfläche verwenden, werden die Benutzer zur SSO-Anmeldeseite geleitet und aufgefordert, Ihre Single Sign-On-Anmeldedaten einzugeben.

>[!IMPORTANT]
>
>Benutzer werden während des Authentifizierungsprozesses über eine E-Mail-Adresse identifiziert. Das bedeutet, dass das für Ihre SSO-Anmeldung verwendete E-Mail-Konto die E-Mail-Adresse des in Ihrem Konto registrierten Benutzers sein muss.

## Active Directory Federation Services (AD FS)

Die Active Directory Federation Services (AD FS) ist ein [!DNL Microsoft] Software-Komponente, die auf Windows Server-Betriebssystemen installiert werden kann, um Benutzern Single-Sign-On-Zugriff auf Systeme und Anwendungen zu ermöglichen, die sich über Unternehmensgrenzen hinweg befinden. Weitere Informationen finden Sie unter &quot;Active Directory Federation Services&quot;auf der Microsoft Developer Network-Website.

Die [!DNL Workfront Proof] Das System unterstützt SAML 2.0 und ist nur mit AD FS Version 2.0 oder höher kompatibel.

Siehe [Single Sign-on [!DNL Workfront Proof]: AD FS-Konfiguration](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) für detaillierte Anweisungen.
