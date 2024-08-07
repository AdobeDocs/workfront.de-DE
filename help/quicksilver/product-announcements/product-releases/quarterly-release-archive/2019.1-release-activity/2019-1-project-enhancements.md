---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 Projektverbesserungen
description: Auf dieser Seite werden alle in Version 2019.1 enthaltenen Projektverbesserungen beschrieben. Die Funktion ist derzeit in der Vorschauumgebung verfügbar. Sie wird in der Produktionsumgebung im bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%

---

# 2019.1 Projektverbesserungen

Auf dieser Seite werden alle in Version 2019.1 enthaltenen Projektverbesserungen beschrieben. Die Funktion ist derzeit in der Vorschauumgebung verfügbar. Sie wird in der Produktionsumgebung im bereitgestellt.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die in Version 2019.1 vorgenommen wurden, finden Sie unter &quot;Übersicht über die Veröffentlichungsaktivität 2019.1&quot;.

**Für Administratoren**

* [Wiederherstellen von Vorlagen aus dem Papierkorb](#restore-templates-from-the-recycle-bin)
* [Zeitstempel für Datumsfelder in Startseite anzeigen](#show-timestamps-for-date-fields-in-home)
* [Alle unter den Projekteigenschaften verfügbaren Durationstypen](#all-duration-types-available-under-project-preferences)

**Für alle Benutzer**

* [Agile Verbesserungen](#agile-improvements)
* [Aufgaben und Probleme aus einer Liste zu einer Iteration hinzufügen](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [Neue Papiergrößen für den Export von Gantt-Diagrammen](#new-paper-sizes-for-gantt-chart-export)
* [Entfernen des Zugriffs auf Dialogfelder im Gantt-Diagramm im Bearbeitungsmodus](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [Anzeigen von Aufgabeninformationen im Gantt-Diagramm für Projektlisten in einem Programm oder Portfolio](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [Zugriff auf das Gantt-Diagramm für Aufgabenlisten auf Vorlagen](#access-the-task-list-gantt-chart-on-templates)
* [Die Projektansicht im Gantt-Diagramm wurde umbenannt](#renamed-the-project-view-on-the-gantt-chart)
* [Was-Wenn-Szenarios im Aufgabenlisten-Gantt-Diagramm](#what-if-scenarios-in-the-task-list-gantt-chart)
* [Verbesserungen der Aufgabenliste](#task-list-improvements)
* [Listen im Vollbildmodus anzeigen](#display-lists-in-full-screen)
* [Neue Listen in zusätzlichen Bereichen](#new-lists-in-additional-areas)
* [Versenden eines gelieferten Berichts im XLSX-Format](#send-a-delivered-report-in-xlsx-format)
* [Audit-Protokolle exportieren](#export-audit-logs)

## Wiederherstellen von Vorlagen aus dem Papierkorb {#restore-templates-from-the-recycle-bin}

Workfront-Administratoren können jetzt Vorlagen aus dem Papierkorb wiederherstellen. Wie bei anderen gelöschten Elementen können Sie eine Vorlage bis zu 30 Tage nach dem Zeitpunkt des Löschens wiederherstellen.

Weitere Informationen finden Sie unter &quot;Wiederherstellen gelöschter Elemente&quot;.

## Anzeigen von Zeitstempeln für Datumsfelder auf der Startseite {#show-timestamps-for-date-fields-in-home}

Als Workfront-Administrator können Sie jetzt mithilfe von Layoutvorlagen festlegen, ob Zeitstempel für Fälligkeitsdaten in der Arbeitsliste und im Kalender angezeigt oder ausgeblendet werden sollen. Standardmäßig sind Zeitstempel sowohl für Vorlagen- als auch für Nicht-Vorlagenbenutzer sichtbar.

Weitere Informationen finden Sie unter &quot;Anpassen des Startbereichs&quot;im Artikel &quot;Erstellen und Verwalten von Layoutvorlagen&quot;.

## Alle unter den Projekteigenschaften verfügbaren Durationstypen {#all-duration-types-available-under-project-preferences}

Beim Festlegen des Standardtyps für Aufgaben und Problemlaufzeit unter Einrichtung > Projekteinstellungen können Sie eine der folgenden Optionen verwenden:

Einfach

Leistungsgesteuert

Berechnete Zuweisung

Berechnete Arbeit

Wenn Sie zuvor entweder &quot;Einfach&quot;oder &quot;Aufwandsgesteuert&quot;als Standarddauer festgelegt haben, konnten Sie weder &quot;Berechnete Zuweisung&quot;noch &quot;Berechnete Arbeit&quot;auswählen.

Weitere Informationen zum Festlegen der Standardeinstellungen für Aufgaben und Ausgabedauer finden Sie unter &quot;Voreinstellungen für Aufgaben und Probleme&quot;

## Agile Verbesserungen {#agile-improvements}

Die folgenden Verbesserungen sind jetzt im Agile-Tool verfügbar:

Kanban

Fügen Sie Aufgaben und Probleme einem Kanban-Board aus einer beliebigen Aufgabenliste oder einem beliebigen Bericht hinzu.

Zuvor konnten Sie nur aus dem Rückstand Aufgaben zum Kanban-Board hinzufügen. Es konnten keine Probleme hinzugefügt werden.

Filtern Sie die Kanban-Pinnwand nach einzelnen Benutzern im Team.

Weitere Informationen finden Sie unter &quot;Verwenden des Kanban-Board&quot;.

Anzeigen und Verwalten von Problemen im Kanban-Backlog.

Weitere Informationen finden Sie unter &quot;Verwenden des Kanban Board&quot;.

Zuvor war es nicht möglich, Probleme auf einem Kanban-Board hinzuzufügen oder zu verwalten.

Scrum

Filtern Sie das Traumboard nach einzelnen Benutzern im Team.

Weitere Informationen finden Sie unter &quot;Verwenden des Scrum Agile Story Board&quot;.

Zuvor war es nicht möglich, nach Benutzern auf Kanban- oder Trommelboards zu filtern.

## Hinzufügen von Aufgaben und Problemen aus einer Liste zu einer Iteration {#add-tasks-and-issues-from-a-list-to-an-iteration}

Sie können jetzt eine Aufgaben- oder Problemliste, einen Bericht oder ein Dashboard verwenden, um einer Iteration Meldungen hinzuzufügen. Sie können auch mehrere Teams in einer Iteration Geschichten zuweisen lassen.

Zuvor konnten Sie einer Iteration nur auf der Seite mit den Aufgaben- oder Problemdetailseiten eine Geschichte hinzufügen und Sie konnten Geschichten nur zu Iterationen hinzufügen, die von Ihrem Team erstellt wurden.

Weitere Informationen finden Sie unter &quot;Erstellen und Verwalten von Agile Iterationen&quot;.

## Versand eines zugestellten Berichts im XLSX-Format {#send-a-delivered-report-in-xlsx-format}

Jetzt können Sie die Bereitstellung eines Berichts im MS Excel-Format (.xlsx) planen, zusätzlich zu allen anderen aktuellen Formaten.

Zuvor konnten Sie einen Bericht nur in den folgenden Formaten bereitstellen:

HTML

PDF

MS Excel (.xls)

TSV

Informationen zur Planung von Berichten für die Bereitstellung finden Sie unter &quot;Einrichten von Berichtbereitstellungen&quot;.

## Verbesserungen der Aufgabenliste {#task-list-improvements}

[Aktualisieren Sie 18.3 Beta 4, wobei dies aus ] entfernt wurde.

Die neu entworfenen Aufgabenlisten wurden nach einer kurzen Entfernung während der Beta-Version 18.3 von neu aktiviert. Wir haben außerdem die folgenden zusätzlichen Funktionen zu den Aufgabenlisten hinzugefügt, die nicht Teil der ursprünglichen Version waren:

Ersetzen des Kontextmenüs durch ein Mehr -Symbol beim Inline-Bearbeiten einer Aufgabe.

Die Optionen, die beim Inline-Bearbeiten mehrerer Aufgaben im Kontextmenü verfügbar waren, wurden jetzt in die Symbole oben in der Aufgabenliste verschoben.

Standardmäßig werden in Aufgabenlisten 2000 Aufgaben angezeigt.

Wenn Workfront die Zeitpläne neu berechnet, wurden die Fragezeichen neben den Aufgaben, deren Daten aktualisiert werden, durch graue Bereiche ersetzt.

Weitere Informationen zum Inline-Bearbeiten von Aufgaben finden Sie unter &quot;Kopieren und Duplizieren von Aufgaben&quot;und unter &quot;Erstellen von Vorgängerbeziehungen durch Verketten von Aufgaben&quot;.

Weitere Informationen zur Neuberechnung von Projektzeitplänen finden Sie unter &quot;Neuberechnung von Zeitplänen für Projekte&quot;.

## Anzeigen von Listen im Vollbildmodus {#display-lists-in-full-screen}

Wenn eine Liste von Projekten oder Aufgaben größer ist als die Größe Ihres Bildschirms, wird die Liste beim Bildlauf automatisch im gesamten Browserfenster angezeigt. Dadurch erhöht sich die Anzahl an Informationen, die Sie gleichzeitig sehen, und Sie können Listen einfacher verwalten.

Sie können die folgenden Listen im Vollbildmodus anzeigen:

Eine Liste der Projekte in den folgenden Registerkarten und Unterregisterkarten:

Projekte, an denen ich mitwirke

Projekte in meinem Besitz

Alle Projekte

Registerkarte &quot;Projekte&quot;in einem Portfolio

Registerkarte &quot;Projekte&quot;im Programm

Eine Liste der Aufgaben in den folgenden Registerkarten:

Registerkarte &quot;Aufgaben&quot;in einem Projekt

Registerkarte &quot;Unteraufgaben&quot;in einer Aufgabe

Informationen zum Anzeigen von Objekten in Listen finden Sie unter &quot;Anzeigen von Elementen in einer Liste&quot;.

## Neue Listen in zusätzlichen Bereichen {#new-lists-in-additional-areas}

Wir haben die Leistung verbessert und das Erscheinungsbild des Projekts und der Aufgabenlisten in den folgenden Bereichen verbessert:

Registerkarte &quot;Portfolios und Programme&quot;im Bereich &quot;Projekte&quot;

Registerkarte &quot;Unteraufgaben&quot;auf Aufgabenebene

Vor dieser Verbesserung waren die neuen Listen nur in den folgenden Bereichen verfügbar:

Registerkarte &quot;Projekte&quot;im Projektbereich

Registerkarte &quot;Aufgaben&quot;auf Projektebene

Informationen zum Anzeigen von Objekten in Listen finden Sie unter &quot;Anzeigen von Elementen in einer Liste&quot;.

## Anzeigen von Aufgabeninformationen im Gantt-Diagramm für die Projektliste in einem Programm oder Portfolio {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

Sie können jetzt Informationen zu den Aufgaben eines Projekts im Gantt-Diagramm für die Projektliste in einem Programm oder Portfolio anzeigen.

Zuvor konnten Sie Informationen zu Aufgaben nur im Gantt-Diagramm für die Projektliste auf der Registerkarte Projekte anzeigen.

Weitere Informationen finden Sie unter &quot;Anzeigen von Informationen im Gantt-Diagramm&quot;.

## Was-wenn-Szenarios im Gantt-Diagramm für Aufgabenliste {#what-if-scenarios-in-the-task-list-gantt-chart}

Sie können jetzt die folgenden Aktionen für die Aufgaben in einem Projekt ausführen, wenn sie im Bearbeitungsmodus des Gantt-Diagramms angezeigt werden:

 Aufgaben hinzufügen

Aufgaben entfernen

Inline-Bearbeitungsaufgaben

Aufgaben duplizieren

Aufgaben neu anordnen

Unteraufgaben ändern

Sie können zwar sehen, wie sich Ihre Änderungen auf die Timeline des Projekts auswirken, sie werden jedoch nicht sofort gespeichert. Sie können sie speichern, um die Projekt-Timeline dauerhaft zu aktualisieren, oder Sie können sie abbrechen.

Zuvor war es nicht möglich, eine Vorschau der Aufgabenlistenänderungen im Gantt-Diagramm anzuzeigen.

Informationen zu Bearbeitungsaufgaben im Gantt-Diagramm finden Sie unter &quot;Aktualisieren von Informationen im Gantt-Diagramm für Aufgabenlisten&quot;.

## Gantt-Diagramm für Aufgabenlisten in Vorlagen aufrufen {#access-the-task-list-gantt-chart-on-templates}

Sie können jetzt auf das Gantt-Diagramm für Aufgabenlisten in einer Projektvorlage zugreifen.

Zuvor war es nicht möglich, das Gantt-Diagramm in der Aufgabenliste in einer Vorlage anzuzeigen.

Weitere Informationen finden Sie unter &quot;Erste Schritte mit dem Gantt-Diagramm&quot;.

## Neue Papiergrößen für den Export von Gantt-Diagrammen {#new-paper-sizes-for-gantt-chart-export}

Jetzt können Sie die Gantt-Grafik in Papiergrößen A1 und A2 drucken.

Zuvor konnten Sie nur nach Brief, Legal, Ledger, A3 (nur für einige Sprachen verfügbar) und A4 exportieren.

Weitere Informationen finden Sie unter &quot;Exportieren des Gantt-Diagramms zu PDF&quot;.

## Die Projektansicht im Gantt-Diagramm wurde umbenannt. {#renamed-the-project-view-on-the-gantt-chart}

Wir haben die Option &quot;Projekt&quot;-Ansicht im Gantt-Diagramm in &quot;Alle anpassen&quot;umbenannt. Die Ansichtsoption funktioniert weiterhin wie zuvor. Der neue Name soll beschreibender darüber sein, was Sie bei Auswahl der Option anzeigen.

Weitere Informationen finden Sie unter &quot;Anzeigen von Informationen im Gantt-Diagramm&quot;.

## Der Zugriff auf Dialogfelder im Gantt-Diagramm während des Bearbeitungsmodus wurde entfernt. {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

Sie können nicht mehr auf das Dialogfeld Erweiterte Zuweisungen zugreifen, während sich das Gantt-Diagramm im Bearbeitungsmodus befindet. Sie können nur Inline-Änderungen vornehmen, während sich das Gantt-Diagramm für die Aufgabenliste im Bearbeitungsmodus befindet.

Zuvor konnten Sie auf das Dialogfeld Erweiterte Zuweisungen zugreifen, während sich das Gantt-Diagramm im Bearbeitungsmodus befand, es jedoch die im Gantt-Diagramm vorgenommenen Änderungen speicherte und den Bearbeitungsmodus beendete.

Weitere Informationen zum Bearbeiten des Gantt-Diagramms &quot;Aufgabenliste&quot;finden Sie unter &quot;Aktualisieren von Informationen im Gantt-Diagramm für Aufgabenliste&quot;.

## Audit-Protokolle exportieren {#export-audit-logs}

Sie können nun Auditprotokolleinträge in eine CSV-Datei exportieren. Sie können bis zu 50.000 Auditprotokolleinträge gleichzeitig in eine CSV-Datei exportieren.

Weitere Informationen finden Sie unter &quot;Verwalten von Auditprotokollen&quot;.
