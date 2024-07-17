---
title: Projektaktualisierungen während des Veröffentlichungszeitrahmens 22.3
description: Projektaktualisierungen während des Veröffentlichungszeitrahmens 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# 2.3 Projektverbesserungen

Auf dieser Seite werden alle Projektverbesserungen beschrieben, die mit Version 22.3 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 11. Juli 2022 bereitgestellt. Eine Liste aller in Version 22.3 verfügbaren Änderungen finden Sie unter [22.3 - Versionsübersicht](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Abwesenheitsvertretung

Jetzt können Sie die Ihnen zugewiesenen Aufgaben und Probleme vorübergehend an andere Benutzer delegieren, wenn Sie planen, für einen kurzen Zeitraum abwesend zu sein. Dadurch wird sichergestellt, dass Ihre Abwesenheit kein Hindernis für die Fertigstellung der Arbeiten wird.

Vor dieser Verbesserung konnten Sie nur Genehmigungen delegieren.

Im Folgenden finden Sie einige Funktionen, die wir mit diesem Update hinzugefügt haben:

* Eine Einstellung im Bereich &quot;Voreinstellungen für Aufgaben und Probleme&quot;unter &quot;Einrichten&quot;für das System oder den Gruppenadministrator, um die Zuweisung in Ihrer Umgebung zu aktivieren.

* Eine neue Option für &quot;Delegieren von Aufgaben und Problemen&quot;im Bereich &quot;Startseite&quot;für Benutzer mit einer Review- oder höheren Lizenz zum Delegieren ihrer Arbeitselemente.

* Angabe der Aufgaben- und Problemkopfzeilen im Bereich &quot;Startseite&quot;und im Bereich &quot;Zuweisungen&quot;, dass Elemente an andere delegiert werden.

* Ereignisbenachrichtigungen im Bereich &quot;Einrichtung&quot;und E-Mail-Benachrichtigungen im Benutzerprofil zum Steuern von E-Mail-Benachrichtigungen über delegierte Arbeiten


>[!NOTE]
>
>Nur Benutzer mit einer Review- oder höheren Lizenz können ihre Arbeit an andere delegieren. Die Arbeit kann jedem Benutzer unabhängig von seiner Zugriffsstufe zugewiesen werden. Delegierte Benutzer erhalten dieselben Berechtigungen wie die Bevollmächtigten für die delegierten Elemente. Wenn diese Berechtigungen niedriger sind als die Zugriffsstufenkonfiguration eines Benutzers, können die delegierten Benutzer daran gehindert werden, einige der Aktivitäten für die Aufgaben und Probleme auszuführen, die ihnen zugewiesen sind.


Weitere Informationen finden Sie unter [Aufgabe delegieren und Problemübersicht](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Neues Erlebnis beim Konvertieren eines Problems in eine Aufgabe

Damit Ihre Verwendung von Workfront mit dem neuen Workfront-Erlebnis konsistent ist, haben wir die Benutzeroberfläche für die Konvertierung eines Problems in eine Aufgabe neu gestaltet.

Diese Aktualisierung umfasst:

* Eine aktualisierte Benutzeroberfläche, die dem Rest des neuen Workfront-Erlebnisses entspricht.

* Zugriff auf die Konvertierung eines Problems in Aufgaben aus einer Liste oder einem Bericht.

* Die standardmäßigen benutzerdefinierten Formulare, die im Bereich &quot;Aufgabeneinstellungen&quot;des Zielprojekts definiert sind, das zur neuen Aufgabe hinzugefügt wurde.


Weitere Informationen finden Sie unter [Konvertieren eines Problems in eine Aufgabe in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Neues Erlebnis beim Konvertieren eines Problems in ein Projekt ohne Vorlage

Damit Ihre Verwendung von Workfront mit dem neuen Workfront-Erlebnis konsistent ist, haben wir die Benutzeroberfläche für die Konvertierung eines Problems in ein Projekt ohne Vorlage neu gestaltet.

Zusätzlich zu einer aktualisierten Benutzeroberfläche, die dem Rest des neuen Workfront-Erlebnisses entspricht, haben wir auch die Möglichkeit hinzugefügt, ein Problem in leere Projekte aus einer Liste oder einem Bericht zu konvertieren.

Weitere Informationen finden Sie unter [Konvertieren eines Problems in ein Projekt in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Smart-Tagging im Aktualisierungs-Stream

Wir haben das Tagging von Benutzern im Aktualisierungsstream verbessert, wenn Sie ein neues Update erstellen oder auf ein vorhandenes antworten. Wenn Sie jetzt einen Benutzer taggen, um ihn in ein Update einzubeziehen, zeigen wir neben seinem Namen und Avatar auch dessen Primäre Rolle und E-Mail-Adresse an. Dies hilft bei der Unterscheidung zwischen mehreren Benutzenden mit ähnlichen oder identischen Namen.

Weitere Informationen finden Sie unter [Taggen anderer Benutzer bei Updates](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Neue Syntax für Berechnungen in benutzerdefinierten Feldern

Zur Vorbereitung auf zukünftige Verbesserungen, die Ihnen beim Hinzufügen von Berechnungen zu benutzerdefinierten Formularen helfen, haben wir die Syntax für referenzierte Felder standardisiert, die Sie zu einer Berechnung hinzufügen. Diese neue Syntax ist einfach zu verwenden, da das System sie für Sie eingibt, wenn Sie mit der Eingabe des Namens eines Felds beginnen und sie dann auswählen.

Weitere Informationen finden Sie im Abschnitt &quot;Berechnung für Ihr berechnetes benutzerdefiniertes Feld erstellen&quot;im Artikel [Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Halten Sie genaue Informationen bereit, wenn zwei Benutzer mit einer gemeinsamen Rolle an einem Genehmigungsprozess beteiligt sind.

Um die Genauigkeit Ihrer Daten für die Validierung der Arbeit sicherzustellen, haben wir die Art und Weise geändert, wie Validierungsinformationen für einen Artikel aufgezeichnet werden, wenn ein Validierungsprozess für mehrere Rollen mit dem Artikel verknüpft ist.

Einige Genehmigungsprozesse erfordern eine Genehmigung durch zwei verschiedene Rollen, und zwei verschiedene Genehmiger haben möglicherweise eine dieser Rollen gemeinsam. Wenn dies geschieht, zeichnet Workfront nach den Genehmigungsentscheidungen jeden Genehmiger und seine jeweilige Rolle auf, die mit dem Genehmigungsprozess verbunden ist.

Vor dieser Änderung wurden beide Genehmigungen für den zweiten Benutzer aufgezeichnet, da er eine der Genehmigungsrollen für den ersten Genehmiger freigegeben hatte. In diesem Fall überschrieb der zweite Genehmiger die Informationen des ersten Genehmigers.

Weitere Informationen zu Genehmigungsprozessen in Workfront finden Sie unter [Übersicht über den Genehmigungsprozess](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Zuordnungszeiten werden nicht mehr entfernt, wenn Änderungen an Zuweisungen vorgenommen werden

>[!NOTE]
>
>Diese Funktion sollte ursprünglich mit Version 22.2 veröffentlicht werden. Es wurde am 21. April 2022 für die Produktion freigegeben.


Um die Genauigkeit Ihrer Daten zu gewährleisten, haben wir eine Änderung vorgenommen, um die Zuordnungszeiten beizubehalten und die Aufgabe Planed Hours bei der Änderung der Aufgabenzuweisungen unverändert zu halten.

Die folgenden Änderungen wurden an Aufgaben mit dem Typ Einfache Dauer vorgenommen:

* Geplante Stunden werden beim Entfernen aller Bevollmächtigten beibehalten.

* Beim Ersetzen von Benutzern und Rollen werden individuelle Zuweisungszuordnungen beibehalten.

* Einzelne Zuweisungszuordnungen bleiben beim Entfernen des Benutzers in der Rolle erhalten. (Aus Version entfernt. Jetzt werden die geplanten Stunden auf 0 gesetzt, nachdem alle Verantwortlichen entfernt wurden.)


Weitere Informationen zu geplanten Stunden finden Sie unter [Übersicht über geplante Stunden](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Erweiterungen für Foren

Die folgenden Verbesserungen wurden zu Adobe Workfront-Pinnwänden hinzugefügt:

* Filteroptionen - Sie können jetzt auf einer Pinnwand nach Fälligkeitsdatum oder Status filtern. Der Filter wurde auch mit ausblendbaren Abschnitten aktualisiert, um die Optionen zu trennen.

* Pinnwand archivieren - Sie können jetzt eine Pinnwand archivieren, während Sie sich in der Pinnwand befinden, anstatt zum Dashboard der Pinnwände wechseln zu müssen.

* Hinzufügen eines Teams zu einer Pinnwand - Wenn Sie nach Mitgliedern suchen, können Sie ein ganzes Team hinzufügen. Wenn Sie ein Team auswählen, werden alle Mitglieder des Teams zum Forum hinzugefügt.

* Bereiche in Spalten ablegen - Wenn Sie eine Karte aus einer Pinnwandspalte in eine andere ziehen, wird jetzt eine graue &quot;Dropzone&quot;angezeigt, in der die Karte platziert wird. Zuvor gab es keinen visuellen Indikator für die Kartenplatzierung.

* Verbundene Karten - Sie können jetzt Karten hinzufügen, die mit Workfront-Aufgaben und -Problemen verbunden sind. Wenn Sie den Namen, die Beschreibung oder den Verantwortlichen auf der Karte oder in der Aufgabe aktualisieren, werden dieselben Felder an der anderen Stelle aktualisiert.

* Statusfeld auf allen Karten - Ad-hoc- und verbundenen Karten wurden ein Statusfeld und eine Schaltfläche zum Markieren abgeschlossen hinzugefügt. Wenn Sie auf &quot;Abschluss markieren&quot;klicken, ändert sich der Status automatisch in &quot;Fertig stellen&quot;.

* Ad-hoc-Karte in verbundene Karte konvertieren - Sie können jetzt eine Ad-hoc-Karte aus den Kartendetails in eine verbundene Karte konvertieren.

* Verbindungskarte trennen - Das Trennen einer verbundenen Karte unterbricht die Verbindung mit dem Workfront-Objekt. Die Karte bleibt als Ad-hoc-Karte auf der Pinnwand, und das Workfront-Objekt ist davon nicht betroffen.

* Statuszuordnung in Spalten - Neue Spalteneinstellungen und Richtlinien ermöglichen es Ihnen, einen Status, einen Bevollmächtigten oder ein Tag zu definieren, der auf Karten angewendet wird, die in diese Spalte verschoben werden. Außerdem wurden die standardmäßigen Spaltennamen auf einer neuen Pinnwand in Spalte 1, Spalte 2 und Spalte 3 geändert.

* Indikator Feldaktualisierung - Beim Speichern einer Karte wird jetzt ein Indikator angezeigt, um zu bestätigen, dass Ihre Aktualisierungen gespeichert wurden.


Weitere Informationen finden Sie unter [Erste Schritte mit Pinnwänden in Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Ordner nur in den fünf oberen Ebenen einer Ordnerhierarchie freigeben

Um die optimale Leistung für Benutzer sicherzustellen, die Ordner freigeben, beschränken wir derzeit die Freigabe auf die fünf obersten Ebenen in einer Ordnerhierarchie eines Objekts.

Jeder Ordner auf der sechsten Ebene oder darunter übernimmt seine Freigabekonfigurationen direkt über dem Ordner.

Weitere Informationen zum Freigeben von Ordnern finden Sie unter [Freigeben eines Dokumentenordners der obersten Ebene](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Workfront-Kampagnen (Beta) - eine neue Methode zur Verwaltung Ihrer Arbeit

>[!NOTE]
>
>Diese Funktion soll am 9. Januar 2023 aus der Vorschau entfernt werden. Weitere Informationen finden Sie auf der Seite [23.1 - Versionsübersicht](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Diese Funktion ist in der Produktionsversion 22.3 nicht enthalten. Es wird mit einer zukünftigen Version für die Produktion freigegeben.


>[!NOTE]
>
>Diese Funktion ist nur als Beta-Version verfügbar und befindet sich derzeit im Aufbau. Mit zukünftigen Versionen werden wir weiterhin Funktionen für den Campaign-Workflow hinzufügen. Die Teilnahme am Betaprogramm für Workfront-Kampagnen ist freiwillig.

Wir führen ein neues Objekt in Adobe Workfront ein, das die Art und Weise, wie Sie Arbeit verwalten, verändern kann.

Mit Workfront Campaigns können Sie Projekte aus verschiedenen Portfolios und Programmen in einem neuen Arbeitscontainer organisieren. Dieser neue Container wird sich in zukünftigen Versionen weiterentwickeln und schließlich alle Arbeitsobjekte einschließen, die derzeit in separaten Silos verwaltet werden.

Diese Version enthält die folgenden Funktionen:

* Ein neues Workfront-Objekt namens Campaign

* Ein neuer Kampagnenbereich (Beta) im Hauptmenü

* Eine Liste der Kampagnen im Kampagnenbereich

* Eine Seite mit Kampagnendetails mit zusätzlichen Informationen zu einer Kampagne

* Möglichkeit zum Hinzufügen von Projekten zu einer Kampagne

* Möglichkeit, Informationen zu einer Kampagne zu bearbeiten

* Möglichkeit, das Kampagnenobjekt aus der Layout-Vorlage umzubenennen

  System- und Gruppenadministratoren von Workfront können den Bereich Kampagnen (Beta) im Hauptmenü einer Layout-Vorlage hinzufügen. Dadurch wird sie für alle Benutzer verfügbar, die der Vorlage zugewiesen sind. Sobald die Kampagne verfügbar ist, kann jeder in Workfront eine Kampagne erstellen.




