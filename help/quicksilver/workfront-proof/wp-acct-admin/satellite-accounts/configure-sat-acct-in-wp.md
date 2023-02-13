---
product-previous: workfront-proof
product-area: documents;system-administration;setup
navigation-topic: satellite-accounts
title: Konfigurieren Sie ein Satellitenkonto in [!DNL Workfront Proof]
description: Satellitenkonten sind gebührenpflichtige Konten, die Sie in Ihrem eigenen [!DNL Workfront] Kontonachweis. Weitere Informationen finden Sie unter "Satellitenkonten in [!DNL Workfront] Testversand.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 82c6dff3-6187-4145-951c-3f5312049b59
source-git-commit: 5be053a6ee99404673f6f3258a423ef5e5c7f431
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 1%

---

# Konfigurieren Sie ein Satellitenkonto in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Satellitenkonten sind gebührenpflichtige Konten, die Sie in Ihrem eigenen [!DNL Workfront Proof] -Konto. Weitere Informationen finden Sie unter [Satellitenkonten in [!DNL Workfront] Testversand](../../../workfront-proof/wp-acct-admin/satellite-accounts/sat-accts-in-wp.md).

Jeder Abrechnungsadministrator kann ein Satellitenkonto erstellen. Informationen zu Rechnungsadministratoren finden Sie unter [[!UICONTROL Profile für Testberechtigungen] in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
> Satellitenkonten müssen in einem unserer [!UICONTROL Standard] oder höheren Plänen.

## Erstellen eines Satellitenkontos {#creating-a-satellite-account}

So erstellen Sie ein Satellitenkonto:

1. Navigieren Sie zu [!UICONTROL Rechnungsstellung] Seite.\
   Weitere Informationen zur Rechnungsseite finden Sie unter  [Die [!DNL Workfront Proof] [!UICONTROL Rechnungsstellung] Seite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. Klicken Sie auf **[!UICONTROL Neuer Satellit]** Kontoschaltfläche. (1)

   Ein Popup-Fenster wird angezeigt.

   ![new_satellite_account.png](assets/new-satellite-account-350x156.png)

1. Geben Sie die Details Ihres Kunden ein, einschließlich aller relevanten Angebotscodes.
1. Klicken Sie auf **[!UICONTROL Speichern]**. Das Satellitenkonto wird automatisch im [!UICONTROL Konten] Dropdown-Menü oben im [!UICONTROL Rechnungsstellung] Seite.
1. Wählen Sie im Dropdown-Menü das neue Satellitenkonto aus.
1. Fahren Sie mit [Auswählen eines Plans für Ihr Satellitenkonto](#selecting-a-plan-for-your-satellite-account) , um Ihr Satellitenkonto zu aktualisieren.

## Auswählen eines Plans für Ihr Satellitenkonto {#selecting-a-plan-for-your-satellite-account}

Nachdem Sie das Satellitenkonto eingerichtet haben, wie unter [Erstellen eines Satellitenkontos](#creating-a-satellite-account)müssen Sie sie auf den gewünschten Plan aktualisieren.

1. Navigieren Sie zu [!UICONTROL Rechnungsstellung] Seite.\
   Weitere Informationen zur Rechnungsseite finden Sie unter  [Die [!DNL Workfront Proof] [!UICONTROL Rechnungsstellung] Seite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

1. Im **[!UICONTROL Ihre Konten]** Wählen Sie oben auf der Seite (1) das entsprechende Satellitenkonto aus.

   Die Abrechnungsseite für das Satellite-Konto wird angezeigt und die Abrechnungs-Kontaktdaten aus Ihrem Konto werden automatisch repliziert.

   ![satellite_account_change_plan.png](assets/satellite-account-change-plan-350x156.png)

1. Klicken Sie auf **[!UICONTROL Plan ändern]** rechts oben auf der Seite. (2)\
   Oder\
   Öffnen Sie das Popup-Fenster, indem Sie auf Ihren aktuellen oder nächsten Planungsnamen klicken. (3)

1. Upgrade oder Downgrade Ihres Plans.

## Hinzufügen von Benutzern zu Ihrem Satelliten-Konto

Nachdem Sie das Satellitenkonto auf Ihren ausgewählten Plan aktualisiert haben, müssen Sie Benutzer zum Konto hinzufügen.

1. Anmelden bei [!DNL Workfront Proof] als [!DNL Workfront Proof] Administrator.
1. Klicken **[!UICONTROL Kontoeinstellungen]**.
1. Wählen Sie im Dropdown-Menü oben auf der Seite das entsprechende Satellitenkonto aus. (1)\
   Die Seite mit den Kontoeinstellungen für das Satellitenkonto wird angezeigt.
1. Klicken Sie auf **[!UICONTROL Neuer Benutzer]** rechts oben auf der Seite. (2)\
   Die [!DNL New User] angezeigt.

1. Geben Sie die Details des Benutzers ein und klicken Sie auf **[!UICONTROL Speichern]**.\
   Der Benutzer erhält eine E-Mail-Benachrichtigung, über die er Zugriff auf das Konto erhält.

Benutzer, die zum Satellitenkonto hinzugefügt wurden, erscheinen als Mitglieder in der Kontaktliste des Hub-Kontos.

Ebenso erscheinen Benutzer im Hub-Konto als Mitglieder in den Kontakten des Satelliten-Kontos.

Um eine vollständige Liste aller Benutzer im Satellitenkonto anzuzeigen, klicken Sie auf die Schaltfläche **[!UICONTROL Benutzer]** Registerkarte.

![SA_New_User.png](assets/sa-new-user-350x156.png)

## Verknüpfen vorhandener separater Konten mit Ihrem Hub-Konto

Wenn Sie zuvor andere separate Konten für Ihre Kunden erstellt haben, können diese in Satellitenkonten umgewandelt werden.

Wir kümmern uns darum für Sie, indem wir sie mit Ihrer [!DNL Workfront Proof] -Konto (dies ist ein Hub-Konto).

Sie müssen uns lediglich die folgenden Informationen zur Verfügung stellen:

* Der Name Ihres [!DNL Workfront Proof] Konto und die E-Mail-Adresse, die Sie für die Einrichtung verwendet haben
* Die Namen der einzelnen Konten, die mit Ihrem Konto verknüpft werden sollen, und die E-Mail-Adressen, die zum Einrichten der separaten Konten verwendet werden.
