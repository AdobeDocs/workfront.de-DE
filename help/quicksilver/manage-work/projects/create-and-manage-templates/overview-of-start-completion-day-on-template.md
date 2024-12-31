---
product-area: templates
navigation-topic: templates-navigation-topic
title: Übersicht über Start- und Abschlusstage in einer Vorlage
description: Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind. Während Projekte bestimmte Start- und Abschlussdaten haben, haben Vorlagen allgemeine Start- und Abschlusstage, die angeben, wo diese Termine auf das Projekt fallen, basierend auf der gesamten Zeitleiste des Projekts.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Übersicht über Start- und Abschlusstage in einer Vorlage

Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind. Während Projekte bestimmte Start- und Abschlussdaten haben, haben Vorlagen allgemeine Start- und Abschlusstage, die angeben, wo diese Termine auf das Projekt fallen, basierend auf der gesamten Zeitleiste des Projekts.

**Beispiel** Wenn das Startdatum eines Projekts der 1. April ist und Sie möchten, dass eine Aufgabe am 3. April (zwei Tage nach dem Projektstart) beginnt, sollte die entsprechende Aufgabe in der Vorlage, die das Projekt erstellt, am 2. Tag der Vorlage beginnen, wobei der erste Tag der Vorlage als Tag 0 gilt.

## Starttag

Beachten Sie beim Arbeiten mit Vorlagen und Vorlagenaufgaben Folgendes:

* Standardmäßig haben Vorlagen den Starttag 0 und die Vorlagenaufgaben und die Vorlage zeigen den Starttag 0 an. Der Starttag der Vorlagenaufgaben kann sich ändern, aber das ändert nichts am Starttag der Vorlage.
* Der Starttag einer Vorlagenaufgabe stellt die Anzahl der Werktage dar, die Workfront zum geplanten Startdatum der Aufgabe hinzufügt, wenn ein Projekt aus der Vorlage erstellt wird. Beispiel: Sie haben eine Vorlage mit nur einer Aufgabe und der Starttag der Vorlagenaufgabe ist 4. Der Starttag der Vorlage ist immer noch 0. Wenn Sie ein Projekt in dieser Vorlage erstellen, dessen Planungsmodus das Startdatum und das geplante Startdatum des Projekts der 1. November 2019 ist, fügt die neu erstellte Aufgabe diesem Datum 4 Tage hinzu und setzt ihren Wert für das geplante Startdatum auf den 5. November 2019.

Im Folgenden finden Sie einige Aktionen, die den Starttag der Vorlagenaufgaben ändern können:

* Aktualisieren der Dauer von Vorgänger-Vorlagenaufgaben
* Aufgabenbeschränkungen aktualisieren

  Bei Verwendung datumsbasierter Aufgabenbeschränkungen können Sie den Starttag der Vorlagenaufgaben manuell aktualisieren. Einige Beispiele für datumsbasierte Aufgabeneinschränkungen sind feste Termine, Beginn nicht früher als, Start nicht später als, muss am beginnen.

* Vorlagenaufgabe-Vorgänger aktualisieren

## Tag der Fertigstellung

Der Abschlusstag der Vorlage ist der Tag, an dem die letzte Vorlagenaufgabe abgeschlossen ist. Standardmäßig weisen alle Vorlagenaufgaben und die Vorlage den Abschlusstag 1 auf, da Workfront davon ausgeht, dass jede Vorlagenaufgabe eine Dauer von 1 Tag hat. Das Abschlussdatum der Vorlagenaufgaben kann sich ändern, was sich auch auf das Abschlussdatum der Vorlage auswirkt. Der Tag der Fertigstellung der Vorlage wird zum geplanten Abschlussdatum des zukünftigen Projekts und die Tage der Fertigstellung der Vorlagenaufgaben werden zu den geplanten Abschlussdaten der zukünftigen Projektaufgaben.

Im Folgenden finden Sie einige Aktionen, die den Abschlusstag der Vorlagenaufgaben ändern können:

* Aktualisieren der Dauer der Vorlagenaufgaben
* Aufgabenbeschränkungen aktualisieren

  Bei Verwendung datumsbasierter Aufgabenbeschränkungen können Sie das Abschlussdatum der Vorlagenaufgaben manuell aktualisieren. Einige Beispiele für datumsbasierte Aufgabeneinschränkungen sind feste Termine, Beenden nicht früher als, Beenden nicht später als, Muss Beenden am.

* Vorlagenaufgabe-Vorgänger aktualisieren

## Arbeiten mit Vorlagen, deren Abschluss geplant ist

Sie können eine Vorlage ab dem Abschlusstag planen. Weitere Informationen finden Sie unter [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Beachten Sie beim Arbeiten mit Vorlagen, die ab dem Abschlussdatum geplant sind, Folgendes:

* Wenn Sie den Anfangstag ändern, wird die Aufgabenbeschränkung auf „Start am“ festgelegt.
* Wenn Sie das Abschlussdatum ändern, wird die Aufgabenbeschränkung auf „Muss abgeschlossen sein am“ gesetzt.
* Wenn die Vorlage für den Abschlusstag geplant ist, wird der Einschränkungstag für Aufgaben auf Basis des Abschlusstages berechnet.

  **Beispiel** Die Dauer Ihrer Vorlage beträgt 285 Tage, und Sie haben eine Vorlagenaufgabe mit einer Dauer von 60 Tagen. Wenn Sie die Aufgabenbeschränkung auf „Start am“ und den Einschränkungstag auf 120 setzen, haben Sie einen Starttag von 165 (285 - 120) und einen Abschlusstag von 225 (165 + 60). Wenn Sie also den Starttag bearbeiten, wird er tatsächlich als Einschränkungstag interpretiert.
