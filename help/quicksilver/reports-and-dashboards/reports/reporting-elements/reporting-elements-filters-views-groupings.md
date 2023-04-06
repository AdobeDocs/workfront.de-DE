---
product-area: reporting
navigation-topic: reporting-elements
title: '"Berichterstellungselemente: Filter, Ansichten und Gruppierungen'
description: Die Hauptelemente, die jede Liste und jeder Bericht in Workfront aufweisen muss, sind Filter, Ansichten und Gruppierungen. Jedes Element liefert unterschiedliche Informationen in jedem Bericht.
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Berichterstellungselemente: Filter, Ansichten und Gruppierungen

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

Es gibt mehrere Elemente, die eine Liste oder einen Bericht in Adobe Workfront ermöglichen. Die wichtigsten Elemente jeder Liste und jedes Berichts sind ein Filter, eine Ansicht und eine Gruppierung. Jedes Element liefert unterschiedliche Informationen in jedem Bericht.

## Überlegungen zu Berichterstellungselementen

Beachten Sie beim Arbeiten mit Filtern, Ansichten und Gruppierungen Folgendes:

* Berichterstellungselemente sind die Bausteine für die Berichterstellung. Sie definieren das Erscheinungsbild eines Berichts oder einer Liste sowie die im Bericht oder in der Liste enthaltenen Informationen.
* Berichte in Workfront sind für ein Objekt spezifisch. Sie müssen Ihr Hauptobjekt für einen Bericht definieren, bevor Sie den Bericht erstellen können. Daher sind alle Berichterstellungselemente objektspezifisch.
* Ihr Workfront-Administrator muss Ihnen Zugriff auf Filter, Ansichten und Gruppierungen in Ihrer Zugriffsebene gewähren, damit Sie diese in Listen und Berichten anzeigen oder bearbeiten können.

   Informationen zum Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen finden Sie unter [Zugriff auf Filter, Ansichten und Gruppierungen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Ihr Workfront-Administrator muss Ihnen Zugriff auf Berichte, Dashboards und Kalender in Ihrer Zugriffsebene gewähren, damit Sie Berichte anzeigen oder bearbeiten können.

   Informationen zur Gewährung des Zugriffs auf Berichte, Dashboards und Kalender finden Sie unter [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Wenn Sie einen Filter, eine Ansicht oder eine Gruppierung in einem Bericht oder einer Liste auswählen, behält Workfront diese Auswahl für die Listen dieses Objekts auch dann bei, wenn Sie sich abmelden oder Ihren Browser schließen. Wenn Sie beispielsweise eine bestimmte Ansicht für einen Aufgabenbericht auswählen, wird diese Auswahl für andere Aufgabenlisten angezeigt, z. B. die Liste der Aufgaben für ein Projekt.

## Filter

Der Filter steuert die Ergebnisse, die in einem Bericht angezeigt werden, und schränkt die Ergebnisse in der Regel von Allgemein zu Spezifisch ein. Es funktioniert wie ein Sieb, das nur die benötigten Informationen erfasst und diese Informationen in Ihren Bericht zurückbringt.

Wenn Sie beispielsweise nur Aufgaben sehen möchten, die dem angemeldeten Benutzer zugewiesen sind, können Sie einen Filter mit dem Titel &quot;Meine Aufgaben&quot;erstellen, die Kriterien definieren, die für den Filter erfüllt sein müssen, und den Bericht ausführen, um nur die dem angemeldeten Benutzer zugewiesenen Aufgaben anzuzeigen.

Einige Attribute von Filtern sind:

* Workfront bietet standardmäßig eine Reihe von Filtern für verschiedene Objekte.
* Sie können Filter anpassen, die Ihnen gehören oder die Sie verwalten.

   Weitere Informationen zu Filtern finden Sie im Artikel [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![Symbol für Filter](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## Ansichten

Durch Definition der Ansicht eines Berichts legen Sie fest, welche Informationen Sie in den Bericht aufnehmen. Wie alle Berichterstellungselemente basieren Ansichten auf einem Objekttyp.\
Beispielsweise könnte eine Ansicht für einen Aufgabenbericht Fälligkeitsdaten anzeigen, wichtige Finanzdetails wie Kosten einschließen oder zur Anzeige von Zuweisungen und Versanddatumsdetails verwendet werden. Ansichten können verwendet werden, um eine Vielzahl von Details zu den Daten im Bericht bereitzustellen.

Einige Attribute von Ansichten sind:

* Sie können eine standardmäßige Workfront-Ansicht verwenden oder eine eigene erstellen.
* Sie können nach Ausführung eines Berichts über das Dropdown-Feld Ansicht weitere Ansichten anwenden.
* Zusätzliche Ansichten ersetzen vorübergehend die Ansicht, die beim Erstellen des Berichts definiert wird. Die Standardansicht wird jedoch angezeigt, wenn Sie das nächste Mal zum Bericht zurückkehren.

   Weitere Informationen zu Ansichten finden Sie im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Gruppierungen

Durch eine Gruppierung wird gesteuert, wie Sie Daten organisieren, was das Lesen und Verstehen erleichtert. Gruppierungen erstellen horizontale Balken in einem Bericht, die die Ergebnisse nach gemeinsamen Attributen zusammenführen. Sie definieren die Kriterien dafür, wie Sie die Ergebnisse Ihres Berichts bei der Erstellung der Gruppierung gruppieren möchten.

Wenn Sie z. B. eine Liste von Aufgaben, die sich über mehrere Projekte erstrecken, nach ihrem Projektnamen gruppieren, werden alle entsprechenden Aufgaben organisiert, die zu einem einzigen Projekt unter diesem Namen gehören.

Einige Attribute von Gruppierungen sind:

* Gruppierungen sind ein obligatorisches Berichterstellungselement, wenn Sie Ihrem Bericht zu einem späteren Zeitpunkt ein Diagramm hinzufügen möchten.
* Die Gruppierungen zeigen einen aggregierten Wert in den Ergebnissen an. &#x200B;
* Gruppierungen bestimmen die Achse in Diagrammen.
* Gruppierungen bestimmen die Header-Identifizierung in Matrix-Berichten.\
   Weitere Informationen zu Matrix-Berichten finden Sie im Artikel [Erstellen eines Matrix-Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* Mithilfe von Gruppierungen können Sie die Registerkarte &quot;Zusammenfassung&quot;eines Berichts erstellen und die aggregierten Werte des Berichts angeben.
* Workfront bietet standardmäßig eine Reihe von Gruppierungen für verschiedene Objekte.
* Sie können Gruppen anpassen, deren Inhaber Sie sind oder die Sie verwalten.

   Weitere Informationen zu Gruppierungen finden Sie unter [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Sonstige Berichterstellungselemente

Zusätzlich zu Filtern, Ansichten und Gruppierungen können Sie auch die folgenden Elemente zu einem Bericht hinzufügen:

* **Eingabeaufforderung**: Ein offener Filter, der bei jeder Ausführung eines Berichts unterschiedlich angepasst und angewendet werden kann.\
   Weitere Informationen zu Eingabeaufforderungen finden Sie im Artikel [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **Diagramm**: Sie können Ihre Berichte erweitern, indem Sie ihnen ein Diagramm hinzufügen und die Informationen visuell darstellen.\
   Weitere Informationen zu Diagrammen in Berichten finden Sie im Artikel [Diagramm zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
