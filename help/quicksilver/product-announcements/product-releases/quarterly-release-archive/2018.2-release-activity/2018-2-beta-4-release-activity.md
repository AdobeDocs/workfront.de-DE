---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 4 2018.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 4 Version 2018.2 verfügbar waren. Die Funktion wird am 17. Mai 2018 in der Vorschau-Umgebung verfügbar sein. Sie wird ab Juli 2018 in der Produktionsumgebung verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# Versionsaktivität von Beta 4 2018.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 4 Version 2018.2 verfügbar waren. Die Funktion wird am 17. Mai 2018 in der Vorschau-Umgebung verfügbar sein. Sie wird ab Juli 2018 in der Produktionsumgebung verfügbar sein.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.2 finden Sie unter  Übersicht über die Versionsaktivität [2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die Beta 4-Version 2018.2 enthält die Verbesserungen für Workfront-Administratoren und andere Benutzende:

**Für Administratoren**

* [Systemeinstellung: Sitzungsinformationen auf externen Seiten](#system-setting-session-information-in-external-pages)

**Für alle Benutzer**

* [Verbesserungen am Limit für laufende Arbeiten (Work In Progress, WIP) auf dem Kanban-Board](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [Verbesserte Benutzeroberfläche zum Konfigurieren von Status für ein Agile-Team](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [Aktualisierte Arbeitsliste (linker Bereich) im Bereich Startseite](#updated-work-list-left-panel-in-the-home-area)
* [Neuer Desktop Proofing Viewer für das Proofing interaktiver (Rich-Media-)Inhalte](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content) 
* [Exportieren Sie die Benutzeransicht im Ressourcenplaner](#export-the-user-view-in-the-resource-planner)
* [Support für Google Team Drives](#support-for-google-team-drives)
* [Neue Exportbegrenzung für das Gantt-Diagramm](#new-export-limit-for-the-gantt-chart)
* [Die Option Aus Zwischenablage einfügen wird jetzt bei Verwendung von Internet Explorer oder Safari als abgeblendet angezeigt](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [Neue Beta-Umgebung für Android zusammen mit neuen Funktionen](#new-beta-environment-for-android-along-with-new-features)
* [Beispiele für Filter für Nachrichten zu Ereignisabonnements](#examples-of-filters-for-event-subscriptions-messages)

## Verbesserte Grenzwerte für laufende Arbeiten (Work In Progress, WIP) auf dem Kanban-Board {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### Konfigurieren Sie Work In Progress (WIP)-Beschränkungen für jede Spalte auf dem Kanban-Board

Jetzt können Sie die Work In Progress (WIP)-Beschränkungen für jede Spalte auf der Kanban-Pinnwand konfigurieren. 

Vor dieser Änderung konnten Sie nur eine WIP-Beschränkung konfigurieren, die für alle Spalten auf dem Kanban-Board galt. 

Weitere Informationen finden Sie in diesem Abschnitt .  [Konfigurieren des Work In Progress (WIP)-Limits](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) im Artikel  [Kanban konfigurieren](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

### Aktualisieren Sie das Work In Progress (WIP)-Limit direkt über das Kanban-Board

Jetzt können Team-Mitglieder mit Bearbeitungsrechten für das Team die WIP-Beschränkung direkt über das Kanban-Board aktualisieren.

Vor dieser Änderung konnten Sie die WIP-Beschränkung nur im Bereich Team-Einstellungen aktualisieren.

Weitere Informationen finden Sie unter  Im Artikel .

## Verbesserte Benutzeroberfläche zum Konfigurieren von Status für ein Agile-Team {#improved-interface-for-configuring-statuses-for-an-agile-team}

Die Benutzeroberfläche zum Konfigurieren von Status für ein agiles Team wurde mit den folgenden Verbesserungen aktualisiert:

* Neues Erscheinungsbild
* Statusspalten per Drag &amp; Drop neu anordnen 

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Kanban konfigurieren](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [Konfigurieren von Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Aktualisierte Arbeitsliste (linker Bereich) im Bereich Startseite {#updated-work-list-left-panel-in-the-home-area}

Die Arbeitsliste im Bereich Startseite enthält die folgenden Verbesserungen:

* Ungelesene Gegenstände stechen jetzt durch fett gedruckte und blaue Punkte hervor.

  Elemente, die außerhalb des Home-Bereichs angezeigt werden, werden im Home-Bereich weiterhin als Ungelesen angezeigt.

  Weitere Informationen finden Sie unter [Elemente in der Arbeitsliste im Bereich Startseite anzeigen](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Probleme werden jetzt durch ein Problem-Symbol gekennzeichnet, das neben dem Problem angezeigt wird.
* Genehmigungen werden nun nach Validierungstyp unterschieden, wobei der Typ der Genehmigung angezeigt wird. Zu den möglichen Validierungstypen gehören Aufgabe, Projekt, Problem, Zugriff, Dokument, Arbeitszeittabelle und Testversand.

  Vor dieser Änderung wurden Genehmigungen nur durch das Wort „Genehmigung“ gekennzeichnet.

* Elemente werden jetzt danach unterschieden, ob sie startbereit sind. Mögliche Optionen sind „Bereit zum Start“, „Nicht bereit“ oder „Bearbeiten“.

  Diese Informationen werden für Genehmigungen nicht angezeigt, da Genehmigungen immer startbereit sind.

* Jedes Mal, wenn ein Dokument an das Element angehängt wird, wird unter dem Namen des Elements ein Dokumentsymbol angezeigt.
* Sie können jetzt Gruppierungen innerhalb der Arbeitsliste reduzieren und erweitern, um besser steuern zu können, welche Informationen sichtbar sind. Die Gruppierungen sind „Verspätet“, „Projekte“, „Daten“ und „Abgeschlossen“.

  Standardmäßig wird der Abschnitt Diese Woche erweitert und alle anderen Gruppierungen werden reduziert.

* Wählen Sie aus, ob Elemente nach dem geplanten Abschlussdatum oder dem Commit-Datum sortiert werden sollen.
* Die Anzahl der Elemente in jeder Gruppierung wird jetzt in Klammern neben dem Gruppierungstitel angezeigt.

  Diese Zahl ist für die abgeschlossene Gruppierung nicht verfügbar.

  Weitere Informationen finden Sie unter [Elemente in der Arbeitsliste im Bereich Startseite anzeigen](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Ändern der Größe der Arbeitsliste per Drag &amp; Drop. Sie können die Größe der Arbeitsliste so ändern, dass sie bis zu die Hälfte des Bildschirms einnimmt. Die eingestellte Größe wird bei Ihrem nächsten Zugriff auf die Startseite beibehalten.

  Vor dieser Änderung konnte die Größe der Arbeitsliste nicht geändert werden.

* Bei Anfragen wird jetzt der Benutzeravatar des Benutzers angezeigt, der die Anfrage gestellt hat, mit dem Text &quot;[Genehmiger_name] für den Ihre Genehmigung erforderlich ist.“
* Beim Erstellen einer neuen persönlichen Aufgabe wird die Schaltfläche „Aufgaben“ jetzt als „Persönlich“ gekennzeichnet.

  Weitere Informationen finden Sie unter [Erstellen von Arbeitselementen aus dem ](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)) im Artikel [Erstellen von Arbeitselementen aus dem ](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Verspätete Elemente werden erst nach einer Stunde nach dem geplanten Abschlussdatum als verspätet angezeigt.

Weitere Informationen zum Bereich „Startseite“ finden Sie unter [Verwenden des Bereichs „Startseite](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Neuer Desktop Proofing Viewer für Proofing von interaktiven Inhalten (Rich-Media) {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

Mit dem neuen Desktop Proofing Viewer können Sie interaktive Inhalte prüfen. Im Gegensatz zur vorhandenen Proofing Viewer- und der neuen Proofing Viewer-Komponente, die im Browser ausgeführt werden, ist der Desktop Proofing Viewer eine Anwendung, die auf Ihrer Workstation ausgeführt wird.

Vor dem neuen Desktop Proofing Viewer konnten Sie interaktive Inhalte nur im alten Proofing Viewer prüfen. 

Der Desktop Proofing Viewer bietet folgende Verbesserungen gegenüber dem alten Proofing Viewer für das Proofing interaktiver Inhalte:

* Überprüfen von ungesicherten (HTTP-)Sites

  Mit dem alten Proofing Viewer konnten Sie nur sichere (HTTPS-)Sites überprüfen

* Überprüfen Sie iframe-geschützte Websites (Websites, die davor geschützt sind, in einem iframe angezeigt zu werden).

  Der alte Proofing Viewer unterstützte keine Überprüfung für Sites, die davor geschützt sind, in einem iFrame angezeigt zu werden.

* Anzeigen von Inhalten mit vorkonfigurierten Auflösungen für verschiedene Geräte Sie können beispielsweise sehen, wie Inhalte auf verschiedenen Standard-Desktop-Auflösungen oder auf einzelnen Geräten wie einem iPhone 8 angezeigt werden. 

Weitere Informationen zum Herunterladen, Installieren und Verwenden des Desktop Proofing Viewers finden Sie unter .

Weitere Informationen zu den Funktionsunterschieden zwischen dem Desktop Proofing Viewer und den browserbasierten Proofing Viewern finden Sie unter [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer - Übersicht](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

## Exportieren der Benutzeransicht im Ressourcenplaner {#export-the-user-view-in-the-resource-planner}

Der Export der Daten aus dem Ressourcenplaner wurde vorübergehend deaktiviert, während sie in der Benutzeransicht angezeigt wurden, um Leistungsprobleme zu beheben. Mit dieser Version aktivieren wir den Datenexport erneut, wenn der Ressourcenplaner in der Benutzeransicht angezeigt wird.

Weitere Informationen zum Exportieren der Ressourcenplaner-Daten nach Excel finden Sie im Abschnitt „Exportoption“ in [Übersicht über die Ressourcenplaner-](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Informationen zur Teilnahme an unserem aktuellen Beta-Programm für den Ressourcenplaner finden Sie unter [Resource Planner Performance Beta.](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront?profile.language=de)

## Systemeinstellung: Sitzungsinformationen auf externen Seiten {#system-setting-session-information-in-external-pages}

Der Workfront-Administrator kann jetzt die Verwendung von Sitzungsinformationen (z. B. Sitzungs-ID) beim Erstellen einer externen Seite einschränken.

Vor dieser Änderung konnten Benutzende, die externe Seiten erstellen konnten, beliebige Sitzungsinformationen verwenden, wenn sie andere Sites in ein Workfront-Dashboard einbetteten. 

Weitere Informationen zum Konfigurieren Ihrer Systemeinstellungen in Workfront finden Sie unter [Konfigurieren von Systemsicherheitseinstellungen](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Unterstützung für Google Team Drives {#support-for-google-team-drives}

Sie können jetzt ein Dokument oder einen Ordner auf einem Google Team Drive von Workfront aus verknüpfen.

Vor dieser Verbesserung konnten Sie ein Dokument oder einen Ordner verknüpfen, der sich nur auf dem Google My Drive befindet.

Weitere Informationen zum Verknüpfen von Dokumenten und Ordnern aus verschiedenen Programmen mit Workfront finden Sie unter [Verknüpfen von Dokumenten aus externen Programmen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Neue Exportbeschränkung für das Gantt-Diagramm {#new-export-limit-for-the-gantt-chart}

Im Gantt-Diagramm können Sie jetzt bis zu 500 Aufgaben exportieren.

Zuvor konnten Sie nur bis zu 250 Aufgaben exportieren.

Weitere Informationen finden Sie unter [Exportieren des Gantt-Diagramms nach PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Die Option Aus Zwischenablage einfügen wird jetzt bei Verwendung von Internet Explorer oder Safari als abgeblendet angezeigt {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

Die Option Aus Zwischenablage einfügen wird jetzt abgeblendet angezeigt, wenn der Internet Explorer oder Safari verwendet werden, mit einer QuickInfo, die erklärt, dass nur die Browser Chrome und Firefox für diese Funktion unterstützt werden.

Vor dieser Änderung wurde diese Option bei der Verwendung von Internet Explorer oder Safari nicht angezeigt. 

Weitere Informationen zum Einfügen von Bildern aus der Zwischenablage finden Sie unter [Einfügen von Bildern aus der Zwischenablage](../../../../documents/managing-documents/paste-image-clipboard.md).

## Neue Beta-Umgebung für Android zusammen mit neuen Funktionen {#new-beta-environment-for-android-along-with-new-features}

Sie können jetzt die neuesten Funktionen erleben, an denen unser Team für die Mobile App arbeitet, bevor sie für die allgemeine Öffentlichkeit freigegeben werden, indem Sie sich als Betatester anmelden. Diese Umgebung wird derzeit nur für Android-Smartphones für die Workfront-Mobile-App unterstützt.

Weitere Informationen dazu, wie Sie sich als Betatester für die Workfront Mobile App anmelden, finden Sie unter .

Die folgenden Verbesserungen sind jetzt in der Beta-Version der Mobile App verfügbar:

* Neue Kontoseite

  Sie können jetzt auf der neuen Kontoseite Ihre Kontoinformationen anzeigen sowie Ihre Mobile-Einstellungen verwalten, Feedback senden oder sich abmelden.

  Vor dieser Verbesserung konnten Sie Ihre Kontoinformationen in der Mobile App nicht anzeigen und über das Workfront-Hauptmenü auf Ihre Einstellungen zugreifen, Feedback senden und sich abmelden.

* Neues unteres Navigationsfenster

  Unten im Bildschirm ist jetzt eine hervorgehobene Navigationsleiste verfügbar, mit der alle Bereiche der Mobile App gestartet werden können.

  Vor dieser Verbesserung wurden die Funktionsbereiche im Hauptmenü von Workfront aufgeführt. Das Workfront-Hauptmenü wurde entfernt und durch die neue untere Navigationsleiste ersetzt.

  Weitere Informationen zum Konfigurieren der neuen Navigationsleiste finden Sie im Abschnitt „Konfigurieren Ihrer Mobile App“ in .

* Neue Benachrichtigungslistenansicht

  Ein verbessertes Erscheinungsbild der Benachrichtigungsliste ermöglicht es Ihnen, die Benachrichtigungen in Ihrer Liste einfach danach zu unterscheiden, welche Art von Benachrichtigungen sie sind und ob sie gelesen wurden.

* Das Suchfeld wurde an eine markantere Position verschoben.

* Neue AnmeldeerfahrungEs gibt eine neue, optimierte Anmeldeerfahrung.

* Neues Tutorial-Erlebnis

  Neue Tutorials stehen jetzt zur Verfügung, die Benutzer beim ersten Anmelden kurz durch die App führen. Vor diesem Erlebnis wurden die Tutorials nur gestartet, wenn Benutzer auf bestimmte Funktionsbereiche zugegriffen haben.

## Beispiele für Filter für Nachrichten zu Ereignisabonnements {#examples-of-filters-for-event-subscriptions-messages}

Um zu demonstrieren, wie Sie Ereignisabonnements so filtern können, dass nur die für Ihr Unternehmen relevanten Nachrichten empfangen werden, sind jetzt Beispiel-Code-Snippets zum Filtern des Flusses von Ereignissen verfügbar, die zu Ihren Endpunkten kommen. Weitere Informationen zum Anzeigen der Filterbeispiele finden Sie unter [Filtern von Ereignisabonnementnachrichten](../../../../wf-api/api/filter-event-sub-messages.md).
