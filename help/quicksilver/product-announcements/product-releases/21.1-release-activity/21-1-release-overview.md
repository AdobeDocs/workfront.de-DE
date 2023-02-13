---
content-type: release-notes
keywords: notes,vierteljährlich,update
navigation-topic: product-releases
title: Übersicht über die Version 21.1
description: Die Version 21.1 wurde in der Produktionsumgebung in der Woche von zur Verfügung gestellt.
author: Luke
feature: Product Announcements
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '3635'
ht-degree: 0%

---

# Übersicht über die Version 21.1

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

Auf dieser Seite finden Sie Informationen zur Funktionalität von Adobe Workfront Classic und dem neuen Adobe Workfront-Erlebnis, das in Version 21.1 enthalten ist.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

Mit dieser Version veröffentlichen wir neue Funktionen und Verbesserungen, die Ihnen helfen, das Comeback 2021 mit anpassbaren Strategien, automatisierten Arbeitsabläufen und einer vernetzten digitalen Infrastruktur zu führen, um im gesamten Unternehmen Erfolg zu ermöglichen.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

Diese Verbesserungen sind derzeit verfügbar

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the Preview environment and will be made available
</MadCap:conditionalText>
-->

in der Produktionsumgebung.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
-->

Sie wurden in der Woche vom 15. Februar 2021 veröffentlicht.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Adobe Workfront-Verbesserungen

