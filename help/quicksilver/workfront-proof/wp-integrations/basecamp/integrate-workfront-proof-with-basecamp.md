---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrieren von [!DNL Workfront Proof] mit [!DNL Basecamp]
description: Wenn Sie [!DNL Basecamp] für das Projektmanagement verwenden, können Sie Ihrem Projektteam mithilfe von [!DNL Workfront Proof] umfassendere Prüfungs- und Validierungstools anbieten.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Integrieren von [!DNL Workfront Proof] mit [!DNL Basecamp]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie [!DNL Basecamp] für das Projektmanagement verwenden, können Sie Ihrem Projektteam umfassendere Prüfungs- und Validierungstools mit [!DNL Workfront Proof] anbieten.

## Die [!DNL Basecamp]-Integration mit [!DNL Workfront]

Durch die Integration mit [!DNL Basecamp] können Benutzer Testsendungen innerhalb von [!DNL Basecamp] anzeigen, überprüfen und genehmigen. Benutzer können Testsendungen an Ihr [!DNL Workfront Proof]-Konto senden und sie mit Ihrem [!DNL Basecamp] -Projekt verbinden. Ihre Validierer können mit [!DNL Basecamp] Kommentare abgeben und Entscheidungen treffen, indem sie den in Ihre Basecamp-Nachricht eingebetteten Mini-Testversand verwenden.

Wenn es mit [!DNL Workfront Proof] integriert ist, verfügt [!DNL Basecamp] über die folgende Testfunktion:

* Benutzer können Testsendungen innerhalb von [!DNL Basecamp Classic] überprüfen und genehmigen.
* Benutzer haben Überprüfungs-Tools sofort verfügbar.
* Projektprüfungsteams erhalten eine Nachricht in [!DNL Basecamp] mit einem kleinen Testversand zur Überprüfung und Genehmigung.
* Benutzer können zur Überprüfung und Genehmigung zu einem ganzseitigen Testversand wechseln.
* Benutzer können sowohl Mini- als auch Vollbildsendungen Kommentare und Markups hinzufügen.

  >[!NOTE]
  >
  >Nachdem ein Kommentar beantwortet wurde, kann er nicht mehr bearbeitet oder gelöscht werden.

* Überprüfer können auf die Markierungen und reagieren, die von anderen Validierern vorgenommen wurden.
* Benutzer werden benachrichtigt, wenn eine neue Testversion verfügbar ist.
* Benutzer, die keine [!DNL Workfront Proof] -Benutzer sind, können in [!DNL Basecamp] an einem Testversand arbeiten.

Die Integration von [!DNL Workfront Proof] mit [!DNL Basecamp] muss auf zwei Ebenen eingerichtet werden:

