---
product-area: templates
navigation-topic: templates-navigation-topic
title: Übersicht über Start- und Endtage in einer Vorlage
description: Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind. Während Projekte bestimmte Start- und Enddatumswerte aufweisen, enthalten Vorlagen allgemeine Start- und Fertigstellungstage, die anhand des Gesamtzeitplans des Projekts zeigen, wohin diese Daten in das Projekt fallen.
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Übersicht über Start- und Endtage in einer Vorlage

Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind. Während Projekte bestimmte Start- und Enddatumswerte aufweisen, enthalten Vorlagen allgemeine Start- und Fertigstellungstage, die anhand des Gesamtzeitplans des Projekts zeigen, wohin diese Daten in das Projekt fallen.

**Beispiel:** Wenn das Startdatum eines Projekts der 1. April ist und Sie möchten, dass eine Aufgabe am 3. April (zwei Tage nach Projektbeginn) beginnt, sollte die entsprechende Aufgabe auf der Vorlage, die das Projekt erstellt, an Tag 2 der Vorlage beginnen, wobei der erste Tag der Vorlage als Tag 0 gilt.

## Starttag

Beachten Sie beim Arbeiten mit Vorlagen und Vorlagenaufgaben Folgendes:

* Standardmäßig haben Vorlagen den Starttag 0 und die Vorlagenaufgaben und die Vorlage den Starttag 0. Der Starttag der Vorlagenaufgaben kann sich ändern, aber der Starttag der Vorlage wird dadurch nicht geändert.
* Der Starttag einer Vorlagenaufgabe stellt die Anzahl der Geschäftstage dar, die Workfront dem geplanten Startdatum der Aufgabe hinzufügt, wenn ein Projekt aus der Vorlage erstellt wird. Sie können beispielsweise eine Vorlage mit nur einer Aufgabe und den Starttag der Vorlagenaufgabe 4 haben. Der Starttag der Vorlage ist immer noch 0. Wenn Sie ein Projekt aus dieser Vorlage erstellen, bei dem der Planungsmodus des Projekts &quot;Startdatum&quot;ist und das geplante Startdatum des Projekts der 1. November 2019 ist, fügt die neu erstellte Aufgabe diesem Datum 4 Tage hinzu und setzt den Wert für das geplante Startdatum auf den 5. November 2019.

Im Folgenden finden Sie einige Aktionen, die den Starttag der Vorlagenaufgaben ändern können:

* Aktualisieren der Dauer der Vorlagenaufgaben
* Aktualisieren der Aufgabenbegrenzungen

   Bei Verwendung datumsbasierter Aufgabenbegrenzungen können Sie den Starttag der Vorlagenaufgaben manuell aktualisieren. Beispiele für datumsbasierte Aufgabenbeschränkungen sind &quot;Feste Datumswerte&quot;, &quot;Anfang nicht früher als&quot;, &quot;Anfang nicht später als&quot;, &quot;Muss beginnen&quot;.

* Vorlagenaufgaben aktualisieren

## Tag der Fertigstellung

Der Abschlusstag der Vorlage ist der Tag, an dem die letzte Vorlagenaufgabe abgeschlossen ist. Standardmäßig wird für alle Vorlagenaufgaben und die Vorlage der Tag &quot;Abschluss&quot;von 1 angezeigt, da Workfront davon ausgeht, dass jede Vorlagenaufgabe eine Dauer von 1 Tag hat. Der Abschlusstag der Vorlagenaufgaben kann sich ändern. Dadurch wird auch der Abschlusstag der Vorlage geändert. Der Abschlusstag der Vorlage wird zum geplanten Abschlussdatum des künftigen Projekts und die Abschlusstage der Vorlagenaufgaben werden zu den geplanten Abschlussdaten der künftigen Projektaufgaben.

Im Folgenden finden Sie einige Aktionen, die den Fertigstellungstag der Vorlagenaufgaben ändern können:

* Aktualisieren der Dauer der Vorlagenaufgaben
* Aktualisieren der Aufgabenbegrenzungen

   Bei Verwendung datumsbasierter Aufgabenbegrenzungen können Sie den Abschlusstag der Vorlagenaufgaben manuell aktualisieren. Beispiele für datumsbasierte Aufgabenbeschränkungen sind &quot;Feste Datumswerte&quot;, &quot;Fertig stellen nicht früher als&quot;, &quot;Später beenden nicht&quot;und &quot;Fertig stellen am&quot;.

* Vorlagenaufgaben aktualisieren

## Arbeiten mit Vorlagen, die nach Abschluss geplant sind

Sie können eine Vorlage ab Fertigstellungstag planen. Weitere Informationen finden Sie unter [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Beachten Sie Folgendes bei der Arbeit mit Vorlagen, die ab dem Abschlussdatum geplant sind:

* Durch Ändern des Startdatums wird die Aufgabenbegrenzung auf &quot;Muss beginnen am&quot;gesetzt.
* Durch Ändern des Abschlussdatums wird die Aufgabenbegrenzung auf &quot;Must Finish On&quot;gesetzt.
* Wenn die Vorlage ab dem Abschlussdatum geplant ist, wird der Tag der Aufgabenbegrenzung ab dem Abschlussdatum berechnet.

   **Beispiel:** Die Dauer Ihrer Vorlage beträgt 285 Tage, und Sie haben eine Vorlagenaufgabe mit einer Dauer von 60 Tagen. Wenn Sie die Aufgabenbegrenzung auf &quot;Must Start On and Constraint Day&quot;auf &quot;120&quot;setzen, wird der Starttag 165 (285 - 120) und der Abschlusstag 225 (165 + 60) sein. Wenn Sie also den Starttag bearbeiten, wird er tatsächlich als Beschränkungstag interpretiert.
