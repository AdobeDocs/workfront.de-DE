---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: workflow-examples
title: Interne und dann externe Überprüfung in [!DNL Workfront Proof]
description: Erfahren Sie, wie Sie Workfront Proof für Überprüfungen außerhalb Ihres Unternehmens verwenden.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c54246e9-edb8-4d98-81e1-faf7ee75f81e
source-git-commit: 153951e3bba91d67bcfe5fbf22c0970743f0dc6e
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Interne und dann externe Überprüfung in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Wenn Ihr Unternehmen interne Überprüfungen durchführt, bevor Sie Korrekturabzüge für Kunden freigeben, schlagen wir zwei Möglichkeiten vor, [!DNL Workfront Proof] zur Verbesserung Ihres Workflows zu verwenden:

## Kunden sehen interne Kommentare

Diese Option zeigt einen Workflow, bei dem Kunden alle internen Kommentare anzeigen können.

Der Designer gibt den Korrekturabzug zuerst an den Projekt-Manager (und alle anderen Kollegen) weiter. Kollegen prüfen den Korrekturabzug. Wenn sie ihn genehmigen, können Sie ihn über die Funktion „Freigeben“ für Ihre Kunden freigeben. Weitere Informationen finden Sie unter [Freigeben eines Korrekturabzugs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

![internal_external_-_option_A.png](assets/internal_external_-_option_A.png)

1. **Neuen Korrekturabzug erstellen** - Der Designer erstellt einen neuen Korrekturabzug in [!DNL Workfront Proof] und gibt ihn für interne Prüfer frei. Der Designer macht den Projekt-Manager zum Besitzer des Korrekturabzugs.
1. **Interne Überprüfung** - Der Projektmanager und andere Kollegen prüfen den Testversand.
1. **Korrekturabzug freigeben** - Der Projekt-Manager gibt den Korrekturabzug für den Kunden frei.
1. **Neue Korrekturabzugs-E**-Mail: Der Client erhält die E-Mail mit dem [!UICONTROL Zum Korrekturabzug gehen]. Weitere Informationen finden Sie unter [Neue Korrekturabzugs-E-Mail](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **Korrekturabzug überprüfen** - Der Kunde prüft den Korrekturabzug, fügt Kommentare hinzu und trifft eine Entscheidung.
1. **E-Mail-Warnhinweis** - Der Projekt-Manager erhält einen E-Mail-Warnhinweis (abhängig von seinen Einstellungen für den Korrekturabzug). Weitere Informationen finden Sie unter [Konfigurieren von E-Mail-Benachrichtigungseinstellungen in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

1. **Änderungsanforderung** - Der Projekt-Manager informiert den Designer über die Änderungsanforderungen. Dies kann über die Funktion Kommentare drucken erfolgen. Weitere Informationen finden Sie unter [Drucken und Exportieren von Kommentaren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **Neue Version** (falls erforderlich) - Der Designer ändert die Datei und lädt sie als neue Version in [!DNL Workfront Proof] hoch. Weitere Informationen finden Sie unter .

Sie können diesen Vorgang wiederholen, bis der Korrekturabzug genehmigt wurde.

## Der Client sieht nur seine eigene Version

Diese Option veranschaulicht einen Workflow, bei dem der Proofing-Prozess vom Projekt-Manager verwaltet wird, der alle neuen Versionen erstellt (sofern erforderlich) und den Korrekturabzug für den Client freigibt. Der Designer muss nicht in den Überprüfungsprozess eingebunden werden.)

![internal_external_-_option_B.png](assets/internal_external_-_option_B.png)

1. **Neuen Korrekturabzug erstellen** - Der Designer erstellt einen neuen Korrekturabzug in [!DNL Workfront Proof] und gibt ihn für interne Prüfer frei. Der Designer macht den Projekt-Manager zum Besitzer des Korrekturabzugs oder gibt ihm alternativ die Rolle [!UICONTROL Autor] für den Korrekturabzug (siehe [Rollen für Korrekturabzüge verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

1. **Interne Überprüfung** - Der Projektmanager und andere Kollegen prüfen den Testversand. Weitere Informationen finden Sie unter [Testsendungen im Web Proofing Viewer überprüfen](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer) und [Testsendungen im Desktop Proofing Viewer überprüfen.](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)

1. **Neue Version** - Der Projekt-Manager erstellt eine neue Version (oder eine Kopie) des Korrekturabzugs und gibt ihn für den Client frei. Siehe [Kopieren von Korrekturabzügen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) und [Freigeben eines Korrekturabzugs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

1. **Neue Korrekturabzugs-E**-Mail: Der Client erhält die E-Mail mit einem [!UICONTROL Link Zum Korrekturabzug gehen]. Weitere Informationen finden Sie unter [Neue Korrekturabzugs-E-Mail](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **[!UICONTROL Korrekturabzug überprüfen]** - Der Kunde prüft den Korrekturabzug, fügt Kommentare hinzu und trifft eine Entscheidung.
1. Der Client kann nur die Version des Korrekturabzugs sehen, die explizit für ihn freigegeben wurde. Er kann die interne Version nicht sehen.
1. **[!UICONTROL E-Mail-]**: Der Projekt-Manager erhält eine E-Mail mit einer Zusammenfassung der Überprüfung durch den Kunden (je nach den Einstellungen für den Testversand).
1. **Änderungsanforderung** - Der Projekt-Manager informiert den Designer über die Änderungsanforderungen. Dies kann über die Funktion Kommentare drucken erfolgen. Weitere Informationen finden Sie unter [Drucken und Exportieren von Kommentaren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **Neue Version** (falls erforderlich) - Der Designer ändert die Datei und lädt sie als neue Version in [!DNL Workfront Proof] hoch. Weitere Informationen finden Sie unter .

Sie können diesen Vorgang wiederholen, bis der Korrekturabzug genehmigt wurde.
