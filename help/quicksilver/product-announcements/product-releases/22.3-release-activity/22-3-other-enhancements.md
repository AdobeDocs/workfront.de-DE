---
title: sonstige Aktualisierungen während des Zeitrahmens der Version 22.3
description: sonstige Aktualisierungen während des Zeitrahmens der Version 22.3
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 2.3 Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 22.3 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 11. Juli 2022 bereitgestellt. Eine Liste aller in Version 22.3 verfügbaren Änderungen finden Sie unter [2.3 Versionsübersicht](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Aktualisierte Timesheets

Wir verbessern und aktualisieren Ihr Erlebnis bei der Arbeit mit Timesheets weiter. Die folgenden Funktionen sind in diesem Update enthalten:

* Ein neues Erscheinungsbild, das dem neuen Workfront-Erlebnis entspricht.

* Autosave-Funktion, um Ihre angemeldeten Stunden und Stunden-Kommentare automatisch zu speichern, wenn Sie sie in der Sekunde hinzufügen.

* Ein intuitiveres Seitenlayout für die Übereinstimmung mit anderen Objektseiten. Zum Beispiel haben wir dem Timesheet einen linken Bereich hinzugefügt. Die Timesheet-Aktualisierungen werden jetzt im Abschnitt Updates im linken Bereich angezeigt. Sie können auch ein Timesheet aus der Timesheet-Seite löschen und das Timesheet zu Ihrer Favoritenliste hinzufügen.

* Ein besseres Erlebnis beim Suchen und Hinzufügen von Projekten, Aufgaben oder Problemen zum Timesheet. Dies entspricht dem Erlebnis in allen anderen Listen in Workfront.

* Das Bedienfeld Zusammenfassung steht für Aufgaben und Probleme zum Hinzufügen von Kommentaren oder zum Aktualisieren von Informationen direkt vom Timesheet aus zur Verfügung.


Mit der aktuellen Aktualisierung wurden auch die folgenden Funktionen eingestellt:

* Das Erstellen einer Aufgabe aus einer Aktualisierung wurde entfernt. Diese Funktion wurde seit der Version 2018.2 aus den Aktualisierungsbereichen aller anderen Objekte entfernt, war jedoch weiterhin im Aktualisierungsstream des Zeitplans verfügbar.

* Die &quot;Aufwendungen aus einem Zeitblatt hinzufügen. &quot;Die Voreinstellung wurde aus dem Bereich &quot;Zeitblatt &amp; Stunden Voreinstellungen&quot;des Setups entfernt und Sie können die Ausgaben nicht mehr aus dem Zeitblatt protokollieren. Sie können die Ausgaben weiterhin über die Aufgaben- und Projektseiten protokollieren.


Weitere Informationen finden Sie in den folgenden Artikeln:

* [Grundlegendes zum Layout des Zeitplans](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Zeitblatt- und Stundenvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Verbesserungen am linken Navigationsbereich

Das linke Navigationsfenster in Adobe Workfront wurde um einige Verbesserungen erweitert.

* Das Erscheinungsbild des linken Navigationsfensters wurde auf die Designstandards der Adobe aktualisiert, einschließlich Farben und Schriftarten.

* Der Link &quot;Benutzerspezifischen Abschnitt hinzufügen&quot;am unteren Rand des Bedienfelds wurde in &quot;Dashboard hinzufügen&quot;umbenannt, um dessen Funktion besser zu erklären.

## Automatische Aktualisierung der Token-Rotation in Ihren benutzerdefinierten OAuth2-Anwendungen aktivieren

Um Ihnen mehr Kontrolle über die Sicherheit Ihrer benutzerdefinierten OAuth2-Anwendungen zu ermöglichen, haben wir die Option hinzugefügt, um die Rotation des Aktualisierungs-Tokens zu aktivieren. Wenn diese Option aktiviert ist, erstellt und sendet Ihre Anwendung jedes Mal, wenn ein Aktualisierungstoken verwendet wird, automatisch ein neues Aktualisierungstoken und deaktiviert das alte.

Ihr Programm muss das neue Aktualisierungstoken nach jeder Aktualisierung speichern. Workfront speichert dieses Aktualisierungstoken nicht.

Zuvor liefen Aktualisierungstoken nach einer bestimmten Zeitdauer ab, die in den benutzerdefinierten OAuth2-Anwendungseinstellungen konfiguriert war.

Weitere Informationen finden Sie unter [OAuth2-Anwendungen für Workfront-Integrationen erstellen](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Verwenden Sie PKCE in Ihren benutzerdefinierten OAuth2-Integrationen für Einzelseiten-Webanwendungen.

Sie können jetzt Single-Page-Webanwendungen in Ihren benutzerdefinierten Integrationen mit PKCE erstellen. PKCE ist ein sicherer Autorisierungsfluss, der gut mit dynamisch aktualisierten Anwendungen wie Apps funktioniert, aber für alle OAuth2-Clients nützlich ist. Statt eines statischen Client-Geheimnisses verwendet PKCE eine dynamisch generierte Zeichenfolge, wodurch das Risiko eines durchgesickerten Client-Geheimnisses entfällt.

Zuvor verwendeten die verfügbaren Optionen für benutzerdefinierte OAuth2-Anwendungen entweder den Namen und das Kennwort eines Benutzers oder ein Client-Geheimnis.

Weitere Informationen finden Sie unter [OAuth2-Anwendungen für Workfront-Integrationen erstellen](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
