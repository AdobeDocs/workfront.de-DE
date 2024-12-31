---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über geplante und geschätzte Termine
description: Es gibt verschiedene Datumstypen, die den zeitlichen Ablauf von Aufgaben zwischen dem Start und dem Abschluss anzeigen.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Übersicht über geplante und geschätzte Termine

<!--Audited: 07/2024-->

Es gibt verschiedene Datumstypen, die den zeitlichen Ablauf von Aufgaben zwischen dem Start und dem Abschluss anzeigen. Im Folgenden finden Sie einige Daten, die die Zeitleiste von Aufgaben anzeigen:

* Geplanter Start und geplante Abschlussdaten
* Voraussichtlicher Beginn und voraussichtliche Abschlussdaten
* Geschätzter Start und geschätzte Fälligkeitsdaten
* Tatsächliche Start- und Abschlussdaten

In diesem Artikel werden die Unterschiede zwischen den geschätzten und den voraussichtlichen Terminen für Projekte beschrieben.

Beim erstmaligen Erstellen der Aufgabe sollten die geplanten, prognostizierten und geschätzten Termine normalerweise übereinstimmen. Es gibt einige Ausnahmen.

Weitere Informationen zu Projekt-, Aufgaben- und Problemdaten in Adobe Workfront finden Sie [Übersicht über Projekt-, Aufgaben- und Problemdaten in Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Übersicht über geplante Termine

Die geplanten Termine sind die Termine, die der Projektbesitzer als Start- und Enddatum der Aufgaben definiert. Sie oder der Projektbesitzer können die geplanten Termine für eine Aufgabe manuell ändern.

## Übersicht über tatsächliche Termine

Wenn eine Aufgabe zum ersten Mal erstellt wird, hat sie keine tatsächlichen Daten, da sie noch nicht gestartet oder abgeschlossen ist.

## Übersicht über geplante und geschätzte Termine

Während der Laufzeit eines Projekts entsprechen die voraussichtlichen und geschätzten Termine eher der Realität des Projekts, da sie berücksichtigen, was sich auf den tatsächlichen Beginn und das Ende einer Aufgabe auswirken kann. Dies führt dazu, dass sie von den geplanten Terminen abweichen.

Beachten Sie beim Arbeiten mit voraussichtlichen und geschätzten Terminen für Aufgaben Folgendes:

* Sie können weder den voraussichtlichen noch den voraussichtlichen Termin von Aufgaben manuell ändern. Beide werden von Adobe Workfront berechnet.
* Wenn Sie eine Aufgabe erstellen, sollten das voraussichtliche und das voraussichtliche Datum identisch sein. Sie sollten die tatsächlichen Zeiten veranschaulichen, zu denen die Aufgabe beginnen oder enden kann.\
  Bestimmte Aktualisierungen, die Sie an Aufgaben vornehmen, wirken sich direkt auf die Werte der voraussichtlichen und geschätzten Termine aus.

  Wenn ein(e) Benutzende(r) beispielsweise eine Aufgabe startet oder abschließt, zeigt die Aufgabe die aktuellen Start- und Abschlussdaten an, die sich auf den geplanten und geschätzten Termin der Aufgabe auswirken. Wenn ein Verantwortlicher für die Aufgabe das Commit-Datum ändert, wirkt sich dieses Datum auch auf das voraussichtliche Datum der Aufgabe aus.

## Differenz zwischen voraussichtlichen und geschätzten Daten

Der Unterschied zwischen dem voraussichtlichen und dem voraussichtlichen Datum beträgt:

* Voraussichtliche Termine werden von Benutzenden beeinflusst, die die folgenden Aktualisierungen an der Aufgabe vornehmen:

   * Einschränkungsdatum durch Hinzufügen einer festen Aufgabenbeschränkung hinzufügen
   * Commit-Datum hinzufügen

* Geschätzte Termine berücksichtigen nur den tatsächlichen Fortschritt einer Aufgabe zu einem bestimmten Zeitpunkt.

**Beispiel:** Wenn eine Aufgabe ein geplantes Startdatum (20. September) und ein geplantes Abschlussdatum (24. September) hat und diese Aufgabe gemäß Einschränkung abgeschlossen sein muss, das geplante Abschlussdatum (24. September). Diese Aufgabe hat eine Dauer von 4 Tagen.

Das geschätzte Abschlussdatum wird auf Grundlage des aktuellen Fortschritts der Arbeit an der Aufgabe berechnet. Wenn also heute der 23. September ist und die Aufgabe noch nicht begonnen hat, ist das geschätzte Abschlussdatum der 27. September (es sollte nach 4 Tagen abgeschlossen sein, vorausgesetzt, die Arbeit wird heute begonnen).

Wenn die Aufgabe heute zu 50 % abgeschlossen ist, ist das geschätzte Abschlussdatum der 25. September (es sollte nach 2 Tagen abgeschlossen sein, was der Hälfte der Dauer der Aufgabe entspricht).


### Erfahren Sie, wann die voraussichtlichen Termine für Aufgaben aktualisiert werden {#understand-when-projected-dates-update-on-tasks}

Die voraussichtlichen Termine können entweder mit anderen Aufgabenterminen übereinstimmen oder sie werden von Workfront unter Berücksichtigung des tatsächlichen Fortschritts der Aufgabe berechnet.

In der folgenden Liste werden mehrere Szenarien angezeigt, in denen die voraussichtlichen Termine von Aufgaben während der Laufzeit eines Projekts geändert werden, je nachdem, was im realen Leben mit der Aufgabe geschieht:

* Wenn eine Aufgabe als Abgeschlossen markiert ist:

  `Projected Dates = Estimated Dates = Actual Dates`

* Wenn eine Aufgabe ein tatsächliches Startdatum hat:

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* Wenn eine Aufgabe kein tatsächliches Startdatum hat, aber eine erzwungene Begrenzung für das geplante Startdatum (Muss beginnen am) besteht, das in der Zukunft liegt:

  `Projected Start Date = Constraint Date`

  Weitere Informationen zum Einschränkungsdatum finden Sie im [Glossar der Adobe Workfront-Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Wenn eine Aufgabe kein tatsächliches Startdatum hat und die Aufgabe kein erzwungenes Einschränkungsdatum aufweist:

  `Projected Start Date = the next available date in the future that falls within working schedule`

* Wenn der Verantwortliche das Commit-Datum aktualisiert:

  `Projected Completion Date = Commit Date`

  Weitere Informationen über das Commit-Datum finden Sie [Übersicht über das Commit-Datum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Wenn die Aufgabe kein aktualisiertes Commit-Datum hat und die Aufgabe eine erzwungene Einschränkung (muss abgeschlossen sein am) für das geplante Abschlussdatum aufweist, das in der Zukunft liegt:

  `Projected Completion Date = Constraint Date`

* Wenn eine Aufgabe kein aktualisiertes Commit-Datum, kein erzwungenes Einschränkungsdatum in der Zukunft oder kein Einschränkungsdatum in der Vergangenheit hat:

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### Erfahren Sie, wann die voraussichtlichen Termine für Aufgaben aktualisiert werden {#understand-when-the-estimated-dates-update-on-tasks}

Im Vergleich zu den oben beschriebenen Szenarien für die voraussichtlichen Termine spiegeln die voraussichtlichen Termine immer die tatsächliche Analyse von Workfront wider, wann die Aufgabe gestartet oder abgeschlossen wird, unabhängig vom Einschränkungs- oder Commit-Datum.

## Was die Zeitleiste einer Aufgabe beeinflusst

Im Folgenden finden Sie einige Beispiele dafür, was sich auf die Echtzeit-Timeline einer Aufgabe auswirken kann:

* Aufgabenfortschritt in Bezug auf die geplanten Termine und den aktuellen Tag
* Prozent abgeschlossen der Aufgabe bis jetzt
* Vorgängerbeziehung
* Vorgänger-Fortschritt
* Benutzerzuordnung

  >[!NOTE]
  >
  >Die Benutzerzuordnung kann sich auf das geschätzte Abschlussdatum einer Aufgabe auswirken, wenn sie sich auf die Geschwindigkeit auswirkt, mit der die Aufgabe abgeschlossen werden kann. Wenn der Aufgabendauer-Typ beispielsweise leistungsgesteuert ist, können Sie den Abschluss der Aufgabe beschleunigen, indem Sie Bevollmächtigte hinzufügen. Dies hat zur Folge, dass sich das geschätzte Abschlussdatum ändert.
