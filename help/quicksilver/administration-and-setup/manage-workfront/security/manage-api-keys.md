---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API-Schlüssel verwalten
description: Um Sicherheitslücken in der API zu minimieren, können Adobe Workfront-Admins die API-Schlüssel verwalten, mit denen Anwendungen für einen Benutzerzugriff auf Workfront ermöglicht werden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 8934c3f5681c09c00769442900013844ee7a80ef
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 2%

---

# API-Schlüssel verwalten

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Um Sicherheitslücken in der API zu minimieren, können Adobe Workfront-Admins die API-Schlüssel verwalten, mit denen Anwendungen für einen Benutzerzugriff auf Workfront ermöglicht werden.

Sie können Ihren aktuellen Administrator-API-Schlüssel zurücksetzen oder entfernen, API-Schlüssel für den Ablauf konfigurieren und die API-Schlüssel für alle Benutzer entfernen.

Beispiele für Programme, die die Workfront-API nutzen:

* Dokumentenintegrationen wie Dropbox, Google Drive und Workfront DAM
* Workfront Mobile Apps

>[!IMPORTANT]
>
>Beim Zurücksetzen oder Entfernen eines API-Schlüssels muss jede Anwendung, die die Workfront-API nutzt und sich über diesen API-Schlüssel bei Workfront authentifiziert, neu konfiguriert werden, um den Zugriff auf Workfront wiederzuerlangen.

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

## Workfront-API-Schlüssel

Jeder Benutzer in Workfront verfügt über einen eindeutigen API-Schlüssel. Dieser Schlüssel wird pro Benutzer generiert, wenn der Benutzer auf eine Integration zugreift, die die Workfront-API nutzt (z. B. die Workfront Mobile App oder eine Dokumentenintegration).

>[!NOTE]
>
> API-Schlüssel, die Sie in der Produktionsumgebung generieren, werden während der wöchentlichen Aktualisierung in Ihre Vorschau-Umgebung kopiert. Alle API-Schlüssel, die Sie in der Vorschau-Umgebung generieren, werden während der wöchentlichen Aktualisierung mit Ihren Produktions-API-Schlüsseln überschrieben.

Workfront-Administratoren verfügen außerdem über einen eindeutigen API-Schlüssel. Wenn eine Anwendung einen Administrator-API-Schlüssel für den Zugriff auf Workfront verwendet, hat die Anwendung Administratorzugriff auf Workfront.

## Administrator-API-Schlüssel verwalten

Sie können den API-Schlüssel für Ihr Administrator-Benutzerkonto generieren, zurücksetzen oder entfernen.

>[!NOTE]
>
>Sie können auch einen API-Schlüssel über die API generieren. Weitere Informationen finden Sie im Abschnitt [Ereignisabonnement-API](../../../wf-api/general/event-subs-api.md) in [Ereignisabonnement-API](../../../wf-api/general/event-subs-api.md).

{{step-1-to-setup}}

1. Klicken Sie auf **System >** **Kundeninformationen.**
1. (Bedingt) Führen Sie eine der folgenden Aktionen aus:

   So generieren Sie einen API-Schlüssel: Klicken Sie **Abschnitt** API-Schlüsseleinstellungen **auf API-Schlüssel generieren**.

   Oder\
   Zurücksetzen eines API-Schlüssels: Klicken Sie im Abschnitt **API** Schlüsseleinstellungen“ auf **Zurücksetzen** und dann auf **Zurücksetzen.**

   Oder

   So entfernen Sie den API-Schlüssel: Klicken Sie im Abschnitt **API** Schlüsseleinstellungen **auf „Entfernen** und dann auf **Entfernen**.

## Generieren eines API-Schlüssels für Benutzer ohne Administratorrechte

Sie können API-Schlüssel für Benutzer in anderen Rollen als Workfront-Admins generieren und verwalten.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

