---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integration  [!DNL Workfront Proof]  Basecamp Classic
description: Wenn Sie für  [!DNL Basecamp]  Projektmanagement verwenden, können Sie Ihrem Projektteam umfangreichere Überprüfungs- und Genehmigungs-Tools anbieten, indem Sie Folgendes verwenden [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Integrieren von [!DNL Workfront Proof] mit [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie [!DNL Basecamp] für das Projekt-Management verwenden, können Sie Ihrem Projekt-Team umfassendere Überprüfungs- und Genehmigungs-Tools mit [!DNL Workfront Proof] anbieten.

## Grundlegendes zur [!DNL Basecamp] Integration mit [!DNL Workfront]

Durch die Integration mit [!DNL Basecamp] können Benutzer Korrekturabzüge in [!DNL Basecamp] anzeigen, überprüfen und genehmigen. Benutzer können Testsendungen an Ihr [!DNL Workfront Proof]-Konto senden und sie mit Ihrem [!DNL Basecamp] Projekt verbinden. Ihre Validierungsverantwortlichen können [Entscheidung über einen Korrekturabzug im Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) über [!DNL Basecamp] treffen, indem sie den in Ihrer Basecamp-Nachricht eingebetteten Minikorrekturabzug verwenden.

Bei der Integration mit [!DNL Workfront Proof] können Benutzende [!DNL Basecamp] mit -Korrekturabzügen Folgendes durchführen:

* Benutzer können Korrekturabzüge in [!DNL Basecamp Classic] überprüfen und genehmigen.
* Die Benutzer verfügen über Prüfwerkzeuge, die jederzeit verfügbar sind.
* Projektüberprüfungs-Teams erhalten eine Nachricht in [!DNL Basecamp] mit einem Mini-Korrekturabzug zur Überprüfung und Genehmigung.
* Benutzer können zur Überprüfung und Genehmigung zu einem ganzseitigen Korrekturabzug wechseln.
* Benutzende können sowohl zu kleinen als auch zu großen Korrekturabzügen Kommentare und Markierungen hinzufügen.

  >[!NOTE]
  >
  >Nachdem ein Kommentar beantwortet wurde, kann er nicht mehr bearbeitet oder gelöscht werden.

* Reviewer können auf die von anderen Reviewern vorgenommenen Korrekturabzüge und Markierungen reagieren.
* Benutzer werden benachrichtigt, wenn eine neue Version des Korrekturabzugs verfügbar ist.
* Benutzende, die keine [!DNL Workfront Proof] sind, können in [!DNL Basecamp] an einem Korrekturabzug arbeiten.

Die Integration von [!DNL Workfront Proof] mit [!DNL Basecamp] muss auf zwei Ebenen erfolgen:

* Konfigurieren Sie [!DNL Basecamp] in [Kontoeinstellungen:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Dadurch wird die Basecamp-Integration für Ihre gesamte Organisation aktiviert.
* Weitere Informationen finden Sie unter [Aktivieren der  [!DNL Basecamp] -Integration mit [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Konfigurieren von [!DNL Basecamp] in [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Dadurch können Ersteller von Korrekturabzügen und Besitzer von Korrekturabzügen eine Verbindung zu ihrem persönlichen [!DNL Basecamp] herstellen und [!DNL Workfront Proof] Zugriff autorisieren. Weitere Informationen finden Sie unter [Persönliche Einstellungen konfigurieren](#configuring-personal-settings).

Sie können [!DNL Workfront] entweder mit [!DNL Basecamp] oder [!DNL Basecamp Classic] integrieren. Jede Version von [!DNL Basecamp] verwendet eine andere API und erfordert daher unterschiedliche Konfigurationsverfahren.

Informationen zum Konfigurieren von [!DNL Basecamp Classic] finden Sie unter [Aktivieren  [!DNL Basecamp]  Integration mit [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in diesem Artikel.

Informationen zum Konfigurieren von [!DNL Basecamp] finden Sie unter [Integrieren [!DNL Workfront Proof] mit [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Aktivieren der [!DNL Basecamp] Integration mit [!DNL Workfront Proof]

Als [Profile für Korrekturabzugsberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) oder [Profile für Korrekturabzugsberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) können Sie die Basecamp-Integration für das gesamte Konto in Ihren [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) einrichten.

1. Navigieren Sie zu [Kontoeinstellungen.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Öffnen Sie die **[!UICONTROL Integrationen]** (1).
1. Um die Basecamp-Integration zu aktivieren, klicken Sie auf **[!UICONTROL Aktivieren]** (2).
1. Stellen Sie sicher, dass [!DNL Basecamp Classic] die Version ist, mit der Sie integrieren (3).
1. (Bedingt) Wenn keine [!DNL Basecamp] URL angezeigt wird (4), klicken Sie auf **[!UICONTROL Bearbeiten]** und geben Sie die URL für Ihr [!DNL Basecamp] Konto ein (ohne http://).
1. Klicken Sie **[!UICONTROL Speichern]** (5).\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Optional) Überprüfen Sie Ihre [!DNL Basecamp]-URL in Ihrem Browser, nachdem Sie sich bei Ihrem [!DNL Basecamp Classic]-Konto angemeldet haben (6).

   ![basecamp_URL.png](assets/basecamp-url-350x75.png)

   Sobald Sie [!DNL Workfront Proof] mit [!DNL Basecamp] integrieren, können Ihre Benutzerinnen und Benutzer ihre persönlichen Einstellungen konfigurieren. Informationen zum Einrichten persönlicher Einstellungen finden Sie unter [Persönliche Einstellungen konfigurieren](#configuring-personal-settings).

   Wenn Sie [!DNL Basecamp] Integration nicht aktivieren können, ist Ihre [!DNL Workfront Proof]-Konto-ID möglicherweise nicht mit der in [!DNL Basecamp] verwendeten Konto-ID identisch.

## Persönliche Einstellungen konfigurieren

Nachdem Sie [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) für Ihre Organisation eingerichtet haben, sollten alle Ihre Autoren, die Korrekturabzüge erstellen/senden, ihre [persönlichen Einstellungen“](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Diese Schritte sind am einfachsten durchzuführen, wenn Sie Ihre [!DNL Basecamp] Sitzung in einem Browser-Fenster und Ihre [!DNL Workfront Proof] in einem anderen Fenster geöffnet haben.

* [Abrufen Ihres  [!DNL Basecamp] -API-Tokens](#retrieving-your-basecamp-api-token)
* [Hinzufügen Ihres  [!DNL Basecamp] -API-Tokens zu Ihren persönlichen Einstellungen](#adding-your-basecamp-api-token-to-your-personal-settings)

### Abrufen Ihres [!DNL Basecamp] API-Tokens

Um die Integration auf individueller Ebene in [!DNL Workfront Proof] abzuschließen, benötigen Benutzerinnen und Benutzer ihr individuelles Authentifizierungstoken für die [!DNL Basecamp]-API.

So rufen Sie Ihr [!DNL Basecamp]-API-Token ab:

1. Melden Sie sich bei Ihrem [!DNL Basecamp] Konto an.
1. Klicken Sie **[!UICONTROL Meine Info]** (1) in der oberen rechten Ecke des Bildschirms.\
   Die Seite [!UICONTROL Meine Info] wird angezeigt.\
   ![basecamp_integration_-_token1.png](assets/basecamp-integration---token1-350x334.png)

1. Klicken Sie im Abschnitt [!UICONTROL Authentifizierungstoken] auf **[!UICONTROL Token anzeigen]** (2), um Ihre persönlichen Authentifizierungstoken anzuzeigen.
1. Wählen Sie das **[!UICONTROL Token für Feed]** Leser oder die **[!UICONTROL Basecamp-API]** (3) aus und kopieren Sie dann das Token in die Zwischenablage.

1. Fügen Sie Ihr [!DNL Basecamp]-API-Token in das Feld [!UICONTROL Token für Feed]Leser oder die [!UICONTROL Basecamp-API] ein.\
   ![basecamp_integration_-_token2.png](assets/basecamp-integration---token2-350x178.png)

### Hinzufügen Ihres [!DNL Basecamp]-API-Tokens zu Ihren persönlichen Einstellungen

So fügen Sie das [!DNL Basecamp]-API-Token in Ihre [!DNL Workfront Proof] ein [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Navigieren Sie zu [[!UICONTROL Integrationen] - Benutzereinstellungen](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) in Ihren [Persönlichen Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1).\
   Ein Administrator muss zunächst die [!DNL Basecamp Classic] aktivieren, damit Sie Ihre persönlichen Einstellungen aktivieren können. Weitere Informationen zum Einrichten der Integration finden Sie unter [Aktivieren  [!DNL Basecamp]  Integration mit [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in diesem Artikel.

1. Fügen Sie im Feld [!DNL Basecamp]-API-Token (2) das Token, das Sie soeben von Ihrer [!DNL Basecamp] Seite [!UICONTROL Meine &#x200B;]) kopiert haben, in das Feld ein (3).\
   Informationen zum Kopieren Ihres [!DNL Basecamp]-API-Tokens finden Sie unter [Abrufen Ihres  [!DNL Basecamp] -API-](#retrieving-your-basecamp-api-token)) in diesem Artikel.

1. Klicken Sie **[!UICONTROL Speichern]** (4).

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Ihre [!DNL Workfront Proof] [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) sind jetzt in Ihr [!DNL Basecamp Classic]-Konto integriert.
