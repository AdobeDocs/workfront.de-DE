---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Daten exportieren
description: Einige der Gründe für den Export von Daten sind - EDIT ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '2116'
ht-degree: 0%

---

# Daten exportieren

Sie können Adobe Workfront-Daten aus verschiedenen Listen, Berichten, Dashboards und Suchvorgängen exportieren.
Die Informationen in diesem Artikel gelten nicht für die folgenden Exporte:

* Exportieren von Informationen aus Diagrammberichten

   Weitere Informationen zum Exportieren eines Diagrammberichts finden Sie unter [Diagramm zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Exportieren von Informationen aus der Gantt-Grafik.

   Weitere Informationen zum Exportieren der Gantt-Grafik finden Sie unter [Gantt-Diagramm in PDF exportieren](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* Exportieren von Informationen aus dem Ressourcenplaner.

   Weitere Informationen zum Exportieren der Informationen aus dem Ressourcen-Planer finden Sie unter &quot;Exportoption&quot;in [Navigationsübersicht über den Ressourcenplaner](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Einige der Gründe für den Export von Daten sind:

* Sie möchten eine Kopie Ihrer Daten an eine Person außerhalb von Workfront übermitteln.
* Sie möchten die Ergebnisse eines Berichts als Anlage an einen externen Benutzer senden.
* Sie möchten eine externe Sicherung Ihrer Workfront-Daten erstellen.
* Innerhalb der Workfront-Webanwendung ist die Anzeige von nur 2.000 Ergebnissen auf einer Seite begrenzt. Wenn Ihr Bericht mehr als 2.000 Ergebnisse liefert, können Sie den Bericht in eines der unten genannten Formate exportieren und alle Ergebnisse im Bericht in einer Liste anzeigen lassen.

Sie können einen Bericht entweder manuell über die Benutzeroberfläche von Workfront exportieren oder einen Versand für einen Bericht planen, der Ihnen zu einem späteren Zeitpunkt übermittelt wird. Weitere Informationen zur Planung bereitgestellter Berichte finden Sie unter [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender oder höher zum Exportieren von Berichten anzeigen</p> <p>Zugriff auf die Objekte, die Sie in einer Liste anzeigen, um die Liste zu exportieren</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder höherer Berechtigungen für einen Bericht oder ein Dashboard, um den Bericht oder das Dashboard zu exportieren</p> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die Sie in einer Liste anzeigen, um die Liste zu exportieren</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzungen

Der Bericht muss erstellt werden, bevor die Daten exportiert werden können.

Weitere Informationen zum Erstellen von Berichten finden Sie unter [Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Exportformate und -beschränkungen

* [Exportformate](#export-formats)
* [Ausfuhrbeschränkungen](#export-limits)

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
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."])</p>
-->

Die Anzeige von Berichten in Workfront sowie der Export durch einen manuellen Export, einen gelieferten Bericht oder über die API unterliegt verschiedenen Einschränkungen.

* **50.000 Zeilen:** Die Anzahl der Datenzeilen, die in einem Berichtsexport für PDF- und tabulatorgetrennte Dateien zulässig sind.

   * Bei Excel .xls-Dateien beträgt diese Beschränkung **65.000 Zeilen**.
   * Bei Excel .xlsx-Dateien beträgt diese Beschränkung **100.000 Zeilen**.
   * Diese Beschränkungen schließen die Spaltenüberschriften sowie die Zeilen für Gruppierungen im Bericht aus. Wenn beispielsweise ein Bericht 6 Gruppierungen und 50.000 Zeilen oder Daten enthält, enthält die exportierte Datei 50.000 Zeilen.

   >[!NOTE]
   >
   >Wenn Ihr Bericht mehr Elemente enthält, die diese Beschränkungen überschreiten, erhalten Sie eine Fehlermeldung, dass der Export nicht erfolgreich ist. Reduzieren Sie die Anzahl der Elemente auf dem Bildschirm auf eine Zahl, die kleiner oder gleich diesen Beschränkungen ist, um die Ergebnisse exportieren zu können.

   Wenn Ihr Bericht mehr als 50.000/65.000/100.000 Zeilen enthält und Sie alle Daten exportieren möchten, empfehlen wir, Filter oder Eingabeaufforderungen zu verwenden, um kleinere Datenmengen zu erhalten und mehrere Exporte durchzuführen.

   Informationen zur Verwendung von Filtern finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   Informationen zur Verwendung von Eingabeaufforderungen finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Diese Beschränkungen gelten für:

   * Ein manueller Export eines Berichts.
   * Ein terminierter Bericht.
   * Export über eine API-Integration.
   * Daten, die über einen Kick-Start exportiert wurden.

      Weitere Informationen zum Exportieren von Daten über Schnellstarts finden Sie unter [Daten aus Adobe Workfront über Kick-Starts exportieren](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)

      >[!NOTE]
      >
      >Sie können 50.000 Zeilen in eine Kick-Start-Datei exportieren. Sie können die Daten jedoch nur in eine Excel-Formatdatei exportieren. 

   * Exportieren von Nutzungsinformationen für ein Projekt.

      Weitere Informationen zum Exportieren von Nutzungsinformationen für ein Projekt finden Sie unter [Übersicht über den Bericht &quot;Ressourcenauslastung&quot;](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **Dateigröße von 10 MB:** Dateigrößenbeschränkung für jeden exportierten Bericht, der für die Bereitstellung geplant ist. Wenn eine an eine E-Mail angehängte exportierte Datei größer als 5 MB ist, wird ein Link, über den die Datei heruntergeladen werden kann, per E-Mail anstelle des angehängten exportierten Berichts gesendet.
* **65.530 Hyperlinks:** Dies ist eine Beschränkung, die Excel für Dokumente mit mehr als 65.530 Hyperlinks vorschreibt. Diese Dokumente können nicht geöffnet werden, wenn sie manuell exportiert oder in einem gelieferten Bericht gesendet werden. Beachten Sie, dass ein Excel-Dokument möglicherweise nur 200 Datenzeilen enthält. Wenn jedoch mehr als 65.530 Links innerhalb des Dokuments vorhanden sind, wird das Dokument nicht geöffnet. Diese Beschränkung gilt nur für Excel-Dateien, nicht aber für die anderen unterstützten Formate. 
* **256 Spalten**: Dies ist eine Begrenzung, die Excel für Dokumente mit mehr als 256 Spalten vorschreibt. Diese Dokumente können nicht manuell exportiert oder in einem gelieferten Bericht gesendet werden. Diese Beschränkung gilt nur für Excel-Dateien, nicht aber für die anderen unterstützten Formate.

Wenn Sie versuchen, Daten über den Grenzwert hinaus zu exportieren, erhalten Sie möglicherweise nicht alle erwarteten Daten im Export. Stattdessen wird ein geänderter Bericht innerhalb der Grenze erstellt.

Darüber hinaus werden Berichte angehalten, deren Ausführung länger als 60 Minuten dauert.

Wenden Sie sich an den technischen Support von Workfront, wenn Sie Bedenken oder Probleme bezüglich Ihrer Beschränkung haben.

## Daten exportieren

* [Daten aus einem Bericht oder einer Liste exportieren](#export-data-from-a-report-or-list)
* [Daten aus einem Dashboard exportieren](#export-data-from-a-dashboard)

### Daten aus einem Bericht oder einer Liste exportieren {#export-data-from-a-report-or-list}

1. Markieren Sie den Bericht oder die Liste, den/die Sie exportieren möchten.
1. Wählen Sie die Elemente aus, die Sie exportieren möchten. (Bei Auswahl einzelner Elemente werden nur die von Ihnen ausgewählten Elemente exportiert.)

   Wählen Sie beispielsweise in einem Projekt die Aufgaben aus, die Sie exportieren möchten.

   Oder

   Lassen Sie alle Elemente deaktiviert, um die gesamte Liste zu exportieren.

1. Klicken **Export** und wählen Sie ein Format aus.

   >[!NOTE]
   Um einen Dashboard-Bericht zu exportieren, benötigen Sie eine Planungslizenz.\
   ![](assets/nwe-dashboard-export-note-350x271.png)

   Oder

   Klicken Sie auf **Export** icon ![](assets/export-icon-nwe.png)und wählen Sie ein Format aus.

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
1. Fahren Sie mit [Exportierte Dokumente verwenden](#use-the-exported-document).

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

* [Dateinamen für exportierte Listen](#file-names-for-exported-lists)
* [Dateinamen für exportierte Berichte](#file-names-for-exported-reports)

#### Dateinamen für exportierte Listen {#file-names-for-exported-lists}

Wenn Sie eine Objektliste exportieren, wird der Objekttyp in der exportierten Datei im Dateinamen und im Titel der Liste angezeigt.

Wenn Sie eine Liste von Aufgaben oder Problemen exportieren, wird die **Dateiname** kann einer der folgenden sein:

* Wenn Sie Aufgaben- und Problemlisten in ein Projekt exportieren:

   * *The_project_name_Exported_Tasks*(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*
   * *The_project_name_Exported_Issues*(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

* Wenn Sie Aufgaben- und Problemlisten in eine Aufgabe (Unteraufgaben) exportieren:

   * **Die_Projektname_die_Task_name_Exported_Tasks**(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*
   * **The_project_name_the_task_name_Exported_Issues**(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

Wenn Sie eine Liste anderer Objekte aus einem Projekt in eine PDF-Datei exportieren, zeigt der Dateiname des exportierten Dokuments den Typ der exportierten Objekte an.\
Beispielsweise kann der Dateiname wie folgt lauten:

* *Exportiert_Benutzer*, wenn Sie die Registerkarte Personen im Projekt (*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*
* *Exportierte_Risiken*, wenn eine Liste von Risiken für das Projekt exportiert wird (*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

#### Dateinamen für exportierte Berichte {#file-names-for-exported-reports}

Wenn Sie einen Bericht exportieren, lautet der Dateiname des exportierten Berichts:

*Der_Berichtsname*(*in PDF-, Excel-, Excel- (.xlsx) oder tabulatorgetrennten Formaten)*

### Titel {#titles}

Wenn Sie eine Objektliste exportieren, erhält nur die PDF-Datei einen Titel. Wenn Sie eine Liste oder einen Bericht in Excel, Excel (.xlsx) oder tabulatorgetrennte Formate exportieren, hat die Datei keinen Titel.

* [Titel für exportierte Listen](#titles-for-exported-lists)
* [Titel für exportierte Berichte](#titles-for-exported-reports)

#### Titel für exportierte Listen {#titles-for-exported-lists}

Wenn Sie Aufgaben- und Problemlisten in ein Projekt in eine PDF-Datei exportieren, lautet der Titel des exportierten Dokuments einer der folgenden:

* *Projektname - Exportierte Aufgaben*
* *Projektname - Exportierte Probleme*

Wenn Sie Aufgaben- und Problemlisten in eine PDF-Datei exportieren, ist die Kachel des exportierten Dokuments eine der folgenden:

* *Projektname - Aufgabenname - Exportierte Aufgaben*
* *Projektname - Aufgabenname - Exportierte Probleme*

Wenn Sie eine Liste anderer Objekte aus einem Projekt in eine PDF-Datei exportieren, zeigt der Titel des exportierten Dokuments den Typ der exportierten Objekte an.\
Der Titel kann beispielsweise wie folgt lauten:

* *Exportierte Benutzer*, wenn Sie die Registerkarte Personen im Projekt exportieren.
* *Exportierte Risiken*, wenn eine Liste von Risiken für das Projekt exportiert wird.

#### Titel für exportierte Berichte {#titles-for-exported-reports}

Ein Bericht, der in eine PDF-Datei exportiert wird, hat einen Titel.

Wenn der Bericht in Excel, Excel (.xlsx) oder tabulatorgetrennte Formate exportiert wird, hat der exportierte Bericht keinen Titel. Der Titel der exportierten Datei ist der Name des Berichts, wie er in der Workfront-Webanwendung angezeigt wird.

Wenn der Bericht eine Beschreibung enthält, wird er in die exportierte Datei aufgenommen.

### Zeitstempel {#timestamps}

Ein Zeitstempel wird auf dem exportierten Dokument aus dem Kontext des Benutzers angezeigt, der das Element exportiert hat.

Der Zeitstempel umfasst:

* Datum
* Uhrzeit
* Zeitzone, in der das Element exportiert wurde

Je nach Dokumenttyp werden Zeitstempel an verschiedenen Stellen angezeigt:

* **PDF:** Die Zeitstempel werden in der Fußzeile jeder Seite und im Dateinamen angezeigt.
* **Excel:** Im Dateinamen werden Zeitstempel angezeigt.

### Formatierung {#formatting}

Wenn Sie ein Projekt in .pdf exportieren, werden alle Unteraufgaben als eingerückt zu ihren übergeordneten Aufgaben angezeigt. Exportierte Listen reduzieren keine übergeordneten Aufgaben.

Sie erhalten immer den Standard-Tab eines Berichts, wenn ein Bericht gesendet oder für einen Versand geplant wird, es sei denn, der Bericht verfügt über eine spezielle Ansicht.

Wenn Ihr Bericht in der Webanwendung eine besondere Formatierung aufweist, sollte der Bericht mit der speziellen Formatierung bereitgestellt werden, wenn die Registerkarten Details und Matrix nur für PDF- und Excel-Dateien bereitgestellt werden.

>[!NOTE]
Wenn die zu exportierenden Daten gemeinsame Spalten enthalten und Sie sie in ein Excel- oder Tabulator-Format exportieren, werden diese Spalten in der exportierten Datei getrennt.

Weitere Informationen zum Anpassen der Formatierung in einem Bericht finden Sie unter [Bedingte Formatierung in Ansichten verwenden](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### Links {#links}

Links können auf jedes Objekt in Workfront verweisen, das Verknüpfungen unterstützt. Wenn Sie eine Liste in Workfront in .pdf exportieren, bleiben alle unterstützten Links, die im Originaldokument vorhanden sind, im exportierten Dokument erhalten.

>[!TIP]
Wenn die Zeile `valueformat=HTML` im Textmodus für eine Spalte mit benutzerdefiniertem Feld angezeigt wird und die Link-Werte nicht in einer exportierten PDF-Datei angezeigt werden, müssen Sie zusätzliche Codezeilen für Ihre Spalte im Textmodus eingeben.
Wenn Sie beispielsweise über ein benutzerdefiniertes Feld namens Open Q1 Projects verfügen, das Links enthält, fügen Sie den folgenden Code hinzu:

```
link.url=customDataLabelsAsString(Open Q1 Projects)
linkedname=direct
```

Wenn Sie in ein Excel-Format exportieren, werden nur Links zu Objekten in Workfront in die exportierte Datei aufgenommen und nur an Stellen unterstützt, an denen Sie Links in exportierten Excel-Dokumenten zulassen können, z. B. Berichtbereitstellungen.

## Branding {#branding}

Wenn Ihr Workfront-Administrator Ihrer Workfront-Instanz für die globale Navigationsleiste ein benutzerdefiniertes Branding hinzugefügt hat, enthalten die exportierten PDF-Dateien auch Ihr personalisiertes Logo.

Daten, die in andere Formate exportiert werden, können nicht mit Ihrem Logo personalisiert werden.

Weitere Informationen zum Branding Ihrer Workfront-Instanz und zur globalen Navigationsleiste finden Sie unter [Markieren Sie Ihre Adobe Workfront-Instanz.](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
