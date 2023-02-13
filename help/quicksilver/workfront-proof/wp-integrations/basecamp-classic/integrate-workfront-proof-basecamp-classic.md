---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integrieren [!DNL Workfront Proof] mit Basecamp Classic
description: Wenn Sie [!DNL Basecamp] Für das Projektmanagement können Sie Ihrem Projektteam umfangreiche Überprüfungs- und Validierungstools mit [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Integrieren [!DNL Workfront Proof] mit [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie [!DNL Basecamp] Für das Projektmanagement können Sie Ihrem Projektteam umfangreiche Überprüfungs- und Validierungstools mit [!DNL Workfront Proof].

## Grundlagen zum [!DNL Basecamp] Integration mit [!DNL Workfront]

Integrieren mit [!DNL Basecamp] ermöglicht Benutzern das Anzeigen, Überprüfen und Genehmigen von Testsendungen in [!DNL Basecamp]. Benutzer können Testsendungen an Ihre [!DNL Workfront Proof] -Konto und verbinden Sie sie mit Ihrem [!DNL Basecamp] Projekt. Ihre Validierer können [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp], unter Verwendung des in Ihre Basecamp-Nachricht eingebetteten Mini-Testversands.

Bei Integration in [!DNL Workfront Proof], [!DNL Basecamp] ermöglicht Benutzern Folgendes mit Testsendungen:

* Benutzer können Testsendungen in [!DNL Basecamp Classic].
* Benutzer haben Überprüfungs-Tools sofort verfügbar.
* Projektprüfungsteams erhalten eine Nachricht in [!DNL Basecamp] mit einem kleinen Testversand zur Überprüfung und Validierung.
* Benutzer können zur Überprüfung und Genehmigung zu einem ganzseitigen Testversand wechseln.
* Benutzer können sowohl Mini- als auch Vollbildsendungen Kommentare und Markups hinzufügen.

   >[!NOTE]
   >
   >Nachdem ein Kommentar beantwortet wurde, kann er nicht mehr bearbeitet oder gelöscht werden.

* Überprüfer können auf die Markierungen und reagieren, die von anderen Validierern vorgenommen wurden.
* Benutzer werden benachrichtigt, wenn eine neue Testversion verfügbar ist.
* Benutzer, die nicht [!DNL Workfront Proof] -Benutzer können an einem Testversand in [!DNL Basecamp].

Die Integration von [!DNL Workfront Proof] mit [!DNL Basecamp] muss auf zwei Ebenen eingerichtet werden:

* Konfigurieren [!DNL Basecamp] in [Kontoeinstellungen:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Dies ermöglicht die Basecamp-Integration für Ihre gesamte Organisation.
* Weitere Informationen finden Sie unter [Aktivieren der [!DNL Basecamp] Integration mit [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Konfigurieren [!DNL Basecamp] in [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Dies ermöglicht es Erstellern und Eigentümern von Testsendungen, sich mit ihren persönlichen [!DNL Basecamp] und autorisieren [!DNL Workfront Proof] Zugriff. Weitere Informationen finden Sie unter [Persönliche Einstellungen konfigurieren](#configuring-personal-settings).

Sie können [!DNL Workfront] mit [!DNL Basecamp] oder [!DNL Basecamp Classic]. Jede Version von [!DNL Basecamp] verwendet eine andere API und erfordert daher unterschiedliche Konfigurationsverfahren.

Informationen zur Konfiguration [!DNL Basecamp Classic], siehe [Aktivieren der [!DNL Basecamp] Integration mit [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in diesem Artikel.

Informationen zur Konfiguration [!DNL Basecamp], siehe [Integrieren [!DNL Workfront Proof] mit [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Aktivieren der [!DNL Basecamp] Integration mit [!DNL Workfront Proof]

Als [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) oder [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), können Sie die Basecamp-Integration für das gesamte Konto in Ihrer [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Navigieren Sie zu [Kontoeinstellungen.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Öffnen Sie die **[!UICONTROL Integrationen]** Registerkarte (1).
1. Um die Basecamp-Integration zu aktivieren, klicken Sie auf **[!UICONTROL Aktivieren]** Absatz 2.
1. Stellen Sie sicher, dass [!DNL Basecamp Classic] ist die Version, in die Sie integrieren (3).
1. (Bedingt) Wenn nicht [!DNL Basecamp] URL wird angezeigt (4), klicken Sie auf **[!UICONTROL Bearbeiten]** und geben Sie die URL für Ihre [!DNL Basecamp] -Konto (ohne http://).
1. Klicken **[!UICONTROL Speichern]** Absatz 5.\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Optional) Überprüfen Sie Ihre [!DNL Basecamp] URL in Ihrem Browser nach der Anmeldung bei [!DNL Basecamp Classic] Konto (6).

   ![basecamp_URL.png](assets/basecamp-url-350x75.png)

   Nach der Integration [!DNL Workfront Proof] mit [!DNL Basecamp], können Ihre Benutzer ihre persönlichen Einstellungen konfigurieren. Informationen zum Einrichten von persönlichen Einstellungen finden Sie unter [Persönliche Einstellungen konfigurieren](#configuring-personal-settings).

   Wenn die Option [!DNL Basecamp] Integration, [!DNL Workfront Proof] Die Konto-ID stimmt möglicherweise nicht mit der Konto-ID überein, die Sie in [!DNL Basecamp].

## Persönliche Einstellungen konfigurieren

Nach der Einrichtung [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) für Ihre Organisation sollten alle Autoren, die Testsendungen erstellen/senden, ihre  [persönliche Einstellungen.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Die Durchführung dieser Schritte ist am einfachsten, wenn Sie über [!DNL Basecamp] -Sitzung in einem Browserfenster geöffnet und Ihre [!DNL Workfront Proof] -Sitzung in einem anderen Fenster geöffnet.

* [Abrufen Ihrer [!DNL Basecamp] API-Token](#retrieving-your-basecamp-api-token)
* [Hinzufügen Ihrer [!DNL Basecamp] API-Token zu Ihren persönlichen Einstellungen](#adding-your-basecamp-api-token-to-your-personal-settings)

### Abrufen Ihrer [!DNL Basecamp] API-Token

So schließen Sie die Integration auf individueller Ebene in [!DNL Workfront Proof], benötigen Benutzer ihr individuelles Authentifizierungstoken für die [!DNL Basecamp] API.

So rufen Sie Ihre [!DNL Basecamp] API-Token:

1. Melden Sie sich bei Ihrer [!DNL Basecamp] -Konto.
1. Klicken **[!UICONTROL Meine Informationen]** (1) in der oberen rechten Ecke des Bildschirms.\
   Die [!UICONTROL Meine Informationen] angezeigt.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. Im [!UICONTROL Authentifizierungstoken] Abschnitt, klicken Sie auf **[!UICONTROL Token anzeigen]** (2), um Ihre persönlichen Authentifizierungstoken anzuzeigen.
1. Wählen Sie die **[!UICONTROL Token für Feed-Leser]** oder **[!UICONTROL Basecamp-API]** (3) und kopieren Sie dann das Token in die Zwischenablage.

1. Fügen Sie Ihre [!DNL Basecamp] API-Token in [!UICONTROL Token für Feed-Leser] oder [!UICONTROL Basecamp-API] ankreuzen.\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Hinzufügen Ihrer [!DNL Basecamp] API-Token zu Ihren persönlichen Einstellungen

So fügen Sie die [!DNL Basecamp] API-Token in [!DNL Workfront Proof] [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Navigieren Sie zu [[!UICONTROL Integrationen] - Benutzereinstellungen](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) in [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) Absatz 1.\
   Ein Administrator muss zunächst die Variable [!DNL Basecamp Classic] -Integration, damit Sie Ihre persönlichen Einstellungen aktivieren können. Informationen zum Einrichten der Integration finden Sie unter [Aktivieren der [!DNL Basecamp] Integration mit [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in diesem Artikel.

1. Im [!DNL Basecamp] API-Token-Feld (2) verwenden, fügen Sie das Token ein, das Sie gerade aus Ihrem [!DNL Basecamp] [!UICONTROL Meine Informationen] in das Feld (3).\
   Informationen zum Kopieren Ihrer [!DNL Basecamp] API-Token, siehe [Abrufen Ihrer [!DNL Basecamp] API-Token](#retrieving-your-basecamp-api-token) in diesem Artikel.

1. Klicken **[!UICONTROL Speichern]** 4.

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Ihre [!DNL Workfront Proof] [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) sind jetzt in Ihre [!DNL Basecamp Classic] -Konto.
