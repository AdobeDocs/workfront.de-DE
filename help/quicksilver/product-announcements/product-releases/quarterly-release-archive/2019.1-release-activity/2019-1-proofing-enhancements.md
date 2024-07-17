---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Testversandverbesserungen
description: Auf dieser Seite werden alle in Version 2019.1 enthaltenen Verbesserungen bei der Überprüfung beschrieben. Die Funktion ist jetzt in der Produktionsumgebung verfügbar.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# 2019.1 Testversandverbesserungen

Auf dieser Seite werden alle in Version 2019.1 enthaltenen Verbesserungen bei der Überprüfung beschrieben. Die Funktion ist jetzt in der Produktionsumgebung verfügbar.

Eine Liste aller Änderungen, die in Version 2019.1 vorgenommen wurden, finden Sie unter [Übersicht über die Release-Aktivität 2019.1}.](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md)

## Für Administratoren

* [Konfigurieren der standardmäßigen Testversand-Rolle für Nicht-Empfänger, die einen Testversand öffnen](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## Für alle Benutzer

* [Testen interaktiver Inhalte im Web Proofing Viewer](#proof-interactive-content-in-the-web-proofing-viewer)
* [Die standardmäßige Sortierreihenfolge für Kommentare im Testversand-Viewer ist jetzt von alt auf neu](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [Verbesserte Überprüfung für Kommentare im Testversand-Viewer, der mit einem Videobereich verknüpft ist](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [Link zu Dokumentdetails von einer Benachrichtigung zum Testversand oder dem Testversand-Viewer](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [Ändern Ihrer E-Mail-Benachrichtigungen im Testversand-Viewer](#change-your-email-notifications-in-the-proofing-viewer)
* [Ändern der Hintergrundfarbe im Desktop Proofing Viewer](#change-the-background-color-in-the-desktop-proofing-viewer)
* [Löschen zwischengespeicherter Browserdaten aus einem Testversand im Desktop Testversand-Viewer](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## Konfigurieren der standardmäßigen Testversand-Rolle für Nicht-Empfänger, die einen Testversand öffnen {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Workfront-Administratoren können jetzt die standardmäßige Testversandrolle für Benutzer konfigurieren, die im Testversand-Workflow nicht als Zielgruppe bestimmt wurden, aber über ihr Workfront-Objekt (z. B. Projekt, Aufgabe oder Problem) auf den Testversand zugreifen können.

Bisher war die standardmäßige Testfunktion von Benutzern und Gästen, die Zugriff auf einen Testversand hatten, ohne zum Workflow hinzugefügt zu werden, &quot;Überprüfer&quot;.

Diese Funktion gilt nur für Testsendungen, die in Workfront und nicht in Workfront Proof erstellt wurden.

## Testen interaktiver Inhalte im Web Proofing-Viewer {#proof-interactive-content-in-the-web-proofing-viewer}

Wenn die Sicherheitsrichtlinien Ihres Unternehmens die Verwendung der Standalone Desktop Proofing Viewer App nicht zulassen, kann Ihr Workfront-Administrator jetzt interaktive Inhalte im Web Proofing Viewer aktivieren. Der Inhalt muss in einer ZIP-Datei gebündelt werden, bevor Sie den Testversand erstellen.

Weitere Informationen finden Sie im Artikel .

VIDEO

## Die standardmäßige Sortierreihenfolge für Kommentare im Testversand-Viewer ist jetzt von alt auf neu  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

Im Testversand-Viewer ist die standardmäßige Sortierreihenfolge für Kommentare zu einem Testversand jetzt von alt zu neueste, wie in einer verbalen Konversation.

Zuvor war die standardmäßige Sortierreihenfolge von Neueste zu Älteste.

Sie können eine andere Sortieroption auswählen, die für alle anderen Testsendungen gespeichert wird, die Sie öffnen.

Weitere Informationen finden Sie im Abschnitt im Artikel .

## Erweiterte Überprüfung für Kommentare im Testversand-Viewer, der mit einem Videobereich verknüpft ist {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

Wenn Sie einen Kommentar überprüfen, der mit einer Reihe von Videobildern im Proofing-Viewer verknüpft ist, können Sie jetzt auf Abspielen klicken, um den gesamten Bereich des Filmmaterials anzuzeigen. Die Wiedergabe wird angehalten, wenn sie das Ende des Bereichs erreicht. Der Kommentar bleibt offen, damit Sie nicht verlieren, wo Sie sind.

Zuvor mussten Sie beim Öffnen eines Kommentars für eine Reihe von Videobildern manuell den Anfang des Bereichs finden, indem Sie sich die im Kommentar angezeigten Bildnummern ansehen, bevor Sie auf Abspielen klicken. Andernfalls begann die Wiedergabe des Testversand-Viewers überall dort, wo Sie zuletzt in der Video-Timeline geklickt haben, und sie wurde am Ende des Bereichs nicht angehalten. Außerdem wurde der Kommentar beim Klicken auf Abspielen ausgeblendet, sodass nicht mehr klar war, welcher Kommentar Sie überprüft haben.

Informationen zum Überprüfen von Videoproofs finden Sie unter .

VIDEO

## Link zu Dokumentdetails über eine Testbenachrichtigung oder den Testversand-Viewer {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

Wenn Sie eine E-Mail erhalten, in der Sie zur Überprüfung eines Testversands eingeladen werden, oder Sie einen Testversand im Testversand-Viewer durchführen, können Sie jetzt schnell auf die Seite mit den Dokumentdetails für den Testversand zugreifen. Auf dieser Seite können Sie das Workfront-Objekt (z. B. eine Aufgabe, ein Projekt oder ein Problem) sehen, das mit dem Testversand verknüpft ist. Dies bietet Kontext, der Ihnen dabei hilft, die Arbeit zu verstehen, die Sie für den Testversand benötigen.

Diese Funktion funktioniert möglicherweise nur für neue Benutzer, die Sie Ihrem System hinzufügen. Dieses Problem ist vorübergehend.

Weitere Informationen finden Sie im Artikel .

VIDEO

## E-Mail-Benachrichtigungen im Testversand-Viewer ändern {#change-your-email-notifications-in-the-proofing-viewer}

Jetzt können alle Testversandvalidierer angeben, welche Testversandbenachrichtigungen sie für einen Testversand erhalten möchten. Dies ist besonders wichtig bei der Zusammenarbeit mit externen Interessengruppen.

Zuvor konnte nur der Testversand-Eigentümer oder Traffic-Manager die E-Mail-Warnungen eines Testversands für die Validierer konfigurieren, die er zum Testversand hinzugefügt hat. Externe Mitarbeiter konnten nicht steuern, welche E-Mail-Warnungen sie über den Testversand erhalten haben, da sie weder über den erforderlichen Zugriff auf Workfront noch über die entsprechende Berechtigungsstufe verfügten.

Diese Einstellungen unterscheiden sich von den E-Mail-Warnhinweiseinstellungen, die Sie in Workfront konfigurieren können.

Weitere Informationen finden Sie unter [Benachrichtigungen für Testversand-Kommentare und -Entscheidungen verwalten](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)

VIDEO

## Ändern der Hintergrundfarbe im Desktop Proofing Viewer {#change-the-background-color-in-the-desktop-proofing-viewer}

Jetzt können Sie die Hintergrundfarbe des Desktop Proofing-Viewers von der standardmäßigen nahezu schwarzen Farbe in Weiß ändern. Dies erleichtert die Anzeige von Testsendungen mit transparentem Hintergrund.

Weitere Informationen finden Sie unter [Konfigurieren der Testversand-Viewer-Einstellungen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDEO

## Löschen zwischengespeicherter Browserdaten aus einem Testversand im Desktop Testversand-Viewer {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

Wenn die Cookie- und Cache-Einstellungen Ihres Browsers so eingestellt sind, dass Inhalte wie Popups blockiert werden, kann dieses Blockierungsverhalten auch im Desktop Proofing Viewer auftreten, sodass Prüfer den Popup-Inhalt in Ihrem Testversand nicht sehen und kommentieren können.

Jetzt können Sie die Browser-Cache-Daten löschen, die möglicherweise mit einem Testversand gespeichert werden, sodass alle Inhalte im Desktop Proofing Viewer angezeigt werden und Überprüfer sie sehen und kommentieren können.

Weitere Informationen finden Sie unter [Konfigurieren der Testversand-Viewer-Einstellungen](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

VIDEO
