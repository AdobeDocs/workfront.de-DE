---
product-area: reporting
navigation-topic: reporting-elements
title: 'Berichterstellungselemente: Filter, Ansichten und Gruppierungen'
description: Die Hauptelemente, die jede Liste und jeder Bericht in Workfront haben muss, sind ein Filter, eine Ansicht und eine Gruppierung. Jedes Element liefert verschiedene Informationen innerhalb eines Berichts.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Berichterstellungselemente: Filter, Ansichten und Gruppierungen

<!-- Audited: 11/2024 -->

<!--AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well-->

Es gibt mehrere Elemente, die eine Liste oder einen Bericht in Adobe Workfront ermöglichen. Die Hauptelemente, die jede Liste und jeder Bericht aufweisen muss, sind ein Filter, eine Ansicht und eine Gruppierung. Jedes Element liefert verschiedene Informationen innerhalb eines Berichts.

## Überlegungen zu Reporting-Elementen

Beachten Sie beim Arbeiten mit Filtern, Ansichten und Gruppierungen Folgendes:

* Berichterstellungselemente dienen als Bausteine von Berichten. Sie definieren das Erscheinungsbild eines Berichts oder einer Liste sowie die im Bericht oder der Liste enthaltenen Informationen.
* Berichte in Workfront sind jeweils für ein Objekt spezifisch. Sie müssen Ihr Hauptobjekt für einen Bericht definieren, bevor Sie den Bericht erstellen können. Daher sind alle Berichterstellungselemente objektspezifisch.
* Ihr Workfront-Administrator muss Ihnen Zugriff auf Filter, Ansichten und Gruppierungen auf Ihrer Zugriffsebene gewähren, um sie in Listen und Berichten anzeigen oder bearbeiten zu können.

  Informationen zum Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen finden Sie unter [Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Ihr Workfront-Administrator muss Ihnen Zugriff auf Berichte, Dashboards und Kalender in Ihrer Zugriffsebene gewähren, um Berichte anzeigen oder bearbeiten zu können.

  Informationen zum Gewähren des Zugriffs auf Berichte, Dashboards und Kalender finden Sie unter [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Wenn Sie einen Filter, eine Ansicht oder eine Gruppierung in einem Bericht oder einer Liste auswählen, behält Workfront diese Auswahl für die Listen dieses Objekts auch nach dem Abmelden oder Schließen des Browsers bei. Wenn Sie beispielsweise eine bestimmte Ansicht für einen Aufgabenbericht auswählen, wird diese Auswahl für andere Aufgabenlisten angezeigt, z. B. für die Liste der Aufgaben für ein Projekt.

## Filter

Der Filter steuert die Ergebnisse, die in einem Bericht angezeigt werden, und grenzt die Ergebnisse in der Regel von „Allgemein“ auf „Spezifisch“ ein. Es funktioniert wie ein Sieb, das nur die benötigten Informationen erfasst und an Ihren Bericht zurückgibt.

Wenn Sie beispielsweise nur Aufgaben anzeigen möchten, die dem angemeldeten Benutzer zugewiesen sind, können Sie einen Filter mit dem Titel „Meine Aufgaben“ erstellen, die Kriterien definieren, die für den Filter erfüllt sein müssen, und den Bericht ausführen, um nur Aufgaben anzuzeigen, die dem angemeldeten Benutzer zugewiesen sind.

Einige Attribute von Filtern sind:

* Workfront bietet standardmäßig eine Reihe von Filtern für verschiedene Objekte.
* Sie können Filter anpassen, die Sie besitzen oder verwalten.

  Weitere Informationen zu Filtern finden Sie im Artikel [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Ansichten

Indem Sie die Ansicht eines Berichts definieren, definieren Sie, welche Informationen Sie in den Bericht aufnehmen. Wie alle Berichterstellungselemente basieren Ansichten auf einem Objekttyp.

Beispielsweise kann eine Ansicht für einen Aufgabenbericht Fälligkeitsdaten anzeigen, wichtige finanzielle Details wie Kosten enthalten oder verwendet werden, um Zuweisungen und Lieferdatumsdetails anzuzeigen. Ansichten können verwendet werden, um eine Vielzahl von Details zu den Daten im Bericht bereitzustellen.

Einige Attribute von Ansichten sind:

* Sie können eine standardmäßige Workfront-Ansicht verwenden oder eine eigene erstellen.
* Sie können nach dem Ausführen eines Berichts zusätzliche Ansichten aus dem Dropdown-Feld Ansicht anwenden.
* Zusätzliche Ansichten ersetzen vorübergehend die Ansicht, die beim Erstellen des Berichts definiert wurde. Die Standardansicht wird jedoch angezeigt, wenn Sie das nächste Mal zum Bericht zurückkehren.

  Weitere Informationen zu Ansichten finden Sie im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Gruppierungen

Eine Gruppierung steuert, wie Sie Daten organisieren, sodass sie leichter zu lesen und zu verstehen sind. Gruppierungen erstellen horizontale Balken innerhalb eines Berichts, in denen die Ergebnisse nach gemeinsamen Attributen aufgelistet werden. Sie definieren die Kriterien dafür, wie die Ergebnisse Ihres Berichts bei der Gruppierung gruppiert werden sollen.

Wenn Sie beispielsweise eine Liste von Aufgaben gruppieren, die mehrere Projekte umfassen, werden alle entsprechenden Aufgaben, die zu einem einzelnen Projekt gehören, unter diesem Namen organisiert.

Einige Attribute von Gruppierungen sind:

* Gruppierungen sind ein obligatorisches Berichtselement, wenn Sie Ihrem Bericht später ein Diagramm hinzufügen möchten.
* Gruppierungen zeigen in den Ergebnissen einen Aggregatwert an&#x200B;
* Gruppierungen bestimmen die Achse in Diagrammen.
* Gruppierungen bestimmen die Kopfzeilenidentifizierung in Matrixberichten.\
  Weitere Informationen zu Matrixberichten finden Sie im Artikel [Erstellen eines Matrixberichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Gruppierungen helfen beim Erstellen der Registerkarte Zusammenfassung eines Berichts, wobei die aggregierten Werte des Berichts bereitgestellt werden.
* Workfront bietet standardmäßig eine Reihe von Gruppierungen für verschiedene Objekte.
* Sie können Gruppierungen anpassen, die Sie besitzen oder verwalten.

  Weitere Informationen zu Gruppierungen finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Sonstige Berichterstellungselemente

Zusätzlich zu Filtern, Ansichten und Gruppierungen können Sie einem Bericht auch die folgenden Elemente hinzufügen:

* **Prompt**: Ein offener Filter, der bei jeder Ausführung eines Berichts anders angepasst und angewendet werden kann.\
  Weitere Informationen zu Eingabeaufforderungen finden Sie im Artikel [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Diagramm**: Sie können Ihre Berichte verbessern, indem Sie ihnen ein Diagramm hinzufügen und die Informationen visuell anzeigen.\
  Weitere Informationen zu Diagrammen in Berichten finden Sie im Artikel [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
