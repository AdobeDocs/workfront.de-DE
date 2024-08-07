---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: Die Seite [!DNL Workfront] Testversand der Rechnungsstellung
description: Um auf die Seite [!UICONTROL Rechnungsstellung] zuzugreifen, öffnen Sie das Menü Einstellungen oben rechts im Bildschirm und wählen Sie im Dropdown-Menü die Option Rechnungsstellung .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Die Abrechnungsseite [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

## Die Rechnungsseite

Um auf die Seite [!UICONTROL Rechnungsstellung] zuzugreifen, öffnen Sie das Menü **[!UICONTROL Einstellungen]** oben rechts im Bildschirm und wählen Sie **[!UICONTROL Rechnungsstellung]** im Dropdown-Menü aus.

Die Seite [!UICONTROL Rechnungsstellung] enthält Folgendes:

* Kontoname (1)
* Kontoliste (z. B. wenn Sie über Satellitenkonten verfügen)(2)
* Änderungsplan (3)
* Zahlungsdetails ändern (4)
* Neues Satellitenkonto (5)
* Konto schließen (6)
* Aktuelle Planinformationen (7)
* Rechnungskontakte und -adresse (8)
* Nutzungsstatistiken (9)
* Rechnungsverlauf (10)
* Rechnungsstellung (11)

  ![billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL Aktueller Plan]

In diesem Abschnitt (7) werden die Details Ihres aktuellen Plans angezeigt, einschließlich der folgenden:

* Name des Plans
* Aktuelle Zahlungsmethode
* Start- und Enddatum des aktuellen Plans
* Nächster Planungstyp
* Nächste Planzahlungsmethode

  Weitere Informationen finden Sie unter [Auswählen Ihrer Zahlungsmethode in [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL Rechnungskontakt und -adresse]

In diesem Abschnitt (8) werden die wichtigsten Rechnungskontakte und Adressdaten für Ihr Konto angezeigt.

Der Abrechnungskontakt kann nur von den Benutzern ausgewählt werden, die in Ihrem Konto als Rechnungsadministratoren eingerichtet sind. In den Satellitenkonten können nur die Rechnungsadministratoren aus dem Hauptkonto in dieses Feld eingestellt werden.

![billing_contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> Sie können mehrere Rechnungsadministratoren für Ihr Konto haben, aber nur einer von ihnen, der im Feld [!UICONTROL Rechnungskontakt] ausgewählt ist, erhält alle Abrechnungsbenachrichtigungen und Kontoverwendungswarnungen.

Dazu gehören die folgenden Benachrichtigungs-E-Mails:

* Nutzung des Testversands
* Rechnungen
* Downgrade
* Warnhinweis zur verspäteten Auszahlung/Kontoaussetzung
* Kreditkartenfehler

  ![Billin_CC.png](assets/billin-cc-350x103.png)

Im Feld [!UICONTROL Rechnungsstellung CC] können Sie auch eine E-Mail-Adresse hinzufügen, die in alle E-Mails kopiert werden soll, die mit der Rechnungsstellung in Verbindung stehen. Klicken Sie auf das Feld, um die Zeilenbearbeitung zu aktivieren, und geben Sie eine E-Mail-Adresse Ihrer Wahl ein (dies kann auch die E-Mail-Adresse eines vorhandenen Benutzers sein).

## [!UICONTROL Abrechnungsadresse]

In diesem Abschnitt wird die Inline-Bearbeitung verwendet. Klicken Sie einfach auf die Felder, um den Text einzugeben/zu bearbeiten.

>[!NOTE]
>
> Diese Adresse wird auf Ihren Abonnementrechnungen angegeben. Stellen Sie also sicher, dass diese Daten stets auf dem neuesten Stand sind.

![billing_address.png](assets/billing-address-350x199.png)

## [!UICONTROL Nutzungsstatistiken]

Dieser Abschnitt enthält die Nutzungsstatistiken für Ihr Konto innerhalb des aktuellen Abrechnungszeitraums, einschließlich der folgenden:

* Verwendeter Speicher
* Verwendete Testsendungen
* Verwendete Benutzerbegrenzung

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL Nutzungswarnungen]

Die [[!UICONTROL Testversand-Berechtigungsprofile] in  [!DNL Workfront] Testversand](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), die als Abrechnungskontakt (1) für Ihr Konto festgelegt sind, werden per E-Mail benachrichtigt, wenn Ihr Konto Folgendes erreicht:

* 75 % und dann 98 % Ihrer Speicherkapazität
* 75 % und dann 100 % Ihres Testversands

![billing_contact_1_.png](assets/billing-contact--1--350x74.png)

Sobald die Testsendungen oder Speichergrenzen erreicht sind, sehen Sie auch die Warnhinweise oben auf der Seite [!UICONTROL Rechnungsstellung]:

* Für erreichte Testversandgrenze

  ![Testsendungen_Limit_Reichweite.png](assets/proofs-limit-reached-350x65.png)

* Für die erreichte Speicherbegrenzung

![Storage_limit_received.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>Ihre Testversandanzahl wird bei der Erstellung von Testsendungen in Ihrem Konto verwendet und kann nicht durch Entfernen der Testsendungen wiederhergestellt werden.

Speicherplatz kann durch Löschen der Testsendungen und Dateien und anschließendes Leeren des [!UICONTROL Papierkorb] freigesetzt werden.

Beachten Sie bitte, dass Sie, wenn Sie mehr Testsendungen, Speicher oder Benutzer benötigen, Ihr Konto jederzeit aktualisieren können und es sofort wirksam wird.

## [!UICONTROL Rechnungsverlauf]

Dieser Abschnitt zeigt die Aktivitäten für die letzten Abrechnungszeiträume. Sie können Ihre Rechnungen auch von diesem Abschnitt herunterladen.

Weitere Informationen finden Sie unter &quot;[Herunterladen Ihrer [!DNL Workfront Proof] Rechnung](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md)&quot;.

## [!UICONTROL Abrechnungsaktivität]

In diesem Abschnitt werden die letzten Änderungen an Ihrer Abrechnungseinrichtung angezeigt, z. B. Abonnements, Upgrades, Downgrade und Verlängerungen Ihres [!DNL Workfront Proof]-Plans.

Wenn Sie Ihren Plan auf einen Plan mit einem niedrigeren Benutzerlimit (1) ändern, werden Benutzer, die die neue Grenze überschreiten, automatisch deaktiviert, wenn der neue Plan beginnt. Diese Aktivität wird auch in Ihren Kontoprotokollen (2) erfasst.

![billing_downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
