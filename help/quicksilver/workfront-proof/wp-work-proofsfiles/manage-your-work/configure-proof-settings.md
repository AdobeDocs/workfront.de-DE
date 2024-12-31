---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Konfigurieren Sie die Einstellungen für den Korrekturabzug in [!DNL Workfront Proof]
description: Sie können einen Korrekturabzug konfigurieren, den Sie in Korrekturabzügen erstellen oder bearbeiten.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ca379054-4737-4796-a812-f2ec38b437ba
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 1%

---

# Konfigurieren der Einstellungen für Korrekturabzüge in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Sie können einen Korrekturabzug, den Sie erstellen oder bearbeiten, auf eine der folgenden Arten konfigurieren:

>[!NOTE]
>
>Sie können diese Einstellungen für alle neuen Korrekturabzüge konfigurieren, die Sie erstellen. Weitere Informationen finden Sie unter .

## Korrekturabzug bei letzter Entscheidung sperren

Sie können einen Korrekturabzugsstatus festlegen, der gesperrt wird, wenn die endgültige genehmigende Person ihre Entscheidung trifft. Dies ist nützlich, wenn Sie sicherstellen möchten, dass Ihre Prüfer nicht zum Korrekturabzug zurückkehren und zusätzliche Kommentare hinzufügen oder ihre Entscheidungen ändern können.

