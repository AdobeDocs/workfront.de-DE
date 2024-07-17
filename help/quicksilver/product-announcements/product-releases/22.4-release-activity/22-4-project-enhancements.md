---
title: 2.4 Projektverbesserungen
description: 2.4 Projektverbesserungen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# 2.4 Projektverbesserungen

Auf dieser Seite werden alle Projektverbesserungen beschrieben, die mit Version 22.4 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 3. Oktober 2022 verfügbar gemacht.

Eine Liste aller in Version 22.4 verfügbaren Änderungen finden Sie unter [22.4 - Versionsübersicht](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Details zu Vorgängern jetzt verfügbar

Um die Details der Vorgänger einer Aufgabe anzuzeigen, können Sie jetzt in der Spalte &quot;Vorgänger&quot;den Mauszeiger über die Vorgängernummer bewegen. Im Detailfeld werden die referenzierte Vorgängeraufgabe und das referenzierte Projekt, die geplanten Start- und Enddaten für die Vorgängeraufgabe sowie die Anzahl der Vorgängeraufgaben und Nachfolger angezeigt. Sie können die Projektdetails erweitern, um weitere Informationen zum Projekt anzuzeigen. Zusätzliche Informationen sind für projektübergreifende Vorgänger enthalten.

Weitere Informationen finden Sie unter [Erstellen einer Vorgängerbeziehung in der Aufgabenliste](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Zuweisen mehrerer Teams zu einer Aufgabe oder einem Problem

Um Ihnen viel mehr Flexibilität bei der Verwaltung von Aufgaben und Problemen zu geben, haben wir es ermöglicht, mehrere Teams einer Aufgabe oder einem Problem zuzuweisen. Zuvor konnte nur ein Team einer Aufgabe oder einem Problem zugewiesen werden.

>[!NOTE]
>
>Diese Funktion ist derzeit im Arbeitslastausgleich im Bereich Teams nicht verfügbar.

Weitere Informationen finden Sie unter [Aufgaben zuweisen](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) und [Zuweisen von Problemen](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Smart-Benutzerauswahl für Projektrollen in den Bereichen Bearbeiten und Details

Die Anzeige der Benutzer beim Hinzufügen zu den folgenden Projektfeldern im Feld Bearbeiten und im Abschnitt Details des Projekts wurde verbessert:

* Projektbesitzer

* Projektsponsor

* Ressourcenmanager

Wenn Sie nun einen Benutzer zu einem dieser Felder in den Bereichen Bearbeiten oder Details hinzufügen, werden neben seinem Namen und Avatar auch dessen Primäre Rolle und die E-Mail-Adresse angezeigt. Dies hilft bei der Unterscheidung zwischen mehreren Benutzenden mit ähnlichen oder identischen Namen.

Weitere Informationen finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

HINWEIS: Zusätzliche Benutzerfelder für Projekte, Aufgaben und Probleme werden in zukünftigen Versionen mit dieser Funktion aktualisiert.

[Sehen Sie sich eine Videodemonstration für diese Funktion an.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Berechnete Datumsfelder werden immer basierend auf der koordinierten Weltzeit (UTC) gespeichert.

Jetzt können Sie sicher sein, dass alle Datumsfunktionen in berechneten Feldern konsistent funktionieren und für alle dasselbe Ergebnis liefern, unabhängig davon, wie ein benutzerdefinierter Datenausdruck aktualisiert wird oder wo Benutzer weltweit an dem Objekt zusammenarbeiten.

Alle Berechnungen werden jetzt nach einem Standard - koordinierte Weltzeit (UTC) - und nicht nach den Zeitzonenkonfigurationen berechnet und gespeichert, die für die Instanz Ihres Unternehmens und Ihr individuelles Benutzerprofil festgelegt sind. Berechnungen werden jedoch in einem benutzerdefinierten Formular angezeigt, das auf den individuellen Zeitzonen der einzelnen Benutzer in ihrem Browser basiert.

Zuvor führten die Zeiteinstellungen in Berechnungen zu Verwirrung, wenn sie in diesen Situationen variierten:

* Wenn ein berechneter Feldausdruck mithilfe von &quot;Frühere Berechnungen aktualisieren&quot;im Formular-Builder neu berechnet wurde, wurden die Ergebnisse der Datumsfunktionen anhand der UTC-Zeitzone Ihres Unternehmens ermittelt.

* Wenn jemand das Objekt bearbeitet hat und der dazu geführt hat, dass der berechnete Feldausdruck neu berechnet wurde, wurden die Ergebnisse der Datumsfunktion durch die lokale Zeitzone des Benutzers bestimmt. Die Ergebnisse des berechneten Datumsfelds in diesem Szenario werden ebenfalls auf der Grundlage der UTC berechnet.

Weitere Informationen finden Sie unter [Arbeiten über Zeitzonen hinweg](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Verbesserungen beim benutzerdefinierten Formular: Adobe XD und der Schnellfilter

Basierend auf Ihrem Feedback haben wir die folgenden Verbesserungen eingeführt, um Ihr Benutzererlebnis bei der Verwaltung benutzerdefinierter Formulare zu verbessern:

* Fügen Sie eine Adobe XD-Datei hinzu, um ein benutzerdefiniertes Formular visueller und informativer zu gestalten. Wenn das Formular an ein Objekt angehängt wird, können Benutzer, die mit dem Objekt arbeiten, die XD Datei im Formular anzeigen und damit interagieren.

  Weitere Informationen finden Sie unter [Hinzufügen oder Bearbeiten von Bildern oder anderen Asset-Widgets in einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Verwenden Sie den Schnellfilter , um Elemente in der Liste modernisierter benutzerdefinierter Formulare und Felder einfach zu finden. Genießen Sie außerdem ein verbessertes Erscheinungsbild bei der Verwaltung Ihrer Formulare und Felder.

  Weitere Informationen zum Schnellfilter finden Sie unter [Anwenden des Schnellfilters auf eine Liste](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Sehen Sie sich eine Videodemonstration für diese Funktion an.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Öffentliche Beta - Neues Filtererlebnis für Projekte, Aufgaben und Probleme

Das Filtern in Projekt-, Aufgaben- und Problemlisten wurde neu gestaltet, um Ihnen das schnelle Erstellen und Freigeben von Filtern zu erleichtern. Zu den Funktionen gehören:

* Eine intuitive &quot;Beta-Builder&quot;-Oberfläche zum Erstellen eines neuen Filters

* Die Fähigkeit, einen Filter als Favoriten zu kennzeichnen

* Filterstapelung (Anwenden von mehr als einem gespeicherten Filter)

* Filter duplizieren

* Filter freigeben

* Für Sie freigegebene Filter entfernen


Das neue Filtererlebnis ist auch in den Timesheet-Listen und im Szenario-Planer verfügbar.

Der Textmodus bleibt für die erweiterte Filterbearbeitung verfügbar, und Systemadministratoren können allen Benutzern über die Layoutvorlagen weiterhin Standardfilter zuweisen.

### Wo wird dies verfügbar sein?

* Projekt-/Aufgaben-/Problemlisten

* Szenarienplaner

* Arbeitszeit- tabellen


### Wir wollen Ihr Feedback!

Mit dieser Funktion erhalten Benutzer von Public Beta die Möglichkeit, Feedback direkt an das Team zu senden, das an dem Filtererlebnis arbeitet, indem sie auf die Feedback-Schaltfläche klicken. Wir freuen uns darauf, von Ihnen und Ihren Benutzern über die neue Filtererfahrung in der öffentlichen Beta-Phase zu erfahren. Wenn Ihr Team mit einem Produkt direkt zusammentreffen möchte, um zusätzliches Feedback zu geben, können Sie ein Meeting hier planen: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### Wie geht es weiter?

* Neues Gruppierungs- und Ansichtserlebnis (auch Spalten genannt)

  Wir werden mit der Arbeit an dem neuen Erlebnis für Gruppierungen und Ansichten (auch als Spalten bezeichnet) beginnen, damit es mit dem neuen Filtererlebnis konsistent ist und einige der gleichen großartigen Funktionen wie die neuen Filter aufweist.

* Neue Filter in andere Bereiche von Adobe Workfront implementieren

  Wir werden mit Teams aus dem gesamten Produkt zusammenarbeiten, um die neuen Filtererfahrungen in anderen Bereichen in Workfront zu implementieren.


Wir möchten Ihnen einen Mehrwert bieten, damit wir auch weiterhin mit den neuen Erfahrungen und anderen Bereichen zur Verfügung stehen. Bleiben Sie auf dem Laufenden für spannendere Updates.

Weitere Informationen finden Sie unter [Filterübersicht](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) und [Filter in Adobe Workfront erstellen oder bearbeiten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Sehen Sie sich eine Videodemonstration für diese Funktion an.](https://video.tv.adobe.com/v/3412391/)
