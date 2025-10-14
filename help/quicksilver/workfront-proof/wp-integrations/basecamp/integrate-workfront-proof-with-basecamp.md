---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrieren  [!DNL Workfront Proof] mit [!DNL Basecamp]
description: Wenn Sie für  [!DNL Basecamp]  Projektmanagement verwenden, können Sie Ihrem Projektteam umfangreichere Überprüfungs- und Genehmigungs-Tools anbieten, indem Sie Folgendes verwenden [!DNL Workfront Proof].
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
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie [!DNL Basecamp] für das Projekt-Management verwenden, können Sie Ihrem Projekt-Team umfassendere Überprüfungs- und Genehmigungs-Tools mit [!DNL Workfront Proof] anbieten.

## Grundlegendes zur [!DNL Basecamp] Integration mit [!DNL Workfront]

Durch die Integration mit [!DNL Basecamp] können Benutzer Korrekturabzüge in [!DNL Basecamp] anzeigen, überprüfen und genehmigen. Benutzer können Testsendungen an Ihr [!DNL Workfront Proof]-Konto senden und sie mit Ihrem [!DNL Basecamp] Projekt verbinden. Ihre Validierungsverantwortlichen können mit dem in Ihrer Basecamp-Nachricht eingebetteten Mini-Korrekturabzug Kommentare eingeben und Entscheidungen über [!DNL Basecamp] treffen.

Bei der Integration mit [!DNL Workfront Proof] verfügt [!DNL Basecamp] über die folgenden Proofing-Funktionen:

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

