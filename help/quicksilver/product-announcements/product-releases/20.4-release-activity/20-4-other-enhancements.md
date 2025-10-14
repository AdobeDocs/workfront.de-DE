---
title: 20.4 Weitere Verbesserungen
description: 20.4 Weitere Verbesserungen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4 Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 20.4 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 9. November 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 20.4 verfügbaren Änderungen finden Sie unter Übersicht über Version [20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Neu für Administratoren: Option &quot;Workfront-Umgebung wechseln“ verfügbar

Für ein effizienteres und bequemeres Erlebnis können Gruppenadministratoren und Workfront-Administratoren jetzt schnell von einer beliebigen Seite in Workfront aus zwischen verschiedenen Workfront-Umgebungen wechseln, ohne sich abmelden zu müssen.

In der neuen Workfront-Version wird die Option Zu Classic wechseln im Hauptmenü angezeigt.

In Workfront Classic wird die Option Zum neuen Erlebnis wechseln im Menü angezeigt, das beim Klicken auf das Profilbild oben rechts in der globalen Navigationsleiste angezeigt wird.

Diese Funktion ist jetzt in den [Administrator-Grundlagen, Teil 1 des Lernpfads](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/home) in Workfront One enthalten.

## Verbesserte Verschlüsselung für Workfront Proof

Wir nehmen einige Änderungen vor, um die Verschlüsselung von Daten in Bewegung durch die Workfront Proofing Application zu verbessern. Die schwachen TLS-Chiffren werden am 11. November 2020 eingestellt.

Bitte stellen Sie sicher, dass Sie beim Zugriff auf Workfront einen unterstützten Browser verwenden. Weitere Informationen zu unterstützten Browsern finden Sie unter [Adobe Workfront-Browser-Anforderungen](../../../workfront-basics/workfront-browser-requirements.md).

## Neues Erscheinungsbild für drei E-Mail-Vorlagen

Um die Lesbarkeit und das Gesamterlebnis zu verbessern, haben die folgenden E-Mail-Vorlagen ein neues Erscheinungsbild:

* Neue Arbeitsanfrage
* Eine Ihnen zugewiesene abhängige Aufgabe ist jetzt startbereit
* E-Mail-Benachrichtigung des Teams mit Vorgänger abgeschlossen

Informationen zum Aktivieren von E-Mails für Testzwecke in der Vorschau-Umgebung finden Sie im Abschnitt Verwalten von E-Mails in der Vorschau unter [Eigene E-Mail-Benachrichtigungen ändern](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Neue E-Mail-Benachrichtigungen für Teams

Wir haben die folgende E-Mail-Benachrichtigung für Teams hinzugefügt:

* Ein Vorgänger einer meinem Team zugewiesenen Aufgabe ist abgeschlossen: Das zugewiesene Team erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben als abgeschlossen markiert ist.
* Alle Vorgänger einer meinem Team zugewiesenen Aufgabe sind abgeschlossen: Das zugewiesene Team erhält für jeden Vorgänger, der als abgeschlossen markiert ist, eine E-Mail-Benachrichtigung.

Weitere Informationen finden Sie unter [Benachrichtigungen: Informationen zu meiner Arbeit](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Neu für Administratoren: Verbesserungen bei E-Mail-Benachrichtigungen

Jetzt können Sie mit einem einzigen Klick in Setup eine Ereignis-E-Mail-Benachrichtigung aktivieren oder deaktivieren. Klicken Sie einfach auf den Ein-/Aus-Schalter neben dem Namen der Benachrichtigung.

Beachten Sie außerdem, dass unser moderner Stil die Konfiguration von Ereignisbenachrichtigungen im Bereich E-Mail-Benachrichtigungen jetzt verbessert.

Informationen zum Konfigurieren von E-Mail-Benachrichtigungen finden [&#x200B; unter „Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Diese Funktion ist jetzt im Lernpfad [E-Mail- und In-App-Benachrichtigungen“ &#x200B;](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/home) Workfront One enthalten.

## Neue API-Objekte, die Trigger-Ereignisabonnement-Aktualisierungen aufweisen

Zwei neue API-Objekte, DocumentVersion und ProofApproval, wurden erstellt und sind so konfiguriert, dass Ereignisabonnementaktualisierungen beim Versionieren oder Genehmigen eines Dokuments Trigger werden.

Eine vollständige Liste der mit jedem Objekt verknüpften Felder finden Sie unter [Ressourcenfelder für Ereignisabonnements](../../../wf-api/api/event-sub-resource-fields.md).
