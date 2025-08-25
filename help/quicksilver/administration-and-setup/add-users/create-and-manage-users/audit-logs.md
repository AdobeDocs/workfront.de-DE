---
title: Auditprotokolle
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator können Sie vom Benutzer in den letzten 90 Tagen im System ausgelöste Änderungen mithilfe von Auditprotokollen verfolgen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1523'
ht-degree: 3%

---

# Audit-Protokolle

<!--Audited: 01/2024-->

Als Adobe Workfront-Admin können Sie anhand der unten beschriebenen Auditprotokolle benutzerseitig ausgelöste Änderungen verfolgen, die in den letzten 90 Tagen im System ausgelöst wurden.

Anweisungen zum Anzeigen und Filtern der gewünschten Informationen in diesen Auditprotokollen finden Sie unter [Anzeigen und Exportieren von Auditprotokollen](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Informationen, die Sie in einem Auditprotokoll finden

Die folgenden Felder werden in jedem Auditprotokolleintrag aufgezeichnet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Datum und Uhrzeit</td> 
   <td>Wann die Aktion stattgefunden hat.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Protokolltyp</td> 
   <td>Typ des Auditprotokolls, z. B. Zugriffsebene oder benutzerdefiniertes Formular.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzername</td> 
   <td> <p>Name des Benutzers, der die Aktion ausgeführt hat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktion</td> 
   <td> Vom Benutzer durchgeführte Aktionen, z. B. Ändern, Erstellen und Löschen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objekt</td> 
   <td> Name des durch die Aktion betroffenen Objekts. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Details</td> 
   <td>Weitere Details zur Aktion. Bewegen Sie den Mauszeiger über den Text, um die vollständige Nachricht zu lesen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP-Adresse</td> 
   <td> <p>IP-Adresse des Benutzers, der die Aktion zum Zeitpunkt der Aktion ausgeführt hat.</p> <p>Die IP-Adresse ist für einige Systemaktionen nicht verfügbar.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prüfprotokolltypen und die Aktionen, durch die sie Trigger werden

* [Zugriffsebene](#access-level)
* [Geschäftsregeln](#business-rules)
* [Firma](#company)
* [Bedingung](#condition)
* [Benutzerdefiniertes Feld](#custom-field)
* [Benutzerdefiniertes Formular](#custom-forms)
* [Benutzerdefinierter Abschnitt](#custom-section)
* [Wechselkurs](#exchange-rate)
* [Gruppe](#group)
* [Aufgabengebiete](#job-roles)
* [Anmeldeversuch](#login-attempt)
* [Priorität](#priority)
* [Projektvoreinstellung](#project-preference)
* [Schweregrad](#severity)
* [Status](#status)
* [Voreinstellungen für Aufgaben und Probleme](#tasks-issues-preferences)
* [Benutzerin bzw. Benutzer](#user)

### Zugriffsebene {#access-level}

Das System generiert einen Zugriffsebenen-Protokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Zugriffsebene
* Löscht eine Zugriffsebene
* Ändert eine Zugriffsebene:

   * Ändert den Lizenztyp
   * Ändert Berechtigungen für Projekte, Aufgaben, Probleme, Portfolios, Programme, Berichte, Dokumente, Benutzer oder Vorlagen

     >[!NOTE]
     >
     >Das System zeichnet keine Berechtigungsänderungen an Finanzdaten oder innerhalb der folgenden Zugriffstypen auf: Anzeigen und Bearbeiten.
     >
     >Wenn beispielsweise ein(e) Benutzende(r) den Zugriffstyp Planer von Ansicht in Bearbeiten ändert, zeigt das System keine Informationen an, die im Dropdown-Menü Einstellungen optimieren enthalten sind.

### Geschäftsregeln

Geschäftsregeln sind nur für Kunden verfügbar, die einen Ultimate Workfront-Plan erworben haben. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Geschäftsregeln](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

Das System generiert einen Eintrag im Auditprotokoll für Geschäftsregeln, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Geschäftsregel
* Bearbeitet eine Geschäftsregel:

   * Benennt sie um
   * Fügt Ausdrücke hinzu oder entfernt sie
   * Ändert einen Trigger

* Löscht eine Geschäftsregel

### Firma {#company}

Das System generiert einen Eintrag im Administratorprotokoll eines Unternehmens, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Firma
* Ändert eine Firma:

   * Benennt sie um
   * Fügt Mitglieder hinzu oder entfernt sie
   * Fügt den Wert im Gruppenfeld hinzu, bearbeitet oder löscht ihn.
   * Fügt einen Firmen-Abrechnungssatz für ein Aufgabengebiet hinzu oder bearbeitet ihn.
   * Entfernt einen Abrechnungssatz des Unternehmens für ein Aufgabengebiet
   * Legt sie als primäre Firma für die Organisation fest
   * Hängt ein benutzerdefiniertes Formular an oder entfernt es

* Löscht eine Firma

Weitere Informationen zu Status finden Sie unter [Status - Übersicht](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Bedingung {#condition}

Das System generiert einen Eintrag im Protokoll „Conditioncodeverwaltung“, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Bedingung
* Ändert eine Bedingung:

   * Ändert den Namen
   * Ändert die Farbe
   * Legt sie als Standard fest
   * Ändert oder entfernt die Beschreibung der Bedingung
   * Blendet die Bedingung aus oder ein

* Löscht eine Bedingung

Weitere Informationen zum Konfigurieren von Aufgabengebieten finden Sie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Benutzerdefiniertes Feld {#custom-field}

Das System generiert einen Audit-Protokolleintrag für ein benutzerdefiniertes Feld, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt ein benutzerdefiniertes Feld
* Ändert ein benutzerdefiniertes Feld:

   * Ändert den Namen, die Beschriftung, die Anweisungen oder das Format
   * Ändert den Anzeigetyp

     Dies ist nur verfügbar, wenn es sich bei dem Feld um einen der folgenden Typen handelt: Einzelzeile, Absatz, Dropdown, Kontrollkästchen, Optionsfeld

   * Ändert die Feldgröße

     Dies ist nur verfügbar, wenn es sich bei dem Feld um einen der folgenden Typen handelt: Einzelzeile, Absatz, Text mit Formatierung

   * Fügt Auswahlfelder hinzu, entfernt sie oder blendet sie aus
   * Bearbeitet eine Feldauswahl für Beschriftung oder Wert
   * Konfiguriert die Feldauswahl, die standardmäßig ausgewählt oder nicht ausgewählt werden soll
   * Konfiguriert ein Dropdown-Feld, um mehrere Auswahlmöglichkeiten oder eine einzelne Auswahl zuzulassen.
   * Konfiguriert ein Datumsfeld, in dem die Tageszeit angezeigt oder nicht angezeigt wird
   * Bearbeitet den Hyperlink oder ändert den Wert in einem beschreibenden Textfeld

* Löscht ein benutzerdefiniertes Feld
* Gibt ein benutzerdefiniertes Feld frei

### Benutzerdefiniertes Formular {#custom-form}

Das System generiert einen benutzerdefinierten Forms-Administratorprotokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt ein benutzerdefiniertes Formular
* Ändert ein benutzerdefiniertes Formular:

   * Ändert den Namen oder die Beschreibung
   * Aktiviert oder deaktiviert ist aktiv
   * Fügt ein Feld oder einen Abschnitt hinzu oder entfernt es.
   * Für einen benutzerdefinierten Abschnitt ändert eine Einstellung unter „Zusätzliche Einstellungen“
   * Ändert ein Feld in „erforderlich“ oder „nicht erforderlich“
   * Ändert eine Berechnung in einem benutzerdefinierten Feld
   * Blendet die Formel aus oder ein, die einem berechneten Feld im Hover-Text der Anweisungen zugeordnet ist
   * Aktiviert oder deaktiviert vorherige Berechnungen aktualisieren
   * Fügt Logik zum Überspringen oder Anzeigelogik hinzu oder ändert diese

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Löscht ein benutzerdefiniertes Formular
* Freigeben eines benutzerdefinierten Formulars

### Benutzerdefinierter Abschnitt {#custom-section}

Das System generiert einen Eintrag im Administratorprotokoll für einen benutzerdefinierten Abschnitt, wenn ein Benutzer eine der folgenden Aktionen in einem benutzerdefinierten Formular ausführt:

* Erstellt einen benutzerdefinierten Abschnitt
* Ändert den Namen oder die Beschreibung eines benutzerdefinierten Abschnitts
* Löscht einen benutzerdefinierten Abschnitt

Informationen zu benutzerdefinierten Abschnitten in benutzerdefinierten Formularen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Wechselkurs {#exchange-rate}

Das System generiert einen Wechselkurs-Auditprotokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt einen Wechselkurs
* Wechselkursänderungen:

   * Fügt eine Währung hinzu
   * Ändert den Kurs der Währung
   * Legt die Währung als Basiswährung (Standard) für alle Projekte und Berichte im System fest

* Löscht einen Wechselkurs

Weitere Informationen zum Konfigurieren von Wechselkursen finden Sie unter [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Gruppe {#group}

Das System generiert einen Eintrag im Administratorprotokoll für eine Gruppe, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Gruppe
* Löscht eine Gruppe
* Ändert eine Gruppe:

   * Fügt Benutzer hinzu oder entfernt sie
   * Fügt Untergruppen hinzu oder entfernt sie

### Aufgabengebiete {#job-roles}

Das System generiert einen Eintrag im Administratorprotokoll für Aufgabengebiete, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt ein Aufgabengebiet
* Ändert ein Aufgabengebiet:

   * Ändert den Namen
   * Fügt die Beschreibung hinzu, ändert sie oder entfernt sie
   * Fügt die Kosten pro Stunde (Kosten/Stunde) hinzu, ändert sie oder entfernt sie.
   * Fügt den Abrechnungssatz (Rechnung/Std.) hinzu, ändert ihn oder entfernt ihn.

* Löscht ein Aufgabengebiet

Weitere Informationen zum Konfigurieren von Aufgabengebieten finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Anmeldeversuch {#login-attempt}

Das System generiert einen Prüfprotokolleintrag für den Anmeldeversuch, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Anmelden, Abmelden oder Fehlschlagen eines Anmeldeversuchs in Workfront (im Browser und in der Mobile App)
* Meldet sich bei einer Workfront-Integration (z. B. Workfront für Slack) an, meldet sich ab oder schlägt einen Anmeldeversuch fehl
* Anmelden bei oder Abmelden von der Workfront-API

Wenn ein Workfront-Administrator die Funktion „Anmelden als“ verwendet, werden keine Anmeldeversuche aufgezeichnet.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn Ihr Unternehmen in die Adobe Admin Console integriert wurde. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

### Priorität {#priority}

Das System generiert einen Eintrag im Auditprotokoll „Priorität“, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Priorität
* Ändert eine Priorität:

   * Ändert den Namen
   * Ändert die Farbe
   * Legt sie als Standard fest
   * Fügt die Beschreibung der Priorität hinzu, ändert sie oder entfernt sie
   * Blendet die Priorität aus oder ein

* Löscht eine Priorität

Weitere Informationen zum Konfigurieren von Prioritäten finden Sie unter [Erstellen und Anpassen von Prioritäten](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Projektpräferenz {#project-preference}

Das System generiert einen Projektvoreinstellungs-Auditprotokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt ein benutzerdefiniertes Quartal
* Ändert eine Projektvoreinstellung:

   * Sperrt oder entsperrt sie
   * Ändert eine der Einstellungen
   * Aktiviert, deaktiviert oder bearbeitet es
   * Bearbeitet eine Zeitleistenberechnung

* Löscht ein benutzerdefiniertes Quartal

Weitere Informationen zu Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Schweregrad {#severity}

Das System generiert einen Protokolleintrag für den Schweregrad , wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt einen Problemschweregrad
* Ändert einen Problemschweregrad:

   * Ändert den Namen
   * Ändert die Farbe
   * Legt sie als Standard fest
   * Ändert oder entfernt die Beschreibung des Schweregrads.
   * Blendet den Schweregrad aus oder ein

* Löscht einen Problemschweregrad

Weitere Informationen zum Konfigurieren von Aufgabengebieten finden Sie unter [Erstellen oder Anpassen von Problemschweregraden](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Status {#status}

Das System generiert einen Status-Audit-Protokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt einen Status auf System- oder Gruppenebene
* Ändert einen Status auf System- oder Gruppenebene:

   * Benennt sie um
   * Legt den Status als Standard fest
   * Sperrt oder entsperrt sie
   * Blendet es aus oder ein
   * Ändert die Farbe oder Beschreibung

* Löscht einen Status auf System- oder Gruppenebene

Weitere Informationen zu Status finden Sie unter [Status - Übersicht](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Voreinstellungen für Aufgaben und Probleme {#tasks-issues-preferences}

Das System generiert einen Auditprotokolleintrag mit Einstellungen für Aufgaben und Probleme , wenn ein(e) Benutzende(r) eine Voreinstellung für Aufgaben und Probleme auf eine der folgenden Arten ändert:

* Sperrt oder entsperrt eine Voreinstellung
* Ändert die Einstellung für eine Voreinstellung
* Ändern der Zugriffseinstellung für Aufgaben, Probleme oder Anfragen

Weitere Informationen zu den Voreinstellungen für Aufgaben und Probleme finden Sie unter [Systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Benutzerin bzw. Benutzer {#user}

Das System generiert einen Benutzerüberwachungsprotokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt einen Benutzer

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Dies ist nicht verfügbar, wenn Ihr Unternehmen in die Adobe Admin Console integriert wurde. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

* Löscht einen Benutzer
* Ändert Zugriffsebene, Unternehmen, Team oder Gruppe eines Benutzers
* Aktiviert einen Benutzer
* Deaktiviert einen Benutzer
