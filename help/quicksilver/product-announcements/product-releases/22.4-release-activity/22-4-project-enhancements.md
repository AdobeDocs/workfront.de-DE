---
title: 22.4 Projektverbesserungen
description: 22.4 Projektverbesserungen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 2%

---

# 22.4 Projektverbesserungen

Auf dieser Seite werden alle mit Version 22.4 vorgenommenen Projektverbesserungen in der Vorschau-Umgebung beschrieben. Diese Verbesserungen werden in der Woche vom 3. Oktober 2022 zur Verfügung gestellt.

Eine Liste aller in Version 22.4 verfügbaren Änderungen finden Sie in der Übersicht über [&#x200B; Version 22.4 &#x200B;](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Vorgängerdetails jetzt verfügbar

Um die Details der Vorgänger einer Aufgabe anzuzeigen, können Sie jetzt den Mauszeiger über die Vorgängernummer in der Spalte Vorgänger bewegen. Das Detailfeld zeigt die Vorgängeraufgabe und das Projekt an, auf die verwiesen wird, sowie die geplanten Start- und Enddaten für die Vorgängeraufgabe und die Anzahl der Vorgängeraufgaben und Nachfolger. Sie können die Projektdetails erweitern, um weitere Informationen zum Projekt anzuzeigen. Weitere Informationen sind für projektübergreifende Vorgänger enthalten.

Weitere Informationen finden Sie unter [Erstellen einer Vorgängerbeziehung auf der Aufgabenliste](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Mehrere Teams einer Aufgabe oder einem Problem zuweisen

Wir haben es Ihnen ermöglicht, einer Aufgabe oder einem Problem mehrere Teams zuzuweisen, um Ihnen viel mehr Flexibilität bei der Verwaltung von Aufgaben und Problemen zu bieten. Zuvor konnte nur ein Team einer Aufgabe oder einem Problem zugewiesen werden.

>[!NOTE]
>
>Diese Funktion ist derzeit nicht im Workload Balancer im Bereich Teams verfügbar.

Weitere Informationen finden Sie unter [Aufgaben zuweisen](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) und [Probleme zuweisen](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Intelligente Benutzerauswahl für Projektrollen in den Bereichen Bearbeiten und Details

Wir haben die Art und Weise verbessert, wie Benutzende angezeigt werden, wenn Sie sie den folgenden Projektfeldern aus dem Feld Bearbeiten und dem Abschnitt Details des Projekts hinzufügen:

* Projektbesitzer

* Projektsponsor

* Ressourcenmanager

Wenn Sie jetzt Benutzende zu einem dieser Felder im Bereich Bearbeiten oder Details hinzufügen, werden neben ihrem Namen und Avatar auch ihre Primäre Rolle und ihre E-Mail-Adresse angezeigt. Dies hilft bei der Unterscheidung zwischen mehreren Benutzenden mit ähnlichen oder identischen Namen.

Weitere Informationen finden Sie unter [Projekte &#x200B;](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

HINWEIS: Zusätzliche Benutzerfelder für Projekte, Aufgaben und Probleme werden mit dieser Funktion in zukünftigen Versionen aktualisiert.

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Berechnete Datumsfelder werden immer basierend auf der koordinierten Weltzeit (UTC) gespeichert

Jetzt können Sie sicherstellen, dass alle Datumsfunktionen in berechneten Feldern konsistent funktionieren und für alle dasselbe Ergebnis liefern, unabhängig davon, wie ein benutzerdefinierter Datenausdruck aktualisiert wird oder wo Benutzende auf der ganzen Welt am -Objekt zusammenarbeiten.

Alle Berechnungen werden jetzt von einem Standard - Coordinated Universal Time (UTC) - berechnet und gespeichert, nicht von den Zeitzonenkonfigurationen, die für die Instanz Ihres Unternehmens und Ihr individuelles Benutzerprofil festgelegt wurden. Berechnungen werden jedoch in einem benutzerdefinierten Formular angezeigt, das auf den individuellen Zeitzonen der einzelnen Benutzenden basiert, die in ihrem Browser festgelegt wurden.

Zuvor führten Zeiteinstellungen in Berechnungen zu Verwirrung, wenn sie in diesen Situationen variierten:

* Wenn jemand einen berechneten Feldausdruck mithilfe von „Vorherige Berechnungen aktualisieren“ im Formular-Builder neu berechnet hat, wurden die Ergebnisse der Datumsfunktion durch die UTC-Zeitzone Ihrer Organisation bestimmt.

* Wenn jemand das -Objekt bearbeitet hat und dies dazu geführt hat, dass der Ausdruck für das berechnete Feld neu berechnet wurde, wurden die Ergebnisse der Datumsfunktion anhand der lokalen Zeitzone des Benutzers bestimmt. Die Ergebnisse der berechneten Datumsfelder in diesem Szenario werden ebenfalls auf der Grundlage der UTC berechnet.

Weitere Informationen finden Sie unter [Arbeiten über Zeitzonen hinweg](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Verbesserungen bei benutzerdefinierten Formularen: Adobe XD und der Schnellfilter

Basierend auf Ihrem Feedback haben wir die folgenden Verbesserungen eingeführt, um Ihr Erlebnis beim Verwalten von benutzerdefinierten Formularen zu verbessern:

* Fügen Sie eine Adobe XD-Datei hinzu, um ein benutzerdefiniertes Formular visueller und informativer zu gestalten. Wenn das Formular an ein Objekt angehängt ist, können Benutzende, die mit dem Objekt arbeiten, die XD-Datei im Formular anzeigen und mit ihr interagieren.


* Verwenden Sie den Schnellfilter, um Elemente in der modernisierten Liste der benutzerdefinierten Formulare und Felder einfach zu finden. Sie erhalten außerdem ein verbessertes Erscheinungsbild bei der Verwaltung Ihrer Formulare und Felder.

  Weitere Informationen zum Schnellfilter finden Sie unter [Anwenden des Schnellfilters auf eine Liste](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Öffentliche Beta - Neues Filtererlebnis für Projekte, Aufgaben und Probleme

Die Filterung von Projekt-, Aufgaben- und Problemlisten wurde neu gestaltet, damit Sie Filter schnell erstellen und freigeben können. Zu den Funktionen gehören:

* Eine intuitive „Beta Builder“-Oberfläche zum Erstellen eines neuen Filters

* Die Möglichkeit, einen Filter als Favoriten zu markieren

* Filterstapelung (Anwenden mehrerer gespeicherter Filter)

* Filter duplizieren

* Filter freigeben

* Mit Ihnen geteilte Filter entfernen


Das neue Filtererlebnis ist auch in Arbeitszeittabellenlisten und im Szenario-Planer verfügbar.

Der Textmodus bleibt für die erweiterte Filterbearbeitung verfügbar, und Systemadministratoren können weiterhin Standardfilter für alle Benutzer über die Layout-Vorlagen zuweisen.

### Wo wird dies verfügbar sein?

* Liste der Projekte/Aufgaben/Probleme

* Szenarienplaner

* Arbeitszeit- tabellen


### Wir möchten Ihr Feedback!

Mit diesem Public Beta erhalten Anwender die Möglichkeit, Feedback direkt an das Team zu senden, das am Filtererlebnis arbeitet, indem sie auf die Feedback-Schaltfläche klicken. Wir freuen uns, von Ihnen und Ihren Benutzern über das neue Filtererlebnis in der öffentlichen Beta-Version zu hören. Wenn Ihr Team sich direkt mit dem Produkt treffen möchte, um zusätzliches Feedback zu geben, können Sie hier ein Meeting planen: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&date=2022-08-25

### Wie geht es weiter?

* Neues Erlebnis bei Gruppierungen und Ansichten (auch als Spalten bezeichnet)

  Wir werden mit der Arbeit am neuen Erlebnis für Gruppierungen und Ansichten (auch als Spalten bezeichnet) beginnen, damit es mit dem neuen Filtererlebnis konsistent ist und einige der großartigen Funktionen des neuen Filtererlebnisses hat.

* Neue Filter in anderen Bereichen von Adobe Workfront implementieren

  Wir werden mit Teams aus allen Produktbereichen zusammenarbeiten, um die neuen Filter in anderen Bereichen von Workfront zu implementieren.


Wir möchten Ihnen iterativ einen Mehrwert bieten, sodass wir weiterhin liefern können, wenn die neuen Erlebnisse und andere Bereiche bereit sind. Bleiben Sie dran für weitere spannende Updates.

Weitere Informationen finden Sie unter [Filterübersicht](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) und [Filter in Adobe Workfront erstellen oder bearbeiten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3412391/)
