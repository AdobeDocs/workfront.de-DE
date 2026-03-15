---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Daten exportieren
description: Sie können Adobe Workfront-Daten aus Listen, Berichten, Dashboards und Suchvorgängen exportieren.
author: Courtney
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '2252'
ht-degree: 2%

---

# Exportieren von Daten

<!-- Audited: 5/2025 -->

Sie können Adobe Workfront-Daten aus Listen, Berichten, Dashboards und Suchvorgängen exportieren.

Einige der Gründe für den Datenexport sind:

* Sie möchten einer Person außerhalb von Workfront eine Kopie Ihrer Daten bereitstellen.
* Die Ergebnisse eines Berichts sollen als Anlage an einen externen Benutzer gesendet werden.
* Sie möchten eine externe Sicherung Ihrer Workfront-Daten erstellen.
* Es gibt eine Beschränkung, sodass nur 2.000 Ergebnisse auf einer Seite innerhalb der Workfront-Web-Anwendung angezeigt werden können. Wenn Ihr Bericht mehr als 2.000 erzeugt, können Sie den Bericht in eines der verfügbaren Formate exportieren und alle Ergebnisse im Bericht in einer Liste anzeigen.

Sie können einen Bericht entweder manuell über die Workfront-Benutzeroberfläche exportieren oder einen Versand für einen Bericht planen, der zu einem späteren Zeitpunkt an Sie gesendet wird. Weitere Informationen zur Planung von bereitgestellten Berichten finden Sie unter [Übersicht über die Berichtlieferung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Die Angaben in diesem Artikel gelten nicht für folgende Ausfuhren:

* Exportieren von Informationen aus Diagrammberichten.

  Weitere Informationen zum Exportieren eines Diagrammberichts finden Sie unter [Diagramm zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exportieren von Informationen aus dem Gantt-Diagramm.

  Weitere Informationen zum Exportieren des Gantt-Diagramms finden Sie unter [Exportieren des Gantt-Diagramms nach PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exportieren von Informationen aus dem Ressourcenplaner.

  Weitere Informationen zum Exportieren der Informationen aus dem Ressourcenplaner finden Sie unter „Exportoption“ in [Ressourcenplaner-Navigationsübersicht](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
      <p>Leicht</p>
      <p>Überprüfung</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Berichte, Dashboards und Kalender zum Exportieren von Berichten</p> <p>Zugriff auf die Objekte, die Sie in einer Liste anzeigen, um die Liste zu exportieren, anzeigen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Ändern der Berechtigungen für einen Bericht oder ein Dashboard zum Exportieren des Berichts oder des Dashboards</p> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die Sie in einer Liste anzeigen, um die Liste zu exportieren</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Der Bericht muss erstellt werden, bevor Sie seine Daten exportieren können.

Weitere Informationen zum Erstellen von Berichten finden Sie unter [Erstellen eines benutzerdefinierten Berichts](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) oder [Erstellen einer Kopie eines Berichts](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Exportformate und -beschränkungen

### Exportformate {#export-formats}

Die Informationen können in folgenden Formaten exportiert werden:

* PDF (Hochformat oder Querformat)
* Excel
* Excel (.xlsx)
* Durch Tabulatoren getrennt

>[!NOTE]
>
>Dashboards können entweder gedruckt oder nur in eine PDF-Datei exportiert werden.

### Exportbeschränkungen {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Die Art und Weise, wie Berichte in Workfront angezeigt werden, sowie die Art und Weise, wie sie über einen manuellen Export, einen bereitgestellten Bericht oder über die API exportiert werden, sind verschiedenen Einschränkungen unterworfen.

* **50.000 Zellen:** Die maximale Anzahl von Zellen, die in einem Berichtsexport für Excel-Dateien zulässig ist.
* **50.000 Zeilen:** Die Anzahl der Datenzeilen, die in einem Berichtsexport für Dateien mit PDF und durch Tabulatoren getrennte Dateien zulässig ist.

   * Bei Excel-Dateien beträgt dieser Grenzwert **65.000 Zeilen**.
   * Bei Excel-Dateien (.xlsx) beträgt dieser Grenzwert **100.000 Zeilen**.
   * Diese Grenzwerte schließen die Spaltenüberschriften sowie Zeilen für Gruppierungen im Bericht aus. Wenn ein Bericht beispielsweise 6 Gruppierungen und 50.000 Datenzeilen enthält, enthält die exportierte Datei 50.000 Zeilen.

  >[!IMPORTANT]
  >
  >Das Exportieren eines Berichts, der einen Sammlungsverweis in einer Spalte enthält, kann zu einem Fehler führen, auch wenn der Bericht ansonsten innerhalb der aufgelisteten Exportbeschränkungen liegt. Wenn die referenzierte Auflistung zu groß ist, wird der Exportvorgang beendet und es wird ein Fehler ausgegeben.
  >
  >Um diesen Fehler zu vermeiden, schließen Sie entweder Spalten aus, die auf große Sammlungen verweisen, oder reduzieren Sie die Größe der referenzierten Sammlungen vor dem Export.

  Wenn Ihr Bericht mehr Elemente als diese Grenzwerte enthält, wird eine Fehlermeldung angezeigt, dass der Export nicht erfolgreich war. Reduzieren Sie die Anzahl der Elemente, die auf dem Bildschirm angezeigt werden, auf einen Wert, der kleiner oder gleich diesen Grenzwerten ist, damit Sie die Ergebnisse exportieren können.

  Wenn Ihr Bericht mehr als 50.000/65.000/100.000 Zeilen umfasst und Sie alle Daten exportieren möchten, empfehlen wir, Filter oder Eingabeaufforderungen zu verwenden, um kleinere Datenmengen zu erhalten und mehrere Exporte durchzuführen.

  Informationen zur Verwendung von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Informationen zur Verwendung von Eingabeaufforderungen finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Diese Beschränkungen gelten für:

   * Ein manueller Export eines Berichts.
   * Ein terminierter Bericht.
   * Ein Export über eine API-Integration.
   * Daten werden durch einen Kickstart exportiert.

     Weitere Informationen zum Exportieren von Daten über Kickstarts finden Sie unter [Exportieren von Daten aus Adobe Workfront über Kickstarts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >Sie können 50.000 Zeilen in einer Kickstart-Datei exportieren, die Daten jedoch nur in eine Excel-Formatdatei exportieren.

   * Exportieren von Nutzungsinformationen für ein Projekt.

     Weitere Informationen zum Exportieren von Nutzungsinformationen für ein Projekt finden Sie unter [Übersicht über den Bericht zur Ressourcenauslastung](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10 MB Dateigröße** Dateigrößenbeschränkung für exportierte Berichte, deren Bereitstellung geplant ist. Wenn eine exportierte Datei, die an eine E-Mail angehängt ist, größer als 5 MB ist, wird ein Link, über den die Datei heruntergeladen werden kann, anstelle des angehängten exportierten Berichts per E-Mail gesendet.
* **65.530 Hyperlinks:** Dies ist eine von Excel auferlegte Grenze für Dokumente, die mehr als 65.530 Hyperlinks enthalten. Diese Dokumente können nicht geöffnet werden, wenn sie manuell exportiert oder in einem zugestellten Bericht gesendet werden. Beachten Sie, dass ein Excel-Dokument möglicherweise nur 200 Datenzeilen enthält. Wenn das Dokument jedoch mehr als 65.530 Links enthält, wird es nicht geöffnet. Diese Beschränkung besteht nur für Excel-Dateien, nicht für die anderen unterstützten Formate.
* **256 Spalten**: Dies ist eine Beschränkung, die Excel für Dokumente vorschreibt, die mehr als 256 Spalten enthalten. Diese Dokumente können nicht manuell exportiert oder in einem bereitgestellten Bericht gesendet werden. Diese Beschränkung besteht nur für Excel-Dateien, nicht für die anderen unterstützten Formate.

  >[!IMPORTANT]
  >
  >Der Export eines Berichts, der eine Berichtsspalte enthält, kann zu einem Fehler führen, auch wenn der Bericht anderweitig innerhalb der aufgelisteten Exportbeschränkungen liegt.
  >
  >Wenn Sie die Exportfunktion verwenden, um einen Bericht mit einer Berichtsspalte für andere freizugeben, sollten Sie den Bericht stattdessen freigeben, indem Sie ihn veröffentlichen. Weitere Informationen zum Veröffentlichen eines Berichts finden Sie unter [Freigeben eines Berichts in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
  >
  >Wenn Sie die Exportfunktion verwenden, um Daten extern auszuwerten, empfehlen wir stattdessen die Verwendung von Workfront Data Connect. Weitere Informationen finden Sie unter [Übersicht über Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

Wenn Sie versuchen, Daten über das Limit hinaus zu exportieren, erhalten Sie möglicherweise nicht alle erwarteten Daten im Export. Stattdessen wird ein geänderter Bericht innerhalb des Limits erstellt.

Darüber hinaus werden Berichte angehalten, deren Ausführung länger als 60 Minuten dauert.

Wenden Sie sich bei Problemen oder Problemen mit Ihrem Limit an den technischen Support von Workfront.

## Exportieren von Daten

### Exportieren von Daten aus einem Bericht oder einer Liste {#export-data-from-a-report-or-list}

1. Wechseln Sie zu dem Bericht oder der Liste, die Sie exportieren möchten.
1. Wählen Sie die Elemente aus, die Sie exportieren möchten. Wenn Sie einzelne Elemente auswählen, werden nur die ausgewählten Elemente exportiert.

   Wählen Sie beispielsweise in einem Projekt die Aufgaben aus, die Sie exportieren möchten.

   ODER

   Deaktivieren Sie alle Elemente, um die gesamte Liste zu exportieren.

1. Klicken Sie auf **Exportieren**, und wählen Sie dann ein Format aus.

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![Export dashboard note](assets/nwe-dashboard-export-note-350x271.png)
   -->

   ODER

   Klicken Sie auf das Symbol **Exportieren** ![Exportieren](assets/export-icon-nwe.png) und wählen Sie dann ein Format aus.

   Welche Optionen für den PDF-Export verfügbar sind, hängt von den E-Mail-Gebietsschemaeinstellungen in den Workfront-Benutzereinstellungen ab:

   * Nordamerika - Buchstabe - Querformat, Buchstabe - Hochformat, andere Größen

   * Alle Standorte außerhalb Nordamerikas - A4 - Landschaft, A4 - Hochformat, Andere Größen

1. (Bedingt) Abhängig vom verwendeten Betriebssystem haben Sie möglicherweise die Möglichkeit, die Datei zu öffnen oder zu speichern. Öffnen Sie die Datei mit der zugehörigen Anwendung oder speichern Sie sie auf Ihrer Festplatte.
1. Um zu verstehen, wie Informationen in der exportierten Datei angezeigt werden, lesen Sie den Abschnitt [Verwenden des exportierten Dokuments](#use-the-exported-document) in diesem Artikel.

### Exportieren von Daten aus einem Dashboard {#export-data-from-a-dashboard}

Sie können die Informationen von einem Dashboard aus drucken oder als PDF-Datei exportieren.

Weitere Informationen zum Exportieren von Daten aus einem Dashboard finden Sie unter [Dashboard exportieren](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## Exportiertes Dokument verwenden {#use-the-exported-document}

In den folgenden Abschnitten wird beschrieben, wie Informationen in einer exportierten Datei angezeigt werden:

* [Dateinamen](#file-names)
* [Titel](#titles)
* [Zeitstempel](#timestamps)
* [Formatierung](#formatting)
* [Verknüpfungen](#links)
* [Branding](#branding)

### Dateinamen {#file-names}

Unabhängig davon, ob Sie eine Liste von Objekten oder einen Bericht exportieren, hat die exportierte Datei einen Dateinamen und einen Titel. Sie können die exportierte Datei auf Ihrem Computer finden, indem Sie auf den Dateinamen verweisen. Der Titel des Berichts gibt Benutzern einen Hinweis darauf, was die exportierte Datei darstellt, wenn Sie sie für sie freigeben.

#### Dateinamen für exportierte Listen {#file-names-for-exported-lists}

Wenn Sie eine Liste von Objekten exportieren, wird der Objekttyp in der exportierten Datei im Dateinamen und im Titel der Liste angezeigt.

Wenn Sie eine Liste von Aufgaben oder Problemen exportieren, kann der **Dateiname** einer der folgenden sein:

* Wenn Sie Aufgaben- und Problemlisten in ein Projekt exportieren:

   * *Der_Projektname_Exportierte_Aufgaben*(*) in PDF, Excel, Excel (.xlsx) oder tabulatorgetrennten Formaten)*
   * *THE_PROJECT_NAME_EXPORTED_ISSUES*(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

* Beim Exportieren von Aufgaben- und Problemlisten in eine Aufgabe (Teilaufgaben):

   * **The_project_name_the_task_name_exported_Tasks**(*in PDF, Excel, Excel (.xlsx) oder tabulatorgetrennten Formaten)*
   * **The_project_name_the_task_name_exported_Issues**(*in PDF, Excel, Excel (.xlsx) oder tabulatorgetrennten Formaten)*

Wenn Sie eine Liste aller anderen Objekte aus einem Projekt in eine PDF-Datei exportieren, gibt der Dateiname des exportierten Dokuments den Typ der exportierten Objekte an.\
Der Dateiname kann beispielsweise wie folgt lauten:

* *Exportierte_Benutzer* beim Exportieren der Registerkarte „Personen“ im Projekt (*in PDF, Excel, Excel (.xlsx) oder tabulatorgetrennten Formaten)*
* *Exportierte_Risiken* beim Exportieren einer Liste von Risiken für das Projekt (*in PDF, Excel, Excel (.xlsx) oder tabulatorgetrennten Formaten)*

#### Dateinamen für exportierte Berichte {#file-names-for-exported-reports}

Wenn Sie einen Bericht exportieren, lautet der Dateiname des exportierten Berichts:

*The_report_name*(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

### Titel {#titles}

Wenn Sie eine Liste von Objekten exportieren, hat nur die Datei im PDF-Format einen Titel. Wenn Sie eine Liste oder einen Bericht in Excel-, Excel- (.xlsx) oder tabulatorgetrennte Formate exportieren, verfügt die Datei über keinen Titel.

#### Titel für exportierte Listen {#titles-for-exported-lists}

Wenn Sie Aufgaben- und Problemlisten in einem Projekt in eine PDF-Datei exportieren, hat das exportierte Dokument einen der folgenden Titel:

* *Projektname - Exportierte Aufgaben*
* *Projektname - Exportierte Probleme*

Wenn Sie Aufgaben- und Problemlisten in einer Aufgabe in eine PDF-Datei exportieren, weist die Kachel des exportierten Dokuments eine der folgenden Eigenschaften auf:

* *Projektname - Aufgabenname - Exportierte Aufgaben*
* *Projektname - Aufgabenname - Exportierte Probleme*

Wenn Sie eine Liste aller anderen Objekte aus einem Projekt in eine PDF-Datei exportieren, gibt der Titel des exportierten Dokuments den Typ der exportierten Objekte an.\
Der Titel kann beispielsweise lauten:

* *Exportierte Benutzer* beim Exportieren der Registerkarte „Personen“ im Projekt.
* *Exportierte Risiken* beim Exportieren einer Liste von Risiken für das Projekt.

#### Titel für exportierte Berichte {#titles-for-exported-reports}

Ein Bericht, der in eine PDF-Datei exportiert wird, hat einen Titel.

Wenn der Bericht in Excel-, Excel- (.xlsx) oder tabulatorgetrennte Formate exportiert wird, hat der exportierte Bericht keinen Titel. Der Titel der exportierten Datei ist der Name des Berichts, wie er in der Workfront-Webanwendung angezeigt wird.

Wenn der Bericht eine Beschreibung enthält, wird diese in die exportierte Datei aufgenommen.

### Zeitstempel {#timestamps}

Im exportierten Dokument wird ein Zeitstempel aus dem Kontext des Benutzers angezeigt, der das Element exportiert hat.

Der Zeitstempel enthält:

* Datum
* Zeit
* Zeitzone, in der das Element exportiert wurde

Je nach Typ des zu exportierenden Dokuments werden Zeitstempel an verschiedenen Stellen angezeigt:

* **PDF:** Zeitstempel werden in der Fußzeile jeder Seite und im Dateinamen angezeigt.
* **Excel:** Zeitstempel werden im Dateinamen angezeigt.

### Formatierung {#formatting}

Wenn Sie ein Projekt in PDF exportieren, werden alle Teilaufgaben als Einrückung für ihre übergeordneten Aufgaben angezeigt. Exportierte Listen reduzieren keine übergeordneten Aufgaben.

Sie erhalten immer die Standardregisterkarte eines Berichts, wenn ein Bericht gesendet oder für einen Versand geplant wird, es sei denn, der Bericht hat eine spezielle Ansicht.

Wenn Ihr Bericht in der Web-Anwendung eine besondere Formatierung aufweist, sollte der Bericht mit der speziellen Formatierung bereitgestellt werden, wenn die Registerkarten Details und Matrix bereitgestellt werden. Dies gilt nur für PDF- und Excel-Dateien.

>[!NOTE]
>
>Wenn die zu exportierenden Daten freigegebene Spalten enthalten und Sie in ein durch Excel oder Tabulatoren getrenntes Format exportieren, werden diese Spalten in der exportierten Datei getrennt.

Weitere Informationen zum Anpassen der Formatierung in einem Bericht finden Sie unter [Verwenden der bedingten Formatierung in Ansichten](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Links {#links}

Links können auf jedes Objekt in Workfront verweisen, das Verknüpfungen unterstützt. Wenn Sie eine Liste in Workfront auf einen PDF exportieren, bleiben alle unterstützten Verknüpfungen, die im Originaldokument vorhanden sind, im exportierten Dokument live.

>[!TIP]
>
>Wenn die `valueformat=HTML` für eine benutzerdefinierte Feldspalte im Textmodus angezeigt wird und die Verknüpfungswerte nicht in einer exportierten PDF-Datei angezeigt werden, müssen Sie im Textmodus zusätzliche Codezeilen zu Ihrer Spalte eingeben.
>
>Wenn Sie beispielsweise über ein benutzerdefiniertes Feld namens „Open Q1 Projects“ verfügen, das Links enthält, fügen Sie den folgenden Code hinzu:
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Wenn Sie in ein Excel-Format exportieren, werden nur Verknüpfungen zu Objekten in Workfront in die exportierte Datei aufgenommen. Sie werden nur an Stellen unterstützt, an denen Sie Verknüpfungen in exportierten Excel-Dokumenten zulassen können, z. B. bei Berichtslieferungen.

## Branding {#branding}

>[!IMPORTANT]
>
>Das Branding gilt nur für Unternehmen, die noch nicht an Bord der Adobe Experience Cloud sind.
>
>Wenn Ihr Unternehmen bei Adobe Experience Cloud integriert wurde, ist kein Branding verfügbar.

Wenn Ihr Workfront-Administrator Ihrer Workfront-Instanz ein benutzerdefiniertes Branding für die globale Navigationsleiste hinzugefügt hat, enthalten die exportierten PDF-Dateien auch Ihr personalisiertes Logo.

Daten, die in andere Formate exportiert werden, können nicht mit Ihrem Logo personalisiert werden.

Weitere Informationen zum Branding Ihrer Workfront-Instanz und der globalen Navigationsleiste finden Sie unter [Branding Ihrer Adobe Workfront-Instanz](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
