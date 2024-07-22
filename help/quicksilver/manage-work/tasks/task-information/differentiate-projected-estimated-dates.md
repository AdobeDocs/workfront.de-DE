---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über die geplanten und geschätzten Datumswerte
description: Es gibt verschiedene Arten von Daten, die den Zeitablauf von Aufgaben zwischen dem Zeitpunkt, zu dem sie beginnen können, und dem Zeitpunkt, zu dem sie abgeschlossen werden können, anzeigen.
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# Übersicht über die geplanten und geschätzten Datumswerte

<!--Audited: 07/2024-->

Es gibt verschiedene Arten von Daten, die den Zeitablauf von Aufgaben zwischen dem Zeitpunkt, zu dem sie beginnen können, und dem Zeitpunkt, zu dem sie abgeschlossen werden können, anzeigen. Im Folgenden finden Sie einige Daten, die die Zeitleiste von Aufgaben anzeigen:

* Geplante Start- und geplante Abschlussdaten
* Projizierte Start- und geplante Abschlussdaten
* Geschätzte Start- und Fälligkeitsdaten
* Tatsächliche Start- und tatsächliche Abschlussdaten

In diesem Artikel werden die Unterschiede zwischen den geschätzten und den geplanten Daten für Projekte beschrieben.

Wenn die Aufgabe zum ersten Mal erstellt wird, sollten in der Regel die Datumswerte &quot;Geplant&quot;, &quot;Geplant&quot;und &quot;Geplant&quot;übereinstimmen. Es gibt einige Ausnahmen.

Weitere Informationen zu den Projekt-, Aufgaben- und Ausgabedaten in Adobe Workfront finden Sie unter [Überblick über die Projekt-, Aufgaben- und Problemdatumswerte in Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md).

## Übersicht über geplante Datumswerte

Die geplanten Daten sind die Daten, die der Projektinhaber als Start- und Enddatum der Aufgaben definiert. Sie oder der Projekteigentümer können die geplanten Daten für eine Aufgabe manuell ändern.

## Übersicht über die tatsächlichen Daten

Wenn eine Aufgabe zum ersten Mal erstellt wird, hat sie keine tatsächlichen Daten, da sie noch nicht gestartet oder abgeschlossen wurde.

## Übersicht über die geplanten und geschätzten Datumswerte

Während der Laufzeit eines Projekts entsprechen die prognostizierten und geschätzten Datumswerte eher der Realität des Projekts, da sie berücksichtigen, was den tatsächlichen Beginn und das Ende einer Aufgabe beeinflussen kann. Dadurch ändern sie sich von den geplanten Daten.

Beachten Sie Folgendes bei der Arbeit mit prognostizierten und geschätzten Datumswerten für Aufgaben:

* Sie können weder die geschätzten noch die geplanten Daten der Aufgaben manuell ändern. Beide werden von Adobe Workfront berechnet.
* Bei der Erstellung einer Aufgabe sollten die prognostizierten und geplanten Daten identisch sein und die tatsächlichen Zeiten veranschaulichen, zu denen die Aufgaben beginnen oder enden können.\
  Bestimmte Aktualisierungen, die Sie an Aufgaben vornehmen, wirken sich direkt auf die Werte der geplanten und geschätzten Datumswerte aus.

  Wenn der Benutzer z. B. eine Aufgabe startet oder abschließt, zeigt die Aufgabe die tatsächlichen Start- und Abschlussdaten an, die sich auf die geplanten und geschätzten Datumswerte der Aufgabe auswirken. Wenn ein Verantwortlicher für die Aufgabe das Datum des Versands ändert, beeinflusst dieses Datum auch das Datum der geplanten Aufgabe.

## Unterschied zwischen projizierten und geschätzten Datumswerten

Der Unterschied zwischen den prognostizierten und den geschätzten Datumswerten ist:

* Die prognostizierten Datumswerte werden von einem Benutzer beeinflusst, der folgende Aktualisierungen an der Aufgabe vornimmt:

   * Fügen Sie ein Beschränkungsdatum hinzu, indem Sie eine feste Aufgabenbegrenzung hinzufügen
   * Datum des Versands hinzufügen

* Die geschätzten Datumswerte berücksichtigen nur den tatsächlichen Fortschritt einer Aufgabe zu einem bestimmten Zeitpunkt.

