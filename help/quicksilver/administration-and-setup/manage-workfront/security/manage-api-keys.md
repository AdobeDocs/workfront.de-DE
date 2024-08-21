---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API-Schlüssel verwalten
description: Um API-Sicherheitslücken zu minimieren, können Adobe Workfront-Administratoren die API-Schlüssel verwalten, mit denen Anwendungen im Auftrag eines Benutzers auf Workfront zugreifen können.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '1322'
ht-degree: 2%

---

# API-Schlüssel verwalten

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Um API-Sicherheitslücken zu minimieren, können Adobe Workfront-Administratoren die API-Schlüssel verwalten, mit denen Anwendungen im Auftrag eines Benutzers auf Workfront zugreifen können.

Sie können Ihren aktuellen Administrator-API-Schlüssel zurücksetzen oder entfernen, die API-Schlüssel so konfigurieren, dass sie ablaufen, und die API-Schlüssel für alle Benutzer entfernen.

Beispiele für Anwendungen, die die Workfront-API nutzen:

* Dokumentenintegrationen wie Dropbox, Google Drive und Workfront DAM
* Mobile Apps für Workfront

>[!IMPORTANT]
>
>Beim Zurücksetzen oder Entfernen eines API-Schlüssels muss jede Anwendung, die die Workfront-API nutzt und sich über diesen API-Schlüssel bei Workfront authentifiziert, neu konfiguriert werden, um wieder Zugriff auf Workfront zu erhalten.

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

## Workfront-API-Schlüssel

Jeder Benutzer in Workfront verfügt über einen eindeutigen API-Schlüssel. Dieser Schlüssel wird pro Benutzer generiert, wenn der Benutzer auf eine Integration zugreift, die die Workfront-API nutzt (z. B. die mobile Workfront-App oder eine Dokumentintegration).

>[!NOTE]
>
> API-Schlüssel, die Sie in der Produktionsumgebung generieren, werden während der wöchentlichen Aktualisierung in die Vorschauumgebung kopiert. Alle API-Schlüssel, die Sie in der Vorschau-Umgebung generieren, werden während der wöchentlichen Aktualisierung mit Ihren Produktions-API-Schlüsseln überschrieben.

Workfront-Administratoren verfügen auch über einen eindeutigen API-Schlüssel. Wenn eine Anwendung einen Administrator-API-Schlüssel für den Zugriff auf Workfront verwendet, hat die Anwendung Administratorzugriff auf Workfront.

## Verwalten eines API-Schlüssels für Administratoren

Sie können den API-Schlüssel für Ihr Administratorbenutzerkonto generieren, zurücksetzen oder entfernen.

>[!NOTE]
>
>Sie können auch einen API-Schlüssel über die API generieren. Weitere Informationen finden Sie im Abschnitt [Event Subscription API](../../../wf-api/general/event-subs-api.md) in der [Event Subscription API](../../../wf-api/general/event-subs-api.md).

{{step-1-to-setup}}

1. Klicken Sie auf **System >** **Customer Info.**
1. (Bedingt) Führen Sie einen der folgenden Schritte aus:

   So generieren Sie einen API-Schlüssel: Klicken Sie im Abschnitt **API-Schlüsseleinstellungen** auf **API-Schlüssel generieren** .

   Oder\
   Zurücksetzen eines API-Schlüssels: Klicken Sie im Abschnitt **API-Schlüsseleinstellungen** auf **Zurücksetzen** und dann auf **Zurücksetzen** .

   Oder

   Entfernen des API-Schlüssels: Klicken Sie im Abschnitt **API-Schlüsseleinstellungen** auf **Entfernen** und dann auf **Entfernen**.

## API-Schlüssel für Benutzer ohne Administratorrechte generieren

Sie können API-Schlüssel für Benutzer in anderen Rollen als dem Workfront-Administrator generieren und verwalten.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

