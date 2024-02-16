---
content-type: release-notes
navigation-topic: product-releases-archive
title: Aktivität "Beta 4"(Version 2018.2)
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschauumgebung mit Beta-Version 2018.2 verfügbar waren. Die Funktion ist ab dem 17. Mai 2018 in der Vorschau-Umgebung verfügbar. Sie wird im Juli 2018 im Produktionsumfeld zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# Aktivität &quot;Beta 4&quot;(Version 2018.2)

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschauumgebung mit Beta-Version 2018.2 verfügbar waren. Die Funktion ist ab dem 17. Mai 2018 in der Vorschau-Umgebung verfügbar. Sie wird im Juli 2018 im Produktionsumfeld zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.2 vorgenommen wurden, finden Sie unter  [Übersicht über die Versionsaktivität 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die Beta-Version 2018.2 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Systemeinstellung: Sitzungsinformationen auf externen Seiten](#system-setting-session-information-in-external-pages)

**Für alle Benutzer**

* [Laufende Arbeiten (WIP) - Verbesserungen bei der Beschränkung auf das Kanban-Board](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [Verbesserte Benutzeroberfläche zum Konfigurieren von Status für ein Agile-Team](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [Arbeitsliste (linker Bereich) im Startbereich aktualisiert](#updated-work-list-left-panel-in-the-home-area)
* [Neuer Desktop Proofing Viewer für den Proofing interaktiver (Rich Media) Inhalte](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content) 
* [Exportieren der Benutzeransicht in den Ressourcenplaner](#export-the-user-view-in-the-resource-planner)
* [Support für Google-Team-Laufwerke](#support-for-google-team-drives)
* [Neue Exportbeschränkung für das Gantt-Diagramm](#new-export-limit-for-the-gantt-chart)
* [Option &quot;Aus Zwischenablage einfügen&quot;wird jetzt bei Verwendung von Internet Explorer oder Safari als ausgeblendet angezeigt](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [Neue Beta-Umgebung für Android und neue Funktionen](#new-beta-environment-for-android-along-with-new-features)
* [Beispiele für Filter für Meldungen zu Ereignisabonnements](#examples-of-filters-for-event-subscriptions-messages)

## Laufende Arbeiten (WIP) - Verbesserungen bei der Beschränkung auf das Kanban-Board {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### Konfigurieren der Einschränkungen für laufende Arbeiten (WIP) für jede Spalte auf dem Kanban-Board

Jetzt können Sie die Work in Progress (WIP)-Beschränkungen für jede Spalte auf dem Kanban-Board konfigurieren. 

Vor dieser Änderung konnten Sie nur eine WIP-Begrenzung konfigurieren, die für alle Spalten auf der Kanban-Pinnwand galt. 

Weitere Informationen finden Sie im Abschnitt .  [Konfigurieren der Grenze für laufende Arbeit (WIP)](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4) im Artikel  [Kanban konfigurieren](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

### Direkte Aktualisierung des Grenzwerts für laufende Arbeiten (WIP) durch das Kanban-Board

Jetzt können Teammitglieder mit Bearbeitungsrechten für das Team die WIP-Grenze direkt über das Kanban-Board aktualisieren.

Vor dieser Änderung können Sie die WIP-Beschränkung nur im Bereich Team Settings aktualisieren.

Weitere Informationen finden Sie im Artikel .

## Verbesserte Benutzeroberfläche zum Konfigurieren von Status für ein Agile-Team {#improved-interface-for-configuring-statuses-for-an-agile-team}

Die Benutzeroberfläche zum Konfigurieren von Status für ein agiles Team wurde mit folgenden Verbesserungen aktualisiert:

* Neues Erscheinungsbild
* Neuanordnen von Statusspalten per Drag &amp; Drop 

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Kanban konfigurieren](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [Konfigurieren von Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Arbeitsliste (linker Bereich) im Startbereich aktualisiert {#updated-work-list-left-panel-in-the-home-area}

Die Arbeitsliste im Bereich &quot;Startseite&quot;enthält folgende Verbesserungen:

* Ungelesene Elemente lassen sich jetzt durch Fettdruck und einen blauen Punkt hervorheben.

  Elemente, die außerhalb des Startbereichs angezeigt werden, werden weiterhin im Startbereich als Ungelesen angezeigt.

  Weitere Informationen finden Sie unter [Anzeigen von Elementen in der Arbeitsliste im Startbereich](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Probleme werden jetzt durch ein Symbol für ein Problem unterschieden, das neben dem Problem angezeigt wird.
* Genehmigungen werden nun nach Genehmigungstyp unterschieden, wobei der Typ der Genehmigung angezeigt wird. Mögliche Validierungstypen sind &quot;Aufgabe&quot;, &quot;Projekt&quot;, &quot;Problem&quot;, &quot;Zugriff&quot;, &quot;Dokument&quot;, &quot;Datenblatt&quot;und &quot;Testversand&quot;.

  Vor dieser Änderung wurden Genehmigungen nur durch das Wort &quot;Genehmigung&quot;unterschieden.

* Elemente werden nun danach unterschieden, ob sie startbereit sind. Mögliche Optionen sind &quot;Bereit zum Start&quot;, &quot;Nicht bereit&quot;oder &quot;Arbeiten am&quot;.

  Diese Informationen werden nicht für Genehmigungen angezeigt, da Genehmigungen immer startbereit sind.

* Jedes Mal, wenn ein Dokument an das Element angehängt wird, wird unter dem Namen des Elements ein Dokumentsymbol angezeigt.
* Sie können jetzt Gruppierungen innerhalb der Arbeitsliste reduzieren und erweitern, um besser steuern zu können, welche Informationen sichtbar sind. Die Gruppierungen sind &quot;Verspätet&quot;, &quot;Projekte&quot;, &quot;Datumsangaben&quot;und &quot;Abgeschlossen&quot;.

  Standardmäßig wird der Abschnitt Diese Woche erweitert und alle anderen Gruppierungen werden reduziert.

* Wählen Sie aus, ob die Elemente nach dem geplanten Abschlussdatum oder dem Veröffentlichungsdatum sortiert werden sollen.
* Die Anzahl der Elemente in jeder Gruppierung wird nun in Klammern neben dem Gruppierungstitel angezeigt.

  Diese Zahl steht für die Gruppe Abgeschlossen nicht zur Verfügung.

  Weitere Informationen finden Sie unter [Anzeigen von Elementen in der Arbeitsliste im Startbereich](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

* Passen Sie die Größe der Arbeitsliste per Drag &amp; Drop an. Sie können die Größe der Arbeitsliste ändern, um bis zu die Hälfte des Bildschirms zu verbrauchen. Die von Ihnen festgelegte Größe wird beibehalten, wenn Sie das nächste Mal auf Home zugreifen.

  Vor dieser Änderung konnte die Größe der Arbeitsliste nicht geändert werden.

* Für Anfragen wird nun der Benutzeravatar des Benutzers angezeigt, der die Anfrage gestellt hat, mit dem Text &quot;[Genehmiger_Name] Ich möchte Ihre Genehmigung einholen.&quot;
* Bei der Erstellung einer neuen persönlichen Aufgabe wird die Schaltfläche &quot;Aufgaben&quot;jetzt als &quot;persönlich&quot;bezeichnet.

  Weitere Informationen finden Sie unter [Erstellen von Arbeitselementen aus dem Startbereich](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) im Artikel [Erstellen von Arbeitselementen aus dem Startbereich](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Verspätete Elemente werden nur als spät angegeben, nachdem eine Stunde nach dem geplanten Abschlussdatum vergangen ist.

Weitere Informationen zum Startbereich finden Sie unter [Verwenden des Startbereichs](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Neuer Desktop Proofing Viewer für den Proofing interaktiver (Rich Media) Inhalte {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

Mit dem neuen Desktop Proofing Viewer können Sie interaktive Inhalte testen. Im Gegensatz zum vorhandenen alten Testversand-Viewer und dem neuen Testversand-Viewer, der im Browser ausgeführt wird, ist der Desktop Proofing Viewer eine Anwendung, die auf Ihrer Workstation ausgeführt wird.

Vor dem neuen Desktop Proofing Viewer konnten Sie interaktive Inhalte nur im alten Testversand-Viewer testen. 

Der Desktop Proofing Viewer enthält die folgenden Verbesserungen gegenüber dem alten Proofing-Viewer für das Testen interaktiver Inhalte:

* Überprüfen nicht gesicherter (HTTP) Sites

  Mit dem alten Testversand-Viewer konnten Sie nur sichere (HTTPS) Sites überprüfen

* Überprüfen Sie iframe-geschützte Sites (Sites, die vor der Anzeige in einem iframe geschützt sind).

  Der alte Testversand-Viewer unterstützte keine Überprüfung für Sites, die vor der Anzeige in einem iframe geschützt sind.

* Anzeigen von Inhalten mit vorkonfigurierten Auflösungen für verschiedene Geräte Sie können beispielsweise sehen, wie Inhalte auf verschiedenen Desktop-Auflösungen oder auf einzelnen Geräten wie iPhone 8 angezeigt werden. 

Weitere Informationen zum Herunterladen, Installieren und Verwenden des Desktop Proofing Viewers finden Sie unter .

Informationen zu den Funktionsunterschieden zwischen dem Desktop Proofing Viewer und den browserbasierten Proofing-Viewern finden Sie unter [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer - Übersicht](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

## Exportieren der Benutzeransicht in den Ressourcenplaner {#export-the-user-view-in-the-resource-planner}

Der Export der Daten aus dem Ressourcen-Planer wurde vorübergehend deaktiviert, wenn er in der Benutzeransicht angezeigt wurde, um einige Leistungsprobleme zu beheben. Mit dieser Version wird der Export von Daten erneut aktiviert, wenn der Ressourcen-Planer in der Benutzeransicht angezeigt wird.

Weitere Informationen zum Exportieren der Ressourcenplandaten in Excel finden Sie im Abschnitt &quot;Exportoption&quot;unter [Navigationsübersicht über den Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Informationen zur Teilnahme an unserem aktuellen Betaprogramm für den Ressourcen-Planer finden Sie unter [Beta-Leistung des Ressourcenplaners.](http://community.workfront.com/discussions/community-home/digestviewer/viewthread?GroupId=457&amp;MessageKey=8b018ed9-97a2-4f9d-a93b-01a7b09b6350&amp;CommunityKey=0425cafc-f0ec-47fc-be20-a21dc073d520&amp;tab=digestviewer&amp;ReturnUrl=%2fdiscussions%2fcommunity-home%2fdigestviewer%3fCommunityKey%3d0425cafc-f0ec-47fc-be20-a21dc073d520)

## Systemeinstellung: Sitzungsinformationen auf externen Seiten {#system-setting-session-information-in-external-pages}

Der Workfront-Administrator kann jetzt die Verwendung von Sitzungsinformationen (z. B. Sitzungs-ID) beim Erstellen einer externen Seite einschränken.

Vor dieser Änderung konnten Benutzer, die externe Seiten erstellen konnten, beim Einbetten anderer Sites in ein Workfront-Dashboard alle Sitzungsinformationen verwenden. 

Weitere Informationen zum Konfigurieren der Systemeinstellungen in Workfront finden Sie unter [Systemsicherheitsvoreinstellungen konfigurieren](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Support für Google-Team-Laufwerke {#support-for-google-team-drives}

Sie können jetzt ein Dokument oder einen Ordner auf einem Google Team Drive von Workfront aus verknüpfen.

Vor dieser Verbesserung könnten Sie ein Dokument oder einen Ordner verknüpfen, der sich nur auf dem Google My Drive befindet.

Weitere Informationen zum Verknüpfen von Dokumenten und Ordnern aus verschiedenen Anwendungen mit Workfront finden Sie unter [Verknüpfen von Dokumenten mit externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Neue Exportbeschränkung für das Gantt-Diagramm {#new-export-limit-for-the-gantt-chart}

Sie können nun bis zu 500 Aufgaben in die Gantt-Grafik exportieren.

Zuvor konnten Sie nur bis zu 250 Aufgaben exportieren.

Weitere Informationen finden Sie unter [Gantt-Diagramm in PDF exportieren](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

## Option &quot;Aus Zwischenablage einfügen&quot;wird jetzt bei Verwendung von Internet Explorer oder Safari als ausgeblendet angezeigt {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

Die Option Aus Zwischenablage einfügen wird jetzt bei Verwendung des Internet Explorer- oder Safari-Browsers als abgeblendet angezeigt. Eine QuickInfo erklärt, dass nur die Chrome- und Firefox-Browser für diese Funktion unterstützt werden.

Vor dieser Änderung wurde diese Option bei Verwendung von Internet Explorer oder Safari nicht angezeigt. 

Weitere Informationen zum Einfügen von Bildern aus der Zwischenablage finden Sie unter [Bilder aus der Zwischenablage einfügen](../../../../documents/managing-documents/paste-image-clipboard.md).

## Neue Beta-Umgebung für Android und neue Funktionen {#new-beta-environment-for-android-along-with-new-features}

Sie können jetzt die neuesten Funktionen, an denen unser Team für die mobile App arbeitet, erleben, bevor sie der allgemeinen Öffentlichkeit zugänglich gemacht werden, indem Sie sich als Beta-Tester anmelden. Diese Umgebung wird derzeit nur für Android-Smartphones für die Workfront-Mobile-App unterstützt.

Weitere Informationen dazu, wie Sie sich als Beta-Tester für die mobile Workfront-App anmelden, finden Sie unter .

Die folgenden Verbesserungen sind jetzt in der Betaversion der Mobile App verfügbar:

* Neue Kontoseite

  Sie können jetzt Ihre Kontoinformationen anzeigen sowie Ihre Mobile-Einstellungen verwalten, Feedback senden oder sich von der neuen Kontoseite abmelden.

  Vor dieser Verbesserung konnten Sie Ihre Kontoinformationen nicht in der Mobile App anzeigen und auf Ihre Einstellungen zugreifen, Feedback senden und sich über das Workfront-Hauptmenü abmelden.

* Neues Navigationsfenster unten

  Unten im Bildschirm ist jetzt eine auffälligere Navigationsleiste verfügbar, die alle Bereiche der App startet.

  Vor dieser Verbesserung wurden die Funktionsbereiche im Hauptmenü von Workfront aufgelistet. Das Hauptmenü von Workfront wurde entfernt und durch die neue untere Navigationsleiste ersetzt.

  Weitere Informationen zum Konfigurieren der neuen Navigationsleiste finden Sie im Abschnitt &quot;Konfigurieren Ihrer Mobile App&quot;in .

* Neue Listenansicht für Benachrichtigungen

  Durch ein verbessertes Erscheinungsbild der Benachrichtigungsliste können Sie die Benachrichtigungen in Ihrer Liste einfach danach unterscheiden, welche Art sie sind und ob sie gelesen wurden.

* Das Suchfeld wurde an eine auffälligere Position verschoben.

* Neues AnmeldeerlebnisEs gibt ein neues, optimiertes Anmeldeerlebnis.

* Neues Tutorial-Erlebnis

  Es stehen jetzt neue Tutorials zur Verfügung, mit denen Benutzer bei der ersten Anmeldung kurz durch die App geführt werden können. Vor diesem Erlebnis wurden die Tutorials nur gestartet, wenn Benutzer auf bestimmte Funktionsbereiche zugegriffen haben.

## Beispiele für Filter für Meldungen zu Ereignisabonnements {#examples-of-filters-for-event-subscriptions-messages}

Um zu demonstrieren, wie Sie Ereignisabos filtern können, um nur die für Ihr Unternehmen relevanten Nachrichten zu erhalten, stehen jetzt Beispielcode-Snippets zum Filtern des Ereignisflusses, der zu Ihren Endpunkten kommt, zur Verfügung. Weitere Informationen zur Anzeige der Filterbeispiele finden Sie unter [Filtern von Ereignis-Abonnementnachrichten](../../../../wf-api/api/filter-event-sub-messages.md).
