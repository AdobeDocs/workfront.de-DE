---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Microsoft 365 Excel verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2577'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Microsoft 365 Excel], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Microsoft office 365 Excel]müssen Sie über ein Microsoft-Konto verfügen.

## [!DNL Microsoft Office 365 Excel] Module und ihre Felder

Bei der Konfiguration [!DNL Microsoft 365 Excel] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Microsoft 365 Excel] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Arbeitsmappe](#workbook)
* [Arbeitsblatt](#worksheet)
* [Tabelle](#table)
* [Sonstige](#other)

### Arbeitsmappe

* [Arbeitsmappen ansehen](#watch-workbooks)
* [Arbeitsmappen durchsuchen](#search-workbooks)
* [Arbeitsmappe herunterladen](#download-a-workbook)

#### [!UICONTROL Arbeitsmappen ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn eine Arbeitsmappe erstellt wird.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td> <p>Wählen Sie den Ordner aus, den Sie nach neuen Arbeitsmappen suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Sie können einen Filter festlegen, der nur auf Arbeitsmappen überwacht, die den von Ihnen ausgewählten Kriterien entsprechen.</p> <p>Geben Sie für jeden Filter das Feld, das der Filter auswerten soll, den Operator und den Wert ein, die der Filter zulassen soll. Sie können mehrere Filter verwenden, indem Sie UND- oder ODER-Regeln hinzufügen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsmappen ein oder ordnen Sie sie zu, die das Modul während des Ausführungszyklus eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitsmappen durchsuchen]

Dieses Aktionsmodul sucht nach [!DNL Excel] Arbeitsmappen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td> <p>Wählen Sie den Ordner aus, nach dem Sie nach Arbeitsmappen suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Sie können einen Filter festlegen, um nur nach Arbeitsmappen zu suchen, die den von Ihnen ausgewählten Kriterien entsprechen.</p> <p>Geben Sie für jeden Filter das Feld, das der Filter auswerten soll, den Operator und den Wert ein, die der Filter zulassen soll. Sie können mehrere Filter verwenden, indem Sie UND- oder ODER-Regeln hinzufügen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsblättern ein oder ordnen Sie sie zu, die das Modul während der Ausführung jedes Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitsmappe herunterladen]

Dieses Aktionsmodul lädt den Inhalt der angegebenen Excel-Arbeitsmappe herunter.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitsmappe herunterladen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Arbeitsmappe für das herunterzuladende Modul identifizieren möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Durch manuelles Eingeben einer Kennung]</strong> </p> <p>Geben Sie im Feld [!UICONTROL Arbeitsmappen-ID] die Kennung der Arbeitsmappe ein oder ordnen Sie sie zu, die das Modul herunterladen soll.</p> </li> 
     <li> <p><strong>[!UICONTROL Durch Auswahl aus dem Pfad]</strong> </p> <p>Wählen Sie im Feld [!UICONTROL Arbeitsmappe] die Arbeitsmappe aus, die das Modul herunterladen soll.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbeitsblatt

* [[!UICONTROL Tabellenzeilen ansehen]](#watch-worksheet-rows)
* [[!UICONTROL Arbeitsblätter auflisten]](#list-worksheets)
* [[!UICONTROL Zeilen eines Arbeitsblatts auflisten]](#list-worksheet-rows)
* [[!UICONTROL Arbeitsblatt hinzufügen]](#add-a-worksheet)
* [[!UICONTROL Eine Tabellenzeile hinzufügen]](#add-a-worksheet-row)
* [[!UICONTROL Eine Tabellenzeile aktualisieren]](#update-a-worksheet-row)
* [[!UICONTROL Eine Tabellenzeile löschen]](#delete-a-worksheet-row)

#### [!UICONTROL Tabellenzeilen ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn dem Blatt eine neue Zeile hinzugefügt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt enthält, das Sie für neue Zeilen überwachen möchten.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Excel-Blatt aus, das Sie für neue Zeilen überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsblattzeilen ein oder ordnen Sie sie zu, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitsblätter auflisten]

Dieses Aktionsmodul ruft eine Liste von Arbeitsblättern in der angegebenen Arbeitsmappe ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Arbeitsblätter enthält, die vom Modul aufgelistet werden sollen.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsblättern ein oder ordnen Sie sie zu, die das Modul während der Ausführung jedes Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Zeilen eines Arbeitsblatts auflisten]

Dieses Aktionsmodul ruft eine Liste von Zeilen im angegebenen Arbeitsblatt ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt mit den Zeilen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Zeilen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsblattzeilen ein oder ordnen Sie sie zu, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitsblatt hinzufügen]

Dieses Aktionsmodul erstellt ein neues Arbeitsblatt innerhalb der ausgewählten Arbeitsmappe.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, der Sie ein Arbeitsblatt hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Geben Sie einen Namen für das neue Arbeitsblatt ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Tabellenzeile hinzufügen]

Dieses Aktionsmodul fügt dem ausgewählten Arbeitsblatt eine neue Zeile hinzu.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt enthält, dem Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, dem Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Typ der eingegebenen Werte]</p> </td> 
   <td> <p>Wählen Sie den Werttyp aus, der in das Arbeitsblatt eingegeben werden soll. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formeln]</strong> </p> <p> Excel versucht, den angegebenen Ausdruck auszuwerten. Die Funktionsnamen in einer Formel sind in englischer Sprache. Beispiel: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formeln local]</strong> </p> <p>Excel versucht, den angegebenen Ausdruck auszuwerten. Die Funktionsnamen entsprechen der Sprache Ihrer Excel-Anwendung. Beispiel: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Wert]</strong> </p> <p>Excel wertet den Wert nicht aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Zeile]</td>
    <td>Geben Sie für jede Spalte den Wert ein, den die Spalte in der neuen Zeile enthalten soll.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Tabellenzeile aktualisieren]

Dieses Aktionsmodul aktualisiert eine vorhandene Arbeitsblattzeile.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt enthält, das die zu aktualisierende Zeile enthält.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die zu aktualisierende Zeile enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Typ der eingegebenen Werte]</p> </td> 
   <td> <p>Wählen Sie den Werttyp aus, der in das Arbeitsblatt eingegeben werden soll. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formeln]</strong> </p> <p> Excel versucht, den angegebenen Ausdruck auszuwerten. Die Funktionsnamen in einer Formel sind in englischer Sprache. Beispiel: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formeln local]</strong> </p> <p>Excel versucht, den angegebenen Ausdruck auszuwerten. Die Funktionsnamen entsprechen der Sprache Ihrer Excel-Anwendung. Beispiel: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Wert]</strong> </p> <p>Excel wertet den Wert nicht aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zeilen-ID]</td> 
   <td>Wählen Sie die Nummer der zu aktualisierenden Zeile aus.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Zeile]</td>
    <td>Geben Sie für jede Spalte den Wert ein, den die Spalte in der neuen Zeile enthalten soll.</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Tabellenzeile löschen]

Dieses Aktionsmodul löscht eine Zeile aus einem Arbeitsblatt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt enthält, das die zu löschende Zeile enthält.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt]</td>
   <td> <p> Wählen Sie das Arbeitsblatt aus, das die zu löschende Zeile enthält.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Zeilen-ID]</td>
   <td>Geben Sie die Kennung der Zeile ein, die Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### Tabelle

* [[!UICONTROL Tabellenzeilen anzeigen]](#watch-table-rows)
* [[!UICONTROL Tabellen auflisten]](#list-tables)
* [[!UICONTROL Tabellenzeilen auflisten]](#list-table-rows)
* [[!UICONTROL Tabelle abrufen]](#get-a-table)
* [[!UICONTROL Tabelle hinzufügen]](#add-a-table)
* [[!UICONTROL Tabellenzeile hinzufügen]](#add-a-table-row)
* [[!UICONTROL Tabelle aktualisieren]](#update-a-table)
* [[!UICONTROL Tabelle löschen]](#delete-a-table)

#### [!UICONTROL Tabellenzeilen anzeigen]

Dieser Trigger startet ein Szenario, wenn einer Tabelle eine neue Zeile hinzugefügt wird.

>[!NOTE]
>
>Die Tabelle hier bezieht sich auf das eingebettete Tabellenelement in der Arbeitsmappe. Nicht die gesamte Tabelle (Arbeitsmappe/Blatt).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Arbeitsmappe]</p> </td> 
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Tabelle enthält, die Sie sehen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p> Wählen Sie das Arbeitsblatt aus, das die zu überwachende Tabelle enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tabelle]</p> </td> 
   <td> <p>Wählen Sie die Tabelle aus, die Sie sehen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Zeilen ein oder ordnen Sie sie zu, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabellen auflisten]

Dieses Suchmodul ruft eine Liste aller Tabellenobjekte ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Tabellen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Tabellen enthält, die Sie auflisten möchten</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Tabellen ein oder ordnen Sie sie zu, die das Modul während der einzelnen Szenario-Ausführungszyklen zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabellenzeilen auflisten]

Dieses Suchmodul ruft eine Liste aller Tabellenzeilen in einer Arbeitsmappe ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Tabelle mit den Zeilen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Tabelle mit den Zeilen enthält, die Sie auflisten möchten</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Tabelle] </td>
   <td> <p>Wählen Sie die Tabelle aus, die die Zeilen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Tabellenzeilen ein oder ordnen Sie sie zu, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabelle abrufen]

Dieses Aktionsmodul ruft Metadaten für die angegebene Tabelle ab.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Verbindung]</p>
   </td> 
   <td> 
     <p>Anweisungen zum Verbinden Ihres Office 365-Kontos mit [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle abrufen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Tabelle identifizieren möchten, die Sie abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Manuell eingeben]</strong> </p> <p>Geben Sie im Feld [!UICONTROL Arbeitsmappen-ID] die Kennung der Arbeitsmappe ein oder ordnen Sie sie zu, die die abzurufende Tabelle enthält.</p> <p>Geben Sie im Feld [!UICONTROL Tabellenname] den Namen der Tabelle ein, die Sie abrufen möchten, oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Aus Liste auswählen]</strong> </p> <p>Wählen Sie die Arbeitsmappe und das Arbeitsblatt aus, die die abzurufende Tabelle enthalten, und wählen Sie dann die Tabelle aus.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabelle hinzufügen]

