---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Korrekturabzug-Verbesserungen für 2019.1
description: Auf dieser Seite werden alle in der Version 2019.1 enthaltenen Proofing-Verbesserungen beschrieben. Die Funktion ist jetzt in der Produktionsumgebung verfügbar.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Korrekturabzug-Verbesserungen für 2019.1

Auf dieser Seite werden alle in der Version 2019.1 enthaltenen Proofing-Verbesserungen beschrieben. Die Funktion ist jetzt in der Produktionsumgebung verfügbar.

Eine Liste aller in 2019.1 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität von 2019.1](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md).

## Für Administratoren

* [Standard-Proofing-Rolle für Nicht-Empfänger konfigurieren, die einen Korrekturabzug öffnen](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## Für alle Benutzer

* [Korrekturabzug für interaktive Inhalte in der Web-Korrekturabzugsanzeige](#proof-interactive-content-in-the-web-proofing-viewer)
* [Die standardmäßige Sortierreihenfolge für Kommentare im Proofing Viewer ist jetzt von „Von alt nach aktuell“](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [Verbesserte Überprüfung von Kommentaren im Proofing Viewer, der mit einer Reihe von Videos verknüpft ist](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [Link zu Dokumentdetails aus einer Korrekturabzugsbenachrichtigung oder der Proofing Viewer](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [Ändern von E-Mail-Benachrichtigungen im Proofing Viewer](#change-your-email-notifications-in-the-proofing-viewer)
* [Ändern der Hintergrundfarbe im Desktop Proofing Viewer](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Löschen zwischengespeicherter Browser-Daten aus einem Korrekturabzug im Desktop Proofing Viewer](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Standard-Proofing-Rolle für Nicht-Empfänger konfigurieren, die einen Korrekturabzug öffnen {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Workfront-Admins können jetzt die standardmäßige Proofing-Rolle für Benutzende konfigurieren, die keine designierten Empfängerinnen und Empfänger im Workflow des Korrekturabzugs sind, aber über das zugehörige Workfront-Objekt (z. B. Projekt, Aufgabe oder Problem) Zugriff auf den Korrekturabzug haben.

Zuvor war die standardmäßige Proofing-Rolle von Benutzern und Gästen, die Zugriff auf einen Korrekturabzug hatten, ohne zum Workflow hinzugefügt zu werden, „Prüfer“.

Diese Funktion gilt nur für Korrekturabzüge, die in Workfront und nicht in Workfront Proof erstellt wurden.

## Korrekturabzug für interaktive Inhalte in der Web-Korrekturabzugsanzeige {#proof-interactive-content-in-the-web-proofing-viewer}

Wenn die Sicherheitsrichtlinien Ihres Unternehmens die Verwendung der eigenständigen Desktop Proofing Viewer-App nicht zulassen, kann Ihr Workfront-Administrator jetzt interaktive Inhalte im Web Proofing Viewer aktivieren. Der Inhalt muss in einer ZIP-Datei gebündelt werden, bevor Sie den Korrekturabzug erstellen.

Weitere Informationen finden Sie im Artikel .

VIDEO

## Die standardmäßige Sortierreihenfolge für Kommentare im Proofing Viewer ist jetzt von „Von alt nach aktuell“  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

In der Proofing Viewer ist die standardmäßige Sortierreihenfolge für Kommentare zu einem Korrekturabzug jetzt von Alt nach Neu , wie in einer verbalen Konversation.

Zuvor war die Standard-Sortierreihenfolge Spätestes zu Ältestes.

Sie können eine andere Sortieroption auswählen. Diese wird für alle anderen von Ihnen geöffneten Korrekturabzüge gespeichert.

Weitere Informationen finden Sie im Abschnitt des Artikels .

## Die Überprüfung von Kommentaren im Proofing Viewer, die mit einer Reihe von Videos verknüpft sind, wurde verbessert {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

Wenn Sie einen Kommentar durchgehen, der mit einer Reihe von Videomaterial in der Proofing Viewer verknüpft ist, können Sie jetzt auf Abspielen klicken, um das gesamte Spektrum von Filmmaterial anzuzeigen. Die Wiedergabe wird angehalten, wenn sie das Ende des Bereichs erreicht. Der Kommentar bleibt offen, sodass Sie nicht den Überblick verlieren, wo Sie sind.

Zuvor mussten Sie beim Öffnen eines Kommentars für eine Reihe von Videomaterial den Anfang des Bereichs manuell finden, indem Sie sich die im Kommentar angezeigten Framenummern ansahen, bevor Sie auf Abspielen klicken. Andernfalls begann die Korrekturabzugsanzeige mit der Wiedergabe an den Stellen, an denen Sie das letzte Mal in der Video-Zeitleiste geklickt haben, und wurde am Ende des Bereichs nicht angehalten. Außerdem wurde der Kommentar ausgeblendet, wenn Sie auf „Abspielen“ geklickt haben, sodass nicht mehr klar war, welchen Kommentar Sie geprüft haben.

Informationen zum Überprüfen von Videoprüfungen finden Sie unter .

VIDEO

## Link zu Dokumentdetails aus einer Korrekturabzugsbenachrichtigung oder der Korrekturabzugsanzeige {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

Wenn Sie eine E-Mail erhalten, in der Sie eingeladen werden, einen Korrekturabzug zu prüfen, oder einen Korrekturabzug in der Korrekturabzugsansicht prüfen, können Sie jetzt schnell auf die Dokumentdetailseite für den Korrekturabzug zugreifen. Auf dieser Seite wird das Workfront-Objekt (z. B. eine Aufgabe, ein Projekt oder ein Problem) angezeigt, das mit dem Korrekturabzug verknüpft ist. Dies bietet Kontext, der Ihnen dabei hilft, die Arbeit zu verstehen, die Sie am Korrekturabzug durchführen müssen.

Diese Funktion funktioniert möglicherweise nur für neue Benutzer, die Sie Ihrem System hinzufügen. Dieses Problem ist temporär.

Weitere Informationen finden Sie im Artikel .

VIDEO

## E-Mail-Benachrichtigungen in der Proofing-Anzeige ändern {#change-your-email-notifications-in-the-proofing-viewer}

Jetzt können alle Proofing-Reviewer angeben, welche Proofing-Benachrichtigungen sie für einen Korrekturabzug erhalten möchten. Dies ist besonders wichtig bei der Zusammenarbeit mit externen Stakeholdern.

Zuvor konnten nur der Testversand-Verantwortliche oder der Traffic-Manager die E-Mail-Warnungen für Testsendungen für die Prüfer konfigurieren, die sie zum Testversand hinzugefügt haben. Externe Mitwirkende konnten nicht steuern, welche E-Mail-Warnungen sie bezüglich des Korrekturabzugs erhalten haben, da sie weder über den erforderlichen Zugriff auf Workfront noch über die entsprechende Berechtigungsstufe verfügten.

Diese Einstellungen sind unabhängig von den E-Mail-Warnhinweiseinstellungen, die Sie in Workfront konfigurieren können.

Weitere Informationen finden Sie unter [Verwalten von Benachrichtigungen für Kommentare und Entscheidungen zu Korrekturabzügen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VIDEO

## Ändern der Hintergrundfarbe im Desktop Proofing Viewer {#change-the-background-color-in-the-desktop-proofing-viewer}

Jetzt können Sie die Hintergrundfarbe des Desktop Proofing Viewers von der Standardfarbe für Beinahe-Schwarz in Weiß ändern. Dies erleichtert die Anzeige von Korrekturabzugsinhalten mit transparentem Hintergrund.

Weitere Informationen finden Sie unter [Konfigurieren der Einstellungen für Proofing Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDEO

## Löschen zwischengespeicherter Browser-Daten aus einem Korrekturabzug im Desktop Proofing Viewer {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

Wenn die Cookie- und Cache-Einstellungen Ihres Browsers so eingestellt sind, dass Inhalte wie Popups blockiert werden, kann dieses Blockierverhalten auch im Desktop Proofing Viewer auftreten, sodass es für Prüfer unmöglich ist, den Popup-Inhalt in Ihrem Korrekturabzug zu sehen und zu kommentieren.

Jetzt können Sie die Browser-Cache-Daten löschen, die mit einem Korrekturabzug gespeichert werden können, damit alle Inhalte im Desktop Proofing Viewer angezeigt werden und Prüfer sie sehen und kommentieren können.

Weitere Informationen finden Sie unter [Konfigurieren der Einstellungen für Proofing Viewer](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDEO
