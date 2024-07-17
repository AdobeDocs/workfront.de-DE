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

# [!UICONTROL Verspätete Testversand] E-Mail

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Die E-Mail &quot;[!UICONTROL Verspäteter Testversand]&quot; wird an Empfänger gesendet, wenn ein Testversand nahe der Frist oder dem Endtermin liegt. Diese Arten von E-Mails können nicht auf Testversandebene deaktiviert werden, sind jedoch auf Konto- und Benutzerebene konfigurierbar.

* [!UICONTROL Verspätete Testversand] -E-Mails werden automatisch an die validierungsverantwortlichen Benutzer gesendet, wenn ein Testversand seinen Termin erreicht und nicht alle Überprüfungen oder Entscheidungen getroffen wurden.

  Diese E-Mails sind standardmäßig aktiviert und können nicht für alle Konten angepasst werden. Benutzer können sie jedoch in ihren Testversandeinstellungen deaktivieren.

* Eventuelle E-Mails werden den Validierungsverantwortlichen gesendet, wenn ein Testversand nahe der Frist liegt. Sie sind standardmäßig deaktiviert und können in den [!UICONTROL Kontoeinstellungen] aktiviert werden. Nach der Aktivierung können sie auch in den [!UICONTROL Testversandstandardwerten] angepasst werden.

Diese Benachrichtigungen können nicht angepasst werden.

Folgende Personen werden benachrichtigt:

* Der Eigentümer wird nur dann in der Warnung [!UICONTROL E-Mail] zur Verspätung von Testsendungen aktiviert, wenn die Standardwerte für die Testsendungen des Eigentümers] aktiviert sind.[!UICONTROL 
* Jeder Genehmiger, der sich noch nicht zum Testversand entschieden hat. Informationen zu Entscheidungen finden Sie unter [Entscheidungsfindung für einen Testversand im Testversand-Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) .

>[!NOTE]
>
>Wenn die E-Mail-Benachrichtigungen in den [!UICONTROL Kontoeinstellungen] standardmäßig deaktiviert sind, werden keine [!UICONTROL verspäteten Testversand]-E-Mails gesendet, selbst wenn die Validierer und Genehmiger noch keine Kommentare und Entscheidungen übermittelt haben. Sie können auch die Option [!UICONTROL Verspätete Testversand] -E-Mails in den Testversandstandardeinstellungen deaktivieren.

Beachten Sie Folgendes zu Testversandbenachrichtigungen:

* Ihr [!DNL Workfront] -Administrator oder [!DNL Workfront Proof] -Administrator kann das Logo Ihres Unternehmens in Ihre E-Mail-Benachrichtigungen aufnehmen, wie unter [Marke der [!DNL Workfront Proof] Site](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md) beschrieben.
* Wenn Sie mehrere Testsendungen für dieselben Validierer freigeben müssen und nicht möchten, dass sie mehrere E-Mails erhalten, können Sie sie gleichzeitig hochladen. Alle validierungsverantwortlichen Benutzer erhalten eine E-Mail, in der alle Testsendungen detailliert beschrieben werden, einschließlich einer persönlichen URL für jeden Testversand.

  >[!NOTE]
  >
  >Der Ersteller der Testsendungen erhält für jeden erstellten Testversand eine separate E-Mail vom Typ [!UICONTROL Testversand durchgeführt] . Weitere Informationen finden Sie unter [Die E-Mail [!UICONTROL Proof Made]](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md).

* Wenn Sie oder Ihre Validierer keine erwartete E-Mail-Benachrichtigung erhalten, finden Sie weitere Informationen unter [Konfigurieren von [!DNL Workfront Proof] E-Mails, um Spamfilter zu vermeiden](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-wp-emails-avoid-spam-filters.md).