1. (Bedingt) Wenn Ihr Unternehmen die SSO-Zugriffsverwaltung (Single Sign-On) verwendet, deaktivieren Sie vorübergehend die Option, für die eine SSO-Authentifizierung erforderlich ist.

   {{step-1-to-setup}}

   1. Erweitern Sie **System** und klicken Sie dann auf **Single Sign-on (SSO)**.
   1. Wählen Sie im Feld **Typ** den SSO-Typ aus, den Ihr Unternehmen verwendet.
   1. Scrollen Sie bei ausgewähltem Typ nach unten und deaktivieren Sie das Kontrollkästchen **Aktivieren** .
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Klicken Sie auf **Speichern**.


1. Geben Sie in der Adressleiste eines Browsers den folgenden API-Aufruf ein:

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**Benutzername**&amp;password=**password**&amp;method=PUT

   Ersetzen Sie `<domain>` durch Ihren Workfront-Domänennamen und den Benutzernamen und das Kennwort durch die Workfront-Anmeldeinformationen des Benutzers.

1. (Bedingt) Aktivieren Sie die Option, für die eine SSO-Authentifizierung erforderlich ist, wenn Sie sie in Schritt 1 deaktiviert haben.

   {{step-1-to-setup}}

   1. Erweitern Sie **System** und klicken Sie dann auf **Single Sign-on (SSO)**.

   1. Wählen Sie Ihre SSO-Methode im Dropdownmenü **Typ** aus.
   1. Aktivieren Sie das Kontrollkästchen, für das eine SSO-Authentifizierung erforderlich ist.

## Konfigurieren, wann API-Schlüssel ablaufen

Sie können API-Schlüssel so konfigurieren, dass sie für alle Benutzer in Ihrem System ablaufen. Wenn der API-Schlüssel eines Benutzers abläuft, muss der Benutzer sich erneut bei allen Anwendungen authentifizieren, die die Workfront-API für den Zugriff auf Workfront verwenden. Sie können die Häufigkeit ändern, mit der die API-Schlüssel ablaufen. Sie können auch konfigurieren, ob API-Schlüssel ablaufen, wenn das Kennwort eines Benutzers abläuft.

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Kunden-Info**.
1. Wählen Sie im Bereich **API-Schlüsseleinstellungen** in der Dropdown-Liste **Nach der Erstellung** die API-Schlüssel **, die in der Dropdownliste** ablaufen, den Zeitrahmen aus, in dem die API-Schlüssel ablaufen sollen.

   Wenn Sie diese Option ändern, beginnt der neue Zeitrahmen mit dem Zeitpunkt, zu dem Sie die Änderung vorgenommen haben. Wenn Sie diese Option beispielsweise von *1 Monat* in *6 Monate* ändern, laufen die API-Schlüssel 6 Monate ab dem Zeitpunkt ab, zu dem Sie die Änderung vornehmen.

   Standardmäßig laufen API-Schlüssel jeden Monat ab.

