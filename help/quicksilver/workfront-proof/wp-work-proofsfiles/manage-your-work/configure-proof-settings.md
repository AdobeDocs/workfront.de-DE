---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Konfigurieren der Testversandeinstellungen in  [!DNL Workfront Proof]
description: Sie können einen Testversand konfigurieren, den Sie in Testsendungen erstellen oder bearbeiten.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%

---

# Konfigurieren der Testversandeinstellungen in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Sie haben folgende Möglichkeiten, einen Testversand zu konfigurieren, den Sie erstellen oder bearbeiten:

>[!NOTE]
>
>Sie können diese Einstellungen für alle neuen Testsendungen konfigurieren, die Sie erstellen. Weitere Informationen finden Sie unter .

## Sperren des Testversands, wenn die letzte Entscheidung getroffen wurde

Sie können einen Testversandstatus festlegen, der gesperrt wird, wenn der endgültige Genehmiger seine Entscheidung trifft. Dies ist nützlich, wenn Sie sicherstellen möchten, dass Ihre Prüfer nicht zum Testversand zurückkehren und zusätzliche Kommentare hinzufügen oder ihre Entscheidungen ändern können.

1. Erstellen Sie einen neuen Testversand, wie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Testversanddetails für einen vorhandenen Testversand, wie unter [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Wählen Sie für einen neuen Testversand unter **[!UICONTROL Testversandeinstellungen]** die Option **[!UICONTROL Testversand sperren, wenn alle erforderlichen Entscheidungen getroffen werden]**.\
   Oder\
   Wählen Sie für einen vorhandenen Testversand unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Testversand sperren, wenn alle Entscheidungen getroffen werden]**.

