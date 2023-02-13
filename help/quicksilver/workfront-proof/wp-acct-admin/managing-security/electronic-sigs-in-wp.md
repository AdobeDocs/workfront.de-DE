---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Grundlagen zu elektronischen Signaturen in [!DNL Workfront Proof]
description: Elektronische Signaturen ermöglichen es Ihnen, die Sicherheit Ihrer Testsendungen zu verbessern und Industriestandards wie ISO zu erfüllen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Grundlagen zu elektronischen Signaturen in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Elektronische Signaturen ermöglichen es Ihnen, die Sicherheit Ihrer Testsendungen zu verbessern und Industriestandards wie ISO zu erfüllen.

Diese Einstellung kann auf Kontoebene als obligatorisch oder nicht obligatorisch festgelegt werden. Wenn dies standardmäßig obligatorisch ist, ist es für alle in Ihrem Konto erstellten Testsendungen aktiviert und kann nicht auf Testversandebene deaktiviert werden. Wenn diese Einstellung standardmäßig nicht obligatorisch ist, können Sie sie auf Testversandebene aktivieren/deaktivieren.

Weitere Informationen finden Sie unter .

Wenn die Einstellung für die elektronische Signatur für einen Testversand aktiviert ist, fordert ein Feld für die elektronische Signatur jeden Validierer, der eine Entscheidung über den Testversand trifft, auf, seine E-Mail-Adresse und sein Passwort anzugeben.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## Elektronische Signaturen auf der [!UICONTROL Testversanddetails] Seite

Wenn ein Validierer seine Entscheidung trifft, indem er seine Entscheidung über die [!UICONTROL Testversanddetails] Seite (1) und [!UICONTROL Elektronische Signatur] wird ein Popup-Fenster angezeigt, in dem sie aufgefordert werden, ihre Details einzugeben (2) und ihre Entscheidung zu bestätigen (3).

Das Popup-Fenster zeigt den standardmäßigen Nachrichtensatz an (falls vorhanden) und der Validierer muss seine E-Mail-Adresse und sein Kennwort eingeben.

Die [!UICONTROL Elektronische Signatur] Popup-Fenster werden im Testversand-Viewer und auch auf der [!UICONTROL Testversanddetails] Seite, wenn der Validierer beschließt, seine Entscheidung auf dieser Ebene zu treffen.

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

Wenn die Variable [!UICONTROL Single Sign-on] aktiviert ist, werden die E-Mail- und Kennwortdetails nicht im [!UICONTROL Elektronische Signatur] angezeigt, wenn Sie eine Entscheidung treffen.

Klicken Sie stattdessen auf [!UICONTROL Bestätigen] (4) in diesem Popup wird der Validierer zum [!UICONTROL Single Sign-on] Seite.

Nach Eingabe der SSO-Anmeldeinformationen wird der Überprüfer automatisch zurück zum [!UICONTROL Testversanddetails] Seite (oder zurück zum [!UICONTROL Proof Viewer] wenn die Entscheidung von dort getroffen wird).

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> Wenn die Entscheidung elektronisch unterzeichnet wird, **[!UICONTROL Signatursymbol]** (5) neben der Entscheidung im [!UICONTROL Workflow] im Abschnitt [!UICONTROL Testversanddetails] Seite. Wenn die Entscheidung nicht vom Prüfer, sondern von einer anderen Person geändert wird, die über Bearbeitungsrechte für den Testversand verfügt, wird diese Person nicht aufgefordert, die Entscheidung elektronisch zu unterzeichnen, und neben der Entscheidung wird kein Signatursymbol angezeigt (6).

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)Weitere Informationen zum Single Sign-on finden Sie unter [Single-Sign-On in Workfront Testversand](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

Weitere Informationen zur Seite &quot;Testversand-Details&quot;finden Sie unter [Testversanddetails verwalten in [!DNL Workfront] Testversand](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