1. Um API-Schlüssel so zu konfigurieren, dass sie zum Zeitpunkt des Ablaufs der Passwörter der Benutzer ablaufen, wählen Sie **API-Schlüssel entfernen, wenn das Passwort eines Benutzers abläuft**.

   Standardmäßig ist diese Option nicht ausgewählt.

   Weitere Informationen zum Konfigurieren des Ablaufs von Benutzerkennwörtern finden Sie unter [Systemsicherheitsvoreinstellungen konfigurieren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Klicken Sie auf **Speichern**.

## Entfernen Sie die API-Schlüssel für alle Benutzer

Wenn Sie wegen einer bestimmten Sicherheitsverletzung in Bezug auf Ihr Workfront-System besorgt sind, können Sie API-Schlüssel gleichzeitig für alle Benutzer entfernen.

>[!IMPORTANT]
>
>Durch das Entfernen der API-Schlüssel für alle Benutzer werden ALLE API-Schlüssel für alle Benutzer im System ungültig. Dadurch schlagen all Ihre Integrationen in Workfront fehl, bis Sie einen neuen API-Schlüssel in Workfront generieren und alle Ihre Integrationen aktualisieren.

{{step-1-to-setup}}

1. Erweitern Sie **System** und klicken Sie dann auf **Kundeninformationen**.

1. Klicken Sie im Bereich **API-Schlüsseleinstellungen** auf **Alle API-Schlüssel entfernen** und dann auf **Entfernen** **Alle**.

## Einschränken von API-Anmeldungen mit einem X.509-Zertifikat

>[!IMPORTANT]
>
>Das in diesem Abschnitt beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Adobe Business Platform integriert wurden. Die Anmeldung bei Workfront über die Workfront-API ist nicht verfügbar, wenn Ihr Unternehmen in die Adobe Business Platform integriert wurde.
>
>Eine Liste der Vorgehensweisen, die sich je nachdem, ob Ihr Unternehmen in die Adobe Business Platform integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Drittanbieteranwendungen können über die API mit Workfront kommunizieren. Um die Sicherheit Ihrer Workfront-Site zu erhöhen, können Sie Workfront so konfigurieren, dass API-Anmeldeanfragen eingeschränkt werden, indem Sie ein X.509-Zertifikat in Workfront hochladen. Nach der Aktivierung müssen alle Anmeldeanfragen über die API ein Client-Zertifikat zusätzlich zu Benutzername und Kennwort enthalten.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

* [Abrufen des X.509-Zertifikats](#obtain-the-x-509-certificate)
* [Hochladen des Zertifikats in Workfront](#upload-the-certificate-to-workfront)
* [Überprüfen, ob API-Anmeldeaufrufe eingeschränkt sind](#verify-api-login-calls-are-restricted)

### Abrufen des X.509-Zertifikats {#obtain-the-x-509-certificate}

Besorgen Sie sich ein gültiges X.509-Zertifikat von einer vertrauenswürdigen Zertifizierungsstelle (z. B. Verisign) und platzieren Sie es an einem temporären Speicherort auf Ihrer Workstation.

### Hochladen des Zertifikats in Workfront {#upload-the-certificate-to-workfront}

Nachdem Sie das X.509-Zertifikat von Ihrer Zertifizierungsstelle erhalten haben, müssen Sie es in Workfront hochladen.

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Erweitern Sie **System** und klicken Sie dann auf **Kundeninformationen**.

1. Wählen Sie im Bereich **API-Schlüsseleinstellungen** die Option **X.509-Zertifikat aktivieren** aus.
1. Suchen Sie auf Ihrer Workstation das zuvor heruntergeladene X.509-Zertifikat und wählen Sie es aus.
1. (Optional) Klicken Sie neben dem Zertifikatnamen auf **Details anzeigen** , um die folgenden Details zum Zertifikat anzuzeigen:

   * Allgemeiner Antragstellername
   * Organisation des Antragstellenden
   * Organisationseinheit des Antragstellenden
   * Allgemeiner Ausstellername
   * Organisation des Zertifikatausstellers
   * Organisationseinheit des Zertifikatausstellers
   * Seriennummer
   * Ausstellungsdatum
   * Ablaufdatum

1. Klicken Sie auf **Speichern**.

### Überprüfen, ob API-Anmeldeaufrufe eingeschränkt sind {#verify-api-login-calls-are-restricted}

Führen Sie vor dem Konfigurieren Ihrer Workfront-Instanz für das Anfordern eines X.509-Zertifikats eine API-Anfrage an den `/login`-Endpunkt mit gültigen Benutzernamen- und Kennwortparametern aus. Sie erhalten eine 200-Antwort, die eine sessionID enthält.

Nachdem Sie das X.509-Zertifikat über die Kundeninformationsseite in Ihrer Workfront-Instanz zur Anforderung gemacht haben, führen Sie einen weiteren Anmeldeversuch durch. Diesmal erhalten Sie eine 500-Fehlerantwort mit der folgenden Meldung: &quot;Nicht vertrauenswürdige Anfrage. Wenden Sie sich an Ihren Systemadministrator und hängen Sie ein Zertifikat an.&quot;

Nachdem Sie bestätigt haben, dass das X.509-Zertifikat erforderlich ist, führen Sie dieselbe Anmeldeanfrage mit einem zusätzlichen Parameter für apiCertificate durch, der auf den Wert Ihres Zertifikats festgelegt ist. Wenn dieser Vorgang korrekt ausgeführt wurde, erhalten Sie eine 200-Antwort, die eine gültige sessionID enthält.
