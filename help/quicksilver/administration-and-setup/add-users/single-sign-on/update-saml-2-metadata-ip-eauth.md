---
title: SAML 2.0-Metadaten in Ihrem IDP bei Verwendung der erweiterten Authentifizierung aktualisieren
description: Als Adobe Workfront-Administrator können Sie Workfront Single Sign-on (SSO) mit jedem Identitätsanbieter integrieren, der das SAML 2.0-Protokoll (Security Assertion Markup Language) unterstützt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 0%

---

# SAML 2.0-Metadaten in Ihrem IDP bei Verwendung der erweiterten Authentifizierung aktualisieren

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Workfront Single Sign-on (SSO) mit jedem Identitätsanbieter integrieren, der das SAML 2.0-Protokoll (Security Assertion Markup Language) unterstützt.

In den folgenden Abschnitten wird der Integrationsprozess beschrieben, wenn Ihr Workfront-Konto auf die erweiterte Authentifizierung aktualisiert wurde (noch nicht für alle Unternehmen verfügbar). Weitere Informationen zur erweiterten Authentifizierung finden Sie unter [Erweiterte Authentifizierung - Übersicht](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Informationen zur Konfiguration von SAML vor der Migration zu Enhanced Authentication finden Sie unter [Aktualisieren von SAML 2.0-Metadaten in Ihrem Identitätsanbieter](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Okta als Identitätsanbieter verwenden

Okta ist ein Beispiel für einen Identitätsanbieter, der SAML 2.0 unterstützt. In diesem Abschnitt wird beschrieben, wie Sie Okta als Identitätsanbieter verwenden. Ähnliche Schritte wären bei der Konfiguration eines anderen Identitätsanbieters erforderlich, der SAML 2.0 unterstützt.

>[!NOTE]
>
>Benutzer werden anhand ihrer E-Mail-Adresse zugeordnet. Um sich mit Okta bei Workfront anmelden zu können, muss in Ihrem Workfront-Kunden eine Benutzerin bzw. ein Benutzer mit derselben (Groß- und Kleinschreibung ignorierenden) E-Mail-Adresse erstellt worden sein.

Füllen Sie die folgenden Abschnitte aus, um Okta als Identitätsanbieter in Workfront zu konfigurieren.

* [Erstellen einer Workfront-App in Okta](#create-a-workfront-app-in-okta)
* [Hinzufügen Ihrer Okta-Instanz als Identitätsanbieter in Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Erstellen einer Workfront-App in Okta {#create-a-workfront-app-in-okta}

1. Melden Sie sich bei Ihrer Okta-Umgebung an.
1. Stellen Sie sicher **dass** Klassische Benutzeroberfläche) in der oberen linken Ecke der Okta-Benutzeroberfläche ausgewählt ist.
1. Klicken Sie im Menü auf **Anwendungen** > **Anwendungen**.

1. Klicken Sie **Anwendung hinzufügen** und anschließend auf **Neue App erstellen**.

1. Wählen Sie **Dialogfeld Neue Anwendungsintegration erstellen** SAML **.0** aus und klicken Sie dann auf **Erstellen**.

1. Geben Sie einen Namen für Ihr Workfront-Programm an und klicken Sie dann auf **Weiter**.
1. Suchen Sie auf der angezeigten Seite SAML-Einstellungen die Informationen, die für die Seite SAML-Einstellungen erforderlich sind:

   1. Öffnen Sie eine separate Browser-Registerkarte oder ein separates Browser-Fenster, ohne die Browser-Registerkarte zu verlassen, auf der die Okta-Benutzeroberfläche angezeigt wird.
   1. Geben Sie die folgende URL im Browser an:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Identifizieren Sie in der resultierenden XML-Datei die Werte für **entityID** und **Location**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Kopieren Sie den Wert aus dem Feld **entityID** in die Zwischenablage Ihres Systems. Schließen Sie nicht diese Browser-Registerkarte.

1. Kehren Sie zur Seite SAML-Einstellungen zurück, die Sie in Schritt 6 geöffnet haben.
1. Fügen Sie den Wert aus dem Feld **entityID** in das Feld **Zielgruppen-URI (SP-Entitäts-ID)** ein.

1. Kopieren Sie in der XML-Datei auf der anderen Browser-Registerkarte den Wert aus dem Feld **Speicherort**.
1. Fügen Sie den Wert aus dem Feld **Standort** in das Feld **Single Sign-On** **URL** ein.

1. Scrollen Sie zum Abschnitt **Attributanweisungen (Optional)** .
1. Geben Sie **Feld** Name“ **email** an.

1. Geben Sie im Feld **Wert** den Wert **user.email** an.

1. (Optional) Fügen Sie erweiterte Werte hinzu.
1. Klicken Sie auf **Weiter**.
1. Wählen Sie **Ich bin Okta-Kunde und füge eine interne App hinzu** und klicken Sie dann auf **Beenden**.

### Hinzufügen Ihrer Okta-Instanz als Identitätsanbieter in Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Dieses Verfahren liefert wichtige Informationen zur Konfiguration von Okta als Identitätsanbieter in Workfront. Weitere Informationen zu anderen Zuordnungen oder Konfigurationsoptionen finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Laden Sie die Identitätsanbieter-Metadaten für Ihre Okta-Instanz herunter:

   1. Melden Sie sich bei Ihrer Okta-Umgebung an.
   1. Stellen Sie sicher **dass** Klassische Benutzeroberfläche) in der oberen linken Ecke der Okta-Benutzeroberfläche ausgewählt ist.
   1. Klicken Sie im Menü auf **Anwendungen** > **Anwendungen**.

   1. Klicken Sie auf die von Ihnen erstellte Workfront-App, wie im Abschnitt &quot;[ einer Workfront-App in Okta“ ](#create-a-workfront-app-in-okta)
   1. Klicken Sie auf der **Anmelden**-Registerkarte auf **Identitätsanbieter-Metadaten**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Die Metadaten werden in einer neuen Browser-Registerkarte als XML geöffnet.

   1. Kopieren Sie die URL, die im Feld Browser-URL angezeigt wird.

1. Melden Sie sich bei Workfront als Workfront-Administrator an.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **System** > **Single Sign-On (SSO)**.

1. (Bedingt) Wenn zwei Registerkarten angezeigt werden, klicken Sie auf die Registerkarte **Neue SSO-Provider**.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Löschen Sie Ihre vorhandenen SSO-Konfigurationseinstellungen auf der Registerkarte **Aktueller SSO-Provider** erst, wenn Ihr Konto auf die erweiterte Authentifizierung aktualisiert wurde und die neue SSO-Konfiguration voll funktionsfähig ist.

1. Klicken Sie auf **Neuer SSO-Provider**.
1. Geben Sie einen Namen wie Okta IDP und dann eine Beschreibung an.
1. Fügen **im Abschnitt „Felder aus Identity Provider-** füllen“ die in Schritt 1 kopierte URL in das Feld **Metadaten-URL** ein.\
   Alternativ können Sie auf **Datei auswählen** klicken, um eine XML-Datei hochzuladen. Es wird jedoch empfohlen, die URL einzufügen.

1. Geben Sie **Abschnitt &quot;** zuordnen“ im Feld **Verzeichnisattribut** &quot;**&quot;**. (**E-Mail** Adresse) ist bereits im Feld **Workfront-** ausgefüllt.)

1. (Optional) Aktivieren Sie **Als Standard-SSO-** festlegen), um nicht authentifizierte Benutzende zur Authentifizierung an den Anmeldebildschirm des Identitätsanbieters statt an den Workfront-Anmeldebildschirm zu senden. Es wird empfohlen, diese Option nur zu aktivieren, wenn alle Benutzenden in Ihrem System über den Identitätsanbieter auf Workfront zugreifen.
1. Aktivieren Sie das **Aktivieren**. Stellen Sie zuvor sicher, dass Benutzer in Ihrem System über die neue Anmeldeerfahrung informiert sind, um sicherzustellen, dass sie den Zugriff auf das Workfront-System nicht verlieren.
1. Klicken Sie **Verbindung testen**.\
   Es sollte eine Meldung angezeigt werden, die Sie darüber informiert, dass die Verbindung erfolgreich hergestellt wurde.

1. Klicken Sie auf **Speichern**.

## Verwenden anderer Identitätsanbieter

Wenn Sie andere Identitätsanbieter als Okta verwenden (z. B. Ping oder Centrify), müssen Sie die Workfront-Metadaten erneut in Ihren Identitätsanbieter hochladen.
