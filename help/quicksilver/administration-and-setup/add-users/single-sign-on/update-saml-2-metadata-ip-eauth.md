---
title: SAML 2.0-Metadaten in Ihrem IDP bei Verwendung der erweiterten Authentifizierung aktualisieren
description: Als Adobe Workfront-Administrator können Sie Workfront Single Sign-On (SSO) mit jedem Identitäts-Provider integrieren, der das SAML 2.0-Protokoll (Security Assertion Markup Language) unterstützt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 0%

---

# SAML 2.0-Metadaten in Ihrem IDP bei Verwendung der erweiterten Authentifizierung aktualisieren

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Als Adobe Workfront-Administrator können Sie Workfront Single Sign-On (SSO) mit jedem Identitäts-Provider integrieren, der das SAML 2.0-Protokoll (Security Assertion Markup Language) unterstützt.

In den folgenden Abschnitten wird der Integrationsprozess beschrieben, wenn Ihr Workfront-Konto auf die erweiterte Authentifizierungsfunktion aktualisiert wurde (noch nicht für alle Organisationen verfügbar). Weitere Informationen zum erweiterten Authentifizierungs-Erlebnis finden Sie unter [Übersicht über die erweiterte Authentifizierung](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Informationen zum Konfigurieren von SAML vor der Migration zum erweiterten Authentifizierungs-Erlebnis finden Sie unter [Aktualisieren der SAML 2.0-Metadaten in Ihrem Identitäts-Provider](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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

+++

## Verwenden Sie Okta als Identitätsanbieter.

Okta ist ein Beispiel für einen Identitätsanbieter, der SAML 2.0 unterstützt. In diesem Abschnitt wird beschrieben, wie Sie Okta als Identitätsanbieter verwenden. Ähnliche Schritte wären beim Konfigurieren eines anderen Identitäts-Providers erforderlich, der SAML 2.0 unterstützt.

>[!NOTE]
>
>Benutzer werden anhand ihrer E-Mail-Adresse zugeordnet. Damit Sie sich mit Okta bei Workfront anmelden können, müssen Sie über einen Benutzer verfügen, der dieselbe E-Mail-Adresse (nicht zwischen Groß- und Kleinschreibung) hat, die in Ihrem Workfront-Kunden erstellt wurde.

Füllen Sie die folgenden Abschnitte aus, um Okta als Ihren Identitätsanbieter in Workfront zu konfigurieren.

* [Erstellen einer Workfront-App in Okta](#create-a-workfront-app-in-okta)
* [Hinzufügen Ihrer Okta-Instanz als Identitätsanbieter in Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Erstellen einer Workfront-App in Okta {#create-a-workfront-app-in-okta}

1. Melden Sie sich bei Ihrer Okta-Umgebung an.
1. Stellen Sie sicher, dass in der oberen linken Ecke der Okta-Oberfläche die Option **Klassische Benutzeroberfläche** ausgewählt ist.
1. Klicken Sie im Menü auf **Anwendungen** > **Anwendungen**.

1. Klicken Sie auf **Anwendung hinzufügen** und dann auf **Neue App erstellen**.

1. Wählen Sie im Dialogfeld **Neue Anwendungsintegration erstellen** die Option **SAML 2.0** und klicken Sie dann auf **Erstellen**.

1. Geben Sie einen Namen für Ihre Workfront-App ein und klicken Sie dann auf **Weiter**.
1. Suchen Sie auf der angezeigten Seite &quot;SAML-Einstellungen&quot;die für die Seite &quot;SAML-Einstellungen&quot;erforderlichen Informationen:

   1. Öffnen Sie, ohne die Browser-Registerkarte zu verlassen, auf der die Okta-Benutzeroberfläche angezeigt wird, eine separate Browser-Registerkarte oder ein separates Fenster.
   1. Geben Sie die folgende URL im Browser an:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Geben Sie in der resultierenden XML-Datei die Werte für **entityID** und **Location** an.

      ![sso-okta.png](assets/sso-okta.png)

   1. Kopieren Sie den Wert aus dem Feld **entityID** in die Zwischenablage Ihres Systems. Schließen Sie diese Browser-Registerkarte nicht.

1. Gehen Sie zurück zur Seite &quot;SAML-Einstellungen&quot;, die Sie in Schritt 6 geöffnet haben.
1. Fügen Sie den Wert aus dem Feld **entityID** in das Feld **Audience URI (SP Entity ID)** ein.

1. Kopieren Sie in der XML-Datei auf der anderen Browser-Registerkarte den Wert aus dem Feld **Position** .
1. Fügen Sie den Wert aus dem Feld **Position** in das Feld **Einzelzeichen auf** **URL** ein.

1. Scrollen Sie zum Abschnitt **Attributanweisungen (optional)** .
1. Geben Sie im Feld **Name** den Wert **email** an.

1. Geben Sie im Feld **Wert** den Wert **user.email** an.

1. (Optional) Fügen Sie erweiterte Werte hinzu.
1. Klicken Sie auf **Weiter**.
1. Wählen Sie &quot;**Ich bin Okta-Kunde und füge eine interne App hinzu&quot;** und klicken Sie dann auf &quot;**Beenden**&quot;.

### Hinzufügen Ihrer Okta-Instanz als Identitätsanbieter in Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Dieses Verfahren liefert wichtige Informationen für die Konfiguration von Okta als Identitätsanbieter in Workfront. Weitere Informationen zu anderen Zuordnungen oder Konfigurationsoptionen finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Laden Sie die Metadaten des Identitätsanbieters für Ihre Okta-Instanz herunter:

   1. Melden Sie sich bei Ihrer Okta-Umgebung an.
   1. Stellen Sie sicher, dass in der oberen linken Ecke der Okta-Oberfläche die Option **Klassische Benutzeroberfläche** ausgewählt ist.
   1. Klicken Sie im Menü auf **Anwendungen** > **Anwendungen**.

   1. Klicken Sie auf die von Ihnen erstellte Workfront-App, wie im Abschnitt [Erstellen einer Workfront-App in Okta](#create-a-workfront-app-in-okta) beschrieben.
   1. Klicken Sie auf der Registerkarte **Anmelden** auf **Metadaten des Identitätsanbieters**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Die Metadaten werden in einer neuen Browser-Registerkarte als XML geöffnet.

   1. Kopieren Sie die URL, die im Feld der Browser-URL angezeigt wird.

1. Melden Sie sich bei Workfront als Workfront-Administrator an.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **System** > **Single Sign-On (SSO)**.

1. (Bedingt) Wenn zwei Registerkarten angezeigt werden, klicken Sie auf die Registerkarte **Neue SSO-Anbieter** .

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Löschen Sie Ihre vorhandenen SSO-Konfigurationseinstellungen nicht auf der Registerkarte **Aktueller SSO-Anbieter**, bis Ihr Konto auf das erweiterte Authentifizierungs-Erlebnis aktualisiert wurde und die neue SSO-Konfiguration vollständig funktioniert.

1. Klicken Sie auf **Neuer SSO-Anbieter**.
1. Geben Sie einen Namen an, z. B. Okta-IDP, und geben Sie dann eine Beschreibung an.
1. Fügen Sie im Abschnitt **Felder aus Identity Provider-Metadaten ausfüllen** die URL, die Sie in Schritt 1 kopiert haben, in das Feld **Metadaten-URL** ein.\
   Alternativ können Sie auf **Datei auswählen** klicken, um eine XML-Datei hochzuladen. Es wird jedoch empfohlen, die URL einzufügen.

1. Geben Sie im Abschnitt **Benutzerattribute zuordnen** im Feld **Ordnerattribut** den Wert **email** ein. (**E-Mail-Adresse** ist bereits im Feld **Workfront-Benutzerattribut** ausgefüllt.)

1. (Optional) Aktivieren Sie **Als Standard-SSO-Anbieter festlegen** , um nicht authentifizierte Benutzer zum Anmeldebildschirm des Identitäts-Providers und nicht zum Workfront-Anmeldebildschirm für die Authentifizierung zu senden. Es wird empfohlen, diese Option nur zu aktivieren, wenn alle Benutzer in Ihrem System über den Identitäts-Provider auf Workfront zugreifen.
1. Aktivieren Sie das Kontrollkästchen **Aktivieren** . Stellen Sie zunächst sicher, dass Benutzer in Ihrem System über die neue Anmeldeerfahrung informiert sind, um sicherzustellen, dass sie den Zugriff auf das Workfront-System nicht verlieren.
1. Klicken Sie auf **Verbindung testen**.\
   Es sollte eine Meldung angezeigt werden, die Sie darüber informiert, dass die Verbindung erfolgreich hergestellt wurde.

1. Klicken Sie auf **Speichern**.

## Andere Identitätsanbieter verwenden

Bei Verwendung anderer Identitätsanbieter als Okta (z. B. Ping oder Centrify) müssen Sie die Workfront-Metadaten erneut in Ihren Identitätsanbieter hochladen.