1. (Bedingt) Wenn Ihre Organisation die Zugriffsverwaltung mit Single Sign-On (SSO) verwendet, deaktivieren Sie vorübergehend die Option, die eine SSO-Authentifizierung erfordert.

   {{step-1-to-setup}}

   1. Erweitern Sie **System** und klicken Sie dann auf **Single Sign-on (SSO)**.
   1. Wählen Sie im Feld **Typ** den SSO-Typ aus, den Ihr Unternehmen verwendet.
   1. Scrollen Sie bei ausgewähltem Typ nach unten und deaktivieren Sie das Kontrollkästchen **Aktivieren**.

      ![SSO aktivieren](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Klicken Sie auf **Speichern**.


1. Geben Sie in der Adressleiste eines Browsers den folgenden API-Aufruf ein:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**username**&amp;password=**password**&amp;method=PUT

   Ersetzen Sie `<domain>` durch Ihren Workfront-Domain-Namen sowie den Benutzernamen und das Kennwort mit den Workfront-Anmeldeinformationen des Benutzers.

1. (Bedingt) Aktivieren Sie die Option, die eine SSO-Authentifizierung erfordert, wenn Sie sie in Schritt 1 deaktiviert haben.

   {{step-1-to-setup}}

   1. Erweitern Sie **System** und klicken Sie dann auf **Single Sign-on (SSO)**.

   1. Wählen Sie die SSO-Methode im Dropdown **Menü** Typ“ aus.
   1. Aktivieren Sie das Kontrollkästchen, das eine SSO-Authentifizierung erfordert.

## Konfigurieren, wann API-Schlüssel ablaufen

Sie können API-Schlüssel so konfigurieren, dass sie für alle Benutzer in Ihrem System ablaufen. Wenn der API-Schlüssel einer Benutzerin oder eines Benutzers abläuft, muss sich die Benutzerin bzw. der Benutzer erneut bei allen Anwendungen authentifizieren, die die Workfront-API für den Zugriff auf Workfront verwenden. Sie können die Häufigkeit ändern, mit der die API-Schlüssel ablaufen. Sie können auch konfigurieren, ob API-Schlüssel ablaufen, wenn das Kennwort eines Benutzers abläuft.

{{step-1-to-setup}}

1. Klicken Sie **System** > **Kundeninformationen**.
1. Wählen Sie im Bereich **API** Schlüsseleinstellungen in der Dropdown-Liste **Nach** Erstellung **API-Schlüssel laufen ab in** den Zeitrahmen aus, in dem die API-Schlüssel ablaufen sollen.

   Wenn Sie diese Option ändern, beginnt der neue Zeitrahmen ab dem Zeitpunkt, an dem Sie die Änderung vorgenommen haben. Wenn Sie diese Option beispielsweise von *1 Monat* auf *6 Monate* ändern, laufen die API-Schlüssel 6 Monate nach der Änderung ab.

   Standardmäßig laufen API-Schlüssel jeden Monat ab.

1. Um API-Schlüssel so zu konfigurieren, dass sie zum Zeitpunkt des Ablaufs der Benutzerkennwörter ablaufen, aktivieren Sie **API-Schlüssel entfernen, wenn das Kennwort eines Benutzers abläuft**.

   Standardmäßig ist diese Option nicht aktiviert.

   Informationen zum Konfigurieren von Benutzerkennwörtern für den Ablauf finden Sie unter [Konfigurieren von Systemsicherheitseinstellungen](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Klicken Sie auf **Speichern**.

## API-Schlüssel für alle Benutzer entfernen

Wenn Sie wegen einer bestimmten Sicherheitsverletzung in Bezug auf Ihr Workfront-System besorgt sind, können Sie API-Schlüssel gleichzeitig für alle Benutzer entfernen.

>[!IMPORTANT]
>
>Das Entfernen von API-Schlüsseln für alle Benutzer macht ALLE API-Schlüssel für alle Benutzer im System ungültig. Diese Aktion führt dazu, dass alle Ihre Integrationen in Workfront fehlschlagen, bis Sie einen neuen API-Schlüssel in Workfront generieren und alle Ihre Integrationen aktualisieren.

{{step-1-to-setup}}

1. Erweitern Sie **System** und klicken Sie dann auf **Kundeninformationen**.

1. Klicken Sie im Bereich **API** Schlüsseleinstellungen auf **Alle API-Schlüssel entfernen** und klicken Sie dann auf **Entfernen** **Alle**.

## Einschränken von API-Anmeldungen mit einem X.509-Zertifikat

>[!IMPORTANT]
>
>Das in diesem Abschnitt beschriebene Verfahren gilt nur für Organisationen, die noch keine Einführung in die Adobe Business Platform erhalten haben. Die Anmeldung bei Workfront über die Workfront-API ist nicht verfügbar, wenn Ihr Unternehmen die Adobe Business-Plattform verwendet hat.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen die Adobe Business Platform verwendet, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

Programme von Drittanbietern können über die API mit Workfront kommunizieren. Um die Sicherheit Ihrer Workfront-Site zu erhöhen, können Sie Workfront so konfigurieren, dass API-Anmeldeanfragen durch Hochladen eines X.509-Zertifikats in Workfront eingeschränkt werden. Nach der Aktivierung müssen alle Anmeldeanfragen über die API zusätzlich zu Benutzername und Kennwort ein Client-Zertifikat enthalten.

* [Erhalten Sie das X.509-Zertifikat](#obtain-the-x-509-certificate)
* [Zertifikat in Workfront hochladen](#upload-the-certificate-to-workfront)
* [Überprüfen, ob API-Anmeldeaufrufe eingeschränkt sind](#verify-api-login-calls-are-restricted)

### X.509-Zertifikat erhalten {#obtain-the-x-509-certificate}

Beschaffen Sie sich ein gültiges X.509-Zertifikat von einer vertrauenswürdigen Zertifizierungsstelle (z. B. Verisign) und speichern Sie es an einem temporären Speicherort auf Ihrer Workstation.

### Hochladen des Zertifikats in Workfront {#upload-the-certificate-to-workfront}

Nachdem Sie das X.509-Zertifikat von Ihrer Zertifizierungsstelle erhalten haben, müssen Sie es in Workfront hochladen.

1. Klicken Sie auf das **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront und dann auf **Setup** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Erweitern Sie **System** und klicken Sie dann auf **Kundeninformationen**.

1. Wählen Sie im Bereich **API** Schlüsseleinstellungen“ die Option **X.509-Zertifikat für API-Anmeldungen erforderlich**.
1. Klicken Sie **Zertifikat ändern**.
1. Navigieren Sie auf Ihrer Workstation zu und wählen Sie das zuvor heruntergeladene X.509-Zertifikat aus.
1. (Optional) Klicken Sie **Details anzeigen** neben dem Zertifikatnamen, um die folgenden Details zum Zertifikat anzuzeigen:

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

Bevor Sie Ihre Workfront-Instanz so konfigurieren, dass ein X.509-Zertifikat erforderlich ist, führen Sie eine API-Anfrage an den `/login`-Endpunkt mit gültigen Benutzernamen- und Kennwortparametern durch. Sie erhalten eine 200-Antwort, die eine Sitzungs-ID enthält.

Nachdem Sie das X.509-Zertifikat über die Kundeninformationsseite in Ihrer Workfront-Instanz zu einer Anforderung gemacht haben, führen Sie einen weiteren Anmeldeversuch durch. Dieses Mal erhalten Sie eine 500-Fehler-Antwort mit der folgenden Meldung: „Nicht vertrauenswürdige Anfrage. Wenden Sie sich an Ihren Systemadministrator und fügen Sie das Zertifikat bei.“

Nachdem Sie bestätigt haben, dass das X.509-Zertifikat erforderlich ist, führen Sie dieselbe Anmeldeanfrage mit einem zusätzlichen Parameter für apiCertificate aus, der auf den Wert Ihres Zertifikats gesetzt ist. Wenn dieser Vorgang korrekt ausgeführt wurde, erhalten Sie eine 200-Antwort, die eine gültige Sitzungs-ID enthält.
