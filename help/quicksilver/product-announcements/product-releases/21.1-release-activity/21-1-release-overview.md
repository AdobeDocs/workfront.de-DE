---
content-type: release-notes
keywords: Anmerkungen,vierteljährlich,aktualisieren
navigation-topic: product-releases
title: Versionsübersicht 21.1
description: Die Version 21.1 wurde in der Woche vom in der Produktionsumgebung bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3659'
ht-degree: 0%

---

# Versionsübersicht 21.1

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

Auf dieser Seite finden Sie Informationen zur Funktionalität von Adobe Workfront Classic und zum neuen Adobe Workfront-Erlebnis, das in Version 21.1 enthalten ist.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

Mit dieser Version veröffentlichen wir neue Funktionen und Verbesserungen, mit denen Sie das Comeback 2021 mit anpassbaren Strategien, automatisierten Arbeitsprozessen und einer vernetzten digitalen Infrastruktur anführen können, um den Erfolg im gesamten Unternehmen zu ermöglichen.

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

* [Verbesserungen für Administratoren](#administrator-enhancements)
* [Verbesserungen beim Ressourcen-Management](#resource-management-enhancements)
* [Verbesserungen beim Projektmanagement](#project-management-enhancements)
* [Verbesserte Analysen](#enhanced-analytics-improvements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Verbesserungen für Mobilgeräte](#mobile-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

### Administrator-Verbesserungen {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Einführung einer neuen Zugriffsebenen-Einstellung für das Kopieren von Projekten</a> </p> <p>Um Ihnen als System-Admin mehr Kontrolle darüber zu geben, was Planende mit einem Projekt tun können, haben wir den Bearbeitungszugriff auf Projekte in der Zugriffsebene granularer gestaltet, indem eine neue Einstellung eingeführt wurde, mit der Sie die Möglichkeit haben, Projekte zu kopieren. Vor dieser Änderung hatten Benutzer, die Sie den Zugriff auf „Projekte bearbeiten“ aktiviert haben, automatisch Zugriff, um sie zu kopieren. Mit der neuen Funktion können Sie Benutzern Zugriff auf die Bearbeitung von Projekten gewähren, ohne diese unbedingt kopieren zu müssen, indem Sie die neue Kopiereinstellung deaktivieren.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">Wählen Sie in einem benutzerdefinierten Formular für ein Objekt alle Elemente in einem Dropdown-Feld mit Mehrfachauswahl aus</a> </p> <p>Wenn Sie auf der Detailseite für ein Objekt ein Dropdown-Feld mit Mehrfachauswahl in einem benutzerdefinierten Formular ausfüllen, können Sie auf Alle auswählen klicken, wenn Sie alle verfügbaren Optionen auswählen müssen.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(derzeit nicht verfügbar, wenn Sie eine neue Anfrage senden.)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">Berechnen Sie alle benutzerdefinierten Formularfelder für ein Objekt neu</a> </p> <p>Jetzt ist es einfacher, sicherzustellen, dass alle Daten in berechneten benutzerdefinierten Feldern für ein Objekt aktuell sind. Mit der neuen Menüoption Ausdrücke neu berechnen können Sie alle Daten in diesen Feldern schnell neu berechnen.</p> <p>Dies ist besonders nützlich, nachdem jemand Daten in einem anderen Objekt bearbeitet hat, auf das ein berechnetes benutzerdefiniertes Feld in Ihrem -Objekt verweist.</p> <p>Zuvor mussten Benutzende Problemumgehungen verwenden, um sicherzustellen, dass alle Daten in berechneten benutzerdefinierten Feldern aktuell waren. Beispielsweise bearbeiteten sie das -Objekt zusammen mit anderen -Objekten, um die für die Massenbearbeitung verfügbare Option „Neuberechnung“ zu verwenden.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 10. Dezember 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">Voreinstellungen für Aufgaben und Probleme für Gruppenadministratoren entsperren</a> </p> <p>Workfront-Administratoren können Gruppenadministratoren nun mehr Autonomie geben, indem sie individuelle Aufgaben- und Problemvoreinstellungen freischalten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für ihre Gruppen konfigurieren, um die individuellen Anforderungen und internen Prozesse jeder Gruppe zu erfüllen.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(vor dem 24. Juni 2021) war diese Version als Teil eines schrittweisen Rollouts nur für Kunden auf Cluster 4 und 6 und einige andere Kunden verfügbar. Jetzt ist es in der Produktion für alle Kunden verfügbar.)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">Zugriffsebenen-Einstellungen für Portfolios und Programme separat konfigurieren</a> </p> <p>Jetzt ist es einfacher, den Benutzerzugriff auf Portfolios und Programme zu verwalten, da Sie deren Zugriffsebenen-Einstellungen separat konfigurieren können.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">Aktivieren Sie beim Bearbeiten von Informationen in einem benutzerdefinierten Formular alle Kontrollkästchen in einer Reihe</a> </p> <p>Wenn Sie auf der Detailseite für ein Objekt ein benutzerdefiniertes Formularfeld ausfüllen, das Kontrollkästchen enthält, können Sie auf Alle auswählen klicken, wenn Sie alle verfügbaren Kontrollkästchen auswählen müssen.</p> <p>Diese Option wird nur angezeigt, wenn das Feld mehr als zwei Kontrollkästchen enthält.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(derzeit nicht verfügbar, wenn eine Anfrage gesendet wird).</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">Konfigurieren Ihrer Workfront auf die Zulassungsliste setzen-E-Mail-Adresse</a> </p> <p>Um Ihre Daten besser zu schützen, können Sie jetzt eine E-Mail-Domain-Zulassungsliste verwenden, um:</p> 
    <ul> 
     <li> <p>Steuern, wohin Workfront-E-Mails gesendet werden können, wenn sie in Workfront gespeicherte Berichte oder Dokumente enthalten</p> </li> 
     <li> <p>E-Mail-Domains können in der E-Mail-Adresse gespeichert werden, die Benutzer in ihrem Benutzerprofil angeben können</p> </li> 
    </ul> <p>Wenn Sie beispielsweise sensible Daten schützen möchten, z. B. einen Bericht, in dem Ihre gefährdeten Kunden aufgeführt sind, können Sie nur Ihre interne E-Mail-Domain oder Ihre Domains in die E-Mail-Zulassungsliste einbeziehen. Auf diese Weise können Benutzende diesen Bericht (oder einen anderen Workfront-Bericht) nicht an eine externe E-Mail-Adresse senden.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit der Version 21.1 </p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Gruppenadministrator für eine Untergruppe zuweisen</a> </p> <p>Um die Unabhängigkeit der verschiedenen Unternehmensebenen zu erleichtern, haben wir die Möglichkeit hinzugefügt, einer Untergruppe einen Gruppenadministrator zuzuweisen. Jetzt können Sie sicherstellen, dass Sie die Verwaltung von Untergruppen an die richtigen Personen delegieren.</p> <p>Zuvor konnte nur eine Gruppe auf oberster Ebene Gruppenadministratoren haben, und diese Administratoren verwalteten alle Untergruppen unter der Gruppe auf oberster Ebene.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">Arbeiten mit Gruppenprojekten und Genehmigungsprozessen im Bereich Gruppen</a> </p> <p>Wenn Sie Gruppenadministrator sind, können Sie die Projekte und Genehmigungsprozesse Ihrer Gruppe einfach anzeigen und damit arbeiten, da sie jetzt im Bereich Gruppen aufgeführt sind. </p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">Konfigurieren von Ereignisbenachrichtigungen für Gruppen</a> <span style="color: #dc143c; font-weight: bold;">Neu in der Vorschau!</span></p> <p>Workfront-Administratoren können Gruppenadministratoren nun mehr Autonomie geben, indem sie Ereignisbenachrichtigungen für ihre Gruppen der obersten Ebene konfigurieren können. Untergruppen übernehmen Ereignisbenachrichtigungskonfigurationen von ihrer übergeordneten Gruppe.</p> <p>Zuvor konnten Ereignisbenachrichtigungen nur von einem Workfront-Administrator auf Systemebene konfiguriert werden, d. h. alle Gruppen mussten denselben Satz an Ereignisbenachrichtigungen verwenden.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 22. Januar 2021</p> <p>Produktionsversion: Mit Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Ursprünglich in der Produktion nur für Kunden auf Cluster 4 im Rahmen eines schrittweisen Rollouts verfügbar; kurz danach für andere Cluster verfügbar)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">Anzeigen der Anzahl der verwendeten und zugewiesenen Lizenzen in einer Gruppe</a> </p> <p>Um zu bestimmen, wie gut Ihre Lizenzen verteilt werden, können Sie jetzt die Anzahl der Lizenzen anzeigen, die in einer Gruppe und allen untergeordneten Gruppen verwendet werden.</p> <p>Wenn Sie eine Gruppe der obersten Ebene verwalten, können Sie sowohl die Anzahl der in einer Gruppe verwendeten Lizenzen (und deren Untergruppen) als auch die maximale Anzahl der für die Gruppe zugewiesenen Lizenzen anzeigen.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbesserungen beim Ressourcen-Management {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">Workload-Balancer für Projekte</a> </p> <p>Der Workload Balancer ist jetzt in einem Projekt verfügbar. Jetzt haben Sie die Möglichkeit, zwischen der Verwendung des Workload-Balancer oder des Zeitplanungstools zur Verwaltung Ihrer Projektressourcen zu wählen.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront-Balancer für ein Team verfügbar</a> </p> <p>Der Workload Balancer ist jetzt in einem Team verfügbar. Jetzt haben Sie die Möglichkeit, zwischen der Verwendung des Workload-Balancer oder des Zeitplanungstools zur Verwaltung Ihrer Team-Ressourcen zu wählen. </p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbesserungen beim Projekt-Management {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Der Export ist jetzt im Abschnitt Metriken eines Projekts verfügbar</a> </p> <p>Um den Status und Fortschritt eines Projekts leichter freizugeben, können Sie jetzt das gesamte Dashboard im Abschnitt Metriken eines Projekts in eine .png-Datei exportieren.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 15. Januar 2021</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">Aktualisieren des Anfrageprozentsatzes, wenn das Projekt oder die Aufgabe aus der Anfrageaktualisierung konvertiert wurde</a> </p> <p>Wir haben die Funktionsweise des Prozentsatzes abgeschlossener Probleme für Probleme aktualisiert, die in Projekte oder Aufgaben konvertiert wurden. Mit der neuen Funktion wird bei der Konvertierung eines Problems in eine Aufgabe oder ein Projekt der Prozentwert der abgeschlossenen Probleme synchron mit dem Prozentwert der abgeschlossenen Aufgaben oder Projekte aktualisiert, wenn die Einstellung „Problemstatus automatisch aktualisieren, wenn sich der Status des Lösungsobjekts ändert“ im Setup aktiviert ist.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">Felder wurden aus der Seite „Neue Anfrage“ entfernt</a> </p> <p>Im Rahmen der Neugestaltung der Seite „Neue Anfrage“ haben wir die Felder für neue Probleme aktualisiert, die im Abschnitt „Warteschlangen-Setup“ eines Projekts eingerichtet werden.</p> <p>Verschiedene Felder für neue Probleme werden nur angezeigt, wenn ein Problem im Abschnitt „Probleme“ des Projekts erstellt wird. Sie werden beim Senden eines Problems über eine Anfrage-Warteschlange im Bereich Anfragen nicht angezeigt.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsversion: Mit der Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Aus der Version entfernt)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Neues Erlebnis beim Senden von Anfragen im Bereich Anfragen</a> </p> <p>Um die Konsistenz mit dem neuen Workfront-Erlebnis zu gewährleisten und beim Senden von Anfragen Effizienz zu erzielen, haben wir das Feld Neue Anfrage im Bereich Anfragen neu gestaltet.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsfreigabe: Mit der Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Aus der Version entfernt; verbleibt in der Vorschau und Veröffentlichung in der Produktion mit 21.2)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Freigeben eines Links zu einer Anfrage-Warteschlange beim Senden einer Anfrage</a> </p> <p>Wir haben es jetzt möglich gemacht, einen Link zu einer Anfrage-Warteschlange, einer Themengruppe oder einem Warteschlangenthema freizugeben, wenn Sie eine Anfrage erstellen.</p> <p>Bevor Sie eine neue Anfrage senden, können Sie einen Link in die Anfrage-Warteschlange, die Themengruppe oder das Warteschlangenthema der Anfrage kopieren und für andere Benutzer freigeben oder ihn in ein Dashboard einbetten.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 13. Januar 2021</p> <p>Produktionsfreigabe: Mit der Version 21.1 <span style="color: #dc143c; font-weight: bold;">(Aus der Version entfernt; verbleibt in der Vorschau und Veröffentlichung in der Produktion mit 21.2)</span></p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Neue Liste gesendeter Anfragen</a> </p> <p>Damit Sie Ihre gesendeten Anfragen einfacher und konsistenter verwalten können, haben wir die Abschnitte Gesendete Anfragen und Alle Anfragen im Bereich Anfragen entfernt und durch eine neue Liste Gesendet ersetzt. Die Liste hat ein vertrautes Erscheinungsbild, das allen anderen Listen im System entspricht, sodass Sie nach verschiedenen Kategorien gesendeter Anfragen filtern und schnell nach einer Anfrage suchen können, die möglicherweise schwer zu finden ist.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">Suchen Sie nach einer Gruppe, die Sie einem Projekt zuweisen möchten, und zeigen Sie deren Details an</a> </p> <p>Es ist jetzt einfacher, sicherzustellen, dass Sie die richtige Gruppe identifizieren, wenn Sie eine Gruppe einem Projekt zuweisen. Bewegen Sie den Mauszeiger über den Namen einer Gruppe, die Sie im Feld Gruppe finden, und klicken Sie dann auf das Informationssymbol, das neben dem Namen angezeigt wird, um die QuickInfo „Gruppendetails“ anzuzeigen.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Bericht zur neuen Benutzerdelegierung</a> </p> <p>Zuvor konnten Informationen für Aufgaben-, Problem- und Projektgenehmigungsdelegationen nur von den Delegierten in ihrem Heimatbereich angezeigt werden. Damit andere Benutzer diese Informationen sehen können, können Planbenutzer jetzt den Bericht Benutzerdelegierung erstellen, der Ihnen Folgendes mitteilt:</p> 
    <ul> 
     <li> <p>Wer hat diese Genehmigungen an einen anderen Benutzer delegiert?</p> </li> 
     <li> <p>Welche Benutzerin bzw. welcher Benutzer diese Genehmigungen erhalten hat</p> </li> 
     <li> <p>Start- und Enddatum dieser Delegationen</p> </li> 
    </ul> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: 21. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Erweiterte Analytics-Verbesserungen {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">Die Seite „Personen“ ist jetzt für alle Cluster verfügbar</a> </p> <p>Die Seite Personen ist jetzt auf Workfront Classic für Cluster 4 verfügbar. Diese Seite enthält die Diagramme für Aktivität nach Team, Ressourcenkapazität und Teamkapazität.</p> <p>Diese Seite war zuvor mit Version 20.3 sowohl in Workfront Classic als auch in der neuen Workfront-Version für alle anderen Cluster verfügbar.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 28. Januar 2021</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis (zuvor verfügbar)</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">Erweiterte Analyse wird jetzt standardmäßig angezeigt</a> </p> <p>Hinweis: Diese Änderung gilt nur für Benutzer, die neu zu Layout-Vorlagen hinzugefügt wurden. Benutzende, die einer benutzerdefinierten Layout-Vorlage zugewiesen sind, sind von dieser Änderung ebenfalls nicht betroffen.</p> <p>In der Standard-Layout-Vorlage ist der Bereich „Analysen“ jetzt standardmäßig aktiviert, d. h. Benutzende, die dieser Layout-Vorlage zugewiesen sind, sehen jetzt den Bereich „Analysen“ in der globalen Navigationsleiste in Workfront Classic und das Hauptmenü in der neuen Workfront-Version.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 6. November 2020</p> <p>Produktionsversion: 3. Dezember 2020</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">Erweiterte Analyse für alle Cluster verfügbar</a> </p> <p>Die erweiterte Analyse ist für alle Workfront-Cluster verfügbar, einschließlich der Kunden in Cluster 6.</p> <p>Zuvor war Enhanced Analytics nicht in Google Cloud Platform verfügbar, was Kunden in Cluster 6 daran hinderte, auf den Analytics-Bereich zuzugreifen. Jetzt können Geschäfts- und Unternehmenskunden auf Cluster 6 auf den Analytics-Bereich zugreifen.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 20. November 2020</p> <p>Produktionsversion: 3. Dezember 2020</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Adobe Workfront-Benachrichtigungsverbesserungen in Microsoft Teams</a> </p> <p>Um die Verwendung von Workfront über Microsoft Teams zu vereinfachen, haben wir verschiedene Verbesserungen zu den Microsoft Teams-Benachrichtigungen hinzugefügt, die von Workfront gesendet werden.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschauversion: Nicht zutreffend</p> <p>Produktionsversion: 12. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Verbesserungen für Mobilgeräte {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Neue Navigations-Breadcrumbs in der Adobe Workfront-App</a> </p> <p>Die Breadcrumb-Navigation wurde zur Mobile App von Workfront hinzugefügt. Jetzt können Sie diese Funktion verwenden, um zu übergeordneten Arbeitselementen innerhalb eines Projekts zu navigieren.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschauversion: Nicht zutreffend</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Rich-Text wird in benutzerdefinierten Formularen in der Workfront-App unterstützt</a> </p> <p>Sie können jetzt Rich-Text-Formatierung in benutzerdefinierten Formulartextfeldern in der Workfront Mobile App verwenden.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschauversion: Nicht zutreffend</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">SSO-Benutzer können sich jetzt mit der Face ID- oder Fingerabdruck-Technologie erneut bei der Workfront-App anmelden</a> </p> <p>Wenn Ihr Unternehmen SSO verwendet, können Sie sich jetzt mit Ihrer Gesicht-ID oder Ihrem Fingerabdruck nach Ablauf der Zeit bei der Workfront-Mobile-App anmelden. Sie müssen sich jedoch zunächst mit Ihren SSO-Anmeldedaten anmelden.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschauversion: Nicht zutreffend</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
--&gt;

### Weitere Verbesserungen {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">Aktualisierungen der Anforderungen für fehlgeschlagene Ereignisabonnements</a> </p> <p>Die Anforderungen für die Soft-Deaktivierung von Ereignisabonnementfehlern werden aktualisiert. Zusätzlich zu den bestehenden Anforderungen werden Ereignisabonnements jetzt vorläufig deaktiviert, wenn sie nicht innerhalb von 2000 Versuchen einen erfolgreichen Versand erreichen. Damit soll die bestehende 70 %-Regel für Fehlschläge gestärkt werden, die unter bestimmten Bedingungen zu übermäßig vielen Fehlern führen kann.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschauversion: Nicht zutreffend</p> <p>Produktionsversion: 11. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Neue Team-Felder für den Daily Digest verfügbar</a> </p> <p>Wir haben die Felder Team-Genehmigung und Zuweisungen zur E-Mail „Tägliche Auswahl der Aktion erforderlich“ hinzugefügt.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">POP-E-Mail-Option in Anfrage-Warteschlangen ersetzen</a> </p> <p>Wir ersetzen die POP-E-Mail-Option für Anfrage-Warteschlangen durch ein neues Workfront-verwaltetes System. Sie können Anfragen weiterhin per E-Mail senden, müssen jedoch stattdessen eine neue von Workfront verwaltete E-Mail-Adresse im Bereich Anfrage-Warteschlange einrichten. </p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 17. Dezember 2020</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">Stundenbearbeitung auf Arbeitszeittabellen beschränken</a> </p> <p>Um mehr Kontrolle über Arbeitszeittabellen und die Stundenbearbeitung zu erhalten, haben wir eine Einstellung hinzugefügt, mit der Sie die Bearbeitung von Arbeitszeittabellen auf Arbeitszeittabellen-Besitzer und Systemadministratoren beschränken können.</p> <p>Zuvor konnten Benutzende, bei denen die Option Arbeitszeittabellen und Stunden in ihrer Zugriffsebene aktiviert war, Stunden in jeder Arbeitszeittabelle bearbeiten.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 21. Januar 2021</p> <p>Produktionsversion: Mit der Version 21.1</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Verbesserte Filter und Ansichten im Arbeitszeittabellen-Bereich</a> </p> <p>Wir haben Filter für Projekte und Probleme sowie Ansichts- und Gruppierungsoptionen zur Suchseite hinzugefügt.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: 21. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">Überstundenfeld in Arbeitszeittabellen ausblenden</a> </p> <p>Sie können jetzt das Feld „Überstunden“ ausblenden, um Benutzerverwirrung zu stillen, wenn Sie die Überstunden in Workfront nicht verfolgen. Sie können das Überstundenfeld für eine Arbeitszeittabelle zur einmaligen Verwendung oder im Arbeitszeittabellen-Profil ausblenden.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 2. Dezember 2020</p> <p>Produktionsversion: 16. Dezember 2020</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">Ein- oder Ausblenden von Elementen in der Breadcrumb-Navigation</a> </p> <p>Um die Anzeige des vollständigen Breadcrumb-Pfads zu vereinfachen, haben wir Funktionen zum Erweitern und Reduzieren hinzugefügt.</p> <p>Jetzt werden alle abgeschnittenen Elemente vor dem Projekt mit dem Text „more“ gruppiert. „3 More“ zeigt beispielsweise an, dass drei Objekte nicht angezeigt werden.</p> <p>Zuvor mussten Sie auf die Auslassungszeichen klicken, um abgeschnittene Objekte in einem Dropdown-Menü anzuzeigen.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 7. Januar 2020</p> <p>Produktionsversion: 21. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Neues Erscheinungsbild für die Breadcrumb-Navigation</a> </p> <p>Damit Benutzende besser erkennen können, wo sie sich in Workfront befinden, und einfacher zwischen Objekten navigieren können, haben wir verschiedene Verbesserungen bei der Breadcrumb-Navigation vorgenommen.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> <p>Beta-Vorschau-Version: 10. Dezember 2020</p> <p>Produktionsversion: 21. Januar 2021</p> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> <p>Das neue Adobe Workfront-Erlebnis </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront-Zielverbesserungen

Die meisten neuen Funktionen der Workfront Goals-Version 21.1. Weitere Informationen zu diesen neuen Funktionen, die jetzt in der Vorschau verfügbar sind, finden Sie unter [Adobe Workfront Goals with the 21.1 release](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Verbesserungen am Workfront-Szenarioplaner

Neue Funktionen in Workfront Scenario Planner Version 21.1. Weitere Informationen zu diesen neuen Funktionen, die jetzt in der Vorschau verfügbar sind, finden Sie unter [Adobe Workfront Scenario Planner mit Version 21.1](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind außerhalb des Veröffentlichungszeitplans für 21.1 in der Produktionsumgebung verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Versionsaktivität von Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)

## API-Verbesserungen

Die API-Version 12 ist jetzt mit Version 20.4 verfügbar.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Informationen zu neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in der API-Version 12](https://experienceleague.adobe.com/de/docs/workfront/using/adobe-workfront-api/api-notes/new-api-version-12).

Weitere Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Wartungs-Updates für Workfront 

Informationen zu den Wartungs-Updates, die während der Version 21.1 vorgenommen wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Ankündigungen

* [Neue IP-Adressen für Workfront-E-Mails mit Version 21.1](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [Zulassungsliste der zusätzlichen IP-Adressen für Ereignisabonnements](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [Zulassungsliste der zusätzlichen Domains, die für den Zugriff auf Workfront erforderlich sind](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Flash-Einstellung](#flash-deprecation)
* Webinar zur Version [21.1](#21-1-release-webinar)
* [Änderung des Veröffentlichungsintervalls für die Vorschau](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### Neue IP-Adressen für Workfront E-Mail mit Version 21.1 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

Um den erfolgreichen E-Mail-Versand zu steigern, fügen wir mit der Produktionsversion 21.1 für die Cluster 1, 2, 3, 4 und 5 neue IP-Adressen hinzu.

Weitere Informationen dazu, welche IP-Adressen Sie für Ihren Cluster hinzufügen müssen, finden Sie unter [Neue IP-Adressen für Adobe Workfront-E-Mails mit Version 21.1](../../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md).

Um herauszufinden, auf welchem Cluster sich Ihre Instanz befindet, navigieren Sie zu Einrichtung > System > Kundeninformationen.

### Zulassungsliste der zusätzlichen IP-Adressen für Ereignisabonnements {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

Um den erfolgreichen Versand von Ereignisabonnements zu steigern, fügen wir im ersten Quartal 2021 mit der Produktionsversion 21.1 vier neue IP-Adressen hinzu. Sie müssen diese IP-Adressen vor Februar 2021 zu Ihrer Zulassungsliste hinzufügen, um sicherzustellen, dass Ihre Benutzerinnen und Benutzer weiterhin Ereignisabonnements erhalten.

Wenden Sie sich an Ihre interne IT- und/oder Sicherheitsabteilung, um Unterstützung beim Hinzufügen der neuen IPs zu erhalten, die im Artikel [Ereignisabonnement-API](../../../wf-api/general/event-subs-api.md) zu finden sind.

### Zulassungsliste der zusätzlichen Domains, die für den Zugriff auf Workfront erforderlich sind {#allowlist-of-additional-domains-required-for-accessing-workfront}

Wenn Ihr Unternehmen eine Firewall verwendet, müssen Sie die folgenden zusätzlichen Domains zu Ihrer Zulassungsliste hinzufügen, um einen unterbrechungsfreien Zugriff auf Workfront sicherzustellen:

* event.split.io
* sdk.split.io

Weitere Informationen finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Flash-Einstellung {#flash-deprecation}

Alle Flash-basierten Tools wurden am 19. November 2020 aus allen Produkten entfernt.

Weitere Informationen zu Ersatzlösungen für jedes spezifische Flash-basierte Tool finden Sie im folgenden Artikel: [Ersatz von Flash-basierten Tools in Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### Webinar zur Version 21.1 {#21-1-release-webinar}

Das Workfront-Webinar Version 21.1 wird am 3. Februar um 11:00 Uhr EDT/16:00 Uhr BST präsentiert. Registrieren Sie sich für das Webinar [hier](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&partnerref=ac&eventid=2934272&sessionid=1&key=5C231B3385686D1E224A49EBE0BF0E37&regTag=&V2=false&sourcepage=register).

### Änderung des Veröffentlichungsintervalls für die Vorschau {#change-in-preview-release-cadence}

Seit dem 20. Mai 2020 stellt Workfront wöchentlich Funktionen in der Vorschau-Umgebung bereit. Vor dieser Änderung wurden die Funktionen normalerweise alle zwei Wochen in der Vorschau-Umgebung veröffentlicht.

Weitere Informationen finden Sie unter [Häufig gestellte Fragen zur Änderung der Workfront-Vorschauversion](https://experienceleague.adobe.com/de/docs/workfront/using/home)

### Workfront One {#workfront-one}

Mit Workfront One entdecken Sie die wichtigsten Inhalte, Ressourcen und Neuigkeiten aus Workfront - alles an einem Ort, mit einer Anmeldung. Wir haben die Sites für Erlebnis, Community und Schulung zusammengeführt, damit Sie leichter finden können, wonach Sie suchen.

[Weitere Informationen zu Workfront One](https://business.adobe.com/de/products/workfront.html).