Dieses Aktionsmodul erstellt ein Tabellenelement im Excel-Arbeitsblatt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitsmappe] </td> 
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt enthält, in das Sie eine Tabelle hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitsblatt] </td> 
   <td> <p>Wählen Sie das Arbeitsblatt aus, dem Sie eine Tabelle hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL hat Kopfzeilen]</td> 
   <td> <p>Aktivieren Sie diese Option, um die erste Zeile als Tabellenüberschriften zu definieren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Adresse]</p> </td> 
   <td> <p>Legen Sie die Größe der Tabelle fest, indem Sie die Zellen oben links und unten rechts angeben. Beispiel: <code>A1:C10</code> erstellt eine Tabelle mit 3 Spalten und 10 Zeilen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabellenzeile hinzufügen]

Dieses Aktionsmodul ändert eine vorhandene Tabelle.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Tabelle enthält, der Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Tabelle enthält, der Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Tabelle]</td>
   <td>Wählen Sie die Tabelle aus, der Sie eine Zeile hinzufügen möchten.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Zeile]</td>
    <td>Geben Sie für jede Spalte den Wert ein, den die Spalte in der neuen Zeile enthalten soll.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Zeilen-ID]</p> </td> 
   <td> <p>Um eine Zeile an einer bestimmten Position auf der Tabelle hinzuzufügen, geben Sie eine Zeilennummer ein oder ordnen Sie sie zu. Das Modul fügt die neue Zeile nach dieser Zeile ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabelle aktualisieren]

Dieses Aktionsmodul aktualisiert eine vorhandene Tabelle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle aktualisieren]</td> 
   <td> <p>Wählen Sie aus, wie Sie die zu aktualisierende Tabelle identifizieren möchten.</p> 
    <ul> 
     <li> <p><strong>Manuell eingeben</strong> </p> <p>Geben Sie im Feld [!UICONTROL Arbeitsmappen-ID] die Kennung der Arbeitsmappe ein oder ordnen Sie sie zu, die die zu aktualisierende Tabelle enthält.</p> <p>Geben Sie im Feld [!UICONTROL Tabellenname] den Namen der Tabelle ein, die Sie aktualisieren möchten, oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Aus Liste auswählen]</strong> </p> <p>Wählen Sie die Arbeitsmappe und das Arbeitsblatt aus, die die zu aktualisierende Tabelle enthalten, und wählen Sie dann die Tabelle aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle aus, die Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>Wenn Sie die Tabelle umbenennen möchten, geben Sie einen neuen Namen für die Tabelle ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kopfzeilen anzeigen]</td> 
   <td> <p>Aktivieren Sie diese Option, um die Kopfzeilen der aktualisierten Tabelle anzuzeigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Summen anzeigen]</td> 
   <td>Aktivieren Sie diese Option, um die Gesamtwerte der Tabelle anzuzeigen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stil]</td> 
   <td>Wählen Sie einen Stil für die neue Tabelle aus.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabelle löschen]

Dieses Aktionsmodul löscht die angegebene Tabelle aus einem [!DNL Excel] Arbeitsblatt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle abrufen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die zu löschende Tabelle identifizieren möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Manuell eingeben]</strong> </p> <p>Geben Sie im Feld [!UICONTROL Arbeitsmappen-ID] die Kennung der Arbeitsmappe ein oder ordnen Sie sie zu, die die zu löschende Tabelle enthält.</p> <p>Geben Sie im Feld [!UICONTROL Tabellenname] den Namen der Tabelle ein, die Sie löschen möchten, oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Aus Liste auswählen]</strong> </p> <p>Wählen Sie die Arbeitsmappe und das Arbeitsblatt aus, die die zu löschende Tabelle enthalten, und wählen Sie dann die Tabelle aus.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

* [[!UICONTROL Daten abrufen]](#retrieve-data)
* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)

#### [!UICONTROL Daten abrufen]

Diese Aktion ruft Daten aus dem definierten Arbeitsblattbereich ab und gibt für jede Zeile ein Bundle zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitsmappe] </td> 
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Daten enthält, die Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitsblatt] </td> 
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Daten enthält, die Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bereich] </td> 
   <td> <p>Geben Sie den Bereich des Arbeitsblatts an, aus dem Sie Daten abrufen möchten, indem Sie die Zellen oben links und unten rechts angeben. Beispiel: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten API-Aufruf durchführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu ein <code>https://graph.microsoft.com</code>. Beispiel:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:   <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
