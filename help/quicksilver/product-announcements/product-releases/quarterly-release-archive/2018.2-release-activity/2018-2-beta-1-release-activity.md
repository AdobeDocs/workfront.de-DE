---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 1 2018.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 1 Version 2018.2 verfügbar waren. Die Funktion wurde am 22. März 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juni 2018 in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# Versionsaktivität von Beta 1 2018.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 1 Version 2018.2 verfügbar waren. Die Funktion wurde am 22. März 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juni 2018 in der Produktionsumgebung bereitgestellt.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller in 2018.2 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die Beta 1-Version 2018.2 enthält die folgenden Verbesserungen:

* [Ändern von Aufgabendaten im Gantt-Diagramm](#modify-task-dates-in-the-gantt-chart)
* [Rufen Sie das Projekt-Gantt-Diagramm über die Registerkarte Aktualisierungen ](#access-the-project-gantt-chart-from-the-updates-tab)vorübergehend entfernt)

* [Verschiedene Links wurden wieder zu Dokumenten in der Dokumentliste hinzugefügt](#various-links-re-introduced-to-documents-on-the-document-list)
* [Verbesserungen an der Benutzeransicht im Ressourcenplaner](#user-view-improvements-in-the-resource-planner)
* [Neues Projektlistenerlebnis](#new-project-list-experience)
* [Registerkarte „Neue Suche nach Aktualisierungen“](#new-look-for-updates-tab)
* [Verbesserungen für Mobilgeräte](#mobile-improvements)

## Aufgabendaten im Gantt-Diagramm ändern {#modify-task-dates-in-the-gantt-chart}

Sie können jetzt die Aufgabenblase ziehen, um die geplanten Start- und Abschlussdaten im Gantt-Diagramm zu ändern. Mit dieser Änderung können Sie Was-wäre-wenn-Szenarien auf Ihr Projekt anwenden, ohne die Timeline zu beeinflussen.

Vor dieser Änderung konnten Sie Aufgabentermine nur in der Aufgabenliste oder auf Aufgabenebene ändern.

Weitere Informationen finden Sie [Informationen aktualisieren in der Aufgabenliste Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Greifen Sie über die Registerkarte Aktualisierungen auf das Projekt-Gantt-Diagramm zu {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Diese Funktion wurde vorübergehend aus der Vorschau-Umgebung entfernt.

Sie können jetzt auf das neue Projekt-Gantt-Diagramm über die Registerkarte Aktualisierungen zugreifen. Wenn ein(e) Benutzende(r) das Commit-Datum einer Aufgabe so ändert, dass es sich auf die Projekt-Zeitleiste auswirkt, können Sie die Auswirkungen im Projekt-Gantt-Diagramm einsehen.

Vor dieser Änderung wurde über den Link Projektzeitleiste das alte Gantt-Diagramm geöffnet.

Weitere Informationen finden Sie unter [Übersicht über das Übertragungsdatum](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Weitere Informationen finden Sie unter Übersicht über den [Portfolio-Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Verschiedene Links wurden wieder zu Dokumenten in der Dokumentliste eingeführt {#various-links-re-introduced-to-documents-on-the-document-list}

In Version 18.1 wurden verschiedene Links aus Dokumenten in der Dokumentliste entfernt und in andere Bereiche der Benutzeroberfläche verschoben (einige als Schaltfläche neben dem Dokumentnamen und einige in einem Dropdown-Menü auf der Schaltfläche). Mit dieser Version werden die folgenden Links unterhalb des Dokumentnamens wieder eingeführt und sind jetzt für einzelne Dokumente in der Dokumentliste verfügbar:

* Korrekturabzug erstellen (verfügbar, wenn noch kein Korrekturabzug generiert wurde)
* Korrekturabzug öffnen (verfügbar, wenn ein Korrekturabzug erstellt wird)
* Dokumentdetails (verfügbar, wenn noch kein Korrekturabzug generiert wurde)
* Korrekturabzugsdetails (verfügbar, wenn ein Korrekturabzug erstellt wird)
* Zusammenfassung drucken

Die folgenden Aktionen werden nicht wieder als Links für das Dokument innerhalb der Dokumentliste eingeführt:

* Freigeben (weiterhin als Schaltfläche im Menü verfügbar)
* Auschecken/Einchecken (noch verfügbar im Dropdown-Menü Mehr im Menü)

Weitere Informationen finden Sie in den folgenden Abschnitten:

*  in 

## Verbesserungen bei der Benutzeransicht im Ressourcenplaner {#user-view-improvements-in-the-resource-planner}

Die Benutzeransicht des Ressourcenplaners enthält jetzt die folgenden Verbesserungen:

* Die Benutzeransicht ist jetzt die Standardansicht und ersetzt die Projektansicht.
* Verbesserte Filter, die Informationen aus der gesamten Datenbank abrufen, anstatt nur die Informationen auf dem Bildschirm.
* Vollbildmodus.
* Die Leistung ist jetzt schneller und effizienter.

   * Neue Beschränkungen für die Anzahl der Benutzer, Projekte, Rollen und Aufgaben, die Sie anzeigen können.
   * Lazy Loading (verzögertes Laden), für schnelleres Laden von Benutzern.

Die folgende Funktion wurde im Ressourcenplaner vorübergehend deaktiviert:

* Exportieren der Daten aus dem Ressourcenplaner bei Verwendung der Benutzeransicht.

Im Vorfeld dieser Verbesserungen haben Sie berichtet, dass der Ressourcenplaner nur langsam geladen wurde und dass bei den angezeigten Daten Abweichungen festgestellt wurden. Mit diesen Verbesserungen sollten diese nun beseitigt werden.

Weitere Informationen zu den Bereichen des Ressourcenplaners finden Sie unter [Übersicht über die Ressourcenplaner-Navigation](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Neues Projektlistenerlebnis {#new-project-list-experience}

Beim Anzeigen einer Liste von Projekten ist jetzt ein neues Erlebnis verfügbar. Zu diesem Erlebnis gehören eine höhere Leistung sowie eine reibungslosere und schnellere Navigation in Listen. Nur die Listen auf der Registerkarte „Projekte“ im Bereich „Projekte“ von Workfront wurden auf diese neue Version aktualisiert.

Die meisten Änderungen betreffen die Schnelligkeit und Effizienz der Liste. Darüber hinaus wurden die folgenden sichtbaren Änderungen eingeführt:

* In der Liste werden standardmäßig bis zu 2.000 Elemente angezeigt.

  Vor dieser Verbesserung wurden in der Liste 100 Elemente angezeigt.

* Gruppierungen sind standardmäßig reduziert.

  Vor dieser Änderung wurden Gruppierungen standardmäßig erweitert.

* Der Bereich für die Auswahl einer Zeile wurde auf die gesamte Zeile erweitert.

Die folgenden Funktionen wurden in den angegebenen Projektlisten vorübergehend deaktiviert:

* Spaltenanpassung (Diese Funktion wurde mit der Beta 5-Version 2018.2 wieder eingeführt)
* Neuanordnung der Spalten
* Die Felder des Statussymbols werden leer angezeigt (diese Funktion wurde mit der Beta-Version 5 von 2018.2 wieder eingeführt)
* Auf das Gantt-Diagramm kann nicht zugegriffen werden (Diese Funktion wurde mit der Beta-Version 3 von 2018.2 wieder eingeführt).

Weitere Informationen zum Arbeiten in Listen finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Registerkarte „Neues Suchen nach Aktualisierungen“ {#new-look-for-updates-tab}

>[!NOTE]
>
>Bei einigen Benutzern wird die Registerkarte Neue Aktualisierungen möglicherweise nicht in der Vorschau-Umgebung angezeigt. Unser Entwicklungs-Team ist derzeit dabei, das Problem zu beheben, und arbeitet daran, das Problem so schnell wie möglich zu beheben.

Das Erscheinungsbild der Registerkarte Aktualisierungen wurde geändert, um es besser an andere Bereiche der Benutzeroberfläche anzupassen. Diese Änderung gilt für Projekte, Aufgaben, Probleme und Dokumente.

In der folgenden Tabelle sind die Aktualisierungen der Registerkarte Aktualisierungen aufgeführt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <p><strong>Vorherige Benutzeraktion</strong> </p> </th> 
   <th> <p><strong>Neue Benutzeraktion</strong> </p> </th> 
   <th> <p><strong>Weitere Informationen finden Sie unter…</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Zeit in einer Arbeitszeittabelle protokollieren</p> </td> 
   <td> <p>Klicken Sie auf den Link Zeit protokollieren .</p> </td> 
   <td> <p>Klicken Sie auf die Schaltfläche Zeit protokollieren .</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Erfassen der Zeit</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Herausfiltern von Systemaktualisierungen auf der Registerkarte „Aktualisierungen“</p> </td> 
   <td> <p>Klicken Sie auf den Link Systemaktualisierungen filtern .</p> </td> 
   <td> <p>Deaktivieren Sie den Umschalter Aktivitätsprotokoll anzeigen .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Arbeit aktualisieren</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anzeigen von Systemaktualisierungen auf der Registerkarte „Aktualisierungen“</p> </td> 
   <td> <p>Klicken Sie auf Alle Updates anzeigen</p> </td> 
   <td> <p>Aktivieren Sie den Umschalter Aktivitätsprotokoll anzeigen .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Arbeit aktualisieren</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tagging anderer Benutzer bei einer Aktualisierung oder einem Kommentar</p> </td> 
   <td> <p>Klicken Sie auf das Symbol Andere in dieses Update einbeziehen .</p> </td> 
   <td> <p>Hinzufügen von Benutzern und Teams im Feld Benachrichtigen</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Arbeit aktualisieren</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anzeige eines Objekts nur durch Benutzer in Ihrer Firma zulassen</p> </td> 
   <td> <p>Klicken Sie auf das Schlosssymbol</p> </td> 
   <td> <p>Aktivieren des Umschalters Privat für „Meine Firma“</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Andere bei Aktualisierungen taggen</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzern außerhalb Ihres Unternehmens erlauben, ein Objekt anzuzeigen</p> </td> 
   <td> <p>Klicken Sie auf das Schlosssymbol</p> </td> 
   <td> <p>Deaktivieren Sie den Umschalter Privat für meine Firma .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Andere bei Aktualisierungen taggen</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hinzufügen einer Antwort oder Aktualisierung zu einem Kommentar oder einer Aktualisierung</p> </td> 
   <td> <p>Klicken Sie auf die Schaltfläche Kommentar .</p> </td> 
   <td> <p>Klicken Sie auf die Schaltfläche Antworten oder Aktualisieren</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Arbeit aktualisieren</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aufgabenstatus aktualisieren</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aktualisierungsbedingung für Aufgaben und Probleme</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Ein Update zu einem Dokument hinzufügen</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Verbesserungen für Mobilgeräte {#mobile-improvements}

Die Mobile App enthält die folgenden Verbesserungen:

* Links, die in anderen Mobile Apps für Sie freigegeben sind, werden jetzt in der Mobile App von Workfront geöffnet.

  Weitere Informationen zur Freigabe von Links finden Sie unter .

  Dieses Update wird manchmal diese Woche für iOS veröffentlicht, und das Android-Update sollte kurz danach folgen.

* Wir haben unsere Support-Anforderungen für die iOS-Plattform aktualisiert, um iPhone X zu unterstützen.

  Weitere Informationen zu unterstützten Mobilgeräten und Betriebssystemen finden Sie unter .
