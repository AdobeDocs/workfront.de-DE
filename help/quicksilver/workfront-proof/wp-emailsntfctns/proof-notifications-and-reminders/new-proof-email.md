---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Neue Testversand-E-Mail
description: Machen Sie diesen Artikel für PiW besser.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Neue Testversand-E-Mail

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Wenn Sie einen neuen Testversand oder eine neue Testversand-Version erstellen, einem Testversand neue Personen hinzufügen oder einen Workflow zu einem Testversand hinzufügen, können Sie entscheiden, ob Sie den Validierern eine E-Mail senden möchten, wie in diesen Artikeln beschrieben wird:

* [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Testsendungen generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

Die E-Mail, die Ihre Empfänger erhalten, wird als [!UICONTROL Neuer Testversand] E-Mail. Diese E-Mail kann nur vom Ersteller des Testversands und von Benutzern, die zum Hinzufügen von Validierern zu einem Testversand berechtigt sind, gesteuert werden. Empfänger können sie nicht deaktivieren.

Die E-Mail zum neuen Testversand enthält:

* Ihre persönliche Nachricht (wenn Sie eine einfügen möchten)
* Wenn Sie immer dieselbe benutzerdefinierte Nachricht an Ihre Validierungsverantwortlichen senden, empfiehlt es sich möglicherweise, sie in Ihrer [!UICONTROL Persönliche Einstellungen] unter [!UICONTROL Standardeinstellungen für die Prüfung] Registerkarte. Weitere Informationen finden Sie unter .
* Persönlicher Link zum Testversand
* **[!UICONTROL Details anzeigen]** -Link, der Sie zum zugehörigen [!DNL Workfront] -Objekt (z. B. ein Projekt, eine Aufgabe oder ein Problem)
* Miniaturansicht des Testversandbilds
* Folgende Testversanddetails:

   * Name des Korrekturabzugs
   * Versionsnummer

      Weitere Informationen finden Sie unter .

   * Liste der validierungsverantwortlichen Benutzer und Fortschritt des Testversands
   * Ein Link zum Freigeben des Testversands für eine andere Person

      Auf diese Weise können Sie die Testversand-URL und/oder den Download-Link für die Originaldatei freigeben. Auf diese Weise können Sie dem Testversand keine Validierungsverantwortlichen hinzufügen. Sie geben nur die öffentliche Testversand-URL frei und der Empfänger erhält Lesezugriff auf den Testversand.

      Siehe [Testversand freigeben in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) für weitere Informationen.

      Wenn dieser Link nicht in der E-Mail Ihres Empfängers angezeigt werden soll, können Sie die [!UICONTROL Öffentliche Freigabe] Testversandeinstellungen

      (Originaldatei und öffentliche URL herunterladen). Siehe [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) für weitere Informationen.

## Das Aktivitätsprotokoll

Senden einer [!UICONTROL Neuer Testversand] E-Mail an einen Validierer im [!UICONTROL Aktivität] Abschnitt [!UICONTROL Testversanddetails] Seite. Siehe  [Verwalten[!UICONTROL  Testversanddetails] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) für weitere Informationen. Sie können überprüfen, ob die [!UICONTROL Neuer Testversand] E-Mail wurde zum Zeitpunkt der Erstellung eines Testversands aktiviert.

![New_Verison_email_-_acitivity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Wenn der Ersteller oder Eigentümer des Testversands [!UICONTROL Proof Made] E-Mails, die standardmäßig deaktiviert sind (in ihren persönlichen Einstellungen), werden nicht empfangen [!UICONTROL Herstellernachweis] oder [!UICONTROL Neuer Testversand] E-Mails auch dann, wenn die [!UICONTROL Personen per E-Mail benachrichtigen] auf der Seite Neuer Testversand aktiviert ist. Weitere Informationen finden Sie unter .
>* Wenn E-Mail-Benachrichtigungen standardmäßig deaktiviert sind, finden Sie unter [!UICONTROL Kontoeinstellungen] Der Ersteller/Eigentümer des Testversands erhält keine [!UICONTROL Herstellernachweis] oder [!UICONTROL Neuer Testversand] E-Mails auch dann, wenn dies in ihren persönlichen Einstellungen und der [!UICONTROL Benachrichtigen] Personen per E-Mail werden auf der Seite Neuer Testversand aktiviert. Weitere Informationen: [Die [!UICONTROL Proof Made] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) und siehe .
>




## Aktivieren Sie die [!UICONTROL Neuer Testversand] E-Mail versenden und eine benutzerdefinierte Nachricht einfügen

Sie können angeben, ob Sie den Validierern bei der Erstellung eines Testversands oder beim Hinzufügen eines Testversands eine E-Mail-Warnung senden möchten.

* [Beim Erstellen eines Testversands](#when-you-create-a-proof)
* [Wenn Sie einen Validierer zu einem Testversand hinzufügen](#when-you-add-a-reviewer-to-a-proof)

### Beim Erstellen eines Testversands {#when-you-create-a-proof}

Wenn Sie einen neuen Testversand im [!UICONTROL Neuer Testversand] Seite, unter der **[!UICONTROL Freigeben]** können Sie auswählen, ob E-Mail-Warnungen gesendet werden sollen:

* Hier können Sie entscheiden, ob Sie [!UICONTROL Personen per E-Mail benachrichtigen] Absatz 1. Wenn Sie diese Option deaktivieren, erhält keiner Ihrer validierenden Benutzer eine E-Mail, um ihm mitzuteilen, dass der Testversand zur Überprüfung bereit ist.
* Sie können auch eine benutzerdefinierte Nachricht in die E-Mail-Benachrichtigung einfügen (2).
* Wenn Sie Ihre eigene benutzerdefinierte Nachricht hinzufügen möchten, können Sie eine benutzerdefinierte Betreffzeile (3) und eine Nachricht im Textkörper der E-Mail (4) einfügen.
* Um die benutzerdefinierte Nachricht zu verwerfen, klicken Sie einfach auf den Link (5).

   >[!NOTE]
   >
   >Wenn Sie immer dieselbe benutzerdefinierte Nachricht an Ihre Validierungsverantwortlichen senden, empfiehlt es sich möglicherweise, sie in Ihren persönlichen Einstellungen unter [!UICONTROL Standardeinstellungen für die Prüfung] Registerkarte. Weitere Informationen finden Sie unter .

![new_proof_page_1.png](assets/new-proof-page-1-350x186.png)

![new_proof_page_2.png](assets/new-proof-page-2-350x283.png)

### Wenn Sie einen Validierer zu einem Testversand hinzufügen {#when-you-add-a-reviewer-to-a-proof}

Sie können auswählen, ob ein neuer Validierer, der einem vorhandenen Testversand hinzugefügt wurde, über den Testversand informiert wird (ähnlich wie oben).

* Fügen Sie zunächst neue Validierungsverantwortliche hinzu, indem Sie auf **[!UICONTROL Diese Version freigeben]** Schaltfläche auf der **[!UICONTROL Testversanddetails]** Seite (1).

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* Es wird ein Feld angezeigt, in dem Sie neue Überprüfer hinzufügen können. Sie können dann entscheiden, ob Sie eine Benachrichtigung per E-Mail (2) erhalten möchten, und eine benutzerdefinierte Nachricht zur E-Mail hinzufügen (3).

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* Wenn Sie eine benutzerdefinierte Nachricht hinzufügen, wird das Feld erweitert und Sie können eine benutzerdefinierte Betreffzeile (4) und benutzerdefinierten Text im Text der E-Mail (5) einfügen. Sie können die benutzerdefinierte Nachricht auch verwerfen, indem Sie auf den Link (6) klicken.

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
