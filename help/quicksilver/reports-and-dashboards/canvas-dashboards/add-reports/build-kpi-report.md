---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Erstellen eines KPI-Berichts in einem Arbeitsflächen-Dashboard
description: Ein KPI-Bericht, der einen einzelnen aggregierten KPI hervorgehoben darstellt, kann zu einem Arbeitsflächen-Dashboard hinzugefügt werden.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: d7caaa0871263fb8ef4224a9c298778f3ee2454a
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 1%

---

# Erstellen eines KPI-Berichts in einem Arbeitsflächen-Dashboard

>[!IMPORTANT]
>
>Die Funktion Canvas-Dashboards ist derzeit nur für Benutzer verfügbar, die an der Beta-Phase teilnehmen. Teile der Funktion sind in dieser Phase möglicherweise nicht vollständig oder funktionieren nicht wie vorgesehen. Bitte senden Sie Feedback zu Ihrem Erlebnis, indem Sie die Anweisungen im Abschnitt [Feedback geben](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) im Artikel Beta-Übersicht für Canvas-Dashboards befolgen.<br>
>Wenn Sie Feedback zu einem möglichen Fehler oder einem technischen Problem haben, senden Sie bitte ein Ticket an den Workfront-Support. Weitere Informationen finden Sie unter [Kundensupport kontaktieren](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Beachten Sie, dass diese Beta-Version bei den folgenden Cloud-Anbietern nicht verfügbar ist:
>
>* Eigene Schlüssel für Amazon Web Services mitbringen
>* Azure
>* Google Cloud Platform

Sie können einen KPI-Bericht erstellen und zu einem Arbeitsflächen-Dashboard hinzufügen, das Ihre wichtigsten Leistungsindikatordaten visuell als eine Zahl darstellt, mit der Sie dann sehen können, wie Ihre Projekte und Teams funktionieren.

![Beispiel für KPI-Bericht](assets/kpi-example-main.png)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebig </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td> 
   <td><p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p>
  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Voraussetzungen

Sie müssen ein Dashboard erstellen, bevor Sie einen KPI-Bericht erstellen können.

## Erstellen eines KPI-Berichts in einem Arbeitsflächen-Dashboard

Es stehen viele Konfigurationsoptionen zum Erstellen eines KPI-Berichts zur Verfügung. In diesem Abschnitt führen wir Sie durch den allgemeinen Prozess der Erstellung eines solchen.

{{step1-to-dashboards}}

1. Klicken Sie im linken Bedienfeld auf **Arbeitsflächen-Dashboards**.

1. Klicken **oben rechts auf** Neues Dashboard“.

1. Geben Sie in das Feld **Dashboard erstellen** den **** Namen“ und die **Beschreibung** des Dashboards ein.

1. Klicken Sie auf **Erstellen**.

1. Wählen Sie im **Bericht hinzufügen** die Option **Bericht erstellen** aus.

1. Wählen Sie auf der linken Seite &quot;**&quot;**.

1. Klicken Sie oben rechts auf **Bericht erstellen**.

1. Gehen Sie wie folgt vor, um den Abschnitt **Details** zu konfigurieren:

   1. Einen Bericht eingeben **Name**.
   1. Einen Bericht eingeben **Beschreibung**.

      >[!NOTE]
      >
      >Die Beschreibung wird als Beschriftung unter dem KPI-Wert verwendet. Wenn Sie keine Beschreibung eingeben, wird eine Beschriftung für Sie basierend auf dem Aggregator und dem Aggregationstyp generiert, den Sie in den folgenden Schritten auswählen.

1. Gehen Sie wie folgt vor, um den Abschnitt **KPI erstellen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **KPI erstellen** ![KPI erstellen](assets/build-kpi-icon.png) .

   1. Klicken Sie **Feld auswählen** und geben Sie dann das Feld an, das Sie dem Bericht hinzufügen möchten.

   1. Wählen Sie in **Dropdown-Liste** Aggregationstyp“ aus, wie die Daten aggregiert werden, um die KPI-Ausgabe zu erzeugen. Die Optionen in diesem Feld variieren je nach dem Typ des Felds, das im vorherigen Schritt ausgewählt wurde.

1. Gehen Sie wie folgt vor, um den Abschnitt **Filter** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Filter** ![Filter](assets/filter-icon.png).

   1. Wählen Sie **Filter bearbeiten** aus.

   1. Klicken Sie **Bedingung hinzufügen** und geben Sie dann das Feld an, nach dem Sie filtern möchten, sowie den Modifikator, der definiert, welche Art von Bedingung das Feld erfüllen muss.

   1. (Optional) Klicken Sie auf **Filtergruppe hinzufügen**, um einen weiteren Satz von Filterkriterien hinzuzufügen. Der Standardoperator zwischen den Sätzen ist UND. Klicken Sie auf den Operator, um ihn in ODER zu ändern.

      Weitere Informationen zu Filtern finden Sie unter [Berichtsfilter in einem Arbeitsflächen-Dashboard bearbeiten](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md).

1. Gehen Sie wie folgt vor, um den Abschnitt **Spalteneinstellungen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Drilldown-**![Spalten-Symbol](assets/drilldown-column.png). Die Felder aus dem Diagramm werden automatisch als Spalten im Vorschauabschnitt auf der rechten Seite angezeigt.

   1. (Optional) Um eine der vorhandenen Spaltenkonfigurationen zu aktualisieren, wählen Sie die Spalte, die Sie aktualisieren möchten, im Abschnitt **Aktuelle Spalten** aus und aktualisieren Sie dann die gewünschten Informationen (z. B. Beschriftung, verknüpfter Status und Formatierungsregeln).

   1. Klicken Sie **Spalte hinzufügen** und wählen Sie dann das Feld aus, das als Spalte in der Tabelle angezeigt werden soll. Wiederholen Sie diesen Vorgang für jede Spalte, die Sie hinzufügen möchten.

1. Gehen Sie wie folgt vor, um den Abschnitt **Drilldown-Gruppeneinstellungen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Gruppeneinstellungen** ![Drilldown-Gruppe](assets/drilldown-group-icon.png) .

   1. Klicken Sie auf **Gruppierung hinzufügen** und wählen Sie dann das Feld aus, das Sie als Gruppierung erstellen möchten.

1. Klicken Sie **Speichern**, um den Bericht zu erstellen und zum Dashboard hinzuzufügen.

## Beispiel für einen KPI-Bericht erstellen

In diesem Abschnitt werden die Schritte zum Erstellen eines KPI-Berichts erläutert, der ausstehende Dokumentgenehmigungen ausgibt.

Weitere Informationen zu KPI-Berichtsbeispielen finden Sie unter [Erstellen eines Berichts-Dashboards zur Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. Klicken Sie im linken Bedienfeld auf **Arbeitsflächen-Dashboards**.

1. Klicken **oben rechts auf** Neues Dashboard“.

1. Geben Sie in das Feld **Dashboard erstellen** den **** Namen“ und die **Beschreibung** des Dashboards ein.

1. Klicken Sie auf **Erstellen**.

1. Wählen Sie im **Bericht hinzufügen** die Option **Bericht erstellen** aus.

1. Wählen Sie auf der linken Seite &quot;**&quot;**.

1. Klicken Sie oben rechts auf **Bericht erstellen**.

1. Gehen Sie wie folgt vor, um den Abschnitt **Details** zu konfigurieren:

   1. Geben Sie *Ausstehend* in das Feld **Name** ein.
   1. Geben Sie *Feld* Beschreibung **„Ausstehende Genehmigungen** ein. Wird als Beschriftung unterhalb des KPI-Werts angezeigt.

1. Gehen Sie wie folgt vor, um den Abschnitt **KPI erstellen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **KPI erstellen** ![KPI erstellen](assets/build-kpi-icon.png).

   1. Klicken Sie **Feld auswählen**.

   1. Suchen Sie den Ordner **Dokumentengenehmigung** und wählen Sie ihn aus.

   1. Wählen Sie **Status** aus.

   1. Wählen **in der Dropdown** Liste Aggregationstyp die Option **Anzahl** aus.

1. Gehen Sie wie folgt vor, um den Abschnitt **Filter** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Filter** ![Filter](assets/filter-icon.png).

   1. Wählen Sie **Filter bearbeiten** aus.

   1. Klicken Sie **Bedingung hinzufügen**.

   1. Klicken Sie in den leeren Bedingungsfilter, klicken Sie auf **Feld auswählen** und wählen Sie dann **Status** aus.
   1. Belassen Sie den Operator **Gleich** und geben Sie dann _Überprüfung ausstehend_ in das Textfeld ein.
      ![Beispiel für ausstehenden KPI-Filter](assets/pending-kpi-filter.png)
1. Klicken **oben** auf dem Bildschirm auf „Speichern“.

## Überlegungen beim Erstellen eines KPI-Berichts

### Berichte mit Finanzdaten

Benutzer mit der Zugriffsebene Anzeigen oder Bearbeiten von Finanzdaten sehen weiterhin Finanzdaten in den Visualisierungen des Arbeitsflächen-Dashboards, auch wenn die Berechtigung zum Anzeigen von Finanzdaten auf der Aufgaben- oder Projektebene entfernt wurde.

* Benutzende ohne finanzielle Datenrechte auf der Zugriffsebene sehen keine finanziellen Daten in Berichten.
* Benutzer, die Finanzdaten sehen, sind auf Datensätze beschränkt, für die sie bereits über Anzeigeberechtigungen verfügen (Projekte, Aufgaben, Probleme usw.). Sie sehen keine finanziellen Werte für Datensätze, auf die sie nicht zugreifen können.
* Ersteller von Berichten sollten Vorsicht walten lassen, wenn sie Finanzdaten in Dashboards einbeziehen, und darauf achten, mit wem sie Dashboards teilen, um unbeabsichtigten Zugriff zu verhindern.

Dies ist eine bekannte Grenze, und wir planen, sie so schnell wie möglich zu beheben.

### Verwenden der Feldauswahl

Die **Abschnitte** Dropdown-Liste im Abschnitt **KPI erstellen** soll die Auswahlmöglichkeiten in einer Feldauswahl einschränken, damit ein Objekt beim Erstellen eines Tabellenberichts leichter zu finden ist. Wählen Sie zunächst ein Basiseinheitsobjekt aus.

* **Alle Abschnitte**: Alle Objekttypen in Workfront Workflow und Workfront Planning.
* **Workfront-Objekte**: Native Workfront-Workflow-Objekte.
* **Planning-Datensatztypen**: Benutzerdefinierte Datensatztypen, die in Workfront Planning definiert sind.

![Dropdown-Liste „Abschnitte](assets/sections-dropdown.png)

Nachdem das Basisobjekt für die Entität ausgewählt wurde, wird **Dropdown-** „Abschnitte“ mit den entsprechenden Feldtypoptionen aktualisiert, aus denen Sie auswählen können.

* **Alle Abschnitte**: Native Felder, benutzerdefinierte Felder und verwandte Objekte.
* **Alle Felder**: Sowohl native als auch benutzerdefinierte Felder (ohne Beziehungen).
* **Benutzerdefinierte Felder**: Kundendefinierte Felder in einem benutzerdefinierten Formular oder einem Planungsdatensatz.
* **Workfront-**: Nur native Felder.
* **Beziehungen**: Verbundene Datensätze.

![Auswahl berichtbarer Objekte](assets/reportable-objects-selection.png)

### Verweisen auf untergeordnete Objekte

Verfügbare Beziehungen für zusätzliche Spalten, Filteroptionen und Gruppierungsattribute sind im Allgemeinen auf Objekte beschränkt, die höher in der Workfront-Objekthierarchie stehen oder die ansonsten eine einzige Auswahl im Basisobjekt der Entität des Berichts aufweisen. Hiervon gibt es einige Ausnahmen, darunter die folgenden:

* Projekt > Aufgaben
* Dokumentengenehmigung > Dokumentengenehmigungsphasen
* Phasen der Dokumentgenehmigung > Teilnehmer an der Dokumentgenehmigungsphase

Bei Verwendung einer der oben aufgeführten hierarchischen Beziehungen wird in der Tabelle für jeden untergeordneten Datensatz eine Zeile angezeigt, die mit dem übergeordneten Objekt verbunden ist.


