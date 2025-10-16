---
title: Projektaktualisierungen im Zeitrahmen der Version 22.3
description: Projektaktualisierungen im Zeitrahmen der Version 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1535'
ht-degree: 0%

---

# 22.3 Projektverbesserungen

Auf dieser Seite werden alle mit Version 22.3 vorgenommenen Projektverbesserungen in der Vorschau-Umgebung beschrieben. Diese Verbesserungen wurden in der Woche vom 11. Juli 2022 in der Produktionsumgebung verfügbar gemacht. Eine Liste aller mit Version 22.3 verfügbaren Änderungen finden Sie unter Übersicht über die Version [22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delegation von Abwesenheitsarbeiten

Jetzt können Sie die Ihnen zugewiesenen Aufgaben und Probleme vorübergehend an andere Benutzer delegieren, wenn Sie für einen kurzen Zeitraum abwesend sein möchten. Dadurch wird sichergestellt, dass Ihre Abwesenheit nicht zu einer Hürde für die Fertigstellung wird.

Vor dieser Verbesserung konnten Sie nur Genehmigungen delegieren.

Im Folgenden finden Sie einige der Funktionen, die wir mit diesem Update hinzugefügt haben:

* Eine Einstellung im Bereich „Voreinstellungen für Aufgaben und Probleme“ unter „Setup“ für den System- oder Gruppenadministrator, um die Delegierung in Ihrer Umgebung zu aktivieren.

* Eine neue Option zum Delegieren von Aufgaben und Problemen im Startseiten-Bereich für Benutzer mit einer Lizenz zum Überprüfen oder einer höheren Lizenz zum Delegieren ihrer Arbeitselemente.

* Angabe, dass Elemente an andere delegiert werden, auf der Startseite und im Bereich „Zuweisungen“ der Aufgaben- und Problemkopfzeilen.

* Ereignisbenachrichtigungen im Bereich Setup und E-Mail-Benachrichtigungen im Benutzerprofil zur Steuerung von E-Mail-Benachrichtigungen über delegierte Arbeit


>[!NOTE]
>
>Nur Benutzer mit einer Review- oder einer höheren Lizenz können ihre Arbeit an andere delegieren. Arbeit kann an jeden Benutzer delegiert werden, unabhängig von dessen Zugriffsebene. Delegierte Benutzer erhalten dieselben Berechtigungen wie die Bevollmächtigten für die delegierten Elemente. Wenn diese Berechtigungen niedriger sind als die Zugriffsebenen-Konfiguration einer Benutzerin oder eines Benutzers, können die delegierten Benutzenden möglicherweise daran gehindert werden, einige der Aktivitäten für die Aufgaben und Probleme auszuführen, die ihnen delegiert wurden.


Weitere Informationen finden Sie unter [Delegieren von Aufgaben und Problemübersicht](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## Neues Erlebnis beim Konvertieren eines Problems in eine Aufgabe

Damit Ihre Verwendung von Workfront mit der neuen Workfront-Version konsistent ist, haben wir die Benutzeroberfläche zum Konvertieren eines Problems in eine Aufgabe neu gestaltet.

Dieses Update enthält:

* Eine aktualisierte Benutzeroberfläche, die dem Rest des neuen Workfront-Erlebnisses entspricht.

* Zugriff zum Konvertieren eines Problems in Aufgaben aus einer Liste oder einem Bericht.

* Die benutzerdefinierten Standardformulare, die im Bereich Aufgabeneinstellungen des Zielprojekts definiert sind, wurden der neuen Aufgabe hinzugefügt.


Weitere Informationen finden Sie unter [Problem in eine Aufgabe konvertieren](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Neues Erlebnis beim Konvertieren eines Problems in ein Projekt ohne Vorlage

Um die Verwendung von Workfront mit der neuen Workfront-Version konsistent zu machen, haben wir die Benutzeroberfläche zum Konvertieren eines Problems in ein Projekt ohne Verwendung einer Vorlage neu gestaltet.

Zusätzlich zu der aktualisierten Benutzeroberfläche, die der neuen Workfront-Version entspricht, haben wir auch die Möglichkeit hinzugefügt, ein Problem aus einer Liste oder einem Bericht in leere Projekte zu konvertieren.

Weitere Informationen finden Sie unter [Konvertieren eines Problems in ein Projekt in Adobe Workfront](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Smart-Tagging im Aktualisierungsverlauf

Wir haben das Tagging von Benutzern im Aktualisierungsverlauf verbessert, wenn Sie eine neue Aktualisierung erstellen oder auf eine vorhandene antworten. Wenn Sie einen Benutzer taggen, um ihn in ein Update aufzunehmen, zeigen wir neben seinem Namen und Avatar auch seine Primäre Rolle und seine E-Mail-Adresse an. Dies hilft bei der Unterscheidung zwischen mehreren Benutzenden mit ähnlichen oder identischen Namen.

Weitere Informationen finden Sie unter [Andere bei Updates taggen](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Neue Syntax für Berechnungen in benutzerdefinierten Feldern

Um uns auf zukünftige Verbesserungen vorzubereiten, die Ihnen beim Hinzufügen von Berechnungen zu benutzerdefinierten Formularen helfen, haben wir die Syntax für referenzierte Felder standardisiert, die Sie zu einer Berechnung hinzufügen. Diese neue Syntax ist einfach zu verwenden, da das System sie für Sie eingibt, wenn Sie mit der Eingabe des Namens eines Felds beginnen und es dann auswählen.

## Präzise Informationen beibehalten, wenn zwei Benutzer mit einer gemeinsamen Rolle an einem Genehmigungsprozess beteiligt sind

Um die Richtigkeit Ihrer Daten für die Validierung von Arbeiten sicherzustellen, haben wir die Art und Weise geändert, wie Validierungsinformationen für einen Artikel aufgezeichnet werden, wenn dem Artikel ein Prozess mit mehreren Rollen zugeordnet ist.

Einige Genehmigungsprozesse erfordern die Genehmigung von zwei verschiedenen Rollen, und zwei verschiedene genehmigende Personen können eine dieser Rollen gemeinsam haben. Wenn dies passiert, nachdem die Genehmigungsentscheidungen getroffen wurden, zeichnet Workfront jede genehmigende Person und ihre jeweilige Rolle auf, die mit dem Genehmigungsprozess verknüpft ist.

Vor dieser Änderung wurden beide Genehmigungen für den zweiten Benutzer aufgezeichnet, da er eine der Genehmigungsrollen mit der ersten genehmigenden Person teilte. In diesem Fall hat die zweite genehmigende Person die Informationen der ersten genehmigenden Person überschrieben.

Weitere Informationen zu Genehmigungsprozessen in Workfront finden Sie unter [Übersicht über Genehmigungsprozesse](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Zuordnungsstunden werden bei Änderungen an Zuweisungen nicht mehr entfernt

>[!NOTE]
>
>Diese Funktion sollte ursprünglich mit Version 22.2 veröffentlicht werden. Es wurde am 21. April 2022 in der Produktionsumgebung veröffentlicht.


Um die Genauigkeit Ihrer Daten zu gewährleisten, haben wir eine Änderung vorgenommen, um die Zuordnungsstunden beizubehalten und die geplanten Stunden für Aufgaben unverändert zu lassen, wenn Änderungen an Zuweisungen für die Aufgabe vorgenommen werden.

Die folgenden Änderungen wurden an Aufgaben mit dem Typ Einfache Dauer vorgenommen:

* Geplante Stunden werden beibehalten, wenn alle Zugewiesenen entfernt werden.

* Einzelne Zuweisungen bleiben beim Ersetzen von Benutzern und Rollen erhalten.

* Einzelne Zuweisungen bleiben bei der Rolle erhalten, wenn Benutzer entfernt werden. (Aus Version entfernt. Die geplanten Stunden werden nun auf 0 gesetzt, nachdem alle Bevollmächtigten entfernt wurden.)


Weitere Informationen zu den geplanten Stunden finden Sie unter [Übersicht über die geplanten Stunden](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Verbesserungen für Pinnwände

Die folgenden Verbesserungen wurden den Adobe Workfront-Pinnwänden hinzugefügt:

* Filteroptionen - Sie können jetzt auf einer Pinnwand nach Fälligkeitsdatum oder Status filtern. Der Filter wurde auch mit ausblendbaren Abschnitten aktualisiert, um die Optionen zu trennen.

* Pinnwand archivieren - Sie können jetzt eine Pinnwand archivieren, während Sie sich auf der Pinnwand befinden, anstatt zum Pinnwand-Dashboard wechseln zu müssen.

* Team zu einem Board hinzufügen - Wenn Sie nach Mitgliedern suchen, können Sie ein ganzes Team hinzufügen. Wenn Sie ein Team auswählen, werden alle Mitglieder des Teams dem Board hinzugefügt.

* Ablagebereiche in Spalten - Beim Ziehen einer Karte von einer Pinnwand in eine andere zeigt eine graue „Ablagefläche“ jetzt an, wo die Karte platziert wird. Zuvor gab es keinen visuellen Indikator für die Platzierung der Karte.

* Verbundene Karten : Sie können jetzt Karten hinzufügen, die mit Workfront-Aufgaben und -Problemen verbunden sind. Wenn Sie den Namen, die Beschreibung oder den Bevollmächtigten auf der Karte oder in der Aufgabe aktualisieren, werden dieselben Felder auch auf der anderen Seite aktualisiert.

* Statusfeld auf allen Karten - Ein Statusfeld und eine Schaltfläche Abgeschlossen markieren wurden sowohl zu Ad-hoc- als auch zu verbundenen Karten hinzugefügt. Wenn Sie auf Fertig stellen klicken, ändert sich der Status automatisch in Fertig stellen.

* Konvertieren einer Ad-hoc-Karte in eine verbundene Karte - Sie haben jetzt die Möglichkeit, aus den Kartendetails eine Ad-hoc-Karte in eine verbundene Karte zu konvertieren.

* Verbundene Karte trennen - Durch das Trennen einer verbundenen Karte wird die Verbindung mit dem Workfront-Objekt unterbrochen. Die Karte verbleibt als Ad-hoc-Karte auf der Pinnwand und das Workfront-Objekt ist davon nicht betroffen.

* Statuszuordnung in Spalten - Mit neuen Spalteneinstellungen und Richtlinien können Sie einen Status, einen Verantwortlichen oder ein Tag definieren, das auf Karten angewendet wird, die in diese Spalte verschoben werden. Außerdem wurden die standardmäßigen Spaltennamen auf einer neuen Pinnwand in Spalte 1, Spalte 2 und Spalte 3 geändert.

* Aktualisierungsanzeige des Feldes : Beim Speichern einer Karte wird jetzt eine Anzeige angezeigt, die bestätigt, dass die Aktualisierungen gespeichert wurden.


Weitere Informationen finden Sie unter [Erste Schritte mit Pinnwänden in Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Freigeben von Ordnern nur in den obersten fünf Ebenen einer Ordnerhierarchie

Um eine optimale Leistung für Benutzer zu gewährleisten, die Ordner freigeben, beschränken wir die Freigabe derzeit auf die fünf obersten Ebenen in einer Ordnerhierarchie für ein Objekt.

Jeder Ordner auf der sechsten Ebene oder darunter erbt seine Freigabekonfigurationen von dem Ordner direkt darüber.

Weitere Informationen zum Freigeben von Ordnern finden Sie [Freigeben eines Dokumentordners der obersten Ebene](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Workfront-Kampagnen (Beta) - eine neue Methode zur Verwaltung Ihrer Arbeit

>[!NOTE]
>
>Diese Funktion wird voraussichtlich am 9. Januar 2023 aus der Vorschau entfernt. Weitere Informationen finden Sie auf der Übersichtsseite zur Version [23.1 &#x200B;](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Diese Funktion wird in der Produktionsversion 22.3 nicht enthalten sein. Es wird mit einer zukünftigen Version in der Produktion veröffentlicht.


>[!NOTE]
>
>Diese Funktion ist nur als Beta-Version verfügbar und befindet sich derzeit im Aufbau. Wir werden bei zukünftigen Versionen weiterhin Funktionen für den Campaign-Workflow hinzufügen. Die Teilnahme am Beta-Programm für Workfront-Kampagnen ist freiwillig.

Wir führen ein neues Objekt in Adobe Workfront ein, das das Potenzial hat, die Verwaltung der Arbeit zu ändern.

Mit Workfront Campaign können Sie Projekte aus verschiedenen Portfolios und Programmen in einem neuen Arbeitscontainer organisieren. Dieser neue Container wird sich in zukünftigen Versionen weiterentwickeln und schließlich alle Arbeitsobjekte enthalten, die derzeit in separaten Silos verwaltet werden.

In dieser Version sind die folgenden Funktionen enthalten:

* Ein neues Workfront-Objekt namens Campaign

* Ein neuer Kampagnenbereich (Beta) im Hauptmenü

* Eine Liste der Kampagnen im Bereich Kampagnen

* Eine Seite mit Kampagnendetails, auf der zusätzliche Informationen zu einer Kampagne angezeigt werden

* Hinzufügen von Projekten zu einer Kampagne

* Möglichkeit, Informationen über eine Kampagne zu bearbeiten

* Möglichkeit zum Umbenennen des Campaign-Objekts über die Layout-Vorlage

  System- und Gruppenadministratoren von Workfront können den Bereich Kampagnen (Beta) in das Hauptmenü einer Layout-Vorlage einfügen. Dadurch ist es für alle der Vorlage zugewiesenen Benutzer verfügbar. Sobald sie verfügbar ist, kann jeder in Workfront eine Kampagne erstellen.




