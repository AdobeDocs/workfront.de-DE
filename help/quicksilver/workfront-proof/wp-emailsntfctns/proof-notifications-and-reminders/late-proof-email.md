---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Verspätete Testversand-E-Mail
description: Die E-Mail zum verspäteten Testversand wird den Empfängern zugestellt, wenn ein Testversand kurz vor Ablauf der Frist oder bis zum Ablauf der Frist liegt. Diese Arten von E-Mails können nicht auf Testversandebene deaktiviert werden, sind jedoch auf Konto- und Benutzerebene konfigurierbar.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 23eb75a7-d7b7-4043-afba-cf45c86ab1ae
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# [!UICONTROL Verspäteter Testversand] email

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Die [!UICONTROL Verspäteter Testversand] E-Mails werden an Empfänger gesendet, wenn ein Testversand kurz vor dem Termin oder dem Ablauf der Frist steht. Diese Arten von E-Mails können nicht auf Testversandebene deaktiviert werden, sind jedoch auf Konto- und Benutzerebene konfigurierbar.

* [!UICONTROL Verspäteter Testversand] E-Mails werden automatisch an die validierungsverantwortlichen Benutzer gesendet, wenn ein Testversand seine Frist erreicht und nicht alle Überprüfungen oder Entscheidungen getroffen wurden.

   Diese E-Mails sind standardmäßig aktiviert und können nicht für alle Konten angepasst werden. Benutzer können sie jedoch in ihren Testversandeinstellungen deaktivieren.

* Eventuelle E-Mails werden den Validierungsverantwortlichen gesendet, wenn ein Testversand nahe der Frist liegt. Sie sind standardmäßig deaktiviert und können im [!UICONTROL Kontoeinstellungen]. Nach der Aktivierung können sie auch im [!UICONTROL Standardeinstellungen für die Prüfung].

Diese Benachrichtigungen können nicht angepasst werden.

Folgende Personen werden benachrichtigt:

* Der Inhaber, nur wenn [!UICONTROL Email] Warnhinweis bei verspäteten Testsendungen wird im Abschnitt [!UICONTROL Standardeinstellungen für die Testversandliste des Eigentümers].
* Jeder Genehmiger, der sich noch nicht zum Testversand entschieden hat. Informationen zu Entscheidungen finden Sie unter [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)

>[!NOTE]
>
>Wenn E-Mail-Benachrichtigungen standardmäßig deaktiviert sind, finden Sie unter [!UICONTROL Kontoeinstellungen], nein [!UICONTROL Verspäteter Testversand] E-Mails werden auch dann gesendet, wenn die validierungsverantwortlichen Benutzer und validierungsverantwortlichen Benutzer ihre Kommentare und Entscheidungen noch nicht übermittelt haben. Sie können auch [!UICONTROL Verspäteter Testversand] E-Mails in den Testversandstandardeinstellungen.

Beachten Sie Folgendes zu Testversandbenachrichtigungen:

* Ihre [!DNL Workfront] Administrator oder [!DNL Workfront Proof] Administratoren können das Logo Ihres Unternehmens in E-Mail-Benachrichtigungen einbeziehen, wie hier beschrieben: [Markieren Sie die [!DNL Workfront Proof] site](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).
* Wenn Sie mehrere Testsendungen für dieselben Validierer freigeben müssen und nicht möchten, dass sie mehrere E-Mails erhalten, können Sie sie gleichzeitig hochladen. Alle validierungsverantwortlichen Benutzer erhalten eine E-Mail, in der alle Testsendungen detailliert beschrieben werden, einschließlich einer persönlichen URL für jeden Testversand.

   >[!NOTE]
   >
   >Der Ersteller der Testsendungen erhält eine separate [!UICONTROL Herstellernachweis] E-Mail für jeden erstellten Testversand. Weitere Informationen finden Sie unter [Die [!UICONTROL Proof Made] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Wenn Sie oder Ihre Validierer keine erwartete E-Mail-Benachrichtigung erhalten, lesen Sie  [Konfigurieren [!DNL Workfront Proof] E-Mails zur Vermeidung von Spam-Filtern](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