1. Erstellen Sie einen neuen Korrekturabzug, wie in [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Korrekturabzugsdetails für einen vorhandenen Korrekturabzug, wie unter [Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Wählen Sie für einen neuen Korrekturabzug unter **[!UICONTROL Korrekturabzugseinstellungen]** die Option **[!UICONTROL Korrekturabzug sperren, wenn alle erforderlichen Entscheidungen getroffen werden]**.\
   Oder\
   Wählen Sie für einen vorhandenen Korrekturabzug unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Korrekturabzug sperren, wenn alle Entscheidungen getroffen werden]** aus.

Weitere Informationen zu Entscheidungen finden Sie unter [Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht treffen](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

## Anmeldung für alle Benutzer verlangen, die den Korrekturabzug überprüfen

Eines der großartigen Dinge an [!DNL Workfront Proof] ist, dass jeder einen Korrekturabzug prüfen kann, man braucht dafür keine eigene [!DNL Workfront Proof]. Empfänger erhalten eine E-Mail mit einer persönlichen URL, über die sie direkt zur Seite des Korrekturabzugs gelangen, ohne sich bei [!DNL Workfront Proof] anmelden zu müssen.

Wenn Sie jedoch höhere Sicherheitsstufen für Ihren Prüfungs- und Genehmigungsprozess benötigen, können Sie die Option Anmeldung beim Korrekturabzug erforderlich verwenden. Das bedeutet, dass nur [!DNL Workfront Proof] Benutzer zum Korrekturabzug hinzugefügt werden können. Und sie müssen ihre E-Mail-Adresse und ihr Passwort eingeben, bevor sie darauf zugreifen können.

>[!NOTE]
>
>* *Damit sich jemand beim Korrekturabzug anmelden kann (wenn „Anmeldung erforderlich“ aktiviert ist), muss er zum Korrekturabzug hinzugefügt worden sein.*
>* *Wenn „Anmeldung erforderlich“ aktiviert ist, können Abonnements nicht aktiviert werden.*

So fordern Sie die Anmeldung für alle Benutzer an, die den Korrekturabzug überprüfen:

1. Erstellen Sie einen neuen Korrekturabzug, wie in [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Korrekturabzugsdetails für einen vorhandenen Korrekturabzug, wie unter [Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Wählen Sie für einen neuen Korrekturabzug unter **[!UICONTROL Korrekturabzugseinstellungen]** die Option **[!UICONTROL Anmeldung erforderlich]** aus.\
   Oder\
   Wählen Sie für einen vorhandenen Korrekturabzug unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Anmeldung erforderlich]** aus.

## Nur eine Entscheidung für den Testversand verlangen

Diese Einstellung ist nützlich, wenn Sie nur eine Person aus einer Gruppe, Abteilung oder Firma benötigen, um eine Entscheidung über den Korrekturabzug zu treffen.

Selbst wenn Sie die Rolle einer genehmigenden Person oder einer prüfenden Person und einer genehmigenden Person mehreren Personen zuweisen, wird der Status des Korrekturabzugs aktualisiert, sobald eine Person eine Entscheidung über einen Korrekturabzug trifft (gemäß der getroffenen Entscheidung). Weitere Informationen zum Korrekturabzugsstatus finden Sie unter [Anzeigen des Fortschritts und Status eines Korrekturabzugs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)

1. Erstellen Sie einen neuen Korrekturabzug, wie in [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Korrekturabzugsdetails für einen vorhandenen Korrekturabzug, wie unter [Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Wählen Sie für einen neuen Korrekturabzug unter **[!UICONTROL Workflow]** die Option **[!UICONTROL Nur eine Entscheidung für diesen Schritt erforderlich]** aus.\
   Oder\
   Wählen Sie für einen vorhandenen Korrekturabzug unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Nur eine Entscheidung erforderlich]** aus.

Weitere Informationen zu Entscheidungen finden Sie unter [Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht treffen](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md#making-a-decision-on-a-proof).

## Entscheidungen müssen elektronisch signiert werden

Sie können von jedem Prüfer, der über den Korrekturabzug entscheidet, eine elektronische Signatur verlangen, um seine E-Mail-Adresse und sein Passwort anzugeben. Wenn ein Validierungsverantwortlicher eine Entscheidungsaufforderung anzeigt, in der er aufgefordert wird, seine E-Mail-Adresse und sein Passwort einzugeben und seine Entscheidung zu bestätigen. Weitere Informationen finden Sie unter [Grundlagen zu elektronischen Signaturen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md)

1. Erstellen Sie einen neuen Korrekturabzug, wie in [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Korrekturabzugsdetails für einen vorhandenen Korrekturabzug, wie unter [Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Wählen Sie für einen neuen Korrekturabzug unter **[!UICONTROL Korrekturabzugseinstellungen]** die Option **[!UICONTROL Entscheidungen müssen elektronisch signiert werden]** aus.\
   Oder\
   Wählen Sie für einen vorhandenen Korrekturabzug unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Entscheidungen müssen elektronisch signiert sein]** aus.

Weitere Informationen zu Entscheidungen finden Sie [Konfigurieren von Genehmigungsentscheidungsoptionen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).

## Benutzer daran hindern, die Originaldatei herunterzuladen

Sie können verhindern, dass Prüfer eines Korrekturabzugs die Originaldatei herunterladen, aus der ein Korrekturabzug erstellt wurde.

1. Erstellen Sie einen neuen Korrekturabzug, wie in [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Korrekturabzugsdetails für einen vorhandenen Korrekturabzug, wie unter [Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Deaktivieren Sie für einen neuen Korrekturabzug unter **[!UICONTROL Korrekturabzugseinstellungen]** die Option **[!UICONTROL Originaldatei herunterladen]**.\
   Oder\
   Wählen Sie für einen vorhandenen Korrekturabzug unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Download der Originaldatei]** aus.

## Anderen Benutzern erlauben, den Korrekturabzug zu abonnieren

Das Abonnement ist eine erweiterte Einstellung, die mit der Korrekturabzugs-URL und dem Mini-Korrekturabzug funktioniert.

Standardmäßig können Personen, die nicht explizit zum Korrekturabzug hinzugefügt wurden und die Korrekturabzugs-URL oder den Mini-Korrekturabzug verwenden, um darauf zuzugreifen, den Korrekturabzug nur im schreibgeschützten Modus anzeigen. Personen, die bereits Prüfer für den Korrekturabzug sind, können sich mit ihrer E-Mail-Adresse anmelden. Weitere Informationen finden Sie unter [Verwalten von Korrekturabzugsrollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)

Durch die Aktivierung des Abonnements für den Korrekturabzug können Personen, die nicht explizit zum Korrekturabzug hinzugefügt wurden, den Korrekturabzug selbst abonnieren (sich also zum Korrekturabzug hinzufügen). Ihnen werden dann die Rolle und der E-Mail-Warnhinweis zugewiesen, die Sie in den Abonnementeinstellungen für sie auswählen.

Wenn das Abonnement für einen Korrekturabzug aktiviert wurde, werden die folgenden Felder aktiv:

* **[!UICONTROL Abonnentenvalidierung erforderlich]** - Abonnenten müssen auf einen Link in einer E-Mail klicken, um auf einen Korrekturabzug zuzugreifen\
   Die Auswahl dieser Option bedeutet, dass die abonnierende Person keinen sofortigen Zugriff auf den Korrekturabzug erhält, sondern einen Link zum Korrekturabzug in einer E-Mail erhält. Mit der Abonnentenvalidierung soll sichergestellt werden, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, zu der sie Zugriff hat.

* **[!UICONTROL Standardrolle für neue Abonnenten]** - Dies ist die Standardrolle für Korrekturabzüge, die allen Reviewern zugewiesen wird, die den Korrekturabzug selbst abonnieren.
* **[!UICONTROL Standard-E-Mail-Warnhinweis für neue Abonnenten]** - Dies ist der standardmäßige E-Mail-Warnhinweis, der allen Reviewern zugewiesen wird, die den Testversand selbst abonnieren.

Siehe auch [Abonnieren eines Korrekturabzugs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)

So lassen Sie es zu, dass andere Benutzer einen Korrekturabzug abonnieren:

1. Erstellen Sie einen neuen Korrekturabzug, wie in [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) beschrieben.\
   Oder\
   Öffnen Sie die Seite mit den Korrekturabzugsdetails für einen vorhandenen Korrekturabzug, wie unter [Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.

1. Deaktivieren Sie für einen neuen Korrekturabzug unter **[!UICONTROL Korrekturabzugseinstellungen]** die Option **[!UICONTROL Korrekturabzug über öffentliche URL oder Einbettungs-Code abonnieren]**.\
   Oder\
   Wählen Sie für einen vorhandenen Korrekturabzug unter **[!UICONTROL Einstellungen]** die Option **[!UICONTROL Abonnement]** aus.
