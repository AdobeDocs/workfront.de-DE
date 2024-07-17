---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: workflow-examples
title: Interner und dann externer Review in [!DNL Workfront Proof]
description: Erfahren Sie, wie Sie Workfront Proof für Überprüfungen außerhalb Ihres Unternehmens verwenden.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: c54246e9-edb8-4d98-81e1-faf7ee75f81e
source-git-commit: 153951e3bba91d67bcfe5fbf22c0970743f0dc6e
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Interner, dann externer Review in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Ihr Unternehmen interne Überprüfungen abschließt, bevor Testsendungen für Kunden freigegeben werden, empfehlen wir zwei Möglichkeiten, mit [!DNL Workfront Proof] Ihren Workflow zu verbessern:

## Kunden sehen interne Kommentare

Diese Option zeigt einen Workflow, in dem Clients alle internen Kommentare sehen können.

Der Designer gibt den Testversand zunächst an den Projektmanager (und andere Kollegen) weiter. Kollegen überprüfen den Testversand und wenn sie ihn validieren, können Sie die Freigabefunktion verwenden, um den Testversand mit Ihren Kunden zu teilen. Weitere Informationen finden Sie unter [Testversand freigeben in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

![internal_external_-_option_a.png](assets/internal_external_-_option_A.png)

1. **Erstellen Sie einen neuen Testversand** - Der Designer erstellt einen neuen Testversand in [!DNL Workfront Proof] und gibt ihn für interne Validierer frei. Der Designer macht den Projektmanager zum Besitzer des Testversands.
1. **Interne Überprüfung** - Der Projektmanager und andere Kollegen überprüfen den Testversand.
1. **Testversand freigeben** - Der Projektmanager gibt den Testversand für den Client frei.
1. **Neue Testversand-E-Mail** - der Kunde erhält die E-Mail zum neuen Testversand mit dem Link [!UICONTROL Gehe zu Testversand] . Weitere Informationen finden Sie unter [Neue Testversand-E-Mail](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **Testversand überprüfen** - der Kunde überprüft den Testversand, fügt Kommentare hinzu und trifft eine Entscheidung.
1. **E-Mail-Warnung** - Der Projektmanager erhält eine E-Mail-Warnung (je nach den Einstellungen für den Testversand). Weitere Informationen finden Sie unter [E-Mail-Benachrichtigungseinstellungen in Workfront Proof konfigurieren](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

1. **Anforderung ändern** - Der Projekt-Manager informiert den Designer über die Änderungsanforderungen. Dies kann mithilfe der Druckkommentar-Funktion erfolgen. Weitere Informationen finden Sie unter [Drucken und Exportieren von Kommentaren in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **Neue Version** (falls erforderlich) - der Designer ändert die Datei und lädt sie als neue Version in [!DNL Workfront Proof] hoch. Weitere Informationen finden Sie unter .

Sie können diesen Vorgang wiederholen, bis der Testversand validiert wurde.

## Der Kunde sieht nur seine eigene Version

Diese Option veranschaulicht einen Workflow, bei dem der Testversand vom Projektmanager verwaltet wird, der neue Versionen erstellt (falls erforderlich) und den Testversand an den Kunden weitergibt. Der Designer muss nicht in den Überprüfungsprozess einbezogen werden.)

![internal_external_-_option_b.png](assets/internal_external_-_option_B.png)

1. **Erstellen eines neuen Testversands** - Der Designer erstellt einen neuen Testversand in [!DNL Workfront Proof] und gibt ihn für interne Validierer frei. Der Designer macht den Projektmanager zum Inhaber des Testversands oder gibt ihm alternativ die Rolle [!UICONTROL Autor] für den Testversand (siehe [Verwalten von Testrollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

1. **Interne Überprüfung** - Der Projektmanager und andere Kollegen überprüfen den Testversand. Weitere Informationen finden Sie unter [Überprüfen von Testsendungen im Web Proofing Viewer](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer) und [Überprüfen von Testsendungen im Desktop Proofing Viewer](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer).

1. **Neue Version** - Der Projekt-Manager erstellt eine neue Version (oder eine Kopie) des Testversands und gibt ihn für den Client frei. Siehe [Kopieren von Testsendungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md) und [Freigeben eines Testversands in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

1. **Neue Testversand-E-Mail** - der Kunde erhält die E-Mail zum neuen Testversand mit dem Link [!UICONTROL Gehe zu Testversand] . Weitere Informationen finden Sie unter [Neue Testversand-E-Mail](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

1. **[!UICONTROL Testversand überprüfen]** - der Kunde überprüft den Testversand, fügt Kommentare hinzu und trifft eine Entscheidung.
1. Der Kunde kann nur die Version des Testversands sehen, der explizit für ihn freigegeben wurde. Er kann die interne Version nicht sehen.
1. **[!UICONTROL E-Mail-Warnhinweis]** - Der Projektmanager erhält eine E-Mail mit einer Zusammenfassung der Überprüfung durch den Kunden (je nach den Einstellungen für den Testversand).
1. **Anforderung ändern** - Der Projekt-Manager informiert den Designer über die Änderungsanforderungen. Dies kann mithilfe der Druckkommentar-Funktion erfolgen. Weitere Informationen finden Sie unter [Drucken und Exportieren von Kommentaren in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/print-and-export-comments.md).

1. **Neue Version** (falls erforderlich) - der Designer ändert die Datei und lädt sie als neue Version in [!DNL Workfront Proof] hoch. Weitere Informationen finden Sie unter .

Sie können diesen Vorgang wiederholen, bis der Testversand validiert wurde.
