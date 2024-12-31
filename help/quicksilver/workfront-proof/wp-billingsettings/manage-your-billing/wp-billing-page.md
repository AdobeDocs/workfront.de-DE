---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: Seite  [!DNL Workfront] Abrechnung - Testversand“
description: Um auf die Seite [!UICONTROL Abrechnung] zuzugreifen, öffnen Sie das Menü Einstellungen oben rechts im Bildschirm und wählen Sie Abrechnung im Dropdown-Menü.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Die Seite „Abrechnung [!DNL Workfront Proof]&quot;

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

## Die Seite Abrechnung

Um auf die Seite [!UICONTROL Abrechnung] zuzugreifen, öffnen Sie das Menü **[!UICONTROL Einstellungen]** oben rechts im Bildschirm und wählen Sie **[!UICONTROL Abrechnung]** im Dropdown-Menü aus.

Die [!UICONTROL Abrechnung] enthält Folgendes:

* Kontoname (1)
* Kontoliste (z. B. wenn Sie über Satellitenkonten verfügen)(2)
* Plan ändern (3)
* Zahlungsdetails ändern (4)
* Neues Satellitenkonto (5)
* Konto schließen (6)
* Aktuelle Plandaten (7)
* Rechnungskontakt und Adresse (8)
* Nutzungsstatistiken (9)
* Rechnungsverlauf (10)
* Aktivität „Abrechnung“ (11)

  ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL Aktueller Plan]

Dieser Abschnitt (7) zeigt die Details Ihres aktuellen Plans, einschließlich der folgenden:

* Der Name des Plans
* Aktuelle Zahlungsmethode
* Aktuelle Start- und Endtermine des Plans
* Nächster Plantyp
* Nächste Planzahlungsmethode

  Weitere Informationen finden Sie unter [Auswählen Ihrer Zahlungsmethode in [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL Rechnungskontakt und Adresse]

In diesem Abschnitt (8) werden die wichtigsten Kontaktdaten zur Rechnungsstellung und die Adresse für Ihr Konto angezeigt.

Der Rechnungskontakt kann nur aus den Benutzern ausgewählt werden, die als Rechnungsadministratoren für Ihr Konto eingerichtet wurden. In den Satellitenkonten können in diesem Feld nur die Abrechnungsadministratoren aus dem Hauptkonto festgelegt werden.

![billing_contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> Sie können mehrere Abrechnungs-Administratoren auf Ihrem Konto haben. Nur einer von ihnen, ausgewählt im Feld [!UICONTROL Abrechnungskontakt], erhält jedoch alle Abrechnungs-Benachrichtigungen und Warnhinweise zur Kontonutzung.

Dazu gehören die folgenden Benachrichtigungs-E-Mails:

* Testversandnutzung
* Rechnungen
* herabstufen
* Warnung bei verspäteter Zahlung/Aussetzung des Kontos
* Kreditkartenfehler

  ![billin_CC.png](assets/billin-cc-350x103.png)

Das Feld [!UICONTROL Billing CC] ermöglicht auch das Hinzufügen einer E-Mail-Adresse, die in alle E-Mails mit Bezug zur Abrechnung kopiert werden soll. Klicken Sie auf das Feld, um die Inline-Bearbeitung zu aktivieren, und geben Sie eine E-Mail-Adresse Ihrer Wahl ein (dies kann auch die E-Mail-Adresse eines bestehenden Benutzers sein).

## [!UICONTROL Rechnungsadresse]

Dieser Abschnitt verwendet die Inline-Bearbeitung. Klicken Sie daher einfach auf die Felder, um den Text einzugeben bzw. zu bearbeiten.

>[!NOTE]
>
> Diese Adresse wird auf Ihren Abonnementrechnungen angegeben, damit Sie stets über die neuesten Daten verfügen.

![billing_address.png](assets/billing-address-350x199.png)

## [!UICONTROL Nutzungsstatistiken]

In diesem Abschnitt werden die Nutzungsstatistiken für Ihr Konto innerhalb des aktuellen Abrechnungszeitraums angezeigt, einschließlich der folgenden:

* Verwendeter Speicher
* Verwendete Korrekturabzüge
* Users limit used

![usage_statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL Nutzungswarnungen]

Die [[!UICONTROL Profile für Korrekturabzugsberechtigungen] in [!DNL Workfront] Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), die in Ihrem Konto als Rechnungskontakt (1) festgelegt sind, werden per E-Mail benachrichtigt, wenn Ihr Konto Folgendes erreicht:

* 75 % und dann 98 % Ihrer Speicherkapazität
* 75 % und dann 100 % Ihrer Proof-Grenze

![billing_contact__1_.png](assets/billing-contact--1--350x74.png)

Sobald die Testsendungen oder Speicherbeschränkungen erreicht sind, werden die Warnhinweise auch oben auf der Seite [!UICONTROL Abrechnung] angezeigt:

* Für Korrekturabzüge wurde das Limit erreicht

  ![Proofs_limit_reached.png](assets/proofs-limit-reached-350x65.png)

* Für das Speicherlimit erreicht

![storage_limit_reached.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>Die Anzahl der Korrekturabzüge wird verwendet, wenn Korrekturabzüge in Ihrem Konto erstellt werden, und kann nicht durch Entfernen der Korrekturabzüge wiederhergestellt werden.

Sie können Speicherplatz freigeben, indem Sie die Testsendungen und Dateien löschen und anschließend den [!UICONTROL Papierkorb] leeren.

Bitte beachten Sie, dass Sie Ihr Konto jederzeit aktualisieren können, wenn Sie weitere Korrekturabzüge, Speicher oder Benutzer benötigen. Dies tritt sofort in Kraft.

## [!UICONTROL Abrechnungsverlauf]

In diesem Abschnitt wird die Aktivität für alle aktuellen Abrechnungszeiträume angezeigt. Sie können Ihre Rechnungen auch von diesem Abschnitt herunterladen.

Weitere Informationen finden Sie unter &quot;[Herunterladen Ihrer  [!DNL Workfront Proof] -Rechnung](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md).

## [!UICONTROL Aktivität „Abrechnung“]

In diesem Abschnitt werden die jüngsten Änderungen an Ihrer Abrechnungskonfiguration angezeigt, z. B. Abonnements, Upgrades, Downgrades und Erneuerungen Ihres [!DNL Workfront Proof].

Wenn Sie Ihren Plan in einen Plan mit einem niedrigeren Benutzerlimit (1) ändern, werden Benutzer, die das neue Limit überschreiten, beim Start des neuen Plans automatisch deaktiviert. Diese Aktivität wird auch in Ihren Kontoprotokollen erfasst (2).

![billing_downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