**Beispiel:** Wenn wir eine Aufgabe haben, die über ein geplantes Startdatum vom 20. September und ein geplantes Abschlussdatum vom 24. September verfügt und bei der sie bei Einschränkung beendet werden muss, ist das geplante Abschlussdatum der 24. September. Diese Aufgabe hat eine Dauer von 4 Tagen.

Das geschätzte Abschlussdatum wird basierend auf dem aktuellen Fortschritt der Arbeit an der Aufgabe berechnet. Wenn heute also der 23. September ist und die Aufgabe noch nicht begonnen hat, ist das geschätzte Abschlussdatum der 27. September (es sollte nach 4 Tagen abgeschlossen sein, vorausgesetzt, die Arbeit wird heute begonnen).

Wenn die Aufgabe heute zu 50 % abgeschlossen ist, liegt das geschätzte Abschlussdatum am 25. September (es sollte nach 2 Tagen abgeschlossen werden, was der Hälfte der Dauer der Aufgabe entspricht).


### Erfahren Sie, wann die prognostizierten Datumswerte die Aufgaben aktualisieren {#understand-when-projected-dates-update-on-tasks}

Die geplanten Datumswerte können entweder mit anderen Aufgabendaten übereinstimmen oder es handelt sich um eine von Workfront durchgeführte Berechnung, bei der der tatsächliche Fortschritt der Aufgabe berücksichtigt wird.

In der folgenden Liste werden verschiedene Szenarien angezeigt, in denen die geplanten Aufgabendaten während der Dauer eines Projekts in Abhängigkeit davon geändert werden, was in der Praxis für die Aufgabe geschieht:

* Wenn eine Aufgabe als abgeschlossen markiert ist:

  `Projected Dates = Estimated Dates = Actual Dates`

* Wenn eine Aufgabe ein tatsächliches Startdatum hat:

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* Wenn eine Aufgabe kein tatsächliches Startdatum hat, aber eine erzwungene Beschränkung für das geplante Startdatum (Muss beginnen am) vorliegt, das in der Zukunft liegt:

  `Projected Start Date = Constraint Date`

  Weitere Informationen zum Beschränkungsdatum finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Wenn eine Aufgabe kein tatsächliches Startdatum hat und die Aufgabe kein erzwungenes Beschränkungsdatum hat:

  `Projected Start Date = the next available date in the future that falls within working schedule`

* Wenn der Bevollmächtigte das Zustimmungsdatum aktualisiert:

  `Projected Completion Date = Commit Date`

  Weitere Informationen zum Datum der Übermittlung finden Sie unter [Übersicht über das Datum der Übermittlung](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

* Wenn die Aufgabe kein aktualisiertes Veröffentlichungsdatum hat und die Aufgabe eine erzwungene Beschränkung (Must Finish On) für das geplante Abschlussdatum aufweist, das in der Zukunft liegt:

  `Projected Completion Date = Constraint Date`

* Wenn eine Aufgabe kein aktualisiertes Veröffentlichungsdatum hat, ein erzwungenes Einschränkungsdatum in der Zukunft oder ein Einschränkungsdatum in der Vergangenheit hat:

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### Erfahren Sie, wann die geschätzten Datumswerte die Aufgaben aktualisieren {#understand-when-the-estimated-dates-update-on-tasks}

Im Vergleich zu den oben beschriebenen Szenarien für die prognostizierten Datumswerte spiegeln die geschätzten Datumswerte immer die reale Analyse von Workfront darüber wider, wann die Aufgabe gestartet oder abgeschlossen wird, unabhängig von der Begrenzung oder den Zusagedaten.

## Einfluss auf die Timeline einer Aufgabe

Im Folgenden finden Sie einige Beispiele dafür, was die tatsächliche Timeline einer Aufgabe beeinflussen kann:

* Aufgabenfortschritt in Bezug auf die geplanten Datumswerte und den aktuellen Tag
* Prozentualer Abschluss der Aufgabe bis jetzt
* Vorgängerbeziehung
* Vorgängerfortschritt
* Benutzerzuweisung

  >[!NOTE]
  >
  >Die Zuordnung von Benutzern kann sich auf das geschätzte Abschlussdatum einer Aufgabe auswirken, wenn sie sich auf die Geschwindigkeit auswirken, mit der die Aufgabe abgeschlossen werden kann. Wenn der Aufgabendauertyp beispielsweise &quot;Aufwandsgesteuert&quot;lautet, können Sie die Aufgabe früher abschließen lassen, indem Sie Zuweisende hinzufügen. Daher ändert sich das geschätzte Abschlussdatum.
