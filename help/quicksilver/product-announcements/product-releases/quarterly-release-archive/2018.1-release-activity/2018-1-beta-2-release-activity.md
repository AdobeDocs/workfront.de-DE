---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 2-Release-Aktivität 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.1 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 14. Dezember 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird im März 2018 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 2%

---

# Beta 2-Release-Aktivität 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.1 verfügbar waren. Die Funktionalität auf dieser Seite wurde am 14. Dezember 2017 in der Vorschau-Umgebung bereitgestellt. Sie wird im März 2018 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.1 vorgenommen wurden, finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Beta 2-Version 2018.1 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Gruppenverwaltung für Benutzer und Layoutvorlagen](#group-administration-for-users-and-layout-templates)

**Für alle Benutzer**

* [Systemweite Breitbildanzeige](#system-wide-widescreen-display)
* [Ändern der Größe des Timeline-Snapshots auf dem Gantt-Diagramm](#resize-timeline-snapshot-on-the-gantt-chart)
* [Interaktiver Ressourcen-Planer im Geschäftsfall](#interactive-resource-planner-in-the-business-case)
* [Visualisierung im Ressourcenplaner - Diagramm für die Benutzerzuordnung](#visualization-in-the-resource-planner-user-allocation-chart)
* [Verbesserungen im Startbereich](#improvements-in-the-home-area)
* [Neue Verbesserungen beim Testversand-Viewer](#new-proofing-viewer-improvements) 

## Gruppenverwaltung für Benutzer und Layoutvorlagen {#group-administration-for-users-and-layout-templates}

Sie können jetzt Gruppenadministratoren in Workfront bestimmen. Das Feld Gruppeninhaber wurde in Gruppenadministrator umbenannt. Benutzer, die als Gruppenadministratoren benannt wurden, verfügen über zusätzliche Berechtigungen zur Verwaltung von Benutzern und Layoutvorlagen für die von ihnen verwalteten Gruppen.

* [Benutzerverwaltung durch Gruppenadministrator](#user-management-by-group-administrator)
* [Verwaltung von Layout-Vorlagen durch Gruppenadministratoren](#layout-template-management-by-group-administrators)

### Benutzerverwaltung nach Gruppenadministrator {#user-management-by-group-administrator}

Wir führen das neue Konzept von **Gruppenadministrator** ein. Um dies zu unterstützen, wurde das Feld **Gruppeneigentümer** in **Gruppenadministrator** umbenannt und die Benutzer, die als Gruppenadministratoren benannt sind, verfügen über zusätzliche Berechtigungen zum Verwalten von Benutzern und Gruppen.

Zusätzlich zu den Berechtigungen, die der Gruppeneigentümer zuvor für die Verwaltung von Benutzern hatte, hat der Gruppenadministrator jetzt den folgenden zusätzlichen Zugriff bei der Verwaltung von Benutzern in den Gruppen, in denen sie als Gruppenadministrator festgelegt sind:

* Melden Sie sich als anderer Benutzer an, der zu einer von ihm verwalteten Gruppe gehört.
* Setzen Sie das Kennwort für einen anderen Benutzer zurück, der zu einer von ihm verwalteten Gruppe gehört.
* Erstellen Sie Layoutvorlagen, die von ihrer Gruppe verwaltet werden. 

Vor dieser Änderung konnte nur der Workfront-Administrator diese Funktionen ausführen.

Weitere Informationen zu Gruppenadministratoren finden Sie im Abschnitt &quot;Grundlegendes zu Gruppenadministratoren&quot;unter [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Verwaltung von Layout-Vorlagen durch Gruppenadministratoren {#layout-template-management-by-group-administrators}

Wir stellen das neue Konzept von **Gruppe mit Administratorzugriff** vor, das Sie mit einer Layout-Vorlage verknüpfen können.

Der Benutzer, der für diese Gruppe als Gruppenadministrator bestimmt wurde, hat Zugriff auf die Verwaltung dieser Layout-Vorlage und die Erstellung neuer Layoutvorlagen, in denen die Gruppen, die er verwaltet, die Administratorgruppen der Vorlagen sind. 

Vor dieser Änderung konnte nur der Workfront-Administrator Layoutvorlagen erstellen.

Weitere Informationen zum Erstellen von Layoutvorlagen finden Sie unter &quot;Erstellen und Verwalten von Layoutvorlagen&quot;.

## Systemweite Breitbildanzeige {#system-wide-widescreen-display}

Wenn Sie eine Seite in Workfront anzeigen, wird jetzt automatisch das gesamte Browser-Fenster ausgefüllt und an Ihre Bildschirmgröße angepasst.

Vor dieser Änderung wurden nur die mit den folgenden Objekten verknüpften Seiten in Widescreen angezeigt:

* Projekte
* Aufgaben
* Probleme
* Berichte
* Dashboards
* Kalender

## Ändern der Größe des Timeline-Schnappschusses im Gantt-Diagramm {#resize-timeline-snapshot-on-the-gantt-chart}

Sie können nun den Timeline-Schnappschuss erweitern, um das gesamte Projekt im Gantt-Diagramm anzuzeigen.

Vor dieser Verbesserung können Sie einen bestimmten Punkt auf dem Timeline-Schnappschuss auswählen, um im Gantt-Diagramm zu ihm zu navigieren.

Weitere Informationen zum Konfigurieren der Anzeige von Informationen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Interaktiver Ressourcen-Planer im Geschäftsfall {#interactive-resource-planner-in-the-business-case}

Als Ressourcen-Manager können Sie jetzt Ressourcen-Pools im Abschnitt &quot;Ressourcenbudgetierung&quot;des Geschäftsfeldes hinzufügen. Sie können Ihre Projektressourcen auch mit dem Ressourcenplaner auf Projektebene einsetzen. Die Budgetierung Ihrer Ressourcen für ein Projekt generiert die budgetierten Arbeitskosten des Projekts.

Vor dieser Änderung konnten Sie die Ressourcen-Budgeting-Informationen im Geschäftsfall anzeigen, wenn das Projekt für Ressourcen im globalen Ressourcen-Planer geplant war.

Weitere Informationen zum Abschließen von Budgeting-Projektressourcen im Geschäftsfall finden Sie unter [Budgetressourcen im Geschäftsfall](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualisierung im Ressourcenplaner - Diagramm für die Benutzerzuordnung {#visualization-in-the-resource-planner-user-allocation-chart}

Sie können nun die gesamte geplante Zuordnung aller Benutzer im Ressourcen-Planer in einer Grafik anzeigen. Das Diagramm ist verfügbar, wenn Sie im Ressourcenplaner die Option **Nach Benutzer anzeigen** auswählen.

Das Diagramm enthält die folgenden Informationen:

* Verfügbarkeit (%) ohne Überallokation für alle Benutzenden
* Überallokation (%) für alle Benutzenden
* Nichtauslastung (%) für alle Benutzenden
* In diesem Zeitraum gibt es eine Überallokation für mindestens einen Benutzer/eine Benutzerin

Vor dieser Änderung konnten Sie die Zuordnung und Verfügbarkeit einzelner Benutzer nur im Tabellenformat anzeigen.

Weitere Informationen über das Diagramm zur Benutzerzuordnung im Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Verbesserungen im Heimbereich {#improvements-in-the-home-area}

Im Bereich Home sind jetzt verschiedene Verbesserungen verfügbar, darunter:

* Verbesserungen beim Erscheinungsbild und Verhalten

   * Das rechte Bedienfeld ist jetzt größer, sodass mehr Platz für Aufgaben- und Probleminformationen zur Verfügung steht.
   * Überfällige Elemente werden jetzt in einer helleren Rot-Schattierung angezeigt, wenn sie im linken Bereich ausgewählt sind.
   * Sie können jetzt die Beziehung zwischen dem linken und dem rechten Bedienfeld leichter erkennen. Das im linken Bereich ausgewählte Dokument verweist auf den rechten Bereich.

* Für ausgewählte Elemente werden Standardfelder angezeigt. 

  Weitere Informationen zu den Standardfeldern finden Sie unter &quot;Erstellen und Verwalten von Layoutvorlagen&quot;.

* Nachdem Sie bei einer Anfrage auf &quot;Bearbeiten&quot;geklickt haben, werden die mit dem Problem verknüpften Felder im rechten Bereich angezeigt.

  Weitere Informationen zum Bearbeiten von Anforderungen aus dem Home-Bereich finden Sie unter [Verwalten von Arbeits- und Teamanfragen im Home-Bereich](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) in [Verwalten von Arbeits- und Teamanfragen im Home-Bereich](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Zeigen Sie auf einen Benutzeravatar auf ein Arbeitselement im linken Bereich, um den Namen des Benutzers anzuzeigen.
* Erweitern Sie den Bereich &quot;Verspätet&quot;im linken Bereich, um alle verspäteten Elemente anzuzeigen (wenn dieser Bereich ausgeblendet wird, werden nur die ersten fünf Elemente angezeigt).
* Nachdem Sie ein Element als &quot;Abgeschlossen&quot;markiert haben, bleibt das Element im linken Bereich, bis Sie ein anderes Element auswählen.\
  Informationen zum Anzeigen abgeschlossener Elemente finden Sie unter [Anzeigen von Elementen in der Arbeitsliste im Startbereich](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) in [Anzeigen von Elementen in der Arbeitsliste im Startbereich](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

Weitere Informationen zur Verwendung des neuen Home-Bereichs sowie Informationen zu den Unterschieden in der Funktionalität zwischen &quot;Meine Arbeit&quot;und &quot;Home&quot;finden Sie unter [Verwenden des Home-Bereichs](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Neue Verbesserungen beim Testversand-Viewer  {#new-proofing-viewer-improvements}

* [Verbessertes Layout und Design](#improved-layout-and-design)
* [Suchkommentare nach Kommentarnummer](#search-comments-by-comment-number)
* [Option zum Bearbeiten des Kommentars neben dem Markup-Indikator](#option-to-edit-comment-next-to-the-markup-indicator)
* [Alle Kommentare als gelesen markieren](#mark-all-comments-as-read)
* [Verbesserungen des linken Menüs](#left-menu-improvements)

### Verbessertes Layout und Design {#improved-layout-and-design}

Der Testversand-Viewer hat ein aktualisiertes Erscheinungsbild. Die  Die folgenden Bereiche des Testversand-Viewers wurden aktualisiert:

* Bereich &quot;Miniaturansichten&quot;

  Weitere Informationen zur Verwendung des Bereichs &quot;Miniaturansichten&quot;finden Sie unter .

* Kommentarbereich\
  Weitere Informationen zum Kommentarbereich finden Sie unter .
* Linker Menübereich

### Suchkommentare nach Kommentarnummer {#search-comments-by-comment-number}

Wenn Sie nun die Kommentarliste im Testversand-Viewer durchsuchen, können Sie die Nummer des Kommentars in das Suchfeld eingeben. Die Kommentarliste wird dann gefiltert, um den gesuchten Kommentar anzuzeigen. 

Weitere Informationen finden Sie unter .

### Option zum Bearbeiten des Kommentars neben dem Markup-Indikator {#option-to-edit-comment-next-to-the-markup-indicator}

Sie können einen vorhandenen Kommentar jetzt einfacher bearbeiten. Nachdem Sie auf eine Kommentaranzeige für den Testversand geklickt haben, wird neben dem Ballon ein Bearbeitungssymbol angezeigt. 

Vor dieser Änderung mussten Sie auf das Bearbeitungssymbol im Kommentarbereich klicken.  

Weitere Informationen finden Sie unter .

### Alle Kommentare als &quot;Gelesen&quot;markieren {#mark-all-comments-as-read}

Beim Anzeigen eines Dokuments im Testversand-Viewer können Sie jetzt alle Kommentare als &quot;Gelesen&quot;markieren.

### Verbesserungen des linken Menüs {#left-menu-improvements}

Das Menü auf der linken Seite des Testversand-Viewers enthält folgende Verbesserungen:

* Aktualisiertes Erscheinungsbild
* Symbol oben im Menü zum Anzeigen oder Ausblenden des Menüs

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* Bewegen Sie den Mauszeiger über das Menü, um das Menü automatisch zu erweitern und neben den Symbolen Beschriftungen anzuzeigen. (Oder aktivieren Sie die Option, damit das Menü immer in der minimierten Ansicht angezeigt wird.)
