---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 2 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.1 verfügbar waren. Die Funktion auf dieser Seite wurde am 14. Dezember 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird ab März 2018 in der Produktionsumgebung verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 2%

---

# Versionsaktivität von Beta 2 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 2 Version 2018.1 verfügbar waren. Die Funktion auf dieser Seite wurde am 14. Dezember 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird ab März 2018 in der Produktionsumgebung verfügbar sein.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.1 finden Sie unter  Übersicht über die Versionsaktivität [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Beta-Version 2018.1 enthält Verbesserungen für Workfront-Administratoren und andere Benutzende:

**Für Administratoren**

* [Gruppenverwaltung für Benutzer und Layoutvorlagen](#group-administration-for-users-and-layout-templates)

**Für alle Benutzer**

* [Systemweite Breitbildanzeige](#system-wide-widescreen-display)
* [Größe der Zeitleisten-Momentaufnahme im Gantt-Diagramm ändern](#resize-timeline-snapshot-on-the-gantt-chart)
* [Interaktiver Ressourcenplaner im Business Case](#interactive-resource-planner-in-the-business-case)
* [Visualisierung im Ressourcenplaner - Benutzerzuordnungsdiagramm](#visualization-in-the-resource-planner-user-allocation-chart)
* [Verbesserungen im Bereich Home](#improvements-in-the-home-area)
* [Neue Korrekturabzugs-Viewer-Verbesserungen](#new-proofing-viewer-improvements) 

## Gruppenverwaltung für Benutzer und Layoutvorlagen {#group-administration-for-users-and-layout-templates}

Sie können jetzt Gruppenadministratoren in Workfront bestimmen. Das Feld Gruppeneigentümer wurde in Gruppenadministrator umbenannt, und Benutzende, die als Gruppenadministratoren festgelegt sind, haben zusätzliche Berechtigungen zum Verwalten von Benutzern und Layout-Vorlagen für die von ihnen verwalteten Gruppen.

* [Benutzerverwaltung durch Gruppenadministrator](#user-management-by-group-administrator)
* [Layoutvorlagenverwaltung durch Gruppenadministratoren](#layout-template-management-by-group-administrators)

### User Management durch Gruppenadministrator {#user-management-by-group-administrator}

Wir führen das neue Konzept des **Gruppenadministrators“**. Dazu wurde das Feld **Gruppeneigentümer** in &quot;**&quot; umbenannt** und die als Gruppenadministratoren benannten Benutzer haben zusätzliche Berechtigungen zum Verwalten von Benutzern und Gruppen.

Zusätzlich zu den Berechtigungen, die der Gruppenbesitzer zuvor zum Verwalten von Benutzern hatte, hat der Gruppenadministrator jetzt den folgenden zusätzlichen Zugriff beim Verwalten von Benutzern innerhalb der Gruppen, in denen er als Gruppenadministrator festgelegt ist:

* Melden Sie sich als ein anderer Benutzer an, der zu einer von ihm verwalteten Gruppe gehört.
* Setzen Sie das Kennwort für einen anderen Benutzer zurück, der zu einer von ihm verwalteten Gruppe gehört.
* Erstellen Sie Layout-Vorlagen, die von ihrer Gruppe verwaltet werden. 

Vor dieser Änderung konnten nur die Workfront-Administratoren diese Funktionen ausführen.

Weitere Informationen zu Gruppenadministratoren finden Sie im Abschnitt „Grundlegendes zu Gruppenadministratoren“ in [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Layoutvorlagenverwaltung durch Gruppenadministratoren {#layout-template-management-by-group-administrators}

Wir führen das neue Konzept der **Gruppe mit Administrationszugriff“ ein** das Sie mit einer Layout-Vorlage verknüpfen können.

Der Benutzer, der in dieser Gruppe als Gruppenadministrator festgelegt wurde, hat Zugriff zum Verwalten dieser Layout-Vorlage und zum Erstellen neuer Layout-Vorlagen, wobei die von ihm verwalteten Gruppen die administrativen Gruppen der Vorlagen sind. 

Vor dieser Änderung konnte nur der Workfront-Administrator Layoutvorlagen erstellen.

Weitere Informationen zum Erstellen von Layout-Vorlagen finden Sie unter „Erstellen und Verwalten von Layout-Vorlagen“.

## Systemweite Breitbildanzeige {#system-wide-widescreen-display}

Wenn Sie eine Seite in Workfront anzeigen, wird jetzt das gesamte Browserfenster automatisch ausgefüllt und an Ihre Bildschirmgröße angepasst.

Vor dieser Änderung wurden nur die mit den folgenden Objekten verknüpften Seiten im Breitbild angezeigt:

* Projekte
* Aufgaben
* Probleme
* Berichte
* Dashboards
* Kalender

## Größe der Zeitleisten-Momentaufnahme im Gantt-Diagramm ändern {#resize-timeline-snapshot-on-the-gantt-chart}

Sie können jetzt den Zeitleisten-Schnappschuss erweitern, um das gesamte Projekt im Gantt-Diagramm anzuzeigen.

Vor dieser Verbesserung konnten Sie einen bestimmten Punkt auf der Zeitleisten-Momentaufnahme auswählen, um im Gantt-Diagramm zu ihr zu navigieren.

Weitere Informationen zum Konfigurieren der Anzeige von Informationen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Interaktiver Ressourcenplaner im Business Case {#interactive-resource-planner-in-the-business-case}

Als Ressourcen-Manager können Sie jetzt Ressourcenpools im Abschnitt Ressourcenbudgetierung des Business Case hinzufügen. Sie können Ihre Projektressourcen auch mit dem Ressourcenplaner auf Projektebene budgetieren. Wenn Sie Ihre Ressourcen für ein Projekt budgetieren, werden die budgetierten Lohnkosten des Projekts generiert.

Vor dieser Änderung konnten Sie Informationen zur Ressourcenbudgetierung im Business Case anzeigen, wenn das Projekt für Ressourcen im globalen Ressourcenplaner budgetiert worden war.

Weitere Informationen zum Abschließen der Budgetierung von Projektressourcen im Business Case finden Sie [Budgetressourcen im Business Case](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

## Visualisierung im Ressourcenplaner - Benutzerzuordnungsdiagramm {#visualization-in-the-resource-planner-user-allocation-chart}

Sie können jetzt die geplante Gesamtzuweisung aller Benutzer im Vergleich zu ihrer Verfügbarkeit in einem Diagramm im Ressourcenplaner anzeigen. Das Diagramm ist verfügbar, wenn Sie **Nach Benutzer anzeigen** im Ressourcenplaner auswählen.

Das Diagramm enthält die folgenden Informationen:

* Verfügbarkeit (%) ohne Überallokation für alle Benutzenden
* Überallokation (%) für alle Benutzenden
* Nichtauslastung (%) für alle Benutzenden
* In diesem Zeitraum gibt es eine Überallokation für mindestens einen Benutzer/eine Benutzerin

Vor dieser Änderung konnten Sie die Zuordnung und Verfügbarkeit einzelner Benutzer nur im Tabellenformat anzeigen.

Weitere Informationen zum Benutzerzuordnungsdiagramm im Ressourcenplaner finden Sie unter [Ressourcenplaner - Übersicht](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Verbesserungen im Bereich Home {#improvements-in-the-home-area}

Im Bereich Startseite stehen jetzt verschiedene Verbesserungen zur Verfügung, darunter:

* Verbesserungen beim Erscheinungsbild

   * Das rechte Bedienfeld ist nun größer, sodass mehr Platz für Aufgaben- und Probleminformationen zur Verfügung steht.
   * Überfällige Elemente werden jetzt in einem helleren Rottöner angezeigt, wenn sie im linken Bedienfeld ausgewählt werden.
   * Sie können jetzt die Beziehung zwischen dem linken Bedienfeld und dem rechten Bedienfeld leichter erkennen. Das ausgewählte Dokument im linken Bereich zeigt auf den rechten Bereich.

* Für ausgewählte Elemente werden Standardfelder angezeigt. 

  Weitere Informationen zu den Standardfeldern finden Sie unter „Erstellen und Verwalten von Layout-Vorlagen“.

* Nachdem Sie bei einer Anfrage auf „Bearbeiten“ geklickt haben, werden die mit dem Problem verknüpften Felder im rechten Bereich angezeigt.

  Weitere Informationen zur Bearbeitung von Anfragen aus dem Bereich „Startseite“ finden Sie unter [Arbeiten und Teamanfragen im Bereich „Startseite](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md) unter [Arbeiten und Teamanfragen im Bereich „Startseite“](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md).

* Zeigen Sie auf einen Benutzeravatar in einem Arbeitselement im linken Bereich, um den Namen des Benutzers anzuzeigen.
* Erweitern Sie den Bereich „Verspätet“ im linken Bereich, um alle verspäteten Elemente anzuzeigen (wenn dieser Bereich reduziert ist, werden nur die ersten 5 Elemente angezeigt).
* Nachdem Sie ein Element als abgeschlossen markiert haben, bleibt das Element im linken Bedienfeld, bis Sie ein anderes Element auswählen.\
  Informationen zum Anzeigen abgeschlossener Elemente finden Sie unter [Elemente in der Arbeitsliste im ](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) anzeigen) unter [Elemente in der Arbeitsliste im ](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) anzeigen.

Weitere Informationen zur Verwendung des neuen Bereichs „Startseite“ sowie Informationen zu Funktionsunterschieden zwischen „Meine Arbeit“ und „Startseite“ [ Sie unter „Verwenden des Bereichs „Startseite](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

## Neue Verbesserungen bei der Korrekturabzugsansicht  {#new-proofing-viewer-improvements}

* [Verbessertes Layout und Design](#improved-layout-and-design)
* [Kommentare nach Kommentarnummer suchen](#search-comments-by-comment-number)
* [Option zum Bearbeiten des Kommentars neben der Markup-Anzeige](#option-to-edit-comment-next-to-the-markup-indicator)
* [Markieren Sie alle Kommentare als gelesen](#mark-all-comments-as-read)
* [Verbesserungen am linken Menü](#left-menu-improvements)

### Verbessertes Layout und Design {#improved-layout-and-design}

Die Korrekturabzugsansicht hat ein aktualisiertes Erscheinungsbild. Die  Die folgenden Bereiche der Korrekturabzugsansicht wurden aktualisiert:

* Bereich „Miniaturen“

  Weitere Informationen zur Verwendung des Bereichs „Miniaturen“ finden Sie unter in .

* Kommentarbereich\
  Weitere Informationen zum Kommentarbereich finden Sie unter .
* Linker Menübereich

### Kommentare nach Kommentarnummer suchen {#search-comments-by-comment-number}

Wenn Sie jetzt die Kommentarliste im Proofing Viewer durchsuchen, können Sie die Nummer des Kommentars in das Suchfeld eingeben. Die Kommentarliste wird dann gefiltert, um den gesuchten Kommentar anzuzeigen. 

Weitere Informationen finden Sie unter in .

### Option zum Bearbeiten des Kommentars neben der Markup-Anzeige {#option-to-edit-comment-next-to-the-markup-indicator}

Sie können jetzt einen vorhandenen Kommentar einfacher bearbeiten. Nachdem Sie auf eine Kommentaranzeige auf dem Korrekturabzug geklickt haben, wird neben der Sprechblase ein Bearbeitungssymbol angezeigt. 

Vor dieser Änderung mussten Sie auf das Symbol „Bearbeiten“ im Kommentarbereich klicken.  

Weitere Informationen finden Sie unter .

### Alle Kommentare als gelesen markieren {#mark-all-comments-as-read}

Beim Anzeigen eines Dokuments in der Korrekturabzugsansicht können Sie jetzt alle Kommentare als gelesen markieren.

### Verbesserungen am linken Menü {#left-menu-improvements}

Das Menü auf der linken Seite der Korrekturabzugsansicht enthält die folgenden Verbesserungen:

* Aktualisiertes Erscheinungsbild
* Symbol am oberen Rand des Menüs, um das Menü ein- oder auszublenden

  ![PROOF_VIEWER_MENU_HIDE.png](assets/proof-viewer-menu-hide.png)

* Bewegen Sie den Mauszeiger über das Menü, um das Menü automatisch zu erweitern und neben Symbolen auch Beschriftungen anzuzeigen. (Oder aktivieren Sie die Option, um das Menü immer in der reduzierten Ansicht zu halten.)
