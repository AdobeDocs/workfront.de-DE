---
title: 20.4 Weitere Verbesserungen
description: 20.4 Weitere Verbesserungen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4 Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 20.4 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab dem 9. November 2020 verfügbar sein.

Eine Liste aller in Version 20.4 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Neu für Administratoren: Option der Workfront-Umgebung wechseln verfügbar

Für ein effizienteres und bequemeres Erlebnis können Gruppenadministratoren und Workfront-Administratoren jetzt schnell zwischen verschiedenen Workfront-Umgebungen von jeder Seite in Workfront wechseln, ohne sich abmelden zu müssen.

Im neuen Workfront-Erlebnis wird die Option Zu Classic wechseln im Hauptmenü angezeigt.

In Workfront Classic wird die Option Zum neuen Erlebnis wechseln im Menü angezeigt, das angezeigt wird, wenn Sie auf das Profilbild in der oberen rechten Ecke der Leiste für globale Navigation klicken.

Diese Funktion ist jetzt im [Administratorgrundlagen, Lernpfad in Teil 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) auf Workfront One.

## Verbesserte Verschlüsselung für Workfront Testversand

Wir nehmen einige Änderungen vor, um die Datenverschlüsselung der Workfront-Testversand-Anwendung für die Dateneingabe in Bewegung zu verbessern. Die schwachen TLS-Chiffren werden am 11. November 2020 eingestellt.

Stellen Sie sicher, dass Sie beim Zugriff auf Workfront einen unterstützten Browser verwenden. Weitere Informationen zu unterstützten Browsern finden Sie unter [Adobe Workfront-Browseranforderungen](../../../workfront-basics/workfront-browser-requirements.md).

## Neues Erscheinungsbild für 3 E-Mail-Vorlagen

Um die Lesbarkeit und das Gesamterlebnis zu verbessern, haben die folgenden E-Mail-Vorlagen ein neues Erscheinungsbild:

* Neue Arbeitsanfrage
* Eine abhängige Aufgabe, der Sie zugewiesen sind, kann jetzt gestartet werden
* Team-E-Mail-Benachrichtigung mit Vorgänger-Abschluss

Informationen zum Aktivieren von E-Mails für Testzwecke in Ihrer Vorschauumgebung finden Sie im Abschnitt E-Mails in der Vorschau verwalten unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Neue E-Mail-Benachrichtigungen für Teams

Wir haben die folgende E-Mail-Benachrichtigung für Teams hinzugefügt:

* Ein Vorgänger einer Aufgabe, die meinem Team zugewiesen wurde, ist abgeschlossen: Das zugewiesene Team erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben als abgeschlossen markiert wurde.
* Alle Vorgänger einer Aufgabe, die meinem Team zugewiesen wurde, sind abgeschlossen: Das zugewiesene Team erhält eine E-Mail-Benachrichtigung für jeden Vorgänger, der als abgeschlossen gekennzeichnet ist.

Weitere Informationen finden Sie unter [Benachrichtigungen: Informationen über die mir zugewiesenen Aufgaben](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## Neu für Administratoren: Verbesserungen bei E-Mail-Benachrichtigungen

Jetzt können Sie mit einem einzigen Klick eine Ereignis-E-Mail-Benachrichtigung in der Einrichtung aktivieren oder deaktivieren. Klicken Sie einfach auf den Ein/Aus-Schalter neben dem Namen der Benachrichtigung.

Beachten Sie außerdem, dass unser moderner Stil jetzt die Konfiguration von Ereignisbenachrichtigungen im Bereich E-Mail-Benachrichtigungen verbessert.

Informationen zum Konfigurieren von E-Mail-Benachrichtigungen finden Sie unter [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

Diese Funktion ist jetzt im [Lernpfad für E-Mail- und In-App-Benachrichtigungen](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) auf Workfront One.

## Neue API-Objekte, die die Trigger-Ereignisabonnement-Aktualisierung durchführen

Zwei neue API-Objekte, documentVersion und proofApproval, wurden erstellt und sind so konfiguriert, dass Trigger-Abonnementaktualisierungen durchgeführt werden, wenn ein Dokument versioniert oder genehmigt wird.

Eine vollständige Liste der Felder, die mit den einzelnen Objekten verknüpft sind, finden Sie unter [Ressourcen-Felder für Ereignisabonnements](../../../wf-api/api/event-sub-resource-fields.md).
