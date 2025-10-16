---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Erstellen eines Diagrammberichts in einem Arbeitsflächen-Dashboard
description: Ein Diagrammbericht, der Ihre Daten als Balken-, Spalten-, Linien- oder Tortendiagramm darstellt, kann zu einem Arbeitsflächen-Dashboard hinzugefügt werden.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 4262cae8-602f-416d-94b9-409eb9d6241c
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 0%

---

# Erstellen eines Diagrammberichts in einem Arbeitsflächen-Dashboard

>[!IMPORTANT]
>
>Die Funktion Canvas-Dashboards ist derzeit nur für Benutzer verfügbar, die an der Beta-Phase teilnehmen. Teile der Funktion sind in dieser Phase möglicherweise nicht vollständig oder funktionieren nicht wie vorgesehen. Bitte senden Sie Feedback zu Ihrem Erlebnis, indem Sie die Anweisungen im Abschnitt [Feedback geben](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) im Artikel Beta-Übersicht für Canvas-Dashboards befolgen.<br>
>&#x200B;>Wenn Sie Feedback zu einem möglichen Fehler oder einem technischen Problem haben, senden Sie bitte ein Ticket an den Workfront-Support. Weitere Informationen finden Sie unter [Kundensupport kontaktieren](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>&#x200B;>Beachten Sie, dass diese Beta-Version bei den folgenden Cloud-Anbietern nicht verfügbar ist:
>
>* Eigene Schlüssel für Amazon Web Services mitbringen
>* Azure
>* Google Cloud Platform

Sie können einen Diagrammbericht erstellen und zu einem Arbeitsflächen-Dashboard hinzufügen, um Ihre Daten als Balken-, Spalten-, Linien- oder Tortendiagramm zu visualisieren.

