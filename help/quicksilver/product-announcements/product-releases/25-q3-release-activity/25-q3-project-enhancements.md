---
title: Projektverbesserungen im dritten Quartal 2025
description: Projektverbesserungen im dritten Quartal 2025
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: a5a61045bad5a97fb1413fac4a5a2666b753fa83
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Projektverbesserungen im dritten Quartal 2025

Auf dieser Seite werden die mit der Version vom dritten Quartal 2025 vorgenommenen Projektverbesserungen für die Vorschau-Umgebung beschrieben. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2025 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Änderung der Art und Weise, wie die tatsächlichen Stunden für API-Aufrufe in der Datenbank gespeichert werden

>[!NOTE]
>
>* Vorschau: 27. Mai 2025
>* Produktions-Schnellveröffentlichung: 27. Mai 2025
>* Produktion für alle Kunden: 27. Mai 2025

Diese Aktualisierung führt zu einer Änderung der Art und Weise, wie die tatsächlichen Stunden für Projekte, Aufgaben und Probleme in der Datenbank gespeichert werden. Ab dieser Aktualisierung verwenden die tatsächlichen Stunden ein `actualWorkRequiredDouble` (mit einem Wert in Stunden).

Vor diesem Update wurden die tatsächlichen Stunden mit einem Wert von `actualWorkRequired` (mit einem Wert in Minuten) gespeichert. Diese Aktualisierung stellt sicher, dass die tatsächlichen Stunden bei der Berechnung mithilfe eines API-Aufrufs genauer gezählt werden.

Aufgrund dieser Änderung müssen Sie möglicherweise alle API-Aufrufe aktualisieren, die auf das ursprüngliche Wertfeld verweisen. Sie sollten keine Änderungen vornehmen, wenn Sie in den API-Aufrufen ein Wertefeld von `actualWorkRequiredExpression` verwenden.

Diese Aktualisierung ändert nicht die Berechnungen für die tatsächlichen Stunden für Projekte, Aufgaben und Probleme in Spalten mit berechneten benutzerdefinierten Feldern.

## Aktualisierung in mithilfe des Schiebereglers Prozent abgeschlossen in einer Aufgaben- oder Problem-Kopfzeile

>[!NOTE]
>
>* Vorschau: 27. Mai 2025
>* Produktions-Schnellveröffentlichung: 27. Mai 2025
>* Produktion für alle Kunden: 27. Mai 2025

Die Funktionsweise des Schiebereglers Prozent abgeschlossen für Aufgaben und Probleme wurde aktualisiert.

Die folgende Funktion ist jetzt verfügbar:

* Wenn Sie die blaue Blase Prozent abgeschlossen in die Kopfzeile einer Aufgabe oder eines Problems schieben, wird der Prozentsatz der Fertigstellung der Aufgabe oder des Problems jetzt in Schritten von fünf Punkten aktualisiert. Vor diesem Update wurden durch Schieben der blauen Blase Prozent abgeschlossen die Aufgaben oder Probleme in Schritten von einem Punkt aktualisiert.

* Sie können auf die blaue Blase doppelklicken und sie manuell mit einer beliebigen Zahl aktualisieren, ohne den Schieberegler zu verwenden. Diese Funktion hat sich nicht geändert.

Es wurden keine weiteren Änderungen zur Aktualisierung des Prozentsatzes der abgeschlossenen Aufgaben und Probleme in anderen Bereichen von Workfront eingeführt.

Weitere Informationen finden Sie unter [Anzeigen und Aktualisieren des Prozentsatzes für abgeschlossene Aufgaben](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

## Mehr Transparenz bei der Verwendung des KI-Assistenten für Projekte, Aufgaben und Probleme

>[!NOTE]
>
>* Vorschau: 19. Mai 2025
>* Produktions-Schnellveröffentlichung: 19. Mai 2025
>* Produktion für alle Kunden: 19. Mai 2025

Um klarer zu machen, wie der KI-Assistent Antworten auf Fragen zu Workfront-Projekten, -Aufgaben und -Problemen findet, haben wir diese Informationen zur Frageantwort hinzugefügt. Jetzt fügt der KI-Assistent seine Suchinformationen in die Ausgabe ein. Sie können diese Informationen verwenden, um zu überprüfen, ob der KI-Assistent die von Ihnen gestellte Frage korrekt identifiziert hat, und um den Kontext der Antwort zu verstehen.

Zuvor waren diese Informationen in der Antwort des KI-Assistenten nicht verfügbar.

Informationen zur Verwendung des KI-Assistenten, um Informationen zu Workfront-Elementen zu erhalten, finden [ unter „Verwenden des KI-Assistenten zur Arbeit mit Projekten, Aufgaben und Problemen](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).