* Konfigurieren Sie [!DNL Basecamp] in den [Kontoeinstellungen:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Dies aktiviert die Basecamp-Integration für Ihre gesamte Organisation. Weitere Informationen finden Sie unter [Aktivieren der Basecamp-Integration mit  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Konfigurieren Sie [!DNL Basecamp] in [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Dadurch können Ersteller und Inhaber von Testsendungen eine Verbindung zu ihrem persönlichen Basecamp-Konto herstellen und den Zugriff auf [!DNL Workfront Proof] genehmigen. Weitere Informationen finden Sie unter [Konfigurieren der persönlichen Einstellungen](#configuring-personal-settings).

Sie können [!DNL Workfront] entweder mit [!DNL Basecamp] oder mit [!DNL Basecamp Classic] integrieren. Jede Version von [!DNL Basecamp] verwendet eine andere API und erfordert daher unterschiedliche Konfigurationsverfahren.

Informationen zum Konfigurieren von [!DNL Basecamp Classic] finden Sie unter [Integrieren [!DNL Workfront Proof] mit [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Aktivieren der [!DNL Basecamp]-Integration mit [!DNL Workfront Proof]

Als [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) oder [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) können Sie die [!DNL Basecamp] -Integration für das gesamte Konto in Ihren [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) einrichten.

1. Erfassen Sie in [!UICONTROL Basecamp] die folgenden Informationen:

   * Die URL für Ihr [!DNL Basecamp]-Konto
   * Die URL im Abschnitt &quot;[!UICONTROL My info]&quot;

1. Melden Sie sich von [!DNL Basecamp] ab.
1. Klicken Sie oben rechts auf **[!UICONTROL Kontoeinstellungen]** .
1. Klicken Sie auf die Registerkarte **[!UICONTROL Integrationen]**.
1. Klicken Sie im Abschnitt **[!UICONTROL [!DNL Basecamp]]** rechts neben **[!UICONTROL [!DNL Basecamp]integration]** auf **[!UICONTROL Enable]**.

1. Überprüfen Sie neben **[!UICONTROL [!DNL Basecamp]version]**, ob die **[!UICONTROL klassische Version]** die Version ist, in die Sie integrieren.

1. (Bedingt) Wenn keine [!DNL Basecamp]-URL angezeigt wird, klicken Sie auf **[!UICONTROL Bearbeiten]**, geben Sie die URL für Ihr [!DNL Basecamp]-Konto ein, ohne &quot;http://&quot;einzuschließen, und klicken Sie dann auf **[!UICONTROL Speichern]**.

1. Klicken Sie in der oberen rechten Ecke des Fensters auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Persönliche Einstellungen]**.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Integrationen]**.
1. Klicken Sie unter &quot;**[!DNL Basecamp]**&quot;rechts neben &quot;**[!UICONTROL Basecamp integration]**&quot;auf &quot;**[!UICONTROL Enable]**&quot;.

1. Klicken Sie in den angezeigten Optionen rechts neben **[!UICONTROL [!DNL Basecamp]API-Token]** auf **[!UICONTROL Bearbeiten]**.

1. Geben Sie in das Feld, das angezeigt wird, die URL im Abschnitt &quot;[!UICONTROL My info]&quot; in [!DNL Basecamp] ein und klicken Sie dann auf **[!UICONTROL Save]**.\
   Nachdem Sie [!DNL Workfront Proof] mit [!DNL Basecamp] integriert haben, können Ihre Benutzer ihre persönlichen Einstellungen konfigurieren. Informationen zum Einrichten von persönlichen Einstellungen finden Sie unter [Persönliche Einstellungen konfigurieren](#configuring-personal-settings) .

1. Wenn Sie die [!DNL Basecamp] -Integration nicht aktivieren können, ist Ihre [!DNL Workfront Proof] -Konto-ID möglicherweise nicht mit der Konto-ID identisch, die Sie in [!DNL Basecamp] verwenden.
1. Nachdem Sie [!DNL Workfront Proof] mit [!DNL Basecamp] integriert haben, können Ihre Benutzer ihre persönlichen Einstellungen konfigurieren. Informationen zum Einrichten von persönlichen Einstellungen finden Sie unter [Konfigurieren von persönlichen Einstellungen](#configuring-personal-settings).

## Persönliche Einstellungen konfigurieren

Nachdem Sie [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) für Ihre Organisation eingerichtet haben, sollte jeder Autor, der Testsendungen erstellt/sendet, seine [persönlichen Einstellungen festlegen.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Navigieren Sie zu **[!UICONTROL Persönlich** &#x200B;**Einstellungen]**.

1. Öffnen Sie die Registerkarte **[!UICONTROL Integrationen]** (1).
1. Um die Integration von [!DNL Basecamp] zu aktivieren, klicken Sie auf **[!UICONTROL Aktivieren]** (2).
1. Klicken Sie auf **[!UICONTROL Verbindung zu Ihrem [!DNL Basecamp] Konto herstellen]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Melden Sie sich bei Ihrem [!DNL Basecamp] -Konto (1) an.\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Klicken Sie auf **[!UICONTROL Ja, ich lasse den Zugriff auf]** zu, um [!DNL Workfront Proof] Zugriff auf Ihr Konto zu erlauben (2).\
   ![basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Optional) Wenn Ihre persönliche Integration aktiv ist (3), können Sie einfach zwischen Ihren [!DNL Basecamp]-Konten wechseln.

   1. Klicken Sie auf **[!UICONTROL Switch [!DNL Basecamp] account]** (4).\

      ![Basecamp_switch_accounts_1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      Mit dem [!UICONTROL Basecamp-Konto wechseln] gelangen Sie zur Seite [!UICONTROL Persönliche Einstellungen] , auf der Sie auswählen können, welche Ihrer [!DNL Basecamp]-Konten Sie in Ihr [!DNL Workfront Proof]-Konto integrieren möchten.

   1. Klicken Sie auf **[!UICONTROL Erneutes Integrieren mit[!DNL Basecamp]]** (5), bevor Sie das [!DNL Basecamp]-Konto auswählen\

      Dadurch wird die Seite [!UICONTROL Persönliche Einstellungen] aktualisiert und Ihre aktuellste Liste der [!DNL Basecamp]-Konten wird angezeigt.

   1. Klicken Sie auf **[!UICONTROL Mit diesem Konto integrieren]** , um es mit [!DNL Workfront Proof] zu verbinden.\

      ![Basecamp_switch_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Sie können jetzt Testsendungen zu [!DNL Basecamp] -Projekten hinzufügen.
