---
product-area: documents
navigation-topic: approvals
title: Dashboard für Überprüfung und Genehmigung erstellen
description: Sie können Genehmigungsmetriken in Leinwand-Dashboards überprüfen.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
exl-id: 48f8605b-c342-493b-96e7-f73248e34b35
source-git-commit: 6abe9f371d8121ccbd66a379ad4b25f47417d885
workflow-type: tm+mt
source-wordcount: '1991'
ht-degree: 1%

---

# Erstellen eines Berichts-Dashboards zur Überprüfung und Genehmigung

Sie können ein Berichts-Dashboard im Bereich Arbeitsfläche-Dashboards erstellen, um sowohl allgemeine als auch detaillierte Informationen zu Überprüfungen und Genehmigungen mit der neuen Dokumentgenehmigungsfunktion anzuzeigen.

>[!IMPORTANT]
>
>Diese Funktion ist nur für Kunden verfügbar, die den neuen Dokumentgenehmigungsdienst verwenden und sich in der Beta-Version der Canvas-Dashboards anmelden.


![Beispiel-Dashboard](assets/whole-dashboard.png)

## Dashboard erstellen

{{step1-to-dashboards}}

1. Klicken Sie im linken Bereich auf **Arbeitsfläche-Dashboards**.
1. Klicken Sie auf **Neues Dashboard**.
1. Benennen Sie Ihr Dashboard.
1. (Optional) Fügen Sie eine Beschreibung hinzu.
1. Klicken Sie auf **Erstellen**.
   ![Dashboard-Namen und -Beschreibung hinzufügen](assets/create-a-dashboard.png)

Nachdem Sie ein Dashboard erstellt haben, können Sie mit dem Hinzufügen von KPIs, Diagrammen und Tabellen beginnen. Weitere Informationen finden Sie in den folgenden Abschnitten:

* [Hinzufügen allgemeiner Überprüfungs- und Genehmigungsinformationen mit KPIs und Diagrammen](#add-high-level-review-and-approval-information-with-kpis-and-charts)
* [Hinzufügen detaillierter Überprüfungs- und Genehmigungsinformationen mit Tabellen](#add-detailed-review-and-approval-information-with-tables)

## Hinzufügen allgemeiner Überprüfungs- und Genehmigungsinformationen mit KPIs und Diagrammen

Sie können allgemeine Informationen zu Dokumentgenehmigungen mit KPIs und Diagrammen anzeigen. Drilldown-Informationen sind derzeit nicht in der Beta-Version verfügbar.

### KPIs

<!--
>>[!IMPORTANT]
>
>New document approvals data currently refreshes during the evenings in the US Mountain timezone. Real-time updates are planned and coming soon.-->

![KPI-Beispiele](assets/kpi-dashboard.png)

#### Ausstehende Genehmigungen

1. [Erstellen Sie ein Dashboard](#create-a-dashboard), wie im Abschnitt oben beschrieben.
1. Klicken Sie auf der Karte **KPI** auf **Hinzufügen**.
1. Geben Sie _Ausstehend_ in das Textfeld **KPI-Titel** ein.
1. Geben Sie _Ausstehende Genehmigungen_ in das Textfeld **KPI-Beschriftung** ein. In diesem Text wird beschrieben, was die KPI anzeigt.
1. Klicken Sie oben auf der Seite auf **KPI-Feld auswählen**.
1. Scrollen Sie nach unten und suchen Sie den Ordner **Dokumentgenehmigung**.
1. Wählen Sie **Status** und dann **Zählung** aus dem Dropdown-Menü.
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**.
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Belassen Sie den Operator als **Equal** und geben Sie im Textfeld _pending review_ ein.
      Beispiel für ![ausstehenden kpi-Filter](assets/pending-kpi-filter.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .


#### Überfällige Genehmigungen

1. [Erstellen Sie ein Dashboard](#create-a-dashboard), wie im Abschnitt oben beschrieben.
1. Klicken Sie auf der Karte **KPI** auf **Hinzufügen**.
1. Geben Sie _Overdue_ in das Textfeld **KPI Title** ein.
1. Geben Sie in das Textfeld **KPI-Beschriftung** in den letzten _die Zeile_ Validierungsstaging-Frist ein. In diesem Text wird beschrieben, was die KPI anzeigt.
1. Klicken Sie oben auf der Seite auf **KPI-Feld auswählen**.
1. Scrollen Sie nach unten und suchen Sie den Ordner **Dokumentgenehmigung**.
1. Wählen Sie **Status** und dann **Zählung** aus dem Dropdown-Menü.
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Deadline** aus.
   1. Ändern Sie den Operator in &quot;**Kleiner als**&quot;, schalten Sie &quot;Relatives Datum ein&quot;um und geben Sie dann &quot;_$$TODAY_&quot;in das Textfeld ein.
      Beispiel für einen überfälligen kpi-Filter ![](assets/overdue-kpi-filter.png)
1. Klicken Sie auf **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in &quot;**Not Contains**&quot;, und geben Sie dann &quot;_authorised_&quot;in das Textfeld ein.
      ![Beispiel für überfällige KPI-Filter 2](assets/overdue-kpi-filter-2.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .


#### Abgeschlossene Genehmigungen

1. [Erstellen Sie ein Dashboard](#create-a-dashboard), wie im Abschnitt oben beschrieben.
1. Klicken Sie auf der Karte **KPI** auf **Hinzufügen**.
1. Geben Sie _Abgeschlossen_ in das Textfeld **KPI-Titel** ein.
1. Geben Sie _Genehmigungsstatusanzahl_ in das Textfeld **KPI-Beschriftung** ein. In diesem Text wird beschrieben, was die KPI anzeigt.
1. Klicken Sie oben auf der Seite auf **KPI-Feld auswählen**.
1. Scrollen Sie nach unten und suchen Sie den Ordner **Dokumentgenehmigung**.
1. Wählen Sie **Status** und dann **Zählung** aus dem Dropdown-Menü.
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in **Enthält** und geben Sie im Textfeld _genehmigt_ ein.
      Beispiel für einen ![abgeschlossenen kpi-Filter](assets/completed-kpi-filter.png)
1. Klicken Sie auf **Bedingung hinzufügen**:
   1. Klicken Sie auf **und** , um es in **oder** zu ändern.
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in **Entspricht** und geben Sie dann im Textfeld _geprüft_ ein.
      Beispiel für einen ![abgeschlossenen kpi-Filter](assets/completed-kpi-filter-2.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .

#### Veraltete Genehmigungen

1. [Erstellen Sie ein Dashboard](#create-a-dashboard), wie im Abschnitt oben beschrieben.
1. Klicken Sie auf der Karte **KPI** auf **Hinzufügen**.
1. Geben Sie _Abgebrochen_ in das Textfeld **KPI-Titel** ein.
1. Geben Sie im Textfeld **KPI-Beschriftung** die _Validierungs-Deadline für einen Zeitraum von 2 Wochen nach_ ein. In diesem Text wird beschrieben, was die KPI anzeigt.
1. Klicken Sie oben auf der Seite auf **KPI-Feld auswählen**.
1. Scrollen Sie nach unten und suchen Sie den Ordner **Staging der Dokumentgenehmigung**.
1. Wählen Sie **Deadline** und dann **Count** aus dem Dropdown-Menü.
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in &quot;**Not Contains**&quot;, und geben Sie im Textfeld _authorised_ ein.
      Beispiel für einen abgebrochenen KPI-Filter ](assets/abandoned-kpi-filter.png)![
1. Klicken Sie auf **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Deadline** aus.
   1. Ändern Sie den Operator in &quot;**Kleiner als**&quot;, schalten Sie dann Relatives Datum ein und geben Sie dann &quot;_$$TODAY-2w_&quot;in das Textfeld ein.
      Beispiel für einen abgebrochenen KPI-Filter ](assets/abandoned-kpi-filter-2.png)![
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .

### Diagramme

![Diagrammbeispiele](assets/chart-dashboard.png)

#### Validierungen nach Entscheidungstraktdiagramm

1. [Erstellen Sie ein Dashboard](#create-a-dashboard), wie im Abschnitt oben beschrieben.
1. Klicken Sie auf der Karte **Diagramm** auf **Hinzufügen**.
1. Geben Sie _Genehmigungen nach Entscheidung_ in das Textfeld **Name** ein.
1. (Optional) Geben Sie eine Beschreibung in das Textfeld **Beschreibung** ein. Dieser Text wird als QuickInfo neben dem Diagrammnamen angezeigt.
1. Klicken Sie auf **Diagrammdetails öffnen**.
1. Lassen Sie im Dropdownmenü **Diagrammtyp** die Option **Balkendiagramm** ausgewählt.
1. Lassen Sie im Dropdown-Menü **Balkentyp** die Option **Einfach** aktiviert.
1. Klicken Sie auf **Feld aktualisieren** für die Achse **Unten (X)** und wählen Sie den ersten Ordner **Dokumentgenehmigung** und dann den Ordner **Status** aus.
1. Stellen Sie den Aggregationstyp auf **Zählung** ein.
1. Klicken Sie auf **Feld aktualisieren** für die Achse **Links (Y)** und wählen Sie die erste Option **Dokumentgenehmigung** und dann die Option **Status** aus.
1. Klicken Sie auf das Symbol für die Registerkarte Filter ![Filter-Registerkarte](assets/filter-tab.png).
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Dokumentversion-Version** aus.
   1. Ändern Sie den Operator in **Is Not Null**.
      ![Filterbeispiel](assets/approvals-by-decision-chart-filter.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .


#### Balkendiagramm der Revisionsleiste

1. [Erstellen Sie ein Dashboard](#create-a-dashboard), wie im Abschnitt oben beschrieben.
1. Klicken Sie auf der Karte **Diagramm** auf **Hinzufügen**.
1. Geben Sie _Revisions_ in das Textfeld **Name** ein.
1. Geben Sie _Anzahl der Revisionen für Dokumente mit unvollständigen Entscheidungen, die vor Ende dieses Monats geplant sind, in das Textfeld **Beschreibung**ein._ Dieser Text wird als QuickInfo neben dem Diagrammnamen angezeigt.
1. Klicken Sie auf **Diagrammdetails öffnen**.
1. Lassen Sie im Dropdownmenü **Diagrammtyp** die Option **Balkendiagramm** ausgewählt.
1. Lassen Sie im Dropdown-Menü **Balkentyp** die Option **Einfach** aktiviert.
1. Klicken Sie auf **Feld aktualisieren** für die Achse **Unten (X)** und wählen Sie den ersten Ordner **Dokumentgenehmigung** und dann den Ordner **Dokumentversion** > **Version** aus.
1. Stellen Sie den Aggregationstyp auf **Zählung** ein.
1. Klicken Sie auf **Feld aktualisieren** für die Achse **Left (Y)** und wählen Sie die erste Option **Document Approval** und dann die Option **Document Version** > **Document** > **Name**.
1. Klicken Sie auf die Registerkarte &quot;Filter&quot;![Filter-Tab-Symbol](assets/filter-tab.png).
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Entscheidungsdatum für Teilnehmer der Genehmigungsstufe**.
   1. Ändern Sie den Operator in **Is Null**.
      Beispiel für einen Diagrammfilter für ![Revisionen](assets/revision-chart-filter.png)
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Deadline der Genehmigungsstufe**.
   1. Ändern Sie den Operator in &quot;**Kleiner als oder gleich**&quot;, schalten Sie dann &quot;relatives Datum einstellen auf&quot;um und geben Sie &quot;_$$TODAYem_&quot;in das Textfeld ein.
      Beispiel für einen Diagrammfilter für ![Revisionen](assets/revision-chart-filter-2.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .

## Hinzufügen detaillierter Überprüfungs- und Genehmigungsinformationen mit Tabellen

![Tabellenbeispiel](assets/table-dashboard.png)

### Liste ausstehender Genehmigungen

1. [Erstellen Sie ein Dashboard](#create-a-dashboard), wie im Abschnitt oben beschrieben.
1. Klicken Sie auf der Karte **Tabelle** auf **Hinzufügen**.
1. Geben Sie _Ausstehende Genehmigungen_ in das Textfeld **Name** ein.
1. (Optional) Geben Sie eine Beschreibung in das Textfeld **Beschreibung** ein. Dieser Text wird als QuickInfo neben dem Diagrammnamen angezeigt.
1. Klicken Sie auf **Spalteneinstellungen öffnen**.
1. Klicken Sie auf **Spalte hinzufügen**, scrollen Sie nach unten und klicken Sie auf den ersten Ordner **Dokumentgenehmigungen** und wählen Sie dann **Status** aus.
1. Fügen Sie die folgenden Spalten hinzu:

   <table>
    <tr>
    <td><strong>Projektname</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Projekt &gt; Name</td>
    </tr>
    <tr>
    <td><strong>Dokumentname</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Geben Sie im Suchfeld _Name_ ein.</td>
    </tr>
    <tr>
    <td><strong>Dokumentversion</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Frist</strong></td>
    <td>Dokument &gt; Genehmigungsstadium &gt; Frist</td>
    </tr>
    <tr>
    <td><strong>Anfrage von</strong></td>
    <td>Dokument &gt; Genehmigungsstadium &gt; Teilnehmer der Genehmigungsphase* &gt; Anforderer &gt; Geben Sie im Suchfeld _Name_ ein.</td>
    </tr>
     <tr>
    <td><strong>Angefordertes Datum</strong></td>
    <td>Dokument &gt; Genehmigungsstadium &gt; Teilnehmer der Genehmigungsphase* &gt; Erstellt unter</td>
    </tr>
     <tr>
    <td><strong>Genehmigende Person</strong></td>
    <td>Dokument &gt; Genehmigungsstufe &gt; Teilnehmer der Genehmigungsstufe* &gt; Teilnehmer &gt; Benutzer &gt; Geben Sie im Suchfeld _Name_ ein.</td>
    </tr>
    <table>

   *Die Teilnehmer der Genehmigungsstufe werden auf den Genehmigungsstadium-Pa gekürzt.

1. Fahren Sie mit [Hinzufügen des erforderlichen Filters unter ](#add-the-required-filter) fort.

#### Hinzufügen des erforderlichen Filters für ausstehende Genehmigungen

1. Klicken Sie auf die Registerkarte &quot;Filter&quot;![Filter-Tab-Symbol](assets/filter-tab.png).
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in **Equal** und geben Sie dann _pending approval_ ein.
      Beispiel für den Filter für die ![ausstehende Genehmigungstabelle](assets/pending-approval-table-filter.png)
1. Fügen Sie optionale Filter wie unten beschrieben hinzu oder klicken Sie oben rechts im Bildschirm auf **Fertig** .

**Optionale Filter**

Um je nach Anwendungsfall genauere Informationen anzuzeigen, können Sie zusätzliche Filterbedingungen hinzufügen. Sie können die Tabelle neu erstellen und neue Filterbedingungen pro Anwendungsfall hinzufügen.

+++ Erweitern, um zusätzliche Filteroptionen anzuzeigen

**Meine Projekte**

1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf &quot;**Feld auswählen**&quot;, wählen Sie dann &quot;**Dokumentversion**&quot;> &quot;**Dokument**&quot;> &quot;**Projekt**&quot;> &quot;**Inhaber**&quot;> geben Sie im Suchfeld &quot;_Name_&quot; ein.
   1. Ändern Sie den Operator in &quot;**Equal**&quot;und wählen Sie dann &quot;**Me (angemeldeter Benutzer)**&quot;, um Projekte in Workfront anzuzeigen, in denen Sie als Projekteigentümer gekennzeichnet sind.
      Beispiel für den Filter für die ![ausstehende Genehmigungstabelle](assets/pending-approvals-my-project-filter.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .

**Von mir eingereichte Genehmigungen**

1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf &quot;**Feld auswählen**&quot;, wählen Sie dann &quot;**Genehmigungsstufe**&quot;> &quot;**Teilnehmer der Genehmigungsstufe**&quot;> &quot;**Anforderer**&quot;> geben Sie im Suchfeld _Name_ ein.
   1. Ändern Sie den Operator in &quot;**Equal**&quot;und wählen Sie dann &quot;**Me (angemeldeter Benutzer)**&quot;, um Projekte in Workfront anzuzeigen, in denen Sie als Projekteigentümer gekennzeichnet sind.
      Beispiel für den Filter für die ![ausstehende Genehmigungstabelle](assets/pending-approvals-my-project-filter.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .

+++

### Liste zu überfälliger Genehmigungen

1. [Erstellen Sie ein Dashboard](#create-a-dashboard), wie im Abschnitt oben beschrieben.
1. Klicken Sie auf der Karte Tabelle auf **Hinzufügen**.
1. Geben Sie _Überfällige Genehmigungen_ in das Textfeld **Name** ein.
1. (Optional) Geben Sie eine Beschreibung in das Textfeld **Beschreibung** ein. Dieser Text wird als QuickInfo neben dem Diagrammnamen angezeigt.
1. Klicken Sie auf **Spalteneinstellungen öffnen**.
1. Klicken Sie auf **Spalte hinzufügen**, scrollen Sie nach unten und klicken Sie auf den ersten Ordner **Dokumentgenehmigungen** und wählen Sie dann **Status** aus.
1. Fügen Sie die folgenden Spalten hinzu:

   <table>
    <tr>
    <td><strong>Projektname</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Projekt &gt; Name</td>
    </tr>
    <tr>
    <td><strong>Dokumentname</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Geben Sie im Suchfeld _Name_ ein.</td>
    </tr>
    <tr>
    <td><strong>Dokumentversion</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Frist</strong></td>
    <td>Dokument &gt; Genehmigungsstadium &gt; Frist</td>
    </tr>
    <tr>
    <td><strong>Anfrage von</strong></td>
    <td>Dokument &gt; Genehmigungsstadium &gt; Teilnehmer der Genehmigungsphase* &gt; Anforderer &gt; Geben Sie im Suchfeld _Name_ ein.</td>
    </tr>
     <tr>
    <td><strong>Angefordertes Datum</strong></td>
    <td>Dokument &gt; Genehmigungsstadium &gt; Teilnehmer der Genehmigungsphase* &gt; Erstellt unter</td>
    </tr>
     <tr>
    <td><strong>Genehmigende Person</strong></td>
    <td>Dokument &gt; Genehmigungsstufe &gt; Teilnehmer der Genehmigungsstufe* &gt; Teilnehmer &gt; Benutzer &gt; Geben Sie im Suchfeld _Name_ ein.</td>
    </tr>
    <table>

   *Die Teilnehmer der Genehmigungsstufe werden auf den Genehmigungsstadium-Pa gekürzt.

1. Fahren Sie mit [Hinzufügen des erforderlichen Filters unter ](#add-the-required-filter-1) fort.

#### Hinzufügen des erforderlichen überfälligen Genehmigungsfilters

1. Klicken Sie auf die Registerkarte &quot;Filter&quot;![Filter-Tab-Symbol](assets/filter-tab.png).
1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Genehmigungsstufe** > **Frist** aus.
   1. Ändern Sie den Operator in **Kleiner als**, schalten Sie **relatives Datum festlegen** ein und geben Sie dann _$$HEUTE_ ein.
      Beispiel für den Filter für die ![überfällige Genehmigungstabelle](assets/overdue-approval.png)
1. Fügen Sie optionale Filter wie unten beschrieben hinzu oder klicken Sie oben rechts im Bildschirm auf **Fertig** .


**Optionale Filter**

Um je nach Anwendungsfall genauere Informationen anzuzeigen, können Sie zusätzliche Filterbedingungen hinzufügen. Sie können die Tabelle neu erstellen und neue, optionale Filterbedingungen pro Anwendungsfall hinzufügen.

+++ Erweitern, um zusätzliche Filteroptionen anzuzeigen

**Meine Projekte**

1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf &quot;**Feld auswählen**&quot;, wählen Sie dann &quot;**Dokumentversion**&quot;> &quot;**Dokument**&quot;> &quot;**Projekt**&quot;> &quot;**Inhaber**&quot;> geben Sie im Suchfeld &quot;_Name_&quot; ein.
   1. Ändern Sie den Operator in &quot;**Equal**&quot;und wählen Sie dann &quot;**Me (angemeldeter Benutzer)**&quot;, um Projekte in Workfront anzuzeigen, in denen Sie als Projekteigentümer gekennzeichnet sind.
      Beispiel für den Filter für die ![ausstehende Genehmigungstabelle](assets/pending-approvals-my-project-filter.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .

**Von mir eingereichte Genehmigungen**

1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf &quot;**Feld auswählen**&quot;, wählen Sie dann &quot;**Genehmigungsstufe**&quot;> &quot;**Teilnehmer der Genehmigungsstufe**&quot;> &quot;**Anforderer**&quot;> geben Sie im Suchfeld _Name_ ein.
   1. Ändern Sie den Operator in &quot;**Equal**&quot;und wählen Sie dann &quot;**Me (angemeldeter Benutzer)**&quot;, um Projekte in Workfront anzuzeigen, in denen Sie als Projekteigentümer gekennzeichnet sind.
      Beispiel für den Filter für die ![ausstehende Genehmigungstabelle](assets/pending-approvals-my-project-filter.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .

**Meine Mannschaft**

1. Klicken Sie auf **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf &quot;**Feld auswählen**&quot;, wählen Sie dann &quot;**Genehmigungsstufe**&quot;> &quot;**Teilnehmer der Genehmigungsstufe**&quot;> &quot;**Teilnehmer-Team**&quot;> geben Sie im Suchfeld _Name_ ein.
   1. Ändern Sie den Operator in &quot;**Equal**&quot;und wählen Sie dann &quot;**Meine Standardteams (angemeldeter Benutzer)**&quot;oder &quot;**Meine anderen Teams (angemeldeter Benutzer)**&quot;, um Projekte anzuzeigen, die entweder Ihrem Standardteam oder anderen Teams, denen Sie angehören, zugewiesen sind.
      Beispiel für den Filter für die ![ausstehende Genehmigungstabelle](assets/approvals-ive-submitted-filter.png)
1. Klicken Sie oben rechts im Bildschirm auf **Fertig** .
+++