Informationen zu Entscheidungen finden Sie unter [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Anmeldung für alle Benutzer erforderlich, die den Testversand überprüfen

Eines der großartigen Dinge an [!DNL Workfront Proof] ist, dass jeder einen Testversand überprüfen kann, dafür braucht man keine eigenen [!DNL Workfront Proof]. Empfänger erhalten eine E-Mail mit einer persönlichen URL, die sie direkt zur Testversand-Seite führt, ohne sich bei [!DNL Workfront Proof] anmelden zu müssen.

Wenn Sie jedoch höhere Sicherheitsstufen für Ihren Überprüfungs- und Genehmigungsprozess benötigen, können Sie die Anmeldung beim Testversand erforderlich machen. Das bedeutet, dass nur [!DNL Workfront Proof] Benutzer zum Testversand hinzugefügt werden können. Und sie müssen ihre E-Mail-Adresse und ihr Passwort eingeben, bevor sie darauf zugreifen können.

>[!NOTE]
>
>* *Damit sich ein Benutzer beim Testversand anmelden kann (wenn die erforderliche Anmeldung aktiviert wurde), muss er zum Testversand hinzugefügt worden sein.*
>* *Wenn die erforderliche Anmeldung aktiviert ist, können Abonnements nicht aktiviert werden.*

So müssen Sie sich für alle Benutzer anmelden, die den Testversand überprüfen:

1. Erstellen Sie einen neuen Testversand, wie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Testversanddetails für einen vorhandenen Testversand, wie unter [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Wählen Sie für einen neuen Testversand unter **[!UICONTROL Testversandeinstellungen]** die Option **[!UICONTROL Anmeldung erforderlich]**.\
   Oder\
   Wählen Sie für einen vorhandenen Testversand unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Anmeldung erforderlich]**.

## Nur eine Entscheidung für den Testversand erforderlich

Diese Einstellung ist nützlich, wenn Sie nur eine Person aus einer Gruppe, Abteilung oder Firma benötigen, um eine Entscheidung über den Testversand zu treffen.

Selbst wenn Sie die Rolle &quot;Genehmiger&quot;, &quot;Validierer&quot;und &quot;Genehmiger&quot;mehreren Personen zuweisen, wird der Status des Testversands aktualisiert, sobald eine Person eine Entscheidung über einen Testversand trifft (entsprechend der getroffenen Entscheidung). Weitere Informationen zum Testversandstatus finden Sie unter [Fortschritt und Status eines Testversands anzeigen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Erstellen Sie einen neuen Testversand, wie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Testversanddetails für einen vorhandenen Testversand, wie unter [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Wählen Sie für einen neuen Testversand unter **[!UICONTROL Workflow]** die Option **[!UICONTROL Nur eine Entscheidung für diese Phase anfordern]** aus.\
   Oder\
   Wählen Sie für einen vorhandenen Testversand unter **[!UICONTROL Einstellungen]** **[!UICONTROL Nur eine Entscheidung erforderlich]** aus.

Informationen zu Entscheidungen finden Sie unter [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Elektronische Unterschrift von Entscheidungen erforderlich

Sie können von jedem Validierer, der über den Testversand entscheidet, eine elektronische Signatur verlangen, um seine E-Mail-Adresse und sein Passwort einzugeben. Wenn ein Validierer eine Entscheidungsaufforderung öffnet, in der er aufgefordert wird, seine E-Mail-Adresse und sein Passwort einzugeben und seine Entscheidung zu bestätigen. Weitere Informationen finden Sie unter [Grundlegendes zu elektronischen Signaturen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Erstellen Sie einen neuen Testversand, wie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Testversanddetails für einen vorhandenen Testversand, wie unter [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Wählen Sie für einen neuen Testversand unter **[!UICONTROL Testversandeinstellungen]** die Option **[!UICONTROL Erfordert die elektronische Unterzeichnung von Entscheidungen]**.\
   Oder\
   Wählen Sie für einen vorhandenen Testversand unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Elektronische Signierung von Entscheidungen erforderlich]**.

Weitere Informationen zu Entscheidungen finden Sie unter [Optionen für Genehmigungsentscheidungen konfigurieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Benutzer nicht erlauben, die Originaldatei herunterzuladen

Sie können die Validierungsverantwortlichen daran hindern, die Originaldatei herunterzuladen, aus der ein Testversand erstellt wurde.

1. Erstellen Sie einen neuen Testversand, wie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Testversanddetails für einen vorhandenen Testversand, wie unter [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Deaktivieren Sie für einen neuen Testversand unter **[!UICONTROL Testversandeinstellungen]** die Option **[!UICONTROL Originaldatei herunterladen]**.\
   Oder\
   Wählen Sie für einen vorhandenen Testversand unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Download der Originaldatei]**.

## Anderen Benutzern das Abonnieren des Testversands ermöglichen

Anmeldung ist eine erweiterte Einstellung, die mit der Proof-URL und dem Mini-Testversand verwendet werden kann.

Standardmäßig können Personen, die nicht speziell zum Testversand hinzugefügt wurden und die die Testversand-URL oder den Mini-Testversand verwenden, nur den Testversand im schreibgeschützten Modus anzeigen. Personen, die bereits für den Testversand validiert haben, können sich mit ihrer E-Mail-Adresse anmelden. Weitere Informationen finden Sie unter [Verwalten von Proof-Rollen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

Durch die Aktivierung des Testversands können Personen, die nicht explizit zum Testversand hinzugefügt wurden, sich für den Testversand anmelden (d. h. sich zum Testversand hinzufügen). Anschließend wird ihnen die Rolle und der E-Mail-Warnhinweis zugewiesen, die Sie in den Abonnementeinstellungen für sie auswählen.

Wenn die Option Anmeldung für einen Testversand aktiviert wurde, werden die folgenden Felder aktiv:

* **[!UICONTROL Validierung der Abonnenten erforderlich]** - Der Abonnent muss auf einen Link in einer E-Mail klicken, um auf einen Testversand zugreifen zu können\
   Wenn Sie diese Option auswählen, erhält der Abonnent keinen sofortigen Zugriff auf den Testversand, sondern einen Link zum Testversand in einer E-Mail. Die Abonnentenvalidierung soll sicherstellen, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, auf die sie Zugriff hat.

* **[!UICONTROL Standardrolle für neue Abonnenten]** - Dies ist die Standardrolle für den Testversand, die allen Validierern zugewiesen wird, die sich selbst für den Testversand angemeldet haben.
* **[!UICONTROL Standard-E-Mail-Warnung für neue Abonnenten]** - Dies ist der Standard-E-Mail-Warnhinweis, der allen Validierern zugewiesen wird, die sich selbst für den Testversand angemeldet haben.

Siehe auch [Abonnieren eines Testversands in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

So können andere Benutzer einen Testversand abonnieren:

1. Erstellen Sie einen neuen Testversand, wie unter [Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) generieren beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Testversanddetails für einen vorhandenen Testversand, wie unter [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Deaktivieren Sie für einen neuen Testversand unter **[!UICONTROL Testversandeinstellungen]** die Option **[!UICONTROL Testversand über öffentliche URL oder Einbettungscode abonnieren]**.\
   Oder\
   Wählen Sie für einen vorhandenen Testversand unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Abonnement]**.
