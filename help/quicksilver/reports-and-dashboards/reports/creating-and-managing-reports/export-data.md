---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Daten exportieren
description: Sie können Adobe Workfront-Daten aus verschiedenen Listen, Berichten, Dashboards und Suchvorgängen exportieren.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2164'
ht-degree: 0%

---

# Daten exportieren

<!-- Audited: 12/2023 -->

Sie können Adobe Workfront-Daten aus verschiedenen Listen, Berichten, Dashboards und Suchvorgängen exportieren.

Einige der Gründe für den Export von Daten sind:

* Sie möchten eine Kopie Ihrer Daten an eine Person außerhalb von Workfront übermitteln.
* Sie möchten die Ergebnisse eines Berichts als Anlage an einen externen Benutzer senden.
* Sie möchten eine externe Sicherung Ihrer Workfront-Daten erstellen.
* Innerhalb der Workfront-Webanwendung ist die Anzeige von nur 2.000 Ergebnissen auf einer Seite begrenzt. Wenn Ihr Bericht mehr als 2.000 Ergebnisse liefert, können Sie den Bericht in eines der verfügbaren Formate exportieren und alle Ergebnisse im Bericht in einer Liste anzeigen.

Sie können einen Bericht entweder manuell über die Benutzeroberfläche von Workfront exportieren oder einen Versand für einen Bericht planen. Dieser Bericht wird Ihnen zu einem späteren Zeitpunkt übermittelt. Weitere Informationen zur Planung bereitgestellter Berichte finden Sie unter [Übersicht über die Berichtbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Die Informationen in diesem Artikel gelten nicht für die folgenden Exporte:

* Exportieren von Informationen aus Diagrammberichten.

  Weitere Informationen zum Exportieren eines Diagrammberichts finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exportieren von Informationen aus der Gantt-Grafik.

  Weitere Informationen zum Exportieren des Gantt-Diagramms finden Sie unter [Exportieren des Gantt-Diagramms in PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exportieren von Informationen aus dem Ressourcenplaner.

  Weitere Informationen zum Exportieren der Informationen aus dem Ressourcenplaner finden Sie unter &quot;Exportoption&quot;in der Navigationsübersicht für den Ressourcenplaner [1}.](../../../resource-mgmt/resource-planning/resource-planner-navigation.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
    <p>Neu: Licht oder höher</p>
    <p>oder</p>
    <p>Aktuell: Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender oder höher zum Exportieren von Berichten anzeigen</p> <p>Zugriff auf die Objekte, die Sie in einer Liste anzeigen, um die Liste zu exportieren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder höherer Berechtigungen für einen Bericht oder ein Dashboard zum Exportieren des Berichts oder Dashboards</p> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die Sie in einer Liste anzeigen, um die Liste zu exportieren</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Der Bericht muss erstellt werden, bevor die Daten exportiert werden können.

Weitere Informationen zum Erstellen von Berichten finden Sie unter [Benutzerspezifischen Bericht erstellen](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) oder [Kopie eines Berichts erstellen](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Exportformate und -beschränkungen

### Exportformate {#export-formats}

Informationen können in den folgenden Formaten exportiert werden:

* PDF (Brief-Querformat oder Hochformat, Recht, Größer und A4)
* Excel (.xls)
* Excel (.xlsx)
* Durch Tabulatoren getrennt

>[!NOTE]
>
>Dashboards können entweder gedruckt oder nur in eine PDF-Datei exportiert werden.

### Ausfuhrbeschränkungen {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Die Anzeige von Berichten in Workfront sowie der Export durch einen manuellen Export, einen gelieferten Bericht oder über die API unterliegt verschiedenen Einschränkungen.

* **50.000 Zellen:** Die maximale Anzahl von Zellen, die in einem Berichtsexport für Excel-Dateien zulässig sind.
* **50.000 Zeilen:** Die Anzahl der Datenzeilen, die in einem Berichtsexport für PDF- und tabulatorgetrennte Dateien zulässig sind.

   * Bei Excel .xls-Dateien beträgt diese Beschränkung **65.000 Zeilen**.
   * Bei Excel .xlsx-Dateien beträgt diese Beschränkung **100.000 Zeilen**.
   * Diese Beschränkungen schließen die Spaltenüberschriften sowie die Zeilen für Gruppierungen im Bericht aus. Wenn beispielsweise ein Bericht 6 Gruppierungen und 50.000 Datenzeilen enthält, enthält die exportierte Datei 50.000 Zeilen.

  >[!IMPORTANT]
  >
  >Das Exportieren eines Berichts mit einer Kollektionsreferenz innerhalb einer Spalte kann zu einem Fehler führen, selbst wenn der Bericht ansonsten innerhalb der aufgeführten Exportbeschränkungen liegt. Wenn die referenzierte Sammlung zu groß ist, ist der Exportvorgang zeitaufwendig und führt anschließend zu einem Fehler.
  >
  >Um diesen Fehler zu vermeiden, schließen Sie vor dem Export Spalten aus, die auf große Sammlungen verweisen, oder reduzieren Sie die Größe der referenzierten Sammlungen.
  >

  Wenn Ihr Bericht mehr Elemente enthält, die diese Beschränkungen überschreiten, erhalten Sie eine Fehlermeldung, dass der Export nicht erfolgreich ist. Reduzieren Sie die Anzahl der Elemente auf dem Bildschirm auf eine Zahl, die kleiner oder gleich diesen Beschränkungen ist, um die Ergebnisse exportieren zu können.

  Wenn Ihr Bericht mehr als 50.000/65.000/100.000 Zeilen enthält und Sie alle Daten exportieren möchten, empfehlen wir, Filter oder Eingabeaufforderungen zu verwenden, um kleinere Datenmengen zu erhalten und mehrere Exporte durchzuführen.

  Informationen zur Verwendung von Filtern finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Informationen zur Verwendung von Eingabeaufforderungen finden Sie unter [Eine Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Diese Beschränkungen gelten für:

   * Ein manueller Export eines Berichts.
   * Ein terminierter Bericht.
   * Export über eine API-Integration.
   * Daten, die über einen Kick-Start exportiert wurden.

     Weitere Informationen zum Exportieren von Daten über Kick-Start finden Sie unter [Daten aus Adobe Workfront über Kick-Starts exportieren](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >Sie können 50.000 Zeilen in eine Kick-Start-Datei exportieren. Sie können die Daten jedoch nur in eine Excel-Formatdatei exportieren.

   * Exportieren von Nutzungsinformationen für ein Projekt.

     Weitere Informationen zum Exportieren von Nutzungsinformationen für ein Projekt finden Sie unter [Überblick über den Bericht &quot;Ressourcenauslastung&quot;](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10 MB Dateigröße:** Maximale Dateigröße für exportierte Berichte, die für die Bereitstellung geplant sind. Wenn eine an eine E-Mail angehängte exportierte Datei größer als 5 MB ist, wird ein Link, über den die Datei heruntergeladen werden kann, per E-Mail anstelle des angehängten exportierten Berichts gesendet.
* **65.530 Hyperlinks:** Dies ist eine Beschränkung, die Excel für Dokumente mit mehr als 65.530 Hyperlinks vorschreibt. Diese Dokumente können nicht geöffnet werden, wenn sie manuell exportiert oder in einem gelieferten Bericht gesendet werden. Beachten Sie, dass ein Excel-Dokument möglicherweise nur 200 Datenzeilen enthält. Wenn jedoch mehr als 65.530 Links innerhalb des Dokuments vorhanden sind, wird das Dokument nicht geöffnet. Diese Beschränkung gilt nur für Excel-Dateien, nicht aber für die anderen unterstützten Formate. 
* **256 Spalten**: Dies ist eine Begrenzung, die Excel für Dokumente mit mehr als 256 Spalten vorgibt. Diese Dokumente können nicht manuell exportiert oder in einem gelieferten Bericht gesendet werden. Diese Beschränkung gilt nur für Excel-Dateien, nicht aber für die anderen unterstützten Formate.

Wenn Sie versuchen, Daten über den Grenzwert hinaus zu exportieren, erhalten Sie möglicherweise nicht alle erwarteten Daten im Export. Stattdessen wird ein geänderter Bericht innerhalb der Grenze erstellt.

Darüber hinaus werden Berichte angehalten, deren Ausführung länger als 60 Minuten dauert.

Wenden Sie sich an den technischen Support von Workfront, wenn Sie Bedenken oder Probleme bezüglich Ihrer Beschränkung haben.

## Daten exportieren

### Daten aus einem Bericht oder einer Liste exportieren {#export-data-from-a-report-or-list}

1. Markieren Sie den Bericht oder die Liste, den/die Sie exportieren möchten.
1. Wählen Sie die Elemente aus, die Sie exportieren möchten. (Bei Auswahl einzelner Elemente werden nur die von Ihnen ausgewählten Elemente exportiert.)

   Wählen Sie beispielsweise in einem Projekt die Aufgaben aus, die Sie exportieren möchten.

   Oder

   Lassen Sie alle Elemente deaktiviert, um die gesamte Liste zu exportieren.

1. Klicken Sie auf **Exportieren** und wählen Sie dann ein Format aus.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![](assets/nwe-dashboard-export-note-350x271.png)
   -->

   Oder

   Klicken Sie auf das Symbol **Exportieren** ![Exportsymbol](assets/export-icon-nwe.png) und wählen Sie dann ein Format aus.

   Welche Optionen zum PDF-Export verfügbar sind, hängt von den Gebietsschemaeinstellungen in Ihren Workfront-Benutzereinstellungen ab:

   * Nordamerika - Buchstabe (Standard), legal, Ledger, A4

     <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * Alle Standorte außerhalb Nordamerikas - A3, A4 (Standard), Brief, legal, Ledger

     <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. (Bedingt) Je nach verwendetem Betriebssystem haben Sie möglicherweise die Möglichkeit, die Datei zu öffnen oder zu speichern. Öffnen Sie die Datei mit der zugehörigen Anwendung oder speichern Sie sie auf Ihrer Festplatte.
1. Fahren Sie mit [Verwenden des exportierten Dokuments](#use-the-exported-document) fort.

### Daten aus einem Dashboard exportieren {#export-data-from-a-dashboard}

Sie können die Informationen aus einem Dashboard drucken oder als PDF-Datei exportieren.

Weitere Informationen zum Exportieren von Daten aus einem Dashboard finden Sie unter [Dashboard exportieren](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Exportierte Dokumente verwenden {#use-the-exported-document}

* [Dateinamen](#file-names)
* [Titel](#titles)
* [Zeitstempel](#timestamps)
* [Formatierung](#formatting)
* [Links](#links)
* [Branding](#branding)

### Dateinamen {#file-names}

Unabhängig davon, ob Sie eine Liste von Objekten oder einen Bericht exportieren, enthält die exportierte Datei einen Dateinamen und einen Titel. Sie können die exportierte Datei auf Ihrem Computer finden, indem Sie auf den Dateinamen verweisen. Der Titel des Berichts gibt Benutzern einen Hinweis darauf, was die exportierte Datei darstellt, wenn Sie sie für sie freigeben.

#### Dateinamen für exportierte Listen {#file-names-for-exported-lists}

Wenn Sie eine Objektliste exportieren, wird der Objekttyp in der exportierten Datei im Dateinamen und im Titel der Liste angezeigt.

Wenn Sie eine Liste von Aufgaben oder Problemen exportieren, kann der **Dateiname** einer der folgenden sein:

* Wenn Sie Aufgaben- und Problemlisten in ein Projekt exportieren:

   * *The_project_name_Exported_Tasks*(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*
   * *The_project_name_Exported_Issues*(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

* Wenn Sie Aufgaben- und Problemlisten in eine Aufgabe (Unteraufgaben) exportieren:

   * **The_project_name_the_task_name_Exported_Tasks**(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*
   * **The_project_name_the_task_name_Exported_Issues**(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

Wenn Sie eine Liste anderer Objekte aus einem Projekt in eine PDF-Datei exportieren, zeigt der Dateiname des exportierten Dokuments den Typ der exportierten Objekte an.\
Beispielsweise kann der Dateiname wie folgt lauten:

* *Exportierte_Benutzer*, beim Export der Registerkarte &quot;Personen&quot;im Projekt(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*
* *Exported_Risks*, beim Exportieren einer Liste von Risiken für das Projekt (*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

#### Dateinamen für exportierte Berichte {#file-names-for-exported-reports}

Wenn Sie einen Bericht exportieren, lautet der Dateiname des exportierten Berichts:

*The_report_name*(*in PDF, Excel, Excel (.xlsx) oder tabulatorgetrennten Formaten)*

### Titel {#titles}

Wenn Sie eine Objektliste exportieren, erhält nur die Datei im PDF-Format einen Titel. Wenn Sie eine Liste oder einen Bericht in die Formate Excel, Excel (.xlsx) oder Tabstopp-getrennte Dateien exportieren, hat die Datei keinen Titel.

#### Titel für exportierte Listen {#titles-for-exported-lists}

Wenn Sie Aufgaben- und Problemlisten in ein Projekt in eine PDF-Datei exportieren, lautet der Titel des exportierten Dokuments einer der folgenden:

* *Projektname - Exportierte Aufgaben*
* *Projektname - Exportierte Probleme*

Wenn Sie Aufgaben- und Problemlisten in einer Aufgabe in eine PDF-Datei exportieren, ist die Kachel des exportierten Dokuments eine der folgenden:

* *Projektname - Aufgabenname - Exportierte Aufgaben*
* *Projektname - Aufgabenname - Exportierte Probleme*

Wenn Sie eine Liste anderer Objekte aus einem Projekt in eine PDF-Datei exportieren, zeigt der Titel des exportierten Dokuments den Typ der exportierten Objekte an.\
Der Titel kann beispielsweise wie folgt lauten:

* *Exportierte Benutzer* beim Export der Registerkarte &quot;Personen&quot;im Projekt.
* *Exportierte Risiken* beim Exportieren einer Liste von Risiken im Projekt.

#### Titel für exportierte Berichte {#titles-for-exported-reports}

Ein Bericht, der in eine PDF-Datei exportiert wird, hat einen Titel.

Wenn der Bericht in die Formate Excel, Excel (.xlsx) oder Tabulator-Getrennt exportiert wird, hat der exportierte Bericht keinen Titel. Der Titel der exportierten Datei ist der Name des Berichts, wie er in der Workfront-Webanwendung angezeigt wird.

Wenn der Bericht eine Beschreibung enthält, wird er in die exportierte Datei aufgenommen.

### Zeitstempel {#timestamps}

Ein Zeitstempel wird auf dem exportierten Dokument aus dem Kontext des Benutzers angezeigt, der das Element exportiert hat.

Der Zeitstempel umfasst:

* Datum
* Uhrzeit
* Zeitzone des Artikelexports

Je nach Dokumenttyp werden Zeitstempel an verschiedenen Stellen angezeigt:

* **PDF:** Zeitstempel werden in der Fußzeile jeder Seite und im Dateinamen angezeigt.
* **Excel:** Zeitstempel werden im Dateinamen angezeigt.

### Formatierung {#formatting}

Wenn Sie ein Projekt in .pdf exportieren, werden alle Unteraufgaben als eingerückt zu ihren übergeordneten Aufgaben angezeigt. Exportierte Listen reduzieren keine übergeordneten Aufgaben.

Sie erhalten immer den Standard-Tab eines Berichts, wenn ein Bericht gesendet oder für einen Versand geplant wird, es sei denn, der Bericht verfügt über eine spezielle Ansicht.

Wenn Ihr Bericht in der Webanwendung eine besondere Formatierung aufweist, sollte der Bericht bei der Auslieferung der Registerkarten Details und Matrix mit der speziellen Formatierung bereitgestellt werden, nur für PDF- und Excel-Dateien.

>[!NOTE]
>
>Wenn die zu exportierenden Daten gemeinsame Spalten enthalten und Sie sie in ein Excel- oder Tabulator-Format exportieren, werden diese Spalten in der exportierten Datei getrennt.

Weitere Informationen zum Anpassen der Formatierung in einem Bericht finden Sie unter [Bedingte Formatierung in Ansichten verwenden](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Links {#links}

Links können auf jedes Objekt in Workfront verweisen, das Verknüpfungen unterstützt. Wenn Sie eine Liste in Workfront in .pdf exportieren, bleiben alle unterstützten Links, die im Originaldokument vorhanden sind, im exportierten Dokument erhalten.

>[!TIP]
>
>Wenn die Zeile `valueformat=HTML` im Textmodus für eine benutzerdefinierte Feldspalte angezeigt wird und die Link-Werte nicht in einer exportierten PDF-Datei angezeigt werden, müssen Sie im Textmodus zusätzliche Codezeilen für Ihre Spalte eingeben.
>
>Wenn Sie beispielsweise über ein benutzerdefiniertes Feld namens Open Q1 Projects verfügen, das Links enthält, fügen Sie den folgenden Code hinzu:
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Wenn Sie in ein Excel-Format exportieren, werden nur Links zu Objekten in Workfront in die exportierte Datei aufgenommen und nur an Stellen unterstützt, an denen Sie Links in exportierten Excel-Dokumenten zulassen können, z. B. Berichtbereitstellungen.

## Branding {#branding}

>[!IMPORTANT]
>
>Branding gilt nur für Unternehmen, die noch nicht in Adobe Experience Cloud integriert sind.
>
>Wenn Ihr Unternehmen in Adobe Experience Cloud integriert wurde, ist kein Branding verfügbar.

Wenn Ihr Workfront-Administrator Ihrer Workfront-Instanz für die globale Navigationsleiste ein benutzerdefiniertes Branding hinzugefügt hat, enthalten die exportierten PDF-Dateien auch Ihr personalisiertes Logo.

Daten, die in andere Formate exportiert werden, können nicht mit Ihrem Logo personalisiert werden.

Weitere Informationen zum Branding Ihrer Workfront-Instanz und der globalen Navigationsleiste finden Sie unter [Markieren Ihrer Adobe Workfront-Instanz](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
