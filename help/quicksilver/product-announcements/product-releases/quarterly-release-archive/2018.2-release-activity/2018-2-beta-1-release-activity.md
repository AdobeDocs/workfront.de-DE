---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 1-Release-Aktivität von 2018.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 1-Version 2018.2 verfügbar waren. Die Funktion wurde am 22. März 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juni 2018 im Produktionsumfeld zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# Beta 1-Release-Aktivität von 2018.2

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit Beta 1-Version 2018.2 verfügbar waren. Die Funktion wurde am 22. März 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juni 2018 im Produktionsumfeld zur Verfügung gestellt.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die in Version 2018.2 vorgenommen wurden, finden Sie unter [Übersicht über die Release-Aktivität 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Beta 1-Version 2018.2 umfasst die folgenden Erweiterungen:

* [Ändern von Aufgabendaten im Gantt-Diagramm](#modify-task-dates-in-the-gantt-chart)
* [Greifen Sie auf das Projekt-Gantt-Diagramm über die Registerkarte &quot;Updates&quot;](#access-the-project-gantt-chart-from-the-updates-tab) zu (vorübergehend entfernt)

* [Verschiedene Links, die zu Dokumenten auf der Dokumentliste neu eingeführt wurden](#various-links-re-introduced-to-documents-on-the-document-list)
* [Verbesserungen der Benutzeransicht im Ressourcenplaner](#user-view-improvements-in-the-resource-planner)
* [Neues Projektelisten-Erlebnis](#new-project-list-experience)
* [Registerkarte &quot;Neue Suche nach Updates&quot;](#new-look-for-updates-tab)
* [Mobile Verbesserungen](#mobile-improvements)

## Ändern von Aufgabendaten im Gantt-Diagramm {#modify-task-dates-in-the-gantt-chart}

Sie können nun die Aufgabenblase ziehen, um die geplanten Start- und geplanten Abschlussdaten im Gantt-Diagramm zu ändern. Mit dieser Änderung können Sie Was-wäre-wenn-Szenarien auf Ihr Projekt anwenden, ohne die Timeline zu beeinträchtigen.

Vor dieser Änderung konnten Sie Aufgabendaten nur in der Aufgabenliste oder auf Aufgabenebene ändern.

Weitere Informationen finden Sie unter [Informationen in der Aufgabenliste aktualisieren Gantt Chart](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Gantt-Diagramm des Projekts über die Registerkarte Aktualisierungen aufrufen {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Diese Funktion wurde vorübergehend aus der Vorschau-Umgebung entfernt.

Sie können nun über den Tab Updates auf das neue Projekt-Gantt-Diagramm zugreifen. Wenn ein Benutzer das Datum des Versands einer Aufgabe so ändert, dass es sich auf die Projekt-Timeline auswirkt, können Sie die Auswirkungen im Projekt-Gantt-Diagramm anzeigen.

Vor dieser Änderung wurde über den Link Projekt-Timeline das Legacy-Gantt-Diagramm geöffnet.

Weitere Informationen finden Sie unter [Übersicht über das Veröffentlichungsdatum](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Weitere Informationen finden Sie unter [Übersicht über Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Verschiedene Links Neu zu Dokumenten auf der Dokumentliste {#various-links-re-introduced-to-documents-on-the-document-list}

In Version 18.1 wurden verschiedene Links aus Dokumenten auf der Dokumentliste entfernt und in andere Bereiche der Benutzeroberfläche verschoben (einige als Schaltfläche neben dem Dokumentnamen und andere in einem Dropdown-Menü auf der Schaltfläche). Die folgenden Links werden mit dieser Version unter dem Dokumentnamen wieder eingefügt und stehen jetzt in einzelnen Dokumenten in der Dokumentliste zur Verfügung:

* Testversand generieren (verfügbar, wenn noch kein Testversand erstellt wurde)
* Offener Testversand (verfügbar bei der Erstellung eines Testversands)
* Dokumentdetails (verfügbar, wenn noch kein Testversand erstellt wurde)
* Testversanddetails (verfügbar bei der Erstellung eines Testversands)
* Zusammenfassung drucken

Die folgenden Aktionen werden nicht erneut als Links auf das Dokument in der Dokumentliste eingefügt:

* Freigabe (weiterhin als Schaltfläche im Menü verfügbar)
* Auschecken/Einchecken (weiterhin im Dropdownmenü Mehr im Menü verfügbar)

Weitere Informationen finden Sie in den folgenden Abschnitten:

*  
*  in 

## Verbesserungen der Benutzeransicht im Ressourcenplaner {#user-view-improvements-in-the-resource-planner}

Die Benutzeransicht des Ressourcen-Planers enthält jetzt die folgenden Verbesserungen:

* Die Benutzeransicht ist jetzt die Standardansicht und ersetzt die Projektansicht.
* Verbesserte Filter, die Informationen aus der gesamten Datenbank abrufen und nicht nur Informationen auf dem Bildschirm.
* Vollbildmodus.
* Die Leistung ist jetzt schneller und effizienter.

   * Neue Beschränkungen für die Anzahl der Benutzer, Projekte, Rollen und Aufgaben, die angezeigt werden können.
   * Lazy Loading, für schnelleres Laden der Benutzer.

Die folgende Funktion wurde im Ressourcen-Planer vorübergehend deaktiviert:

* Exportieren der Daten aus dem Ressourcenplaner bei Verwendung der Benutzeransicht.

Vor diesen Verbesserungen haben Sie berichtet, dass der Ressourcen-Planer langsam geladen wurde und dass Sie Unstimmigkeiten in den angezeigten Daten bemerkt haben. Mit diesen Verbesserungen sollten diese nun beseitigt werden.

Weitere Informationen zu den Bereichen des Ressourcen-Planers finden Sie unter [Navigationsübersicht für den Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Neues Projekt-Listenerlebnis {#new-project-list-experience}

Beim Anzeigen einer Projektliste ist jetzt ein neues Erlebnis verfügbar. Dieses Erlebnis beinhaltet eine höhere Leistung sowie eine reibungslosere und schnellere Listennavigation. Nur die Listen auf der Registerkarte &quot;Projekte&quot;im Bereich &quot;Projekte&quot;von Workfront wurden auf dieses neue Erlebnis aktualisiert.

Die meisten Änderungen betreffen die Geschwindigkeit und Effizienz der Liste. Außerdem wurden die folgenden sichtbaren Änderungen eingeführt:

* Die Liste zeigt standardmäßig bis zu 2.000 Elemente an.

  Vor dieser Verbesserung wurden in der Liste 100 Elemente angezeigt.

* Gruppierungen werden standardmäßig ausgeblendet.

  Vor dieser Änderung wurden die Gruppierungen standardmäßig erweitert.

* Der Bereich für die Auswahl einer Zeile wurde auf die gesamte Zeile erweitert.

Die folgenden Funktionen wurden in den angegebenen Projektlisten vorübergehend deaktiviert:

* Größenanpassung der Spalten (Diese Funktion wurde in Version 2018.2 von Beta 5 neu eingeführt)
* Neuanordnen von Spalten
* Felder mit Statussymbolen werden als leer angezeigt (diese Funktion wurde in Beta 5-Version 2018.2 erneut eingeführt)
* Auf das Gantt-Diagramm kann nicht zugegriffen werden (diese Funktion wurde in Beta 3-Version 2018.2 neu eingeführt).

Weitere Informationen zum Arbeiten in Listen finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Neue Registerkarte &quot;Suchen nach Updates&quot; {#new-look-for-updates-tab}

>[!NOTE]
>
>Für einige Benutzer wird die neue Registerkarte Updates möglicherweise nicht in der Umgebung &quot;Vorschau&quot;angezeigt. Unser Entwicklungsteam behebt derzeit das Problem und arbeitet daran, das Problem so schnell wie möglich zu lösen.

Das Erscheinungsbild der Registerkarte &quot;Updates&quot;wurde geändert, um besser an andere Bereiche der Benutzeroberfläche anzupassen. Diese Änderung gilt für Projekte, Aufgaben, Probleme und Dokumente.

Die folgende Tabelle zeigt die Aktualisierungen, die am Tab Updates vorgenommen wurden:

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
   <th> <p><strong>Weitere Informationen finden Sie unter..</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Protokollierungszeit auf einem Timesheet</p> </td> 
   <td> <p>Klicken Sie auf den Link Protokollzeit .</p> </td> 
   <td> <p>Klicken Sie auf die Schaltfläche Protokollzeit .</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Erfassen der Zeit</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Systemaktualisierungen auf der Registerkarte Updates filtern</p> </td> 
   <td> <p>Klicken Sie auf den Link Systemaktualisierungen filtern .</p> </td> 
   <td> <p>Deaktivieren Sie den Umschalter Aktivitätsprotokoll anzeigen .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update funktioniert</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anzeigen von Systemaktualisierungen auf der Registerkarte Updates</p> </td> 
   <td> <p>Klicken Sie auf Alle Updates anzeigen</p> </td> 
   <td> <p>Aktivieren Sie den Umschalter Aktivitätsprotokoll anzeigen .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update funktioniert</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tagging anderer Benutzer bei Aktualisierungen oder Kommentaren</p> </td> 
   <td> <p>Klicken Sie auf das Symbol Andere in dieses Update einschließen .</p> </td> 
   <td> <p>Hinzufügen von Benutzern und Teams im Feld "Benachrichtigen"</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update funktioniert</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anzeigen eines Objekts nur für Benutzer in Ihrem Unternehmen zulassen</p> </td> 
   <td> <p>Klicken Sie auf das Sperrsymbol</p> </td> 
   <td> <p>Umschalten zwischen Privat und Unternehmen</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Kennzeichnen anderer Benutzer auf Updates</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anzeigen eines Objekts durch Benutzer außerhalb Ihres Unternehmens zulassen</p> </td> 
   <td> <p>Klicken Sie auf das Sperrsymbol</p> </td> 
   <td> <p>Deaktivieren Sie den Umschalter Privat in Unternehmen .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Kennzeichnen anderer Benutzer auf Updates</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hinzufügen einer Antwort oder Aktualisierung zu einem Kommentar oder Aktualisieren</p> </td> 
   <td> <p>Klicken Sie auf die Schaltfläche Kommentar .</p> </td> 
   <td> <p>Klicken Sie auf die Schaltfläche Antwort oder Aktualisieren .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update funktioniert</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aufgabenstatus aktualisieren</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aktualisierungsbedingung für Aufgaben und Probleme</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Hinzufügen eines Updates zu einem Dokument</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Mobile Verbesserungen {#mobile-improvements}

Die Mobile App enthält die folgenden Verbesserungen:

* Links, die für Sie in anderen Mobile Apps freigegeben wurden, werden jetzt in der mobilen Workfront-App geöffnet.

  Weitere Informationen zur Freigabe von Links finden Sie unter .

  Dieses Update wird in einigen Fällen diese Woche für iOS veröffentlicht und die Android-Aktualisierung sollte kurz danach folgen.

* Wir haben unsere Supportanforderungen für die iOS-Plattform aktualisiert, um iPhone X zu unterstützen.

  Weitere Informationen zu unterstützten Mobilgeräten und Betriebssystemen finden Sie in der .
