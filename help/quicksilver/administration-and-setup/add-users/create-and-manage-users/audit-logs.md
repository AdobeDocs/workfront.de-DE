---
title: Auditprotokolle
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Als Adobe Workfront-Administrator können Sie mithilfe von Auditprotokollen Benutzeränderungen verfolgen, die in den letzten 90 Tagen im System ausgelöst wurden.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 3%

---

# Audit-Protokolle

<!--Audited: 01/2024-->

Als Adobe Workfront-Administrator können Sie mithilfe der unten beschriebenen Prüfprotokolle Benutzeränderungen verfolgen, die in den letzten 90 Tagen im System ausgelöst wurden.

Anweisungen zum Anzeigen und Filtern des gewünschten Inhalts in diesen Prüfprotokollen finden Sie unter [Prüfprotokolle anzeigen und exportieren](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Informationen, die Sie in einem Auditprotokoll finden

Die folgenden Felder werden in jedem Auditprotokolleintrag aufgezeichnet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Datum und Uhrzeit</td> 
   <td>Zeitpunkt der Aktion.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Protokolltyp</td> 
   <td>Typ des Auditprotokolls, z. B. Zugriffsebene oder Benutzerdefiniertes Formular.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzername</td> 
   <td> <p>Name des Benutzers, der die Aktion ausgeführt hat.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktion</td> 
   <td> Vom Benutzer ausgeführte Aktionen wie Ändern, Erstellen und Löschen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objekt</td> 
   <td> Name des betroffenen Objekts aufgrund der Aktion. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Details</td> 
   <td>Zusätzliche Details zur Aktion. Bewegen Sie den Mauszeiger über den Text, um die vollständige Nachricht zu lesen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP-Adresse</td> 
   <td> <p>IP-Adresse des Benutzers, der die Aktion zum Zeitpunkt der Aktion ausgeführt hat.</p> <p>Die IP-Adresse ist für einige Systemaktionen nicht verfügbar.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Auditprotokolltypen und die sie Trigger Aktionen

* [Zugriffsebene](#access-level)
* [Verfahrensregeln](#business-rules)
* [Firma](#company)
* [Bedingung](#condition)
* [Benutzerdefiniertes Feld](#custom-field)
* [Benutzerdefiniertes Formular](#custom-forms)
* [Benutzerdefinierter Abschnitt](#custom-section)
* [Wechselkurs](#exchange-rate)
* [Gruppe](#group)
* [Vorgangsrollen](#job-roles)
* [Anmeldeversuch](#login-attempt)
* [Priorität](#priority)
* [Projektreferenz](#project-preference)
* [Schweregrad](#severity)
* [Status](#status)
* [Voreinstellungen für Aufgaben und Probleme](#tasks-issues-preferences)
* [Benutzerin oder Benutzer](#user)

### Zugriffsebene {#access-level}

Das System generiert einen Protokolleintrag auf Zugriffsstufe, wenn ein Benutzer einen der folgenden Schritte ausführt:

* Erstellt eine Zugriffsebene
* Löscht eine Zugriffsebene
* Ändert eine Zugriffsebene:

   * Ändern des Lizenztyps
   * Ändert Berechtigungen für Projekte, Aufgaben, Probleme, Portfolios, Programme, Berichte, Dokumente, Benutzer oder Vorlagen

     >[!NOTE]
     >
     >Das System zeichnet keine Berechtigungsänderungen an Finanzdaten oder den folgenden Zugriffstypen auf: Anzeigen und Bearbeiten.
     >
     >Wenn ein Benutzer beispielsweise den Zugriffstyp Planer von Ansicht zu Bearbeiten ändert, zeigt das System keine Informationen an, die im Dropdown-Menü Einstellungen anpassen enthalten sind.

### Verfahrensregeln

Geschäftsregeln sind nur für Kunden verfügbar, die einen Ultimate Workfront Plan erworben haben. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Geschäftsregeln](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

Das System generiert einen Audit-Protokolleintrag für Geschäftsregeln, wenn ein Benutzer einen der folgenden Schritte ausführt:

* Erstellt eine Geschäftsregel
* Bearbeiten von Geschäftsregeln:

   * Benennt ihn um
   * Fügt Ausdrücke hinzu oder entfernt diese
   * Ändert einen Trigger

* Löscht eine Geschäftsregel

### Firma {#company}

Das System generiert einen Eintrag für das Unternehmensprüfungsprotokoll, wenn ein Benutzer einen der folgenden Schritte ausführt:

* Erstellen eines Unternehmens
* Unternehmen ändern:

   * Benennt ihn um
   * Fügt Mitglieder hinzu oder entfernt Mitglieder
   * Fügt den Wert im Feld Gruppe hinzu, bearbeitet ihn oder löscht ihn
   * Fügt eine Abrechnungsrate für eine Stellenrolle im Unternehmen hinzu oder bearbeitet sie
   * Entfernt eine Abrechnungsrate für eine Jobrolle im Unternehmen
   * Legt es als Hauptunternehmen für die Organisation fest
   * Hängt ein benutzerdefiniertes Formular an oder entfernt es

* Löscht ein Unternehmen

Weitere Informationen zu Statusangaben finden Sie unter [Statusübersicht](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Bedingung {#condition}

Das System generiert einen Bedingungsprüfungsprotokolleintrag, wenn ein Benutzer einen der folgenden Schritte ausführt:

* Erstellt eine Bedingung
* Ändert eine Bedingung:

   * Ändert den Namen
   * Ändert die Farbe
   * Legt es als Standard fest
   * Ändert oder entfernt die Beschreibung der Bedingung
   * Blendet die Bedingung aus oder zeigt sie an

* Löscht eine Bedingung

Weitere Informationen zum Konfigurieren von Auftragsrollen finden Sie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Benutzerdefiniertes Feld {#custom-field}

Das System generiert einen Eintrag des Prüfprotokolls &quot;Benutzerdefiniertes Feld&quot;, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt ein benutzerdefiniertes Feld
* Ändert ein benutzerdefiniertes Feld:

   * Ändert den Namen, den Titel, die Anweisungen oder das Format
   * Ändert den Anzeigetyp

     Dies ist nur verfügbar, wenn das Feld einer der folgenden Typen ist: einzelne Zeile, Absatz, Dropdown, Kontrollkästchen, Optionsfeld

   * Ändern der Feldgröße

     Dies ist nur verfügbar, wenn das Feld einer der folgenden Typen ist: einzelne Zeile, Absatz, Text mit Formatierung

   * Fügt eine Feldauswahl hinzu, entfernt sie oder blendet sie aus
   * Bearbeiten einer Feldauswahlbeschriftung oder eines Feldwerts
   * Konfiguriert die auszuwählende oder nicht standardmäßig ausgewählte Feldauswahl
   * Konfiguriert ein Dropdown-Feld, um mehrere Auswahlen oder nur eine Auswahl zuzulassen
   * Konfiguriert ein Datumsfeld zur Anzeige oder Nichtanzeige der Tageszeit
   * Bearbeiten des Hyperlinks oder Ändern des Werts in einem beschreibenden Textfeld

* Löscht ein benutzerdefiniertes Feld
* Freigeben eines benutzerdefinierten Felds

### Benutzerdefiniertes Formular {#custom-form}

Das System generiert einen benutzerdefinierten Forms-Auditprotokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt ein benutzerdefiniertes Formular
* Ändert das benutzerdefinierte Formular:

   * Ändert Namen oder Beschreibung
   * Aktiviert oder deaktiviert Ist aktiv
   * Fügt ein Feld oder einen Abschnitt hinzu oder entfernt es
   * Für einen benutzerdefinierten Abschnitt ändert eine Einstellung unter &quot;Zusätzliche Einstellungen&quot;.
   * Ändern eines Felds in &quot;Erforderlich&quot;oder &quot;Nicht erforderlich&quot;
   * Änderung einer Berechnung in einem benutzerdefinierten Feld
   * Blendet die mit einem berechneten Feld verknüpfte Formel im Text Anweisungen aus oder zeigt sie an.
   * Aktiviert bzw. deaktiviert die Option Vorherige Berechnungen aktualisieren
   * Fügt eine Logik zum Überspringen oder Ändern der Anzeigelogik hinzu

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Löscht ein benutzerdefiniertes Formular
* Teilt ein benutzerdefiniertes Formular

### Benutzerdefinierter Abschnitt {#custom-section}

Das System generiert einen Auditprotokolleintrag für benutzerdefinierte Abschnitte, wenn ein Benutzer eine der folgenden Aktionen in einem benutzerdefinierten Formular ausführt:

* Erstellt einen benutzerdefinierten Abschnitt
* Ändert den Namen oder die Beschreibung eines benutzerdefinierten Abschnitts
* Löscht einen benutzerdefinierten Abschnitt

Weitere Informationen zu benutzerdefinierten Abschnitten in benutzerdefinierten Formularen finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Wechselkurs {#exchange-rate}

Das System generiert einen Auditprotokolleintrag zum Wechselkurs, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt einen Wechselkurs
* Ändert einen Wechselkurs:

   * Eine Währung hinzufügt
   * Ändert den Wechselkurs für die Währung
   * Legt die Währung als Basiswährung (Standard) für alle Projekte und Berichte im System fest

* Löscht den Wechselkurs

Weitere Informationen zur Konfiguration von Wechselkursen finden Sie unter [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Gruppe {#group}

Das System generiert einen Eintrag für das Gruppenprüfungsprotokoll, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Gruppe
* Löscht eine Gruppe
* Ändert eine Gruppe:

   * Fügt Benutzer hinzu oder entfernt diese
   * Fügt Untergruppen hinzu oder entfernt sie

### Aufgabengebiete {#job-roles}

Das System generiert einen Auditprotokolleintrag &quot;Auftragsrollen&quot;, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Stellenrolle
* Ändert eine Stellenrolle:

   * Ändert den Namen
   * Fügt die Beschreibung hinzu, ändert sie oder entfernt sie
   * Fügt die Kosten pro Stunde hinzu, ändert sie oder entfernt sie (Kosten/Stunden).
   * Fügt den Abrechnungskurs hinzu, ändert ihn oder entfernt ihn (Rechnungsbetrag/Std.)

* Löscht die Auftragsrolle

Weitere Informationen zum Konfigurieren von Auftragsrollen finden Sie unter [Erstellen und Verwalten von Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Anmeldeversuch {#login-attempt}

Das System generiert einen Auditprotokolleintrag für den Anmeldeversuch, wenn ein Benutzer einen der folgenden Schritte ausführt:

* Anmelden, Abmelden oder Fehler bei einem Anmeldeversuch in Workfront (in einem Browser und in der App)
* Anmeldung, Abmeldung oder Fehler bei einem Anmeldeversuch bei einer Workfront-Integration (z. B. Workfront für Slack und Workfront für Salesforce)
* Anmelden oder Abmelden von der Workfront-API

Die Protokolle für Anmeldeversuche werden nicht aufgezeichnet, wenn ein Workfront-Administrator die Funktion Anmelden als verwendet.

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

### Priorität {#priority}

Das System generiert einen Auditprotokolleintrag &quot;Priorität&quot;, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt eine Priorität
* Ändert eine Priorität:

   * Ändert den Namen
   * Ändert die Farbe
   * Legt es als Standard fest
   * Fügt die Beschreibung der Priorität hinzu, ändert sie oder entfernt sie
   * Blendet die Priorität ein oder aus

* Löscht eine Priorität

Weitere Informationen zum Konfigurieren von Prioritäten finden Sie unter [Erstellen und Anpassen von Prioritäten](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Projektpräferenz {#project-preference}

Das System generiert einen Auditprotokolleintrag &quot;Projektvoreinstellungen&quot;, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt ein benutzerdefiniertes Quartal
* Ändert eine Projektvoreinstellung:

   * Sperrt oder entsperrt sie
   * Ändert eine der Einstellungen
   * Aktiviert, deaktiviert oder bearbeitet sie
   * Bearbeiten einer Timeline-Berechnung

* Löscht ein benutzerdefiniertes Quartal

Weitere Informationen zu den Projektanvoreinstellungen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Schweregrad {#severity}

Das System generiert einen Eintrag des Schweregrad-Prüfprotokolls, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt einen Schweregrad eines Problems
* Ändert den Schweregrad eines Problems:

   * Ändert den Namen
   * Ändert die Farbe
   * Legt es als Standard fest
   * Ändert oder entfernt die Beschreibung des Schweregrads
   * Blendet den Schweregrad aus oder zeigt ihn an

* Löscht einen Schweregrad eines Problems

Weitere Informationen zum Konfigurieren von Auftragsrollen finden Sie unter [Erstellen oder Anpassen von Problemabständen](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Status {#status}

Das System generiert einen Status-Auditprotokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Erstellt einen Status auf System- oder Gruppenebene
* Ändert einen Status auf System- oder Gruppenebene:

   * Benennt ihn um
   * Macht es zum Standardstatus
   * Sperrt oder entsperrt sie
   * Blendet es aus oder blendet es ein
   * Ändert die Farbe oder Beschreibung

* Löscht einen Status auf System- oder Gruppenebene

Weitere Informationen zu Statusangaben finden Sie unter [Statusübersicht](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Voreinstellungen für Aufgaben und Probleme {#tasks-issues-preferences}

Das System generiert einen Auditprotokolleintrag &quot;Aufgaben und Probleme - Voreinstellungen&quot;, wenn ein Benutzer eine der folgenden Arten ändert:

* Sperrt oder entsperrt eine Voreinstellung
* Ändert die Einstellung für eine Voreinstellung
* Ändern von Zugriffseinstellungen für Aufgaben, Probleme oder Anforderungen

Weitere Informationen zu den Voreinstellungen für Aufgaben und Probleme finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Benutzerin oder Benutzer {#user}

Das System generiert einen Benutzerprüfungsprotokolleintrag, wenn ein Benutzer eine der folgenden Aktionen ausführt:

* Benutzer erstellen

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Dies ist nicht verfügbar, wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

* Löscht einen Benutzer
* Ändern der Zugriffsebene, des Unternehmens, des Teams oder der Gruppe eines Benutzers
* Aktiviert einen Benutzer
* Deaktiviert einen Benutzer