* [Administratorverbesserungen](#administrator-enhancements)
* [Verbesserungen bei der Ressourcenverwaltung](#resource-management-enhancements)
* [Verbesserungen bei der Projektverwaltung](#project-management-enhancements)
* [Verbesserte Analyse](#enhanced-analytics-improvements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Mobile Verbesserungen](#mobile-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

### Administratorverbesserungen {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungsdaten und -umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Einführung neuer Einstellungen für die Zugriffsebene beim Kopieren von Projekten</a> </p> <p>Damit Sie als Systemadministrator mehr Kontrolle darüber haben, was Planer mit einem Projekt tun können, haben wir den Bearbeitungszugriff auf Projekte auf Zugriffsebene detaillierter gestaltet, indem eine neue Einstellung eingeführt wurde, mit der Sie die Möglichkeit zum Kopieren von Projekten aktivieren oder deaktivieren können. Vor dieser Änderung hatten Benutzer, die den Zugriff auf Projekte bearbeiten aktiviert hatten, automatisch Zugriff auf das Kopieren. Mit der neuen Funktion können Sie jemandem Zugriff auf Projekte gewähren, ohne notwendigerweise darauf zugreifen zu müssen, indem Sie die neue Einstellung Kopieren deaktivieren.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">Wählen Sie in einem benutzerdefinierten Formular für ein Objekt alle Elemente in einem Dropdown-Feld mit Mehrfachauswahl aus</a> </p> <p>Wenn Sie auf der Detailseite für ein Objekt ein Dropdown-Feld mit mehreren Auswahlen in einem benutzerdefinierten Formular ausfüllen, können Sie auf Alle auswählen klicken, wenn Sie alle verfügbaren Optionen auswählen müssen.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Derzeit nicht verfügbar, wenn Sie eine neue Anforderung senden.)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">Neuberechnen aller benutzerdefinierten Formularfelder für ein Objekt</a> </p> <p>Jetzt ist es einfacher sicherzustellen, dass alle Daten in berechneten benutzerdefinierten Feldern für ein Objekt aktuell sind. Mit der neuen Menüoption Ausdrücke neu berechnen können Sie schnell alle Daten in diesen Feldern neu berechnen.</p> <p>Dies ist besonders nützlich, wenn jemand Daten in einem anderen Objekt bearbeitet, auf das in einem berechneten benutzerdefinierten Feld in Ihrem Objekt verwiesen wird.</p> <p>Zuvor mussten Benutzer Umgehungslösungen verwenden, um sicherzustellen, dass alle Daten in berechneten benutzerdefinierten Feldern aktuell waren. Beispielsweise bearbeiteten sie das Objekt zusammen mit anderen Objekten, um die Neuberechnungsoption zu verwenden, die für die Massenbearbeitung verfügbar ist.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 10. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">Entsperren von Aufgaben- und Problemeinstellungen für Gruppenadministratoren</a> </p> <p>Workfront-Administratoren können Gruppenadministratoren jetzt mehr Autonomie gewähren, indem sie einzelne Aufgaben entsperren und Voreinstellungen festlegen. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für ihre Gruppen so konfigurieren, dass sie den individuellen Anforderungen und internen Prozessen jeder Gruppe gerecht werden.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Vor dem 24. Juni 2021 war dies als Teil einer stufenweisen Einführung nur für Kunden auf Cluster 4 und 6 und einige andere Kunden verfügbar. Jetzt ist es in der Produktion für alle Kunden verfügbar.)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Einstellungen für Zugriffsebene separat für Portfolios und Programme konfigurieren</a> </p> <p>Jetzt ist es einfacher, den Benutzerzugriff auf Portfolios und Programme zu verwalten, da Sie die Einstellungen für die Zugriffsebene separat konfigurieren können.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">Auswählen aller Kontrollkästchen in einer Reihe beim Bearbeiten von Informationen in einem benutzerdefinierten Formular</a> </p> <p>Wenn Sie auf der Detailseite für ein Objekt ein Feld mit benutzerdefiniertem Formular mit Kontrollkästchen ausfüllen, können Sie auf Alle auswählen klicken, wenn Sie alle verfügbaren Kontrollkästchen auswählen müssen.</p> <p>Diese Option wird nur angezeigt, wenn das Feld mehr als zwei Kontrollkästchen enthält.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Derzeit nicht verfügbar beim Senden einer Anfrage.)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Konfigurieren Ihrer Workfront-E-Mail-Zulassungsliste</a> </p> <p>Um Ihre Daten besser zu schützen, können Sie jetzt eine E-Mail-Domain-Zulassungsliste für folgende Zwecke verwenden:</p> 
    <ul> 
     <li> <p>Steuern, wohin Workfront-E-Mails gehen können, wenn sie in Workfront gespeicherte Berichte oder Dokumente enthalten</p> </li> 
     <li> <p>E-Mail-Domains steuern können sich in der E-Mail-Adresse befinden, die Benutzer in ihrem Benutzerprofil angeben können.</p> </li> 
    </ul> <p>Wenn Sie beispielsweise sensible Daten schützen möchten, z. B. einen Bericht, der Ihre risikobehafteten Kunden auflistet, können Sie nur Ihre interne E-Mail-Domäne oder Domänen in die E-Mail-Zulassungsliste aufnehmen. Auf diese Weise können Benutzer diesen Bericht (oder einen anderen Workfront-Bericht) nicht an eine externe E-Mail-Adresse senden.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit Version 21.1 </p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Zuweisen eines Gruppenadministrators für eine Untergruppe</a> </p> <p>Um die unabhängige Funktionsweise der Ebenen Ihres Unternehmens zu vereinfachen, haben wir die Möglichkeit hinzugefügt, einen Gruppenadministrator einer Untergruppe zuzuweisen. Nun können Sie sicherstellen, dass Sie die Verwaltung von Untergruppen an die richtigen Personen delegieren.</p> <p>Zuvor konnte nur eine Gruppe der obersten Ebene Gruppenadministratoren haben, und diese Administratoren haben alle Untergruppen unterhalb der Gruppe der obersten Ebene verwaltet.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">Arbeiten mit Gruppenprojekten und Genehmigungsprozessen im Bereich "Gruppen"</a> </p> <p>Wenn Sie Gruppenadministrator sind, können Sie die Projekte und Genehmigungsprozesse Ihrer Gruppe einfach anzeigen und verwenden, nachdem sie im Bereich Gruppen aufgelistet sind. </p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">Ereignisbenachrichtigungen für Gruppen konfigurieren</a> <span style="color: #dc143c; font-weight: bold;">Neu in der Vorschau!</span></p> <p>Workfront-Administratoren können nun Gruppenadministratoren mehr Autonomie gewähren, indem sie ihnen die Möglichkeit geben, Ereignisbenachrichtigungen für ihre Top-Level-Gruppen zu konfigurieren. Untergruppen übernehmen Ereignisbenachrichtigungskonfigurationen von ihrer obersten übergeordneten Gruppe.</p> <p>Zuvor waren Ereignisbenachrichtigungen nur von einem Workfront-Administrator auf Systemebene konfigurierbar, was bedeutet, dass alle Gruppen denselben Satz von Ereignisbenachrichtigungen verwenden mussten.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 22. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Erhältlich zunächst nur für Kunden, die Cluster 4 im Rahmen eines stufenweisen Rollouts nutzen; für andere Cluster kurz darauf verfügbar sind)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">Anzahl der in einer Gruppe verwendeten und zugewiesenen Lizenzen anzeigen</a> </p> <p>Um festzustellen, wie gut Ihre Lizenzen verteilt sind, können Sie jetzt die Anzahl der Lizenzen anzeigen, die in einer Gruppe verwendet werden, sowie alle Untergruppen darunter.</p> <p>Wenn Sie eine Gruppe der obersten Ebene verwalten, können Sie sowohl die Anzahl der in einer Gruppe verwendeten Lizenzen (und deren Untergruppen) als auch die maximale Anzahl der der Gruppe zugewiesenen Lizenzen anzeigen.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbesserungen bei der Ressourcenverwaltung {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungsdaten und -umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">Lastenausgleich für Projekte</a> </p> <p>Der Lastenausgleich ist jetzt in einem Projekt verfügbar. Jetzt haben Sie die Möglichkeit, zwischen der Verwendung des Workload Balancer oder des Planungs-Tools zur Verwaltung Ihrer Projektressourcen auszuwählen.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront Balancer für Teams verfügbar</a> </p> <p>Der Lastenausgleich ist jetzt in einem Team verfügbar. Jetzt können Sie zwischen der Verwendung des Workload Balancer oder des Planungs-Tools zur Verwaltung Ihrer Team-Ressourcen wählen. </p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbesserungen bei der Projektverwaltung {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungsdaten und -umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Export ist jetzt im Abschnitt Metriken eines Projekts verfügbar</a> </p> <p>Um den Status und Fortschritt eines Projekts einfacher freizugeben, können Sie jetzt das gesamte Dashboard im Abschnitt "Metriken"eines Projekts in eine PNG-Datei exportieren.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 15. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">Aktualisierung des Prozentsatzes des Problems, das abgeschlossen ist, wenn das Projekt oder die Aufgabe aus der Problemaktualisierung konvertiert wurde</a> </p> <p>Wir haben die Funktionsweise des Prozentsatzes der Fehlerbehebung bei Problemen aktualisiert, die in Projekte oder Aufgaben konvertiert wurden. Wenn mit der neuen Funktion ein Problem in eine Aufgabe oder ein Projekt konvertiert wird, wird der Prozentsatz der Fertigstellung des Problems synchron mit dem Prozentsatz der Fertigstellung der aufgelösten Aufgabe oder des aufgelösten Projekts aktualisiert, wenn die Einstellung "Automatisch Update Behebbarer Probleme bei Änderung des Status der aufgelösten Objektänderungen"bei der Einrichtung aktiviert ist.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">Aus der Seite "Neue Anforderung"entfernte Felder</a> </p> <p>Im Rahmen der Neugestaltung der Seite "Neue Anforderung"haben wir die Felder für neue Probleme aktualisiert, die im Abschnitt "Warteschlangeneinrichtung"eines Projekts eingerichtet wurden.</p> <p>Verschiedene Felder für neue Probleme werden nur angezeigt, wenn ein Problem im Abschnitt Probleme des Projekts erstellt wird. Sie werden nicht angezeigt, wenn ein Problem mithilfe einer Anforderungswarteschlange im Bereich Anforderungen gesendet wird.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Aus Version entfernt)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Neues Erlebnis beim Senden von Anforderungen im Bereich "Anforderungen"</a> </p> <p>Um die Konsistenz mit dem neuen Workfront-Erlebnis zu gewährleisten und die Effizienz beim Senden von Anforderungen zu steigern, haben wir das Feld "Neue Anforderung"im Bereich "Anforderungen"neu gestaltet.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Aus der Veröffentlichung entfernt; wird weiterhin in der Vorschau angezeigt und mit Version 21.2 für die Produktion freigegeben.)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Link in eine Anforderungswarteschlange freigeben, wenn eine Anforderung gesendet wird</a> </p> <p>Jetzt ist es möglich, einen Link zu einer Anforderungswarteschlange, einer Themengruppe oder einem Warteschlangenthema freizugeben.</p> <p>Bevor Sie eine neue Anforderung senden, können Sie einen Link in die Anforderungswarteschlange, die Themengruppe oder das Warteschlangenthema der Anforderung kopieren und für andere Benutzer freigeben oder in ein Dashboard einbetten.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Aus der Veröffentlichung entfernt; wird weiterhin in der Vorschau angezeigt und mit Version 21.2 für die Produktion freigegeben.)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Neue Liste gesendeter Anforderungen</a> </p> <p>Damit Sie Ihre gesendeten Anfragen einfacher und konsistenter verwalten können, haben wir die Abschnitte Gesendete Anfragen und Alle Anforderungen im Bereich Anforderungen entfernt und durch eine neue Liste ersetzt. Die Liste hat ein bekanntes Erscheinungsbild, das mit allen anderen Listen im System übereinstimmt, sodass Sie nach verschiedenen Kategorien gesendeter Anforderungen filtern und schnell nach einer Anforderung suchen können, die möglicherweise schwierig zu finden ist.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">Suchen Sie nach einer Gruppe, die Sie einem Projekt zuweisen möchten, und zeigen Sie deren Details an.</a> </p> <p>Es ist jetzt einfacher sicherzustellen, dass Sie die richtige Gruppe identifizieren, wenn Sie einem Projekt eine Gruppe zuweisen. Bewegen Sie den Mauszeiger über den Namen einer Gruppe, die Sie im Feld Gruppe finden, und klicken Sie dann auf das Informationssymbol, das neben dem Namen angezeigt wird, um die QuickInfo Gruppendetails anzuzeigen.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Bericht zur neuen Benutzerdelegation</a> </p> <p>Bisher konnten Informationen zu Aufgaben, Themen und Projektgenehmigungen nur vom Delegierten in seinem Heimatbereich eingesehen werden. Damit andere Benutzer diese Informationen sehen können, können Benutzer planen jetzt den Bericht Benutzerdelegation erstellen, in dem Folgendes angegeben wird:</p> 
    <ul> 
     <li> <p>Wer hat diese Genehmigungen an einen anderen Benutzer delegiert</p> </li> 
     <li> <p>Welcher Benutzer wurde diese Genehmigungen zugewiesen?</p> </li> 
     <li> <p>Beginn und Ende dieser Delegationen</p> </li> 
    </ul> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: 21. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbesserte Analyse {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungsdaten und -umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">Die Seite "Personen"ist jetzt für alle Cluster verfügbar.</a> </p> <p>Die Seite "Personen"ist jetzt in Workfront Classic für Cluster 4 verfügbar. Diese Seite enthält die Diagramme für Aktivitäten nach Team, Ressourcenkapazität und Teamkapazität.</p> <p>Diese Seite war bereits mit Version 20.3 von Workfront Classic und dem neuen Workfront-Erlebnis für alle anderen Cluster verfügbar.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 28. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis (zuvor verfügbar)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">Erweiterte Analysen werden jetzt standardmäßig angezeigt</a> </p> <p>Hinweis: Diese Änderung gilt nur für Benutzer, die den Layoutvorlagen neu hinzugefügt wurden. Benutzer, die einer benutzerdefinierten Layout-Vorlage zugewiesen sind, sind ebenfalls von dieser Änderung nicht betroffen.</p> <p>In der Standard-Layout-Vorlage ist der Bereich "Analytics"jetzt standardmäßig aktiviert. Das bedeutet, dass Benutzer, die dieser Layout-Vorlage zugewiesen sind, jetzt den Bereich "Analytics"in der globalen Navigationsleiste in Workfront Classic und das Hauptmenü im neuen Workfront-Erlebnis sehen.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 6. November 2020</p> <p>Produktionsversion: 3. Dezember 2020</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">Erweiterte Analyse für alle Cluster verfügbar</a> </p> <p>Erweiterte Analysen sind für alle Workfront-Cluster verfügbar, auch für Kunden, die Cluster 6 verwenden.</p> <p>Zuvor war die erweiterte Analyse in Google Cloud Platform nicht verfügbar, was verhinderte, dass Kunden auf Cluster 6 auf den Analytics-Bereich zugreifen konnten. Jetzt können Business- und Enterprise-Kunden auf Cluster 6 auf den Bereich Analytics zugreifen.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: 3. Dezember 2020</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Integrationsverbesserungen {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungsdaten und -umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Adobe Workfront-Benachrichtigungsverbesserungen in Microsoft Teams</a> </p> <p>Um Ihnen die Verwendung von Workfront über Microsoft Teams zu vereinfachen, haben wir verschiedene Verbesserungen an Microsoft Teams-Benachrichtigungen hinzugefügt, die von Workfront gesendet werden.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: nicht verfügbar</p> <p>Produktionsversion: 12. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Mobile Verbesserungen {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungsdaten und -umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Neue Navigations-Breadcrumbs in der Adobe Workfront-App</a> </p> <p>Wir haben der mobilen Workfront-App die Breadcrumb-Navigation hinzugefügt. Jetzt können Sie diese Funktion verwenden, um zu übergeordneten Arbeitselementen innerhalb eines Projekts zu navigieren.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: nicht verfügbar</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Rich-Text, der in benutzerdefinierten Formularen in der Workfront-App unterstützt wird</a> </p> <p>Sie können jetzt Rich-Text-Formatierungen in benutzerdefinierten Formulartextfeldern in der mobilen Workfront-App verwenden.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: nicht verfügbar</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">SSO-Benutzer können sich jetzt mit der Face ID oder der Fingerabdruck-Technologie erneut bei der Workfront-App anmelden</a> </p> <p>Wenn Ihr Unternehmen SSO verwendet, können Sie sich jetzt mit Ihrer Face ID oder Ihrem Fingerabdruck nach Ablauf der Sitzung bei der mobilen Workfront-App anmelden. Sie müssen sich jedoch zunächst mit Ihren SSO-Anmeldeinformationen anmelden.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: nicht verfügbar</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
—&gt;

### Weitere Verbesserungen {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungsdaten und -umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Aktualisierungen der Anforderungen an Ereignisabonnements</a> </p> <p>Wir aktualisieren die Soft-disable-Anforderungen für Fehler bei der Ereignisabonnement-Funktion. Zusätzlich zu den bestehenden Anforderungen wird die Option Ereignisabonnements jetzt deaktiviert, wenn sie innerhalb von 2000 Versuchen keinen erfolgreichen Versand erzielen. Damit soll die bestehende 70-%-Ausfallregel verschärft werden, die unter bestimmten Bedingungen zu übermäßigen Fehlschlägen führen kann.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: nicht verfügbar</p> <p>Produktionsversion: 11. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Neue Teamfelder für den täglichen Digest verfügbar</a> </p> <p>Wir haben der E-Mail "Action Needed Daily Digest"Teamgenehmigung und Zuweisungsfelder hinzugefügt.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">POP-E-Mail-Option in Anforderungswarteschlangen ersetzen</a> </p> <p>Wir ersetzen die POP-E-Mail-Option für Anforderungswarteschlangen durch ein neues Workfront-verwaltetes System. Sie können zwar weiterhin Anfragen per E-Mail senden, müssen aber stattdessen eine neue von Workfront verwaltete E-Mail-Adresse im Bereich "Anforderungswarteschlange"einrichten. </p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">Einschränken der Stundenbearbeitung in Timesheets</a> </p> <p>Um eine bessere Kontrolle über Timesheets und die Stundenbearbeitung zu ermöglichen, haben wir eine Einstellung hinzugefügt, mit der Sie die Stundenbearbeitung auf Timesheet-Inhaber und Systemadministratoren beschränken können.</p> <p>Zuvor konnten Benutzer, für die die Option Timesheets &amp; Stunden in ihrer Zugriffsebene aktiviert war, Stunden auf einem beliebigen Zeitblatt bearbeiten.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 21. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Verbesserte Filter und Ansichten im Bereich "Timesheets"</a> </p> <p>Wir haben Filter für Projekte und Probleme sowie Anzeige- und Gruppierungsoptionen zur Suchseite hinzugefügt.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: 21. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">Ausblenden des Zeitverlaufsfeldes in Timesheets</a> </p> <p>Sie können jetzt die Zeitüberschreitungsbox ausblenden, um die Verwirrung der Benutzer zu verringern, wenn Sie Überstunden in Workfront nicht verfolgen. Sie können die Zeitüberschreitungsbox für ein einmalig verwendetes Zeitblatt oder im Timesheet-Profil ausblenden.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: 16. Dezember 2020</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">Erweitern oder Reduzieren von Elementen in der Breadcrumb-Navigation</a> </p> <p>Um die Anzeige des vollständigen Breadcrumb-Pfads zu vereinfachen, haben wir die Funktion zum Erweitern und Reduzieren hinzugefügt.</p> <p>Jetzt werden alle abgeschnittenen Elemente vor dem Projekt mit dem Text "mehr"gruppiert. Beispielsweise gibt "3 weitere"an, dass es 3 Objekte gibt, die nicht angezeigt werden.</p> <p>Zuvor mussten Sie auf die Auslassungspunkte klicken, um abgeschnittene Objekte in einem Dropdown-Menü anzuzeigen.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 7. Januar 2020</p> <p>Produktionsversion: 21. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Neues Erscheinungsbild für die Breadcrumb-Navigation</a> </p> <p>Um Benutzern zu helfen, besser zu erkennen, wo sie sich in Workfront befinden, und einfacher zwischen Objekten zu navigieren, haben wir verschiedene Verbesserungen an der Breadcrumb-Navigation vorgenommen.</p> </td> 
   <td><strong>Verfügbar zu diesen Terminen:</strong> <p>Beta-Vorschau-Version: 10. Dezember 2020</p> <p>Produktionsversion: 21. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
 </tbody> 
</table>

## Verbesserungen bei Workfront-Zielen

Die meisten neuen Funktionen der Workfront Goals-Version 21.1. Informationen zu diesen neuen Funktionen, die jetzt in der Vorschau verfügbar sind, finden Sie unter [Adobe Workfront-Ziele mit Version 21.1](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Verbesserungen am Workfront-Szenario-Planer

Neue Funktionen in der Workfront Scenario Planer-Version mit Version 21.1. Informationen zu diesen neuen Funktionen, die jetzt in der Vorschau verfügbar sind, finden Sie unter [Adobe Workfront-Szenario-Planer mit Version 21.1](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind in der Produktion ab einem Zeitpunkt verfügbar, der außerhalb des Veröffentlichungszeitplans für 21.1 liegt. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## API-Verbesserungen

API-Version 12 ist jetzt mit Version 20.4 verfügbar.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Informationen zu den neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in API Version 12](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

Weitere Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Wartungs-Updates für Workfront 

Informationen zu den Wartungsupdates, die während der Version 21.1 vorgenommen wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Ankündigungen

* [Neue IP-Adressen für Workfront-E-Mails mit Version 21.1](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [Zulassungsliste der zusätzlichen IP-Adressen für Ereignisanmeldungen](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [Zulassungsliste der für den Zugriff auf Workfront erforderlichen zusätzlichen Domänen](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Einstellung von Flashs](#flash-deprecation)
* [Webinar zur Version 21.1](#21-1-release-webinar)
* [Änderung der Vorschau der Release-Kadenz](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### Neue IP-Adressen für Workfront-E-Mails mit Version 21.1 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

Um den erfolgreichen E-Mail-Versand zu verbessern, fügen wir neue IP-Adressen mit der Produktionsversion 21.1 für die Cluster 1, 2, 3, 4 und 5 hinzu.

Weitere Informationen dazu, welche IP-Adressen Sie für Ihren Cluster hinzufügen müssen, finden Sie unter [Neue IP-Adressen für Adobe Workfront-E-Mails mit Version 21.1](../../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md).

Um herauszufinden, auf welchem Cluster sich Ihre Instanz befindet, gehen Sie zu Einrichtung > System > Kundeninformationen.

### Zulassungsliste der zusätzlichen IP-Adressen für Ereignisanmeldungen {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

Um die erfolgreiche Bereitstellung von Ereignisabonnements zu verbessern, fügen wir im ersten Quartal 2021 mit der Produktionsversion 21.1 vier neue IP-Adressen hinzu. Sie müssen diese IP-Adressen vor Februar 2021 zu Ihrer Zulassungsliste hinzufügen, um sicherzustellen, dass Ihre Benutzer weiterhin Ereignisabos erhalten.

Wenden Sie sich an Ihre interne IT- und/oder Sicherheitsabteilung, um Unterstützung beim Hinzufügen der neuen IPs zu erhalten, die im Artikel enthalten sind. [Ereignisabonnement-API](../../../wf-api/general/event-subs-api.md).

### Zulassungsliste der für den Zugriff auf Workfront erforderlichen zusätzlichen Domänen {#allowlist-of-additional-domains-required-for-accessing-workfront}

Wenn Ihr Unternehmen eine Firewall verwendet, müssen Sie die folgenden zusätzlichen Domänen zu Ihrer Zulassungsliste hinzufügen, um einen unterbrechungsfreien Zugriff auf Workfront sicherzustellen:

* event.split.io
* sdk.split.io

Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Einstellung von Flashs {#flash-deprecation}

Alle Flash-basierten Tools wurden am 19. November 2020 aus allen Produkten entfernt.

Weitere Informationen zu Ersatzlösungen für die einzelnen Flash-basierten Tools finden Sie im folgenden Artikel: [Ersetzen von Flash-basierten Tools in Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### Webinar zur Version 21.1 {#21-1-release-webinar}

Das Workfront Release-Webinar 21.1 wird am 3. Februar um 11:00 Uhr EDT / 16:00 Uhr BST vorgestellt. Webinar registrieren [here](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### Änderung der Vorschau der Release-Kadenz {#change-in-preview-release-cadence}

Ab dem 20. Mai 2020 begann Workfront, die Funktionalität wöchentlich in der Vorschau-Umgebung verfügbar zu machen. Vor dieser Änderung wurde die Funktionalität in der Regel alle zwei Wochen in der Vorschau-Umgebung veröffentlicht.

Weitere Informationen finden Sie unter [Häufig gestellte Fragen zur Änderung der Workfront-Vorschau](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### Workfront One {#workfront-one}

Mit Workfront One werden Sie die wichtigsten Inhalte, Ressourcen und Neuigkeiten aus Workfront entdecken - alles an einem Ort, mit nur einer Anmeldung. Wir haben die Sites für Erlebnisse, Community und Schulungen vereinheitlicht, um das, was Sie suchen, leichter zu finden.

[Weitere Informationen zu Workfront One](https://www.workfront.com/campaigns/workfront-one).
