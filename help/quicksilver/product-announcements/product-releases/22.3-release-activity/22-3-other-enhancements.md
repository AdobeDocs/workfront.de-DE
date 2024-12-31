---
title: Weitere Updates während des Zeitrahmens der Version 22.3
description: Weitere Updates während des Zeitrahmens der Version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 22.3 Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 22.3 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 11. Juli 2022 in der Produktionsumgebung verfügbar gemacht. Eine Liste aller mit Version 22.3 verfügbaren Änderungen finden Sie unter Übersicht über die Version [22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Aktualisierte Arbeitszeittabellen

Wir verbessern und aktualisieren Ihr Erlebnis bei der Arbeit mit Arbeitszeittabellen kontinuierlich. Im Folgenden finden Sie einige der Funktionen, die in diesem Update enthalten sind:

* Ein neues Look-and-Feel, das dem neuen Workfront-Erlebnis entspricht.

* Funktion zum automatischen Speichern der protokollierten Stunden und Stundenkommentare, sobald diese hinzugefügt werden.

* Ein intuitiveres Seiten-Layout für andere Objektseiten. Beispielsweise haben wir der Arbeitszeittabelle ein linkes Bedienfeld hinzugefügt. Die Aktualisierungen der Arbeitszeittabelle werden jetzt im Abschnitt Aktualisierungen im linken Bereich angezeigt. Sie können auch eine Arbeitszeittabelle aus der Arbeitszeittabellen-Seite löschen und die Arbeitszeittabelle zur Favoritenliste hinzufügen.

* Ein besseres Erlebnis bei der Suche und beim Hinzufügen von Projekten, Aufgaben oder Problemen zur Arbeitszeittabelle. Dies entspricht dem Erlebnis in allen anderen Listen in Workfront.

* Das Bedienfeld Zusammenfassung steht direkt über die Arbeitszeittabelle für Aufgaben und Probleme zum Hinzufügen von Kommentaren oder Aktualisieren von Informationen zur Verfügung.


Mit dem aktuellen Update haben wir auch die folgenden Funktionen eingestellt:

* Das Erstellen einer Aufgabe aus einer Aktualisierung wurde entfernt. Diese Funktion wurde seit der Version 2018.2 aus den Bereichen Aktualisierungen aller anderen Objekte entfernt, war jedoch weiterhin im Arbeitszeittabellen-Aktualisierungsverlauf verfügbar.

* Die Option „Kosten aus einer Arbeitszeittabelle hinzufügen“. „Die Voreinstellung wurde aus dem Bereich Arbeitszeittabellen- und Stunden-Voreinstellungen von Setup entfernt, und Sie können keine Ausgaben mehr in der Arbeitszeittabelle protokollieren. Sie können Ausgaben weiterhin auf den Aufgaben- und Projektseiten protokollieren.


Weitere Informationen finden Sie in den folgenden Artikeln:

* [Arbeitszeittabellen-Layout verstehen](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Arbeitszeittabelle und Stundeneinstellungen konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Verbesserungen am linken Navigationsbereich

Das linke Navigationsfenster in Adobe Workfront wurde mehrfach verbessert.

* Das Erscheinungsbild des linken Navigationsbereichs wurde auf die Adobe-Designstandards aktualisiert, einschließlich Farben und Schriftarten.

* Der Link „Benutzerdefinierten Abschnitt hinzufügen“ am unteren Rand des Bedienfelds wurde in „Dashboard hinzufügen“ umbenannt, um die Funktion besser zu erklären.

## Aktivieren der automatischen Token-Rotation in Ihren benutzerdefinierten OAuth2-Anwendungen

Um Ihnen mehr Kontrolle über die Sicherheit Ihrer benutzerdefinierten OAuth2-Programme zu ermöglichen, haben wir die Option hinzugefügt, die Token-Rotation zu aktualisieren. Wenn diese Option aktiviert ist, erstellt und sendet Ihre Anwendung jedes Mal, wenn ein Aktualisierungstoken verwendet wird, automatisch ein neues Aktualisierungstoken und deaktiviert das alte.

Die Anwendung muss das neue Aktualisierungstoken nach jeder Aktualisierung speichern. Workfront speichert dieses Aktualisierungstoken nicht.

Zuvor waren Aktualisierungstoken abgelaufen, nachdem eine bestimmte Zeitdauer in den benutzerdefinierten OAuth2-Anwendungseinstellungen konfiguriert wurde.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Verwenden von PKCE in Ihren benutzerdefinierten OAuth2-Integrationen für Single-Page-Web-Anwendungen

Sie können jetzt Single Page Applications (SPAs) in Ihren benutzerdefinierten Integrationen mithilfe von PKCE erstellen. PKCE ist ein sicherer Autorisierungsfluss, der gut mit dynamisch aktualisierten Programmen wie mobilen Apps funktioniert, aber für alle OAuth2-Clients nützlich ist. Anstelle eines statischen Client-Geheimnisses verwendet PKCE eine dynamisch generierte Zeichenfolge, wodurch das Risiko eines Lecks des Client-Geheimnisses vermieden wird.

Zuvor verwendeten die verfügbaren Optionen für benutzerdefinierte OAuth2-Anwendungen entweder den Namen und das Kennwort eines Benutzers oder ein Client-Geheimnis.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