![Diagrammbericht](assets/chart-report-main.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

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

Bevor Sie einen Diagrammbericht erstellen können, müssen Sie ein Dashboard erstellen.

## Erstellen eines Diagrammberichts in einem Arbeitsflächen-Dashboard

Es stehen viele Konfigurationsoptionen zum Erstellen eines Diagrammberichts zur Verfügung. In diesem Abschnitt führen wir Sie durch den allgemeinen Prozess der Erstellung eines solchen.

{{step1-to-dashboards}}

1. Klicken Sie im linken Bedienfeld auf **Arbeitsflächen-Dashboards**.

1. Klicken **oben rechts auf** Neues Dashboard“.

1. Geben Sie in das Feld **Dashboard erstellen** den **&#x200B;**&#x200B;Namen“ und die **Beschreibung** des Dashboards ein.

1. Klicken Sie auf **Erstellen**.

1. Wählen Sie im **Bericht hinzufügen** die Option **Bericht erstellen** aus.

1. Klicken Sie auf der linken Seite auf **Diagramm**.

1. Klicken Sie oben rechts auf **Bericht erstellen**.

1. (Optional) Gehen Sie wie folgt vor, um den Abschnitt **Details** zu konfigurieren:

   1. Einen Bericht eingeben **Name**.

   1. Einen Bericht eingeben **Beschreibung**.

   1. Deaktivieren Sie bei Bedarf das Kontrollkästchen **Zusätzliche Serie als „Andere“ anzeigen**.

      >[!NOTE]
      >
      >Es gibt eine maximale Anzahl von 60 Serien, die in einem Diagramm angezeigt werden können. Wenn dieses Kontrollkästchen aktiviert ist, werden alle Datenreihen über dem Grenzwert in einer **Sonstige** Gruppierung im Diagramm zusammengefasst.

1. Gehen Sie wie folgt vor, um den Abschnitt **Diagramm erstellen** zu konfigurieren:

   1. Klicken Sie im linken Bereich auf das Symbol **Diagramm erstellen** ![Diagramm erstellen](assets/build-chart-icon.png) .

   1. Wählen **in der Dropdown** Liste Diagrammtyp den Diagrammtyp aus, den Sie erstellen möchten:

      * **bar**
      * **Spalte**
      * **Line**
      * **Kreis**

   1. Wählen Sie in **Dropdown-** „Spaltentyp“ den Spaltentyp aus:
      * **Einfach**
      * **Multiserie**
      * **Gestapelt**

   1. Klicken Sie **ersten Abschnitt auf** Feld aktualisieren“. Suchen Sie dann das Feld, das die Daten enthält, die in dem Diagramm zusammengefasst werden sollen, und wählen Sie es aus.
   1. Wählen Sie in **Dropdown-Liste** Aggregationstyp“ aus, wie die Daten aggregiert werden, um die Diagrammausgabe zu erzeugen.

   1. Klicken Sie auf **Feld aktualisieren** unter dem zweiten Abschnitt, suchen und wählen Sie dann das zweite Feld aus, das Sie in der Grafik anzeigen möchten.

1. Gehen Sie wie folgt vor, um den Abschnitt **Filter** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Filter**![&#x200B; Filter](assets/filter-icon.png).
   1. Wählen Sie **Filter bearbeiten** aus.
   1. Klicken Sie **Bedingung hinzufügen** und geben Sie dann das Feld an, nach dem Sie filtern möchten, sowie den Modifikator, der definiert, welche Art von Bedingung das Feld erfüllen muss.
   1. (Optional) Klicken Sie auf **Filtergruppe hinzufügen**, um einen weiteren Satz von Filterkriterien hinzuzufügen. Der Standardoperator zwischen den Sätzen ist UND. Klicken Sie auf den Operator, um ihn in ODER zu ändern.

1. Gehen Sie wie folgt vor, um den Abschnitt **Spalteneinstellungen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Drilldown-**![Spalten-Symbol](assets/drilldown-column.png). Die Felder aus dem Diagramm werden automatisch als Spalten im Vorschauabschnitt auf der rechten Seite angezeigt.

   1. (Optional) Um eine der vorhandenen Spaltenkonfigurationen zu aktualisieren, wählen Sie die Spalte, die Sie aktualisieren möchten, im Abschnitt **Aktuelle Spalten** aus und aktualisieren Sie dann die gewünschten Informationen (z. B. Beschriftung, verknüpfter Status und Bedingungen).

   1. Klicken Sie **Spalte hinzufügen** und wählen Sie dann das Feld aus, das als Spalte in der Tabelle angezeigt werden soll. Wiederholen Sie diesen Vorgang für jede Spalte, die Sie hinzufügen möchten.

1. Gehen Sie wie folgt vor, um den Abschnitt **Drilldown-Gruppeneinstellungen** zu konfigurieren:

   1. Klicken Sie im linken Bereich auf das Symbol **Gruppeneinstellungen** ![Gruppeneinstellungen](assets/drilldown-group-icon.png) .

   1. Klicken Sie auf **Gruppierung hinzufügen** und wählen Sie dann das Feld aus, das Sie als Gruppierung erstellen möchten.

1. Klicken Sie **Speichern**, um den Bericht zu erstellen und zum Dashboard hinzuzufügen.

## Beispiel für das Erstellen eines Diagrammberichts

In diesem Abschnitt werden die Schritte zum Erstellen eines Säulendiagramms erläutert, in dem überfällige Aufgaben nach Projektbesitzer angezeigt werden.

{{step1-to-dashboards}}

1. Klicken Sie im linken Bedienfeld auf **Arbeitsflächen-Dashboards**.

1. Klicken **oben rechts auf** Neues Dashboard“.

1. Geben Sie in das Feld **Dashboard erstellen** den **&#x200B;**&#x200B;Namen“ und die **Beschreibung** des Dashboards ein.

1. Klicken Sie auf **Erstellen**.

1. Wählen Sie im **Bericht hinzufügen** die Option **Bericht erstellen** aus.

1. Klicken Sie auf der linken Seite auf **Diagramm**.

1. Klicken Sie oben rechts auf **Bericht erstellen**.

1. Gehen Sie wie folgt vor, um den Abschnitt **Details** zu konfigurieren:

   1. Geben Sie einen Bericht **Name** ein (z. B. *Überfällige Aufgaben nach Projektbesitzer*).

   1. Einen Bericht eingeben **Beschreibung**.

1. Gehen Sie wie folgt vor, um den Abschnitt **Diagramm erstellen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Diagramm erstellen**.

   1. Wählen **in der Dropdown** Liste „Diagrammtyp“ die Option **Spalte** aus.

   1. Wählen Sie in **Dropdown-** „Spaltentyp“ die Option **Einfach**.

   1. Klicken Sie auf **Feld aktualisieren** unter dem Abschnitt **Untere (X) Achse** und wählen Sie dann das Feld **Aufgabe** > **Projekt** > **Inhaber** > **Name** aus.

      ![Feld aktualisieren](assets/bottom-x-axis.png)

   1. Klicken Sie auf **Feld auswählen** unter dem Abschnitt **Linke (Y) Achse** und suchen Sie dann das Feld **Aufgabe** > **Name** und wählen Sie es aus.

   1. Wählen **in der Dropdown** Liste Aggregationstyp die Option **Anzahl** aus.

      ![Feld vom Typ Aggregation](assets/left-y-axis.png)

1. Gehen Sie wie folgt vor, um den Abschnitt **Filter** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Filter**.

   1. Wählen Sie **Filter bearbeiten** aus.

   1. Klicken Sie **Bedingung hinzufügen**.

   1. Klicken Sie in den leeren Bedingungsbereich und wählen Sie dann **Feld auswählen**.

   1. Wählen Sie das Feld **Prozent abgeschlossen** aus.

   1. Wählen Sie in **Dropdown** Benutzer“ die Option **Kleiner als** aus und geben Sie dann *100* in das Feld „Evaluator“ ein.

   1. Klicken Sie **Bedingung hinzufügen** und dann **Feld auswählen**.

   1. Wählen Sie **Feld „Geplantes**&quot; aus.

   1. Wählen Sie in **Dropdown** Liste „Benutzer“ die Option **Kleiner als** aus.

   1. Schalten Sie **Relatives Datum festlegen** auf **EIN**.

   1. Geben Sie *$$TODAY* in das Feld „Evaluator“ ein.

      Weitere Informationen zu Platzhaltern finden Sie im Abschnitt Datumsbasierte Platzhalterfiltervariablen im Artikel [Bearbeiten von Berichtsfiltern in einem Arbeitsflächen-Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md) .

      ![Evaluator-Feld](assets/add-condition.png)

1. Gehen Sie wie folgt vor, um den Abschnitt **Spalteneinstellungen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Drilldown-**![Spalten](assets/drilldown-column.png) . Die Felder aus dem Diagramm werden automatisch als Spalten im Vorschauabschnitt auf der rechten Seite angezeigt.

   1. Klicken Sie **Spalte hinzufügen** und wählen Sie dann das Feld **Zugewiesen an** > **Name** aus.

   1. Klicken Sie **Spalte hinzufügen** und wählen Sie dann das Feld **Geplantes Startdatum** aus.

   1. Klicken Sie **Spalte hinzufügen** und wählen Sie dann das Feld **Geplantes Abschlussdatum** aus.

   1. Klicken Sie **Spalte hinzufügen** und wählen Sie dann das Feld **Datum der letzten Aktualisierung** aus.

   1. (Optional) Um die Aktualisierungszeit anzuzeigen, wählen Sie die Option **Letztes Aktualisierungsdatum** im Feld **Aktuelle Spalten** und wählen Sie dann eine Zeitwertoption in der Dropdown-Liste **Datumsformat** aus.

1. Gehen Sie wie folgt vor, um den Abschnitt **Drilldown-Gruppeneinstellungen** zu konfigurieren:

   1. Klicken Sie im linken Bereich auf das Symbol **Gruppeneinstellungen** ![Gruppeneinstellungen](assets/drilldown-group-icon.png) .

   1. Klicken Sie auf **Gruppierung hinzufügen** und wählen Sie dann das Feld **Projekt** > **Name** aus.

1. Klicken Sie **Speichern**, um den Bericht zu erstellen und zum Dashboard hinzuzufügen.

## Überlegungen beim Erstellen eines Diagrammberichts

### Verwenden der Feldauswahl

Die **Abschnitte** Dropdown-Liste im Abschnitt **Diagramm erstellen** dient dazu, die Auswahl in einer Feldauswahl einzugrenzen, damit ein Objekt beim Erstellen eines Tabellenberichts leichter zu finden ist. Wählen Sie zunächst ein Basiseinheitsobjekt aus.

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