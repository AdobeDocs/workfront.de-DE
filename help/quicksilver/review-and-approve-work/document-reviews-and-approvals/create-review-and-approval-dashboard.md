---
product-area: documents
navigation-topic: approvals
title: Erstellen eines Überprüfungs- und Validierungs-Dashboards
description: Sie können Genehmigungsmetriken in Arbeitsflächen-Dashboards überprüfen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 48f8605b-c342-493b-96e7-f73248e34b35
source-git-commit: 0aeef516c8e3b94edee6fc177766be032241965f
workflow-type: tm+mt
source-wordcount: '1991'
ht-degree: 1%

---

# Erstellen eines Berichts-Dashboards zur Überprüfung und Genehmigung

Sie können im Bereich der Arbeitsflächen-Dashboards ein Berichts-Dashboard erstellen, um sowohl allgemeine als auch detaillierte Informationen zu Überprüfungen und Genehmigungen mit der Funktion „Einheitliche Genehmigungen“ anzuzeigen.

>[!IMPORTANT]
>
>Diese Funktion ist nur für Kunden verfügbar, die den Service „Einheitliche Genehmigungen“ verwenden und in der Beta-Version der Arbeitsflächen-Dashboards registriert sind.


![Beispiel-Dashboard](assets/whole-dashboard.png)

## Dashboard erstellen

{{step1-to-dashboards}}

1. Klicken Sie im linken Bedienfeld auf **Arbeitsflächen-Dashboards**.
1. Klicken Sie auf **Neues Dashboard**.
1. Benennen Sie Ihr Dashboard.
1. (Optional) Fügen Sie eine Beschreibung hinzu.
1. Klicken Sie auf **Erstellen**.
   ![Dashboard-Namen und -Beschreibung hinzufügen](assets/create-a-dashboard.png)

Nachdem Sie ein Dashboard erstellt haben, können Sie mit dem Hinzufügen von KPIs, Diagrammen und Tabellen beginnen. Weitere Informationen finden Sie in den folgenden Abschnitten:

* [Hinzufügen von allgemeinen Prüf- und Genehmigungsinformationen mit KPIs und Diagrammen](#add-high-level-review-and-approval-information-with-kpis-and-charts)
* [Hinzufügen detaillierter Prüf- und Genehmigungsinformationen mit Tabellen](#add-detailed-review-and-approval-information-with-tables)

## Hinzufügen von allgemeinen Prüf- und Genehmigungsinformationen mit KPIs und Diagrammen

Sie können allgemeine Informationen zu Dokumentgenehmigungen mit KPIs und Diagrammen anzeigen. Drill-down-Informationen sind in der Beta-Version derzeit nicht verfügbar.

### KPIs

![KPI-Beispiele](assets/kpi-dashboard.png)

#### Ausstehende Genehmigungen

1. [Erstellen Sie ein ](#create-a-dashboard), wie im obigen Abschnitt beschrieben.
1. Klicken Sie auf der **KPI**-Karte auf **Hinzufügen**.
1. Geben Sie _Ausstehend_ in das Textfeld **KPI-Titel** ein.
1. Geben Sie _Ausstehende Genehmigungen_ in das Textfeld **KPI-**&quot; ein. In diesem Text wird beschrieben, was der KPI anzeigt.
1. Klicken Sie oben auf der Seite auf **KPI-Feld**.
1. Scrollen Sie nach unten und suchen Sie den **Ordner Dokumentengenehmigung**.
1. Wählen Sie **Status** und wählen Sie dann **Anzahl** aus dem Dropdown-Menü aus.
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**.
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Belassen Sie den Operator **Gleich** und geben Sie _Überprüfung ausstehend_ in das Textfeld ein.

      ![Beispiel für ausstehenden KPI-Filter](assets/pending-kpi-filter.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.


#### Überfällige Genehmigungen

1. [Erstellen Sie ein ](#create-a-dashboard), wie im obigen Abschnitt beschrieben.
1. Klicken Sie auf der **KPI**-Karte auf **Hinzufügen**.
1. Geben Sie _Überfällig_ in das Textfeld **KPI-Titel** ein.
1. Geben Sie _Genehmigungsphase Frist in der Vergangenheit_ in das Textfeld **KPI-** ein. In diesem Text wird beschrieben, was der KPI anzeigt.
1. Klicken Sie oben auf der Seite auf **KPI-Feld**.
1. Scrollen Sie nach unten und suchen Sie den **Ordner Dokumentengenehmigung**.
1. Wählen Sie **Status** und wählen Sie dann **Anzahl** aus dem Dropdown-Menü aus.
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Frist** aus.
   1. Ändern Sie den Operator in **kleiner als** und schalten Sie das relative Datum um. Geben Sie dann _$$TODAY_ in das Textfeld ein.

      ![Beispiel für überfälligen KPI-Filter](assets/overdue-kpi-filter.png)
1. Klicken Sie **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in **Nicht enthält** und geben Sie dann _Genehmigt_ in das Textfeld ein.

      ![Überfälliger KPI-Filter - Beispiel 2](assets/overdue-kpi-filter-2.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.


#### Abgeschlossene Genehmigungen

1. [Erstellen Sie ein ](#create-a-dashboard), wie im obigen Abschnitt beschrieben.
1. Klicken Sie auf der **KPI**-Karte auf **Hinzufügen**.
1. Geben Sie _Abgeschlossen_ in das Textfeld **KPI-Titel** ein.
1. Geben Sie _Anzahl der Genehmigungsstatus_ in das Textfeld **KPI-**&quot; ein. In diesem Text wird beschrieben, was der KPI anzeigt.
1. Klicken Sie oben auf der Seite auf **KPI-Feld**.
1. Scrollen Sie nach unten und suchen Sie den **Ordner Dokumentengenehmigung**.
1. Wählen Sie **Status** und wählen Sie dann **Anzahl** aus dem Dropdown-Menü aus.
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in **Enthält** und geben Sie _Genehmigt_ in das Textfeld ein.

      ![Beispiel für abgeschlossenen KPI-Filter](assets/completed-kpi-filter.png)
1. Klicken Sie **Bedingung hinzufügen**:
   1. Klicken Sie auf **Und**, um sie in **Oder** zu ändern.
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in **Gleich** und geben Sie dann _Überprüft_ in das Textfeld ein.

      ![Beispiel für abgeschlossenen KPI-Filter](assets/completed-kpi-filter-2.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.

#### Abgebrochene Genehmigungen

1. [Erstellen Sie ein ](#create-a-dashboard), wie im obigen Abschnitt beschrieben.
1. Klicken Sie auf der **KPI**-Karte auf **Hinzufügen**.
1. Geben Sie _Abgebrochen_ in das Textfeld **KPI-Titel** ein.
1. Geben Sie _Validierungs-Deadline über 2 Wochen_ im Textfeld **KPI-**&quot; ein. In diesem Text wird beschrieben, was der KPI anzeigt.
1. Klicken Sie oben auf der Seite auf **KPI-Feld**.
1. Scrollen Sie nach unten und suchen Sie den **Ordner Dokumentengenehmigungsphase**.
1. Wählen Sie **Frist** und wählen Sie dann **Anzahl** aus dem Dropdown-Menü aus.
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in **Nicht enthält** und geben Sie _Genehmigt_ in das Textfeld ein.

      ![Beispiel für abgebrochenen KPI-Filter](assets/abandoned-kpi-filter.png)
1. Klicken Sie **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Frist** aus.
   1. Ändern Sie den Operator in **kleiner als**, schalten Sie dann das relative Datum ein und geben Sie dann _$$TODAY-2w_ in das Textfeld ein.

      ![Beispiel für abgebrochenen KPI-Filter](assets/abandoned-kpi-filter-2.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.

### Diagramme

![Diagrammbeispiele](assets/chart-dashboard.png)

#### Validierungen nach Entscheidungsbalkendiagramm

1. [Erstellen Sie ein ](#create-a-dashboard), wie im obigen Abschnitt beschrieben.
1. Klicken Sie in **Karte** Diagramm“ auf **Hinzufügen**.
1. Geben Sie _Genehmigungen durch Entscheidung_ in das Textfeld **Name** ein.
1. (Optional) Geben Sie eine Beschreibung in das Textfeld &quot;**&quot;**. Dieser Text wird als QuickInfo neben dem Diagrammnamen angezeigt.
1. Klicken Sie **Diagrammdetails öffnen**.
1. Lassen Sie **Dropdown-Menü** Diagrammtyp) die Option **Balkendiagramm** ausgewählt.
1. Lassen Sie **Dropdown-Menü** Balkentyp“ **Einfach** ausgewählt.
1. Klicken Sie auf **Feld aktualisieren** für die Achse **Unten (X)** und wählen Sie den ersten Ordner **Dokumentengenehmigung** dann **Status**.
1. Wählen Sie als Aggregationstyp &quot;**&quot;**.
1. Klicken Sie auf **Feld aktualisieren** für die Achse **Links (Y)** und wählen Sie die erste Option **Dokumentengenehmigung** und dann **Status**.
1. Klicken Sie auf die Registerkarte Filter ![Registerkarte Filter](assets/filter-tab.png).
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Dokumentversion**.
   1. Ändern Sie den Operator in **Ist nicht null**.

      ![Filterbeispiel](assets/approvals-by-decision-chart-filter.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.


#### Überarbeitungen Balkendiagramm

1. [Erstellen Sie ein ](#create-a-dashboard), wie im obigen Abschnitt beschrieben.
1. Klicken Sie in **Karte** Diagramm“ auf **Hinzufügen**.
1. Geben Sie _Revisions_ in das Textfeld **Name** ein.
1. Geben Sie _Anzahl der geplanten Revisionen für Dokumente mit unvollständigen Entscheidungen vor Ende dieses Monats_ in das Textfeld **Beschreibung** ein. Dieser Text wird als QuickInfo neben dem Diagrammnamen angezeigt.
1. Klicken Sie **Diagrammdetails öffnen**.
1. Lassen Sie **Dropdown-Menü** Diagrammtyp) die Option **Balkendiagramm** ausgewählt.
1. Lassen Sie **Dropdown-Menü** Balkentyp“ **Einfach** ausgewählt.
1. Klicken Sie auf **Feld aktualisieren** für die Achse **Unten (X)** und wählen Sie den ersten Ordner **Dokumentengenehmigung** dann **Dokumentversion** > **Version**.
1. Wählen Sie als Aggregationstyp &quot;**&quot;**.
1. Klicken Sie auf **Feld aktualisieren** für die Achse **links (Y)** und wählen Sie die erste Option **Dokumentengenehmigung** dann **Dokumentversion** > **Dokument** > **Name**.
1. Klicken Sie auf die Registerkarte ![Filter“ (](assets/filter-tab.png)).
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Datum der Teilnehmerentscheidung für die Genehmigungsphase** aus.
   1. Ändern Sie den Operator in **Ist Null**.

      ![Beispiel für Revisionsdiagrammfilter](assets/revision-chart-filter.png)
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Deadline für Genehmigungsphase** aus.
   1. Ändern Sie den Operator in **Kleiner oder gleich**, schalten Sie dann den Schalter Relatives Datum festlegen ein und geben Sie _$$TODAYem_ in das Textfeld ein.

      ![Beispiel für Revisionsdiagrammfilter](assets/revision-chart-filter-2.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.

## Hinzufügen detaillierter Prüf- und Genehmigungsinformationen mit Tabellen

![Tabellenbeispiel](assets/table-dashboard.png)

### Liste der ausstehenden Genehmigungen

1. [Erstellen Sie ein ](#create-a-dashboard), wie im obigen Abschnitt beschrieben.
1. Klicken Sie in **Karte** Tabelle **auf „Hinzufügen**.
1. Geben Sie _Ausstehende Genehmigungen_ in das Textfeld **Name** ein.
1. (Optional) Geben Sie eine Beschreibung in das Textfeld &quot;**&quot;**. Dieser Text wird als QuickInfo neben dem Diagrammnamen angezeigt.
1. Klicken Sie **Spalteneinstellungen öffnen**.
1. Klicken Sie **Spalte hinzufügen**, scrollen Sie nach unten und klicken Sie auf den ersten **Dokumentengenehmigungen** Ordner und wählen Sie dann **Status** aus.
1. Die folgenden Spalten hinzufügen:

   <table>
    <tr>
    <td><strong>Projektname</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Projekt &gt; Name</td>
    </tr>
    <tr>
    <td><strong>Dokumentname</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Typ _Name_ in das Suchfeld.</td>
    </tr>
    <tr>
    <td><strong>Dokumentversion</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Frist</strong></td>
    <td>Dokumentengenehmigung &gt; Genehmigungsphase &gt; Frist</td>
    </tr>
    <tr>
    <td><strong>Anfrage von</strong></td>
    <td>Dokumentgenehmigung &gt; Genehmigungsphase &gt; Teilnehmer der Genehmigungsphase* &gt; Anforderer &gt; Typ _name_ in der Suchbox.</td>
    </tr>
     <tr>
    <td><strong>Angefordertes Datum</strong></td>
    <td>Dokumentengenehmigung &gt; Genehmigungsphase &gt; Genehmigungsphase &gt; Teilnehmer der Genehmigungsphase* &gt; Erstellt in</td>
    </tr>
     <tr>
    <td><strong>Genehmigende Person</strong></td>
    <td>Dokumentengenehmigung &gt; Genehmigungsphase &gt; Teilnehmer der Genehmigungsphase* &gt; Teilnehmer-Benutzer &gt; Typ _name_ in der Suchbox.</td>
    </tr>
    <table>

   *Teilnehmer der Genehmigungsphase werden auf Genehmigungsphase PA gekürzt.

1. Fahren Sie fort [Fügen Sie unten den erforderlichen Filter hinzu](#add-the-required-filter).

#### Fügen Sie den erforderlichen Filter für ausstehende Genehmigungen hinzu

1. Klicken Sie auf die Registerkarte ![Filter“ (](assets/filter-tab.png)).
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Ändern Sie den Operator in **Gleich** und geben Sie dann _Genehmigung steht aus_.

      ![Filterbeispiel für Tabelle mit ausstehender Genehmigung](assets/pending-approval-table-filter.png)
1. Fügen Sie optionale Filter wie unten beschrieben hinzu oder klicken **oben** auf „Fertig“.

**Optionale Filter**

Um spezifischere Informationen je nach Anwendungsfall anzuzeigen, können Sie zusätzliche Filterbedingungen hinzufügen. Sie können die Tabelle neu erstellen und neue Filterbedingungen pro Anwendungsfall hinzufügen.

+++ Erweitern , um zusätzliche Filteroptionen anzuzeigen

**Meine Projekte**

1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Dokumentversion** > **Dokument** > **Projekt** > **Inhaber** > Typ _Name_ im Suchfeld aus.
   1. Ändern Sie den Operator in **Gleich** und wählen Sie dann **Ich (angemeldeter Benutzer)**, um Projekte in Workfront anzuzeigen, in denen Sie als Projektbesitzer markiert sind.

      ![Filterbeispiel für Tabelle mit ausstehender Genehmigung](assets/pending-approvals-my-project-filter.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.

**Von mir übermittelte Genehmigungen**

1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann im Suchfeld **Genehmigungsphase** > **Teilnehmer der Genehmigungsphase** > **Anforderer** > Typ _Name_ aus.
   1. Ändern Sie den Operator in **Gleich** und wählen Sie dann **Ich (angemeldeter Benutzer)**, um Projekte in Workfront anzuzeigen, in denen Sie als Projektbesitzer markiert sind.

      ![Filterbeispiel für Tabelle mit ausstehender Genehmigung](assets/pending-approvals-my-project-filter.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.

+++

### Liste der überfälligen Genehmigungen

1. [Erstellen Sie ein ](#create-a-dashboard), wie im obigen Abschnitt beschrieben.
1. Klicken Sie in der Karte Tabelle auf **Hinzufügen**.
1. Geben Sie _Überfällige Genehmigungen_ in das Textfeld **Name** ein.
1. (Optional) Geben Sie eine Beschreibung in das Textfeld &quot;**&quot;**. Dieser Text wird als QuickInfo neben dem Diagrammnamen angezeigt.
1. Klicken Sie **Spalteneinstellungen öffnen**.
1. Klicken Sie **Spalte hinzufügen**, scrollen Sie nach unten und klicken Sie auf den ersten **Dokumentengenehmigungen** Ordner und wählen Sie dann **Status** aus.
1. Die folgenden Spalten hinzufügen:

   <table>
    <tr>
    <td><strong>Projektname</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Projekt &gt; Name</td>
    </tr>
    <tr>
    <td><strong>Dokumentname</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Typ _Name_ in das Suchfeld.</td>
    </tr>
    <tr>
    <td><strong>Dokumentversion</strong></td>
    <td>Dokumentversion &gt; Dokument &gt; Version</td>
    </tr>
    <tr>
    <td><strong>Frist</strong></td>
    <td>Dokument &gt; Genehmigungsphase &gt; Frist</td>
    </tr>
    <tr>
    <td><strong>Anfrage von</strong></td>
    <td>Dokument &gt; Genehmigungsphase &gt; Teilnehmer der Genehmigungsphase* &gt; Anforderer &gt; Typ _name_ in der Suchbox.</td>
    </tr>
     <tr>
    <td><strong>Angefordertes Datum</strong></td>
    <td>Dokument &gt; Genehmigungsphase &gt; Teilnehmer der Genehmigungsphase* &gt; Erstellt in</td>
    </tr>
     <tr>
    <td><strong>Genehmigende Person</strong></td>
    <td>Dokument &gt; Genehmigungsphase &gt; Teilnehmer der Genehmigungsphase* &gt; Teilnehmer-Benutzer &gt; Typ _name_ in der Suchbox.</td>
    </tr>
    <table>

   *Teilnehmer der Genehmigungsphase werden auf Genehmigungsphase PA gekürzt.

1. Fahren Sie fort [Fügen Sie unten den erforderlichen Filter hinzu](#add-the-required-filter-1).

#### Fügen Sie den Filter Erforderliche überfällige Genehmigungen hinzu

1. Klicken Sie auf die Registerkarte ![Filter“ (](assets/filter-tab.png)).
1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Genehmigungsphase** > **Frist**.
   1. Ändern Sie den Operator in **Kleiner als**, schalten Sie **Relatives Datum festlegen** ein und geben Sie dann _$$TODAY_ ein.

      ![Beispiel für überfällige Genehmigungstabelle](assets/overdue-approval.png)
1. Fügen Sie optionale Filter wie unten beschrieben hinzu oder klicken **oben** auf „Fertig“.


**Optionale Filter**

Um spezifischere Informationen je nach Anwendungsfall anzuzeigen, können Sie zusätzliche Filterbedingungen hinzufügen. Sie können die Tabelle neu erstellen und neue, optionale Filterbedingungen pro Anwendungsfall hinzufügen.

+++ Erweitern , um zusätzliche Filteroptionen anzuzeigen

**Meine Projekte**

1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Dokumentversion** > **Dokument** > **Projekt** > **Inhaber** > Typ _Name_ im Suchfeld aus.
   1. Ändern Sie den Operator in **Gleich** und wählen Sie dann **Ich (angemeldeter Benutzer)**, um Projekte in Workfront anzuzeigen, in denen Sie als Projektbesitzer markiert sind.

      ![Filterbeispiel für Tabelle mit ausstehender Genehmigung](assets/pending-approvals-my-project-filter.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.

**Von mir übermittelte Genehmigungen**

1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann im Suchfeld **Genehmigungsphase** > **Teilnehmer der Genehmigungsphase** > **Anforderer** > Typ _Name_ aus.
   1. Ändern Sie den Operator in **Gleich** und wählen Sie dann **Ich (angemeldeter Benutzer)**, um Projekte in Workfront anzuzeigen, in denen Sie als Projektbesitzer markiert sind.

      ![Filterbeispiel für Tabelle mit ausstehender Genehmigung](assets/pending-approvals-my-project-filter.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.

**Mein Team**

1. Klicken Sie **Filter bearbeiten** > **Bedingung hinzufügen**:
   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann im Suchfeld **Genehmigungsphase** > **Genehmigungsphase Teilnehmer** > **Teilnehmer-Team** > _Name_ aus.
   1. Ändern Sie den Operator in **Gleich** und wählen Sie dann **Meine Standard-Teams (angemeldeter Benutzer)** oder **Meine anderen Teams (angemeldeter Benutzer)**, um Projekte anzuzeigen, die Ihrem Standard-Team oder anderen Teams, denen Sie angehören, zugewiesen sind.

      ![Filterbeispiel für Tabelle mit ausstehender Genehmigung](assets/approvals-ive-submitted-filter.png)
1. Klicken **oben** auf dem Bildschirm auf „Fertig“.
+++
