---
product-area: reporting
navigation-topic: using-built-in-reports
title: Verwenden von integrierten Adobe Workfront-Berichten
description: Adobe Workfront verfügt über eine umfangreiche Liste integrierter Berichte, die verwendet werden können. Workfront-Admins können integrierte Berichte ausblenden, sodass Benutzende keinen Zugriff darauf haben.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '2978'
ht-degree: 10%

---

# Verwenden von integrierten Adobe Workfront-Berichten

<!--Audited: 11/2024-->

Adobe Workfront verfügt über eine umfangreiche Liste integrierter Berichte, die Sie verwenden können.

Workfront-Admins können integrierte Berichte ausblenden, sodass Benutzende keinen Zugriff darauf haben. Weitere Informationen zum Ausblenden integrierter Berichte finden Sie unter [Integrierte Berichte ausblenden](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Mitwirkender oder höher</p>
      <p>Anfrage oder höher</p>
   </td>
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Anzeigen oder Erweitern des Zugriffs auf Berichte, Dashboards, Kalender</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für einen Bericht zum Hinzufügen oder Bearbeiten eines Filters zu einem Bericht</p> <p>Verwalten von Berechtigungen für einen Filter, um ihn in einer Liste zu bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Übersicht über integrierte Berichte {#overview-of-built-in-reports}

Sie können einen integrierten Bericht erstellen und als neuen Bericht speichern. Weitere Informationen zum Erstellen von Kopien integrierter Berichte finden Sie unter [Erstellen einer neuen Version eines &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#create-a-new-version-of-a-report)) im Artikel [Erstellen einer Kopie eines Berichts](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Die folgenden Berichte sind im Lieferumfang des Workfront-Pakets enthalten. Die Berichte stehen allen Benutzern zur Verfügung, die zumindest Ansichtsrechte für integrierte Berichte in ihrer Zugriffsebene haben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Berichtsname</strong> </th> 
   <th><strong>Berichtsbeschreibung</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Tatsächliche Portfoliokosten nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und Istkosten der Projekte ausgibt. Der Bericht ist nach Programmnamen gruppiert, nach Portfolio-Namen gefragt und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächliche Portfoliokosten nach Projekt</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und Istkosten der Projekte ausgibt. Der Bericht wird nach Projektname gruppiert, nach Portfolio-Name gefragt und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächlicher Portfolioumsatz nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Einnahmen und die tatsächlichen Einnahmen der Projekte ausgibt. Der Bericht ist nach Programmnamen gruppiert, nach Portfolio-Namen gefragt und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächlicher Portfolioumsatz nach Projekt</td> 
   <td>Ein Projektbericht, der die geplanten Einnahmen und die tatsächlichen Einnahmen der Projekte ausgibt. Der Bericht wird nach Projektname gruppiert, nach Portfolio-Name gefragt und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächliche Einnahmen nach Firma</td> 
   <td>Ein Projektbericht, der die tatsächlichen Einnahmen und die Firma der Projekte ausgibt. Der Bericht ist nach Firmenname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Tatsächliche Einnahmen nach Gruppe</td> 
   <td>Ein Projektbericht, der die tatsächlichen Einnahmen und die Gruppe der Projekte ausgibt. Der Bericht ist nach Gruppenname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Alle offenen Arbeitszeittabellen</td> 
   <td>Ein Arbeitszeittabellen-Bericht, der offene Arbeitszeittabellen ausgibt. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Name des Verantwortlichen, Gesamtstunden, Überstunden, Name der genehmigenden Person und Status der Arbeitszeittabellen.</td> 
  </tr> 
  <tr> 
   <td>Genehmigungsarbeitszeittabellen (aufgefordert)</td> 
   <td>Ein Arbeitszeittabellen-Bericht, der eingereichte oder abgelehnte Arbeitszeittabellen ausgibt. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Eigentümer, Gesamtstunden, Überstunden, Name der genehmigenden Person und Status der Arbeitszeittabellen. Der Bericht wird angezeigt durch: Startdatum der Arbeitszeittabelle, Enddatum der Arbeitszeittabelle, Name der genehmigenden Person für Arbeitszeittabelle und Benutzername.</td> 
  </tr> 
  <tr> 
   <td>Gefährdete Projekte</td> 
   <td>Ein Projektbericht, der aktuelle und geplante Projekte ausgibt, die den Status „Gefährdet“ oder „In Schwierigkeiten“ aufweisen. Der Bericht zeigt die folgenden Felder an: die Beschreibung, das geplante Abschlussdatum, das voraussichtliche Abschlussdatum, den Prozentsatz der Fertigstellung, den Status und die Priorität der Projekte. Der Bericht ist nach Portfolio-Namen gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Einnahmenfakturierung nach Firma</td> 
   <td>Ein Projektbericht, der die Firma und den Fakturaerlös der Projekte ausgibt. Der Bericht ist nach Firmenname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Einnahmenfakturierung nach Gruppe</td> 
   <td>Ein Projektbericht, der den Fakturaerlös und die Gruppe der Projekte ausgibt. Der Bericht ist nach Gruppenname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Einnahmenfakturierung nach Monat</td> 
   <td>Ein Rechnungsnachweisbericht, der den Projektnamen, den Fakturaerlös und das Rechnungsdatum der Rechnungsnachweise ausgibt. Der Bericht ist nach dem Monat des Abrechnungsdatums der Abrechnungs-Datensätze gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Abgeschlossene Probleme nach Woche</td> 
   <td>Ein Anfragebericht, der das tatsächliche Abschlussdatum der Anfragen ausgibt. Der Bericht ist nach der Woche des tatsächlichen Abschlussdatums der Probleme gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Abgeschlossene Probleme nach Woche und nutzender Person</td> 
   <td>Ein Anfragebericht, der das tatsächliche Abschlussdatum und die Zuweisung von Anfragen ausgibt. Der Bericht ist nach primär zugewiesener Person und nach Woche des tatsächlichen Abschlussdatums der Probleme gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Aktuelle Projekte</td> 
   <td>Ein Projektbericht, der alle aktuellen Projekte ausgibt. Der Bericht zeigt die folgenden Felder an: die Beschreibung, das geplante Abschlussdatum, das voraussichtliche Abschlussdatum, den Prozentsatz der Fertigstellung, den Status und die Priorität der Projekte.</td> 
  </tr> 
  <tr> 
   <td>Stundenkosten nach Benutzer und Monat</td> 
   <td>Ein Matrix-Stundenbericht, der die Anzahl der protokollierten Stunden und deren Ist-Kosten ausgibt. Der Bericht ist nach Name des Inhabers und dem Monat des Eingabedatums der Stunden gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Stunden nach Benutzer</td> 
   <td>Ein Stundenbericht, der die Anzahl der protokollierten Stunden ausgibt. Der Bericht ist nach Name des Inhabers gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Stunden nach Benutzer und Woche</td> 
   <td>Ein Matrix-Stundenbericht, der die Anzahl der protokollierten Stunden in den letzten vier Wochen und das Eingabedatum der Stunden ausgibt. Der Bericht wird durch das Eingabedatum der Stunden ausgelöst und nach Name des Inhabers und dem Monat des Eingabedatums der Stunden gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Probleme nach Status</td> 
   <td>Ein Problembericht, der den Status von Problemen ausgibt. Der Bericht ist nach Status der Probleme gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Probleme nach Status und Projekt</td> 
   <td>Ein Matrix-Problembericht, der den Status von Problemen in aktuellen Projekten und den Projektnamen ausgibt. Der Bericht ist nach Projektname und Status der Probleme gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Lohnkosten im Vgl. zu sonstigen Aufwendungen nach Portfolio</td> 
   <td>Ein Projektbericht, der die geplanten Lohnkosten, tatsächlichen Lohnkosten, geplanten Ausgaben und tatsächlichen Ausgaben der Projekte ausgibt. Der Bericht ist nach Portfolio-Name gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Lohnkosten im Vgl. zu sonstigen Aufwendungen nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Lohnkosten, tatsächlichen Lohnkosten, geplanten Ausgaben und tatsächlichen Ausgaben der Projekte ausgibt. Der Bericht ist nach Portfolio-Name und Programmname gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Monatliche geplante Portfoliokosten im Vgl. zu Ist-Kosten nach Projekt</td> 
   <td>Ein Matrix-Projektbericht (finanzielle Daten), der das Zuteilungsdatum, die geplanten Gesamtkosten, die Ist-Gesamtkosten und die Kostengesamtabweichung der Projekte ausgibt. Der Bericht ist nach Projektname, Quartal und Monat des Zuteilungsdatums gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Monatlicher geplanter Portfolioertrag im Vgl. zu den Ist-Einnahmen nach Projekt</td> 
   <td>Ein Matrix-Projektbericht (finanzielle Daten), der das Zuteilungsdatum, die geplanten Gesamteinnahmen, die tatsächlichen Gesamteinnahmen und die Gesamt-Einnahmenabweichung der Projekte ausgibt. Der Bericht ist nach Projektname, Quartal und Monat des Zuteilungsdatums gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Monatliche geplante Projektkosten im Vgl. zu Ist-Kosten</td> 
   <td>Ein Matrix-Projektbericht (finanzielle Daten), der das Zuteilungsdatum, die geplanten Gesamtkosten, die Ist-Gesamtkosten und die Kostengesamtabweichung der Projekte ausgibt. Der Bericht ist nach Projektname, Quartal und Monat des Zuteilungsdatums gruppiert und wird nach Projektname angezeigt.</td> 
  </tr> 
  <tr> 
   <td>Monatliche geplante Projekteinnahmen im Vgl. zu den Ist-Einnahmen</td> 
   <td>Ein Matrix-Projektbericht (finanzielle Daten), der das Zuteilungsdatum, die geplanten Gesamteinnahmen, die tatsächlichen Gesamteinnahmen und die Gesamt-Einnahmenabweichung der Projekte ausgibt. Der Bericht ist nach Projektname, Quartal und Monat des Zuteilungsdatums gruppiert und wird nach Projektname angezeigt.</td> 
  </tr> 
  <tr> 
   <td>Meine Dokumente</td> 
   <td>Ein Dokumentbericht, der die vom angemeldeten Benutzer hochgeladenen Dokumente ausgibt. Der Bericht zeigt die folgenden Felder an: Name des Inhabers, Änderungsdatum, Größe, Versionsanzahl, Source und Typ der Dokumente.</td> 
  </tr> 
  <tr> 
   <td>Meine Favoriten</td> 
   <td>Ein Favoritenbericht, der eine Liste von Objekten ausgibt, die vom angemeldeten Benutzer als Favoriten markiert wurden. Der Bericht zeigt die folgenden Felder an: den Objekttyp und den Namen der Favoriten.</td> 
  </tr> 
  <tr> 
   <td>Meine Probleme</td> 
   <td>Ein Anfragebericht, der noch nicht vollständig abgewickelte Anfragen ausgibt, die dem angemeldeten Benutzer zugewiesen wurden. Der Bericht zeigt die folgenden Felder an: Name der Source, Problemtyp, primärer Verantwortlicher, Eingabedatum, Status und Priorität der Probleme.</td> 
  </tr> 
  <tr> 
   <td>Meine Portfolios</td> 
   <td>Ein Portfolio-Bericht, der aktive Portfolios ausgibt, in denen der angemeldete Benutzer Portfolio Manager ist.</td> 
  </tr> 
  <tr> 
   <td>Meine Programme</td> 
   <td>Ein Programmbericht, der Programme und deren Beschreibung ausgibt, wobei der angemeldete Benutzer der Programm-Manager ist.</td> 
  </tr> 
  <tr> 
   <td>Offene Probleme meines Projekts</td> 
   <td>Ein Problembericht, der noch nicht vollständig abgeschlossene Probleme in Projekten ausgibt, bei denen der angemeldete Benutzer zum Projektteam gehört. Der Bericht zeigt die folgenden Felder an: Name der Source, Problemtyp, primärer Verantwortlicher, Eingabedatum, Status und Priorität der Probleme.</td> 
  </tr> 
  <tr> 
   <td>Meine Projekte</td> 
   <td>Ein Projektbericht, der aktuelle Projekte ausgibt, zu deren Projekt-Team der angemeldete Benutzer gehört. Der Bericht zeigt die folgenden Felder an: die Beschreibung, das geplante Abschlussdatum, das voraussichtliche Abschlussdatum, den Prozentsatz der Fertigstellung, den Status und die Priorität der Projekte.</td> 
  </tr> 
  <tr> 
   <td>Meine gesendeten Probleme</td> 
   <td>Ein Anfragebericht, der von der angemeldeten Person gesendete Probleme ausgibt, die in den letzten drei Monaten geschlossen wurden oder aktuell offen sind. Der Bericht zeigt die folgenden Felder an: Name der Source, Anfragetyp, Eingabedatum, Status und Priorität der Anfragen.</td> 
  </tr> 
  <tr> 
   <td>Meine Aufgaben</td> 
   <td>Ein Aufgabenbericht, der noch nicht abgeschlossene Aufgaben in aktuellen Projekten ausgibt, die dem angemeldeten Benutzer zugewiesen sind. Der Bericht zeigt die folgenden Felder an: die geplante Dauer, den Projektnamen, den primären Beauftragten, den geplanten Start, den geplanten Abschluss, den abgeschlossenen Prozentsatz und die Priorität der Aufgaben.</td> 
  </tr> 
  <tr> 
   <td>Meine Arbeitszeittabellen</td> 
   <td>Ein Arbeitszeittabellen-Bericht, der alle Arbeitszeittabellen des angemeldeten Benutzers ausgibt. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Name des Verantwortlichen, Gesamtstunden, Überstunden, Name der genehmigenden Person und Status der Arbeitszeittabellen.</td> 
  </tr> 
  <tr> 
   <td>Meine nicht zugewiesenen Probleme</td> 
   <td>Ein Problembericht, der offene Probleme ausgibt, die einem der Aufgabengebiete des angemeldeten Benutzers und nicht dem Benutzer zugewiesen sind. Der Bericht zeigt die folgenden Felder an: Name der Source, Anfragetyp, Eingabedatum, Status und Priorität der Anfragen.</td> 
  </tr> 
  <tr> 
   <td>Meine nicht zugewiesenen Aufgaben</td> 
   <td>Ein Aufgabenbericht, der noch nicht abgeschlossene Aufgaben ausgibt, die einem der Aufgabengebiete des angemeldeten Benutzers und nicht dem Benutzer zugewiesen sind. Der Bericht zeigt die folgenden Felder an: die geplante Dauer, den Projektnamen, den primären Beauftragten, das geplante Startdatum, das geplante Abschlussdatum, den abgeschlossenen Prozentsatz und die Priorität der Aufgaben.</td> 
  </tr> 
  <tr> 
   <td>Meine anstehenden Aufgaben</td> 
   <td>Ein Aufgabenbericht, der noch nicht abgeschlossene Aufgaben ausgibt, die in den nächsten zwei Wochen beginnen sollten und die unter „Aktuelle Projekte“ aufgeführt sowie dem angemeldeten Benutzer zugewiesen sind. Der Bericht zeigt die folgenden Felder an: den Projektnamen, das geplante Abschlussdatum, das voraussichtliche Abschlussdatum, den abgeschlossenen Prozentsatz und den Status der Aufgaben.</td> 
  </tr> 
  <tr> 
   <td>Offene Arbeitszeittabellen (aufgefordert)</td> 
   <td>Ein Arbeitszeittabellen-Bericht, der offene Arbeitszeittabellen ausgibt. Der Bericht zeigt die folgenden Felder an: Datumsbereich, Eigentümer, Gesamtstunden, Überstunden, Name der genehmigenden Person, Status der Arbeitszeittabellen. Der Bericht wird angezeigt durch: Startdatum der Arbeitszeittabelle, Enddatum der Arbeitszeittabelle, Name der genehmigenden Person für Arbeitszeittabelle und Benutzername.</td> 
  </tr> 
  <tr> 
   <td>Überbudgetiertes Projekt nach Portfolio</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und Istkosten der Projekte ausgibt. Der Bericht ist nach Portfolio-Namen gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Geplante Portfoliokosten nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und Istkosten der Projekte ausgibt. Der Bericht wird nach Portfolio-Name, gruppiert nach Programmname, angezeigt und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplante Portfoliokosten nach Projekt</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und Istkosten der Projekte ausgibt. Der Bericht wird nach Portfolio-Name, gruppiert nach Projektname, angezeigt und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplanter Portfolioumsatz nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Einnahmen und die tatsächlichen Einnahmen der Projekte ausgibt. Der Bericht wird nach Portfolio-Name, gruppiert nach Programmname, angezeigt und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplanter Portfolioumsatz nach Projekt</td> 
   <td>Ein Projektbericht, der die geplanten Einnahmen und die tatsächlichen Einnahmen der Projekte ausgibt. Der Bericht wird nach Portfolio-Name, gruppiert nach Projektname, angezeigt und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplante Kosten im Vgl. zu Istkosten nach Portfolio</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und Istkosten der Projekte nach Portfolio ausgibt. Der Bericht ist nach Portfolio-Name gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplante Kosten im Vgl. zu Istkosten nach Programm</td> 
   <td>Ein Projektbericht, der die geplanten Kosten und Istkosten der Projekte nach Programm ausgibt. Der Bericht ist nach Portfolio-Name gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplante Einnahmen im Vgl. zu tatsächlichen Einnahmen nach Portfolio</td> 
   <td>Ein Projektbericht, der die geplanten Einnahmen und die tatsächlichen Einnahmen der Projekte ausgibt. Der Bericht ist nach Portfolio-Name gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Geplante im Vgl. zu tatsächlichen Einnahmen je Programm</td> 
   <td>Ein Projektbericht, der die geplanten Einnahmen und die tatsächlichen Einnahmen der Projekte ausgibt. Der Bericht ist nach Programmnamen gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Nach Programm und Monat gruppierte Portfoliokosten</td> 
   <td>Ein Matrix-Projektbericht, der die geplanten Kosten, budgetierten Kosten und Istkosten der Projekte ausgibt. Der Bericht ist nach Portfolio-Name, Programmname und dem Monat des geplanten Startdatums der Projekte gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Portfolioprojekte nach Status gruppiert nach Programm</td> 
   <td>Ein Projektbericht, der den Status der Projekte ausgibt. Der Bericht ist nach Programmname und Projektstatus gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Nach Status und Portfolio gruppierte Portfolioprojekte</td> 
   <td>Ein Projektbericht, der den Portfolio-Namen und den Status der Projekte ausgibt. Der Bericht ist nach dem Portfolio-Namen und dem Projektstatus gruppiert und enthält eine Grafik.</td> 
  </tr> 
  <tr> 
   <td>Portfolioumsatz nach Programm</td> 
   <td>Ein Projektbericht, der den Portfolio-Namen, den Programmnamen, die geplanten Einnahmen und die tatsächlichen Einnahmen der Projekte ausgibt. Der Bericht ist nach dem Portfolio-Namen und dem Programmnamen gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Nach Programm und Monat gruppierte Portfolioeinnahmen</td> 
   <td>Ein Matrix-Projektbericht, der die geplanten Einnahmen, tatsächlichen Einnahmen, den Portfolio-Namen und den Programmnamen ausgibt. Der Bericht ist nach dem Portfolio-Namen, dem Programmnamen und dem Monat des geplanten Startdatums der Projekte gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektkosten und -einnahmen nach Aufgabenstatus</td> 
   <td>Ein Matrix-Aufgabenbericht, der die geplanten Kosten, Istkosten, den geplanten Umsatz, tatsächlichen Umsatz und den Projektnamen der Aufgaben ausgibt. Der Bericht ist nach Projektname und Status der Aufgaben gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektkosten im Vgl. zu Einnahmen je Portfolio</td> 
   <td>Ein Projektbericht, der den Portfolio-Namen, die Istkosten und den tatsächlichen Umsatz der Projekte ausgibt. Der Bericht ist nach Portfolio-Name gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Projektkosten nach Monat und Quartal</td> 
   <td>Ein Matrix-Ausgabenbericht, der das Eingabedatum, den geplanten Betrag, den tatsächlichen Betrag und das Projekt der Ausgaben ausgibt. Der Bericht ist nach Projektname, Quartal und Monat des Eingabedatums der Ausgaben gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektstundenkosten nach Stundentyp und Monat</td> 
   <td>Ein Matrix-Stundenbericht, der die folgenden Felder ausgibt: Stunden, Eingabedatum, Istkosten der Projekte, Stundentyp, Projektname. Der Bericht ist nach Projektname, Monat des Eingabedatums der Stunden und Stundentyp gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektlohnkosten und -ausgaben nach Monat und Quartal</td> 
   <td>Ein Matrix-Projektbericht, der die geplanten Lohnkosten, tatsächlichen Lohnkosten, geplanten Ausgaben und tatsächlichen Ausgaben der Projekte ausgibt. Der Bericht ist nach Projektname sowie Quartal und Monat des tatsächlichen Startdatums der Projekte gruppiert.</td> 
  </tr> 
  <tr> 
   <td>Projektleistung</td> 
   <td>Ein Projektbericht, der die folgenden Felder für aktuelle Projekte ausgibt: Fälligkeitsdatum, CPI, SPI, CSI, Geplante Kosten, Budget, EAC und Ausgaben der Projekte.</td> 
  </tr> 
  <tr> 
   <td>Projektanforderungen</td> 
   <td>Ein Projektbericht, der angeforderte Projekte ausgibt. Der Bericht zeigt die folgenden Felder an: die Beschreibung, das geplante Abschlussdatum, das voraussichtliche Abschlussdatum, den Prozentsatz der Fertigstellung, den Status und die Priorität der Projekte.</td> 
  </tr> 
  <tr> 
   <td>Projekte nach Bedingung</td> 
   <td>Ein Projektbericht, der den Zustand der Projekte ausgibt. Der Bericht ist nach Bedingung gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Projekte nach Bedingung und nach Gruppe</td> 
   <td>Ein Projektbericht, der den Verlaufsstatus und die Gruppe der Projekte ausgibt. Der Bericht ist nach Gruppenname und Fortschrittsstatus gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Projekte nach Priorität</td> 
   <td>Ein Projektbericht, der die Priorität von Projekten ausgibt. Der Bericht ist nach Priorität gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Projekte nach Fortschrittsstatus</td> 
   <td>Ein Projektbericht, der den Verlaufsstatus der Projekte ausgibt. Der Bericht ist nach Fortschrittsstatus gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Aufgaben nach Verlaufsstatus</td> 
   <td>Ein Aufgabenbericht, der den Fortschrittsstatus aller Aufgaben in aktuellen Projekten ausgibt. Der Bericht ist nach Fortschrittsstatus gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Aufgaben nach Status</td> 
   <td>Ein Aufgabenbericht, der den Status aller Aufgaben ausgibt. Der Bericht ist nach Status gruppiert und enthält ein Diagramm.</td> 
  </tr> 
  <tr> 
   <td>Zu überprüfende Arbeitszeittabellen</td> 
   <td>Ein Arbeitszeittabellen-Bericht, der eingereichte und abgelehnte Arbeitszeittabellen ausgibt, deren genehmigende Person der angemeldete Benutzer ist. Die Auswertung zeigt die folgenden Felder an: Datumsbereich, Eigentümer, Gesamtstunden, Überstunden, Name der genehmigenden Person und Status der Arbeitszeittabellen.</td> 
  </tr> 
  <tr> 
   <td>Gefährdete Aufgaben</td> 
   <td>Ein Aufgabenbericht, der noch nicht abgeschlossene Aufgaben mit dem Verlaufsstatus „In Verzug“ und einem Übergabedatum vor morgen ausgibt und bei dem der angemeldete Benutzer Teil des Projektteams des Projekts ist, an dem die Aufgaben ausgeführt werden. Der Bericht zeigt die folgenden Felder an: Geplante Dauer, Projektname, primärer Beauftragter, Geplanter Beginn, Geplanter Abschluss, Prozent abgeschlossen und Priorität der Aufgaben.</td> 
  </tr> 
  <tr> 
   <td>Benutzeranmeldungen</td> 
   <td>Ein Benutzerbericht, der die folgenden Felder ausgibt: die eindeutige ID, die Anzahl der Anmeldungen (die Häufigkeit, mit der sich Benutzende seit Beginn mit Workfront angemeldet haben), das letzte Anmeldedatum der Benutzenden. Der Bericht ist nach Zugriffsebene der Benutzer gruppiert.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Auf native Berichte zugreifen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Klicken Sie auf **Berichte**.
1. Klicken Sie **Alle Berichte**.
1. Erweitern Sie das **Filter**-Dropdown-Menü und wählen Sie **Neuer Filter**.

1. Klicken Sie **Filterregel hinzufügen**.
1. Beginnen Sie im Feld **Feldnamen eingeben** mit der Eingabe von **Globale ID**.

1. Wählen Sie unter dem **Report**-Objekt **Globale ID** aus.

1. Wählen Sie im Dropdown-Menü des Filtermodifikators die Option **Ist nicht leer**.\
   ![Globaler ID-Filter für Systemberichte](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Klicken Sie auf **Filter speichern**.\
   Die Berichtsliste zeigt nur integrierte Berichte an.\
   Weitere Informationen zu den verfügbaren integrierten Berichten finden Sie im Abschnitt [Übersicht über integrierte Berichte](#overview-of-built-in-reports) in diesem Artikel.
