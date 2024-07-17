---
product-area: reporting
navigation-topic: using-built-in-reports
title: Integrierte Adobe Workfront-Berichte verwenden
description: Adobe Workfront verfügt über eine umfassende Liste integrierter Berichte, die einsatzbereit sind. Workfront-Administratoren können integrierte Berichte ausblenden, sodass Benutzer keinen Zugriff darauf haben.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '2951'
ht-degree: 10%

---

# Integrierte Adobe Workfront-Berichte verwenden

<!--Audited: 07/2024-->

Adobe Workfront verfügt über eine umfassende Liste integrierter Berichte, die Sie verwenden können.

Workfront-Administratoren können integrierte Berichte ausblenden, sodass Benutzer keinen Zugriff darauf haben.

Weitere Informationen dazu, wie Sie integrierte Berichte ausblenden, finden Sie unter [Integrierte Berichte ausblenden](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Mitarbeiter oder höher</p>  
   <p>Aktuell: Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards, Kalender oder höher anzeigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten, um Filter zu einem Bericht hinzuzufügen oder zu bearbeiten</p> <p>Berechtigungen für einen Filter verwalten, um ihn in einer Liste zu bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überblick über native Berichte {#overview-of-built-in-reports}

Sie können einen integrierten Bericht anpassen und als neuen Bericht speichern. Weitere Informationen zum Anpassen integrierter Berichte finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Die folgenden Berichte werden mit dem Workfront-Paket geliefert. Die Berichte stehen allen Benutzern zur Verfügung, die zumindest Ansichtsrechte für integrierte Berichte in ihrer Zugriffsebene haben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Berichtsname</strong> </th> 
   <th><strong>Berichtbeschreibung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Tatsächliche Portfoliokosten nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und die tatsächlichen Kosten der Projekte anzeigt. Der Bericht ist nach Programmname gruppiert und wird nach Portfolio-Name gefragt. Er enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächliche Portfoliokosten nach Projekt</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und die tatsächlichen Kosten der Projekte anzeigt. Der Bericht wird nach Projektname gruppiert und nach Portfolio-Name gefragt. Er enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächlicher Portfolioumsatz nach Programm</td> 
   <td>Ein Projektbericht, der den geplanten Umsatz und den tatsächlichen Umsatz der Projekte anzeigt. Der Bericht ist nach Programmname gruppiert und wird nach Portfolio-Name gefragt. Er enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächlicher Portfolioumsatz nach Projekt</td> 
   <td>Ein Projektbericht, der den geplanten Umsatz und den tatsächlichen Umsatz der Projekte anzeigt. Der Bericht wird nach Projektname gruppiert und nach Portfolio-Name gefragt. Er enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächliche Einnahmen nach Firma</td> 
   <td>Ein Projektbericht, der den tatsächlichen Umsatz und das Unternehmen der Projekte anzeigt. Der Bericht ist nach Unternehmensname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächliche Einnahmen nach Gruppe</td> 
   <td>Ein Projektbericht, der den tatsächlichen Umsatz und die tatsächliche Gruppe der Projekte anzeigt. Der Bericht ist nach Gruppenname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Alle offenen Arbeitszeittabellen</td> 
   <td>Ein Timesheet-Bericht, der die Option "Open Timesheets"anzeigt. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Name des Eigentümers, Gesamtstunden, Überstunden, Name des Genehmigers und Status der Timesheets.</td> 
  </tr> 
  <tr> 
   <td>Genehmigungsarbeitszeittabellen (aufgefordert)</td> 
   <td>Ein Bericht zum Timesheet, der gesendete oder abgelehnte Timesheets mit Genehmigern anzeigt. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Eigentümer, Gesamtstunden, Überstunden, Name des Genehmigers und Status der Timesheets. Der Bericht wird wie folgt gefragt: Startdatum des Zeitblatts, Enddatum des Zeitblatts, Name des Zeitblatts "Genehmigende Person"und Benutzername.</td> 
  </tr> 
  <tr> 
   <td>Gefährdete Projekte</td> 
   <td>Ein Projektbericht, der aktuelle und geplante Projekte mit einem Risiko- oder Fehlerzustand anzeigt. Der Bericht zeigt die folgenden Felder an: Beschreibung, Geplantes Abschlussdatum, prognostiziertes Abschlussdatum, Prozentualer Abschluss, Status und Priorität der Projekte. Der Bericht ist nach Portfolio gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Einnahmenfakturierung nach Firma</td> 
   <td>Ein Projektbericht, der den Firmen- und Rechnungsumsatz der Projekte anzeigt. Der Bericht ist nach Unternehmensname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Einnahmenfakturierung nach Gruppe</td> 
   <td>Ein Projektbericht, der den Abrechnungsumsatz und die Gruppe der Projekte anzeigt. Der Bericht ist nach Gruppenname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Einnahmenfakturierung nach Monat</td> 
   <td>Ein Abrechnungsdatensatz -Bericht, der den Projektnamen, den Projektabrechnungsumsatz und das Rechnungsdatum der Abrechnungsdatensätze anzeigt. Der Bericht wird nach dem Monat des Rechnungsdatums der Rechnungsdatensätze gruppiert und enthält eine Grafik.</td> 
  </tr> 
  <tr> 
   <td>Abgeschlossene Probleme nach Woche</td> 
   <td>Ein Problembericht, der das tatsächliche Abschlussdatum der Probleme anzeigt. Der Bericht ist nach Woche des tatsächlichen Abschlussdatums der Probleme gruppiert und enthält eine Grafik.</td> 
  </tr> 
  <tr> 
   <td>Abgeschlossene Probleme nach Woche und nutzender Person</td> 
   <td>Ein Problembericht, der das tatsächliche Abschlussdatum und die Zuweisungen der Probleme anzeigt. Der Bericht ist nach dem primären Verantwortlichen und der Woche des tatsächlichen Abschlussdatums der Probleme gruppiert und enthält eine Grafik.</td> 
  </tr> 
  <tr> 
   <td>Aktuelle Projekte</td> 
   <td>Ein Projektbericht, der alle aktuellen Projekte anzeigt. Der Bericht zeigt die folgenden Felder an: Beschreibung, Geplantes Abschlussdatum, prognostiziertes Abschlussdatum, Prozentualer Abschluss, Status und Priorität der Projekte.</td> 
  </tr> 
  <tr> 
   <td>Stundenkosten nach Benutzer und Monat</td> 
   <td>Ein Matrix-Stunden-Bericht, der die Anzahl der protokollierten Stunden und die tatsächlichen Kosten anzeigt. Der Bericht wird nach dem Namen des Eigentümers und dem Monat des Anfangsdatums der Stunden gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Stunden nach Benutzer</td> 
   <td>Ein Stundenbericht, der die Anzahl der protokollierten Stunden anzeigt. Der Bericht ist nach dem Namen des Inhabers gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Stunden nach Benutzer und Woche</td> 
   <td>Ein Matrix-Stunden-Bericht, der die Anzahl der angemeldeten Stunden in den letzten vier Wochen und das Entrypdatum der Stunden anzeigt. Der Bericht wird nach dem Anfangsdatum der Stunden angezeigt und nach dem Eigentümernamen und dem Monat des Anfangsdatums der Stunden gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Probleme nach Status</td> 
   <td>Ein Problembericht, der den Status der Probleme anzeigt. Der Bericht ist nach Status der Probleme gruppiert und enthält eine Grafik.</td> 
  </tr> 
  <tr> 
   <td>Probleme nach Status und Projekt</td> 
   <td>Ein Matrix-Problem -Bericht, der den Status der Probleme in aktuellen Projekten und den Projektnamen anzeigt. Der Bericht ist nach Projektname und Status der Probleme gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Lohnkosten im Vgl. zu sonstigen Aufwendungen nach Portfolio</td> 
   <td>Ein Projektbericht, der die geplanten Arbeitskosten, tatsächlichen Arbeitskosten, geplanten Kosten und tatsächlichen Kosten der Projekte anzeigt. Der Bericht ist nach Portfolio gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Lohnkosten im Vgl. zu sonstigen Aufwendungen nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Arbeitskosten, tatsächlichen Arbeitskosten, geplanten Kosten und tatsächlichen Kosten der Projekte anzeigt. Der Bericht ist nach Portfolio und Programmname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Monatliche geplante Portfoliokosten im Vgl. zu Ist-Kosten nach Projekt</td> 
   <td>Ein Matrix-Projekt-(Finanzdaten-)Bericht, der das Zuordnungsdatum, die Gesamtsumme der geplanten Kosten, die tatsächlichen Gesamtkosten und die Gesamtkostenabweichung der Projekte anzeigt. Der Bericht ist nach Projektname, Quartal und Monat des Zuordnungsdatums gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Monatlicher geplanter Portfolioertrag im Vgl. zu den Ist-Einnahmen nach Projekt</td> 
   <td>Ein Matrix-Projekt-(Finanzdaten-)Bericht, der das Zuordnungsdatum, den Gesamteinnahmen, den tatsächlichen Gesamtumsatz und die Gesamtumsatzabweichung der Projekte anzeigt. Der Bericht ist nach Projektname, Quartal und Monat des Zuordnungsdatums gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Monatliche geplante Projektkosten im Vgl. zu Ist-Kosten</td> 
   <td>Ein Matrix-Projekt-(Finanzdaten-)Bericht, der das Zuordnungsdatum, die Gesamtsumme der geplanten Kosten, die tatsächlichen Gesamtkosten und die Gesamtkostenabweichung der Projekte anzeigt. Der Bericht ist nach Projektname, Quartal und Monat des Zuordnungsdatums gruppiert und wird nach Projektname gefragt.</td> 
  </tr> 
  <tr> 
   <td>Monatliche geplante Projekteinnahmen im Vgl. zu den Ist-Einnahmen</td> 
   <td>Ein Matrix-Projekt-(Finanzdaten-)Bericht, der das Zuordnungsdatum, den Gesamteinnahmen, den tatsächlichen Gesamtumsatz und die Gesamtumsatzabweichung der Projekte anzeigt. Der Bericht ist nach Projektname, Quartal und Monat des Zuordnungsdatums gruppiert und wird nach Projektname gefragt.</td> 
  </tr> 
  <tr> 
   <td>Meine Dokumente</td> 
   <td>Ein Dokumentbericht, der Dokumente anzeigt, die vom angemeldeten Benutzer hochgeladen wurden. Der Bericht zeigt die folgenden Felder an: den Namen des Inhabers, das Änderungsdatum, die Größe, die Versionsanzahl, Source und den Dokumenttyp.</td> 
  </tr> 
  <tr> 
   <td>Meine Favoriten</td> 
   <td>Ein Favoriten -Bericht, der eine Liste von Objekten anzeigt, die vom angemeldeten Benutzer als Favoriten gekennzeichnet wurden. Der Bericht zeigt die folgenden Felder an: den Objekttyp und den Namen der Favoriten.</td> 
  </tr> 
  <tr> 
   <td>Meine Probleme</td> 
   <td>Ein Problembericht, der unvollständige Probleme anzeigt, die dem angemeldeten Benutzer zugewiesen sind. Der Bericht zeigt die folgenden Felder an: Source-Name, Problemtyp, primärer Verantwortlicher, Einstiegsdatum, Status und Priorität der Probleme.</td> 
  </tr> 
  <tr> 
   <td>Meine Portfolios</td> 
   <td>Ein Portfolio -Bericht, der aktive Portfolio anzeigt, bei denen der angemeldete Benutzer der Portfolio-Manager ist.</td> 
  </tr> 
  <tr> 
   <td>Meine Programme</td> 
   <td>Ein Programmbericht, der Programme und deren Beschreibung anzeigt, wobei der angemeldete Benutzer der Programmmanager ist.</td> 
  </tr> 
  <tr> 
   <td>Offene Probleme meines Projekts</td> 
   <td>Ein Problembericht, der unvollständige Probleme in Projekten anzeigt, deren Projektteam den angemeldeten Benutzer enthält. Der Bericht zeigt die folgenden Felder an: Source-Name, Problemtyp, primärer Verantwortlicher, Einstiegsdatum, Status und Priorität der Probleme.</td> 
  </tr> 
  <tr> 
   <td>Meine Projekte</td> 
   <td>Ein Projektbericht, der aktuelle Projekte anzeigt, deren Projektteam den angemeldeten Benutzer enthält. Der Bericht zeigt die folgenden Felder an: Beschreibung, Geplantes Abschlussdatum, prognostiziertes Abschlussdatum, Prozentualer Abschluss, Status und Priorität der Projekte.</td> 
  </tr> 
  <tr> 
   <td>Meine gesendeten Probleme</td> 
   <td>Ein Problembericht, in dem vom angemeldeten Benutzer eingereichte Probleme angezeigt werden, die in den letzten drei Monaten geschlossen wurden oder derzeit geöffnet sind. Der Bericht zeigt die folgenden Felder an: Source-Name, Problemtyp, Einstiegsdatum, Status und Priorität der Probleme.</td> 
  </tr> 
  <tr> 
   <td>Meine Aufgaben</td> 
   <td>Ein Aufgabenbericht, der unvollständige Aufgaben in aktuellen Projekten anzeigt, die dem angemeldeten Benutzer zugewiesen sind. Der Bericht zeigt die folgenden Felder an: die geplante Dauer, den Projektnamen, den Hauptverantwortlichen, den geplanten Start, den geplanten Abschluss, den Abschluss in Prozent und die Priorität der Aufgaben.</td> 
  </tr> 
  <tr> 
   <td>Meine Arbeitszeittabellen</td> 
   <td>Ein Timesheet-Bericht, der alle Timesheets des angemeldeten Benutzers anzeigt. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Name des Eigentümers, Gesamtstunden, Überstunden, Name des Genehmigers und Status der Timesheets.</td> 
  </tr> 
  <tr> 
   <td>Meine nicht zugewiesenen Probleme</td> 
   <td>Ein Problembericht, der offene Probleme anzeigt, die einer der Vorgangsrollen des angemeldeten Benutzers zugewiesen sind und dem Benutzer nicht zugewiesen sind. Der Bericht zeigt die folgenden Felder an: Source-Name, Problemtyp, Einstiegsdatum, Status und Priorität der Probleme.</td> 
  </tr> 
  <tr> 
   <td>Meine nicht zugewiesenen Aufgaben</td> 
   <td>Ein Aufgabenbericht, der unvollständige Aufgaben anzeigt, die einer der Auftragsrollen des angemeldeten Benutzers zugewiesen sind und dem Benutzer nicht zugewiesen sind. Der Bericht zeigt die folgenden Felder an: die geplante Dauer, den Projektnamen, den primären Verantwortlichen, das geplante Startdatum, das geplante Abschlussdatum, den Prozentsatz des Abschlusses und die Priorität der Aufgaben.</td> 
  </tr> 
  <tr> 
   <td>Meine anstehenden Aufgaben</td> 
   <td>Ein Aufgabenbericht, der unvollständige Aufgaben anzeigt, die in den nächsten zwei Wochen beginnen sollen, sich auf aktuelle Projekte bezieht und dem angemeldeten Benutzer zugewiesen ist. Der Bericht zeigt die folgenden Felder an: Projektname, Geplantes Abschlussdatum, prognostiziertes Abschlussdatum, Prozentualer Abschluss und Status der Aufgaben.</td> 
  </tr> 
  <tr> 
   <td>Offene Arbeitszeittabellen (aufgefordert)</td> 
   <td>Ein Timesheet-Bericht, der die Option "Open Timesheets"anzeigt. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Eigentümer, Gesamtstunden, Überstunden, Name des Genehmigers, Status der Timesheets. Der Bericht wird wie folgt gefragt: Startdatum des Zeitblatts, Enddatum des Zeitblatts, Name des Zeitblatts "Genehmigende Person"und Benutzername.</td> 
  </tr> 
  <tr> 
   <td>Überbudgetiertes Projekt nach Portfolio</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und tatsächlichen Kosten der Projekte anzeigt. Der Bericht ist nach Portfolio gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Geplante Portfoliokosten nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und tatsächlichen Kosten der Projekte anzeigt. Der Bericht wird nach Programmname, gruppiert nach Programmname, und enthält ein Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Geplante Portfoliokosten nach Projekt</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und tatsächlichen Kosten der Projekte anzeigt. Der Bericht wird nach Projektname und nach Projektname gruppiert und enthält ein Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Geplanter Portfolioumsatz nach Programm</td> 
   <td>Ein Projektbericht, der den geplanten Umsatz und den tatsächlichen Umsatz der Projekte anzeigt. Der Bericht wird nach Programmname, gruppiert nach Programmname, und enthält ein Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Geplanter Portfolioumsatz nach Projekt</td> 
   <td>Ein Projektbericht, der den geplanten Umsatz und den tatsächlichen Umsatz der Projekte anzeigt. Der Bericht wird nach Projektname und nach Projektname gruppiert und enthält ein Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Geplante Kosten im Vgl. zu Istkosten nach Portfolio</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und tatsächlichen Kosten der Projekte nach Portfolio anzeigt. Der Bericht ist nach Portfolio gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplante Kosten im Vgl. zu Istkosten nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und tatsächlichen Kosten der Projekte nach Programm anzeigt. Der Bericht ist nach Portfolio gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplante Einnahmen im Vgl. zu tatsächlichen Einnahmen nach Portfolio</td> 
   <td>Ein Projektbericht, der den geplanten Umsatz und den tatsächlichen Umsatz der Projekte anzeigt. Der Bericht ist nach Portfolio gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplante im Vgl. zu tatsächlichen Einnahmen je Programm</td> 
   <td>Ein Projektbericht, der den geplanten Umsatz und den tatsächlichen Umsatz der Projekte anzeigt. Der Bericht ist nach Programmname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Nach Programm und Monat gruppierte Portfoliokosten</td> 
   <td>Ein Matrix-Projektbericht, der die geplanten Kosten, die budgetierten Kosten und die tatsächlichen Kosten der Projekte anzeigt. Der Bericht ist nach Projektname, Programmname und Portfolio des geplanten Projektstarts gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Portfolioprojekte nach Status gruppiert nach Programm</td> 
   <td>Ein Projektbericht, der den Status der Projekte anzeigt. Der Bericht ist nach Programmname und Projektstatus gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Nach Status und Portfolio gruppierte Portfolioprojekte</td> 
   <td>Ein Projektbericht, der den Projektnamen und den Projektstatus anzeigt. Der Bericht ist nach Projektname und Projektstatus gruppiert und enthält ein Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Portfolioumsatz nach Programm</td> 
   <td>Ein Projektbericht, der den Projektnamen, den Programmnamen, den geplanten Umsatz und den tatsächlichen Portfolio der Projekte anzeigt. Der Bericht ist nach Portfolio und Programmname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Nach Programm und Monat gruppierte Portfolioeinnahmen</td> 
   <td>Ein Matrix-Projektbericht, der den geplanten Umsatz, den tatsächlichen Umsatz, den Portfolio und den Programmnamen anzeigt. Der Bericht ist nach Projektname, Programmname und Portfolio des geplanten Projektstarts gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektkosten und -einnahmen nach Aufgabenstatus</td> 
   <td>Ein Matrix-Task-Bericht, der die geplanten Kosten, tatsächlichen Kosten, geplanten Umsatz, tatsächlichen Umsatz und den Projektnamen der Aufgaben anzeigt. Der Bericht ist nach Projektname und Status der Aufgaben gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektkosten im Vgl. zu Einnahmen je Portfolio</td> 
   <td>Ein Projektbericht, der den Projektnamen, die tatsächlichen Kosten und den tatsächlichen Portfolio der Projekte anzeigt. Der Bericht ist nach Portfolio gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Projektkosten nach Monat und Quartal</td> 
   <td>Ein Matrix-Spesenbericht, der das Eingangsdatum, den geplanten Betrag, den tatsächlichen Betrag und das Projekt der Ausgaben anzeigt. Der Bericht ist nach Projektname, Quartal und Monat des Ausgabedatums gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektstundenkosten nach Stundentyp und Monat</td> 
   <td>Ein Matrix-Stunden-Bericht, der die folgenden Felder anzeigt: Stunden, Einstiegsdatum, Tatsächliche Kosten der Projekte, Stundentyp, Projektname. Der Bericht ist nach Projektname, Monat des Einstiegsdatums der Stunden und Stündentyp gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektlohnkosten und -ausgaben nach Monat und Quartal</td> 
   <td>Ein Matrix-Projektbericht, der die geplanten Arbeitskosten, tatsächlichen Arbeitskosten, geplanten Kosten und tatsächlichen Kosten der Projekte anzeigt. Der Bericht ist nach Projektname, Quartal und Monat des tatsächlichen Projektstarts gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektleistung</td> 
   <td>Ein Projektbericht, der die folgenden Felder aktueller Projekte anzeigt: Fälligkeitsdatum, CPI, SPI, CSI, Geplante Kosten, Budget, EAC und Ausgaben der Projekte.</td> 
  </tr> 
  <tr> 
   <td>Projektanforderungen</td> 
   <td>Ein Projektbericht, der angeforderte Projekte anzeigt. Der Bericht zeigt die folgenden Felder an: Beschreibung, Geplantes Abschlussdatum, prognostiziertes Abschlussdatum, Prozentualer Abschluss, Status und Priorität der Projekte.</td> 
  </tr> 
  <tr> 
   <td>Projekte nach Bedingung</td> 
   <td>Ein Projektbericht, der die Projektbedingung anzeigt. Der Bericht ist nach Bedingung gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Projekte nach Bedingung und nach Gruppe</td> 
   <td>Ein Projektbericht, der den Fortschrittsstatus und die Gruppe der Projekte anzeigt. Der Bericht ist nach Gruppenname und Fortschrittsstatus gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Projekte nach Priorität</td> 
   <td>Ein Projektbericht, der die Priorität von Projekten anzeigt. Der Bericht ist nach Priorität gruppiert und enthält eine Grafik.</td> 
  </tr> 
  <tr> 
   <td>Projekte nach Fortschrittsstatus</td> 
   <td>Ein Projektbericht, der den Fortschrittsstatus der Projekte anzeigt. Der Bericht ist nach Fortschrittsstatus gruppiert und enthält eine Grafik.</td> 
  </tr> 
  <tr> 
   <td>Aufgaben nach Verlaufsstatus</td> 
   <td>Ein Aufgabenbericht, der den Fortschrittsstatus aller Aufgaben in aktuellen Projekten anzeigt. Der Bericht ist nach Fortschrittsstatus gruppiert und enthält eine Grafik.</td> 
  </tr> 
  <tr> 
   <td>Aufgaben nach Status</td> 
   <td>Ein Aufgabenbericht, der den Status aller Aufgaben anzeigt. Der Bericht ist nach Status gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Zu überprüfende Arbeitszeittabellen</td> 
   <td>Ein Timesheet-Bericht, der die Timesheets "Gesendet"und "Abgelehnt"anzeigt, deren Genehmiger der angemeldete Benutzer ist. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Eigentümer, Gesamtstunden, Überstunden, Name des Genehmigers und Status der Timesheets.</td> 
  </tr> 
  <tr> 
   <td>Gefährdete Aufgaben</td> 
   <td>Ein Aufgabenbericht, der unvollständige Aufgaben mit dem Fortschrittsstatus "Verspätet"oder "Hinter", einem Übergabedatum vor morgen und anzeigt, in dem der angemeldete Benutzer Teil des Projektteams des Projekts ist, in dem die Aufgaben ausgeführt werden. Der Bericht zeigt die folgenden Felder an: "Geplante Dauer", "Projektname", "Hauptverantwortlicher", "Geplanter Start", "Geplanter Abschluss", "Prozent abgeschlossen"und "Priorität"der Aufgaben.</td> 
  </tr> 
  <tr> 
   <td>Benutzeranmeldungen</td> 
   <td>Ein Benutzerbericht, der die folgenden Felder anzeigt: die eindeutige ID, die Anzahl der Anmeldungen (die Anzahl der Anmeldungen seit der Anmeldung des Benutzers mit Workfront) und das Datum der letzten Anmeldung der Benutzer. Der Bericht ist nach der Zugriffsebene der Benutzer gruppiert.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Zugriff auf native Berichte

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Klicken Sie auf **Berichte**.
1. Klicken Sie auf **Alle Berichte**.
1. Erweitern Sie das Dropdownmenü **Filter** und wählen Sie **Neuer Filter** aus.

1. Klicken Sie auf **Filterregel hinzufügen**.
1. Geben Sie im Feld **Feldname eingeben** den Wert **Globale ID** ein.

1. Wählen Sie unter dem Objekt **Bericht** die Option **Globale ID** aus.

1. Wählen Sie im Dropdown-Menü &quot;Filter-Modifikator&quot;die Option **Ist nicht leer**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Klicken Sie auf **Filter speichern**.\
   In der Berichtsliste werden nur integrierte Berichte angezeigt.\
   Weitere Informationen dazu, welche integrierten Berichte verfügbar sind, finden Sie im Abschnitt [Überblick über integrierte Berichte](#overview-of-built-in-reports) in diesem Artikel.