* Konfigurieren Sie [!DNL Basecamp] in [Kontoeinstellungen:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Dadurch wird die Basecamp-Integration für Ihre gesamte Organisation aktiviert. Weitere Informationen finden Sie unter [Aktivieren der Basecamp-Integration mit [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Konfigurieren Sie [!DNL Basecamp] in [Persönliche Einstellungen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Dies ermöglicht es Erstellern von Korrekturabzügen und Inhabern von Korrekturabzügen, eine Verbindung zu ihrem persönlichen Basecamp-Konto herzustellen und [!DNL Workfront Proof] Zugriff zu autorisieren. Weitere Informationen finden Sie unter [Persönliche Einstellungen konfigurieren](#configuring-personal-settings).

Sie können [!DNL Workfront] entweder mit [!DNL Basecamp] oder [!DNL Basecamp Classic] integrieren. Jede Version von [!DNL Basecamp] verwendet eine andere API und erfordert daher unterschiedliche Konfigurationsverfahren.

Informationen zum Konfigurieren von [!DNL Basecamp Classic] finden Sie unter [Integrieren [!DNL Workfront Proof] mit [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Aktivieren der [!DNL Basecamp] Integration mit [!DNL Workfront Proof]

Als [Profile mit Korrekturabzugsberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) oder [Profile mit Korrekturabzugsberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) können Sie die [!DNL Basecamp] Integration für das gesamte Konto in Ihren [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Sammeln [!UICONTROL &#x200B; in &quot;]&quot; die folgenden Informationen:

   * Die URL für Ihr [!DNL Basecamp]
   * Die URL im Abschnitt &quot;[!UICONTROL &#x200B; Informationen]

1. Melden Sie sich von [!DNL Basecamp] ab.
1. Klicken Sie **[!UICONTROL oben]** auf „Kontoeinstellungen“.
1. Klicken Sie auf die **[!UICONTROL Integrationen]**.
1. Klicken Sie im Abschnitt **[!UICONTROL [!DNL Basecamp]]** rechts neben **[!UICONTROL [!DNL Basecamp]Integration]** auf **[!UICONTROL Aktivieren]**.

1. Überprüfen Sie neben **[!UICONTROL [!DNL Basecamp]Version]** ob die **[!UICONTROL Classic-Version]** die Version ist, mit der Sie integrieren.

1. (Bedingt) Wenn keine [!DNL Basecamp] URL angezeigt wird, klicken Sie auf **[!UICONTROL Bearbeiten]**, geben Sie die URL für Ihr [!DNL Basecamp]-Konto ein, ohne &quot;http://&quot; einzuschließen, und klicken Sie dann auf **[!UICONTROL Speichern]**.

1. Klicken Sie in der rechten oberen Ecke des Fensters auf **[!UICONTROL Einstellungen]** > &quot;**[!UICONTROL Einstellungen]**.

1. Klicken Sie auf die **[!UICONTROL Integrationen]**.
1. Klicken Sie unter **[!DNL Basecamp]** rechts neben **[!UICONTROL Basecamp-]** auf **[!UICONTROL Aktivieren]**.

1. Klicken Sie in den angezeigten Optionen rechts neben **[!UICONTROL [!DNL Basecamp]API-]** auf **[!UICONTROL Bearbeiten]**.

1. Geben Sie in das sich öffnende Feld die URL im Abschnitt &quot;[!UICONTROL Meine &#x200B;]&quot; in [!DNL Basecamp] ein und klicken Sie auf **[!UICONTROL Speichern]**.\
   Sobald Sie [!DNL Workfront Proof] mit [!DNL Basecamp] integrieren, können Ihre Benutzerinnen und Benutzer ihre persönlichen Einstellungen konfigurieren. Informationen zum Einrichten persönlicher Einstellungen finden Sie unter [Persönliche Einstellungen konfigurieren](#configuring-personal-settings)

1. Wenn Sie [!DNL Basecamp] Integration nicht aktivieren können, ist Ihre [!DNL Workfront Proof]-Konto-ID möglicherweise nicht mit der in [!DNL Basecamp] verwendeten Konto-ID identisch.
1. Sobald Sie [!DNL Workfront Proof] mit [!DNL Basecamp] integrieren, können Ihre Benutzerinnen und Benutzer ihre persönlichen Einstellungen konfigurieren. Informationen zum Einrichten persönlicher Einstellungen finden Sie unter [Persönliche Einstellungen konfigurieren](#configuring-personal-settings).

## Persönliche Einstellungen konfigurieren

Nachdem Sie [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) für Ihre Organisation eingerichtet haben, sollte jeder Ihrer Autoren, der Korrekturabzüge erstellt/sendet, seine [persönlichen Einstellungen festlegen.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Navigieren Sie zu **[!UICONTROL Personal**&#x200B;**settings]**.

1. Öffnen Sie die **[!UICONTROL Integrationen]** (1).
1. Um die [!DNL Basecamp] zu aktivieren, klicken Sie auf **[!UICONTROL Aktivieren]** (2).
1. Klicken Sie **[!UICONTROL Verbindung zu Ihrem [!DNL Basecamp] Konto herstellen]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Melden Sie sich bei Ihrem [!DNL Basecamp] Konto an (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Klicken Sie **[!UICONTROL Ja, ich gewähre Zugriff]**, um [!DNL Workfront Proof] Zugriff auf Ihr Konto zu autorisieren (2).\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Optional) Wenn Ihre persönliche Integration aktiv ist (3), können Sie einfach zwischen Ihren [!DNL Basecamp] wechseln.

   1. Klicken Sie **[!UICONTROL [!DNL Basecamp] Konto wechseln]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      Mit [!UICONTROL Basecamp-Konto wechseln] gelangen Sie zur Seite [!UICONTROL Persönliche Einstellungen], auf der Sie auswählen können, welches Ihrer [!DNL Basecamp]-Konten Sie in Ihr [!DNL Workfront Proof]-Konto integrieren möchten.

   1. Klicken Sie **[!UICONTROL Erneut mit[!DNL Basecamp]]** integrieren (5), bevor Sie das [!DNL Basecamp] auswählen\

      Dadurch wird die Seite [!UICONTROL Persönliche Einstellungen] aktualisiert und Ihre aktuellste Liste [!DNL Basecamp] Konten angezeigt.

   1. Klicken Sie auf **[!UICONTROL Mit diesem Konto integrieren]**, um es mit [!DNL Workfront Proof] zu verbinden.\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Sie können jetzt Testsendungen zu [!DNL Basecamp] Projekten hinzufügen.
