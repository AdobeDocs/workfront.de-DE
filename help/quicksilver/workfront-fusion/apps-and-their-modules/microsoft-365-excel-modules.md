---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2821'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Microsoft Office 365 Excel-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-365-excel-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Microsoft 365 Excel] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Microsoft office 365 Excel] verwenden zu können, benötigen Sie ein Microsoft-Konto.

## Informationen zur Microsoft Office 365 Excel-API

Der Microsoft Office 365 Excel-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v2.0.16</td> 
  </tr>
 </tbody> 
 </table>



## Verbinden des [!DNL Office 365 Excel]-Services mit [!DNL Workfront Fusion]

Anweisungen zum Verbinden Ihres [!DNL Office 365 Excel]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Einverständnisbildschirm für Berechtigungen alle Berechtigungen angezeigt, die zuvor der Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn ein Benutzer beispielsweise über die über den Excel-Connector gewährten Berechtigungen zum Lesen von Tabellen verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Einverständnisbildschirm für Berechtigungen sowohl die bereits erteilte Berechtigung zum Lesen von Tabellen als auch die neu erforderliche Berechtigung zum Schreiben von E-Mails an.

## [!DNL Microsoft Office 365 Excel] Module und ihre Felder

Beim Konfigurieren [!DNL Microsoft 365 Excel] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Microsoft 365 Excel] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ordner]</td> 
   <td> <p>Wählen Sie den Ordner aus, der auf neue Arbeitsmappen überwacht werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL filter]</p> </td> 
   <td> <p>Sie können einen Filter so einrichten, dass nur Arbeitsmappen überwacht werden, die die von Ihnen ausgewählten Kriterien erfüllen.</p> <p>Geben Sie für jeden Filter das Feld ein, das vom Filter ausgewertet werden soll, den Operator und den Wert, den der Filter zulassen soll. Sie können mehr als einen Filter verwenden, indem Sie AND- oder OR-Regeln hinzufügen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsmappen ein, die das Modul bei jedem Ausführungszyklus des Szenarios zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitsmappen suchen]

Dieses Aktionsmodul sucht nach [!DNL Excel] Arbeitsmappen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ordner]</td> 
   <td> <p>Wählen Sie den Ordner aus, in dem Sie nach Arbeitsmappen suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL filter]</p> </td> 
   <td> <p>Sie können einen Filter festlegen, um nur nach Arbeitsmappen zu suchen, die den von Ihnen ausgewählten Kriterien entsprechen.</p> <p>Geben Sie für jeden Filter das Feld ein, das vom Filter ausgewertet werden soll, den Operator und den Wert, den der Filter zulassen soll. Sie können mehr als einen Filter verwenden, indem Sie AND- oder OR-Regeln hinzufügen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsblättern ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitsmappe herunterladen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Arbeitsmappe für das Modul identifizieren möchten, das heruntergeladen werden soll.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL durch manuelle Eingabe einer ID]</strong> </p> <p>Geben Sie im Feld [!UICONTROL Arbeitsmappen-ID] die ID der spezifischen Arbeitsmappe ein, die das Modul herunterladen soll, oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL durch Auswahl aus dem Pfad]</strong> </p> <p>Wählen Sie im Feld [!UICONTROL Arbeitsmappe] die Arbeitsmappe aus, die das Modul herunterladen soll.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbeitsblatt

* [[!UICONTROL Arbeitsblattzeilen ansehen]](#watch-worksheet-rows)
* [[!UICONTROL Arbeitsblätter auflisten]](#list-worksheets)
* [[!UICONTROL Arbeitsblattzeilen auflisten]](#list-worksheet-rows)
* [[!UICONTROL Arbeitsblatt hinzufügen]](#add-a-worksheet)
* [[!UICONTROL Arbeitsblattzeile hinzufügen]](#add-a-worksheet-row)
* [[!UICONTROL Arbeitsblattzeile aktualisieren]](#update-a-worksheet-row)
* [[!UICONTROL Löschen einer Arbeitsblattzeile]](#delete-a-worksheet-row)

#### [!UICONTROL Arbeitsblattzeilen ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn dem Blatt eine neue Zeile hinzugefügt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt enthält, das auf neue Zeilen überwacht werden soll.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Excel-Blatt aus, das Sie auf neue Zeilen überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsblattzeilen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie diese.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Arbeitsblätter enthält, die das Modul auflisten soll.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsblättern ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitsblattzeilen auflisten]

Dieses Aktionsmodul ruft eine Liste von Zeilen im angegebenen Arbeitsblatt ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt mit den Zeilen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Zeilen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Arbeitsblattzeilen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie diese.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, der Sie ein Arbeitsblatt hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Geben Sie einen Namen für das neue Arbeitsblatt ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitsblattzeile hinzufügen]

Dieses Aktionsmodul fügt dem ausgewählten Arbeitsblatt eine neue Zeile hinzu.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt enthält, dem Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, dem Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Typ der eingegebenen Werte]</p> </td> 
   <td> <p>Wählen Sie den Typ des Werts aus, der in das Arbeitsblatt eingegeben werden soll. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL-Formeln]</strong> </p> <p> Excel versucht, den angegebenen Ausdruck auszuwerten. Die Namen der Funktionen in einer Formel sind in englischer Sprache. Beispiel: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formeln lokal]</strong> </p> <p>Excel versucht, den angegebenen Ausdruck auszuwerten. Die Funktionsnamen sind in der Sprache Ihres Excel-Programms angegeben. Beispiel: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL value]</strong> </p> <p>Excel wertet den Wert nicht aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Geben Sie für jede Spalte den Wert ein, den die Spalte in der neuen Zeile haben soll.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitsblattzeile aktualisieren]

Dieses Aktionsmodul aktualisiert eine vorhandene Arbeitsblattzeile.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt mit der Zeile enthält, die Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Zeile enthält, die Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Typ der eingegebenen Werte]</p> </td> 
   <td> <p>Wählen Sie den Typ des Werts aus, der in das Arbeitsblatt eingegeben werden soll. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL-Formeln]</strong> </p> <p> Excel versucht, den angegebenen Ausdruck auszuwerten. Die Namen der Funktionen in einer Formel sind in englischer Sprache. Beispiel: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formeln lokal]</strong> </p> <p>Excel versucht, den angegebenen Ausdruck auszuwerten. Die Funktionsnamen sind in der Sprache Ihres Excel-Programms angegeben. Beispiel: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL value]</strong> </p> <p>Excel wertet den Wert nicht aus. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row ID]</td> 
   <td>Wählen Sie die Nummer der zu aktualisierenden Zeile aus.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Geben Sie für jede Spalte den Wert ein, den die Spalte in der neuen Zeile haben soll.</td>
   --&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen einer Arbeitsblattzeile]

Dieses Aktionsmodul löscht eine Zeile aus einem Arbeitsblatt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt mit der zu löschenden Zeile enthält.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt]</td>
   <td> <p> Wählen Sie das Arbeitsblatt aus, das die Zeile enthält, die Sie löschen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row ID]</td>
   <td>Geben Sie die ID der Zeile ein, die Sie löschen möchten, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>

### Tabelle

* [[!UICONTROL Überwachen von Tabellenzeilen]](#watch-table-rows)
* [[!UICONTROL Tabellen auflisten]](#list-tables)
* [[!UICONTROL Tabellenzeilen auflisten]](#list-table-rows)
* [[!UICONTROL Tabelle abrufen]](#get-a-table)
* [[!UICONTROL Tabelle hinzufügen]](#add-a-table)
* [[!UICONTROL Tabellenzeile hinzufügen]](#add-a-table-row)
* [[!UICONTROL Aktualisieren einer Tabelle]](#update-a-table)
* [[!UICONTROL Tabelle löschen]](#delete-a-table)

#### [!UICONTROL Überwachen von Tabellenzeilen]

Dieser Trigger startet ein Szenario, wenn einer Tabelle eine neue Zeile hinzugefügt wird.

>[!NOTE]
>
>Die Tabelle hier verweist auf das eingebettete Tabellenelement in der Arbeitsmappe. Nicht die gesamte Tabelle (Arbeitsmappe/Blatt).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Arbeitsmappe]</p> </td> 
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Tabelle enthält, die Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p> Wählen Sie das Arbeitsblatt aus, das die Tabelle enthält, die Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Tabelle]</p> </td> 
   <td> <p>Wählen Sie die Tabelle aus, die Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Zeilen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Tabellen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die aufzulistenden Tabellen enthält</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Tabellen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Tabelle mit den Zeilen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Tabelle mit den Zeilen enthält, die Sie auflisten möchten</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Tabelle] </td>
   <td> <p>Wählen Sie die Tabelle aus, die die Zeilen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Geben Sie die maximale Anzahl von Tabellenzeilen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
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
     <p >[!UICONTROL-Verbindung]</p>
   </td> 
   <td> 
     <p>Anweisungen zum Verbinden Ihres Office 365-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Tabelle abrufen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Tabelle identifizieren möchten, die Sie abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Manuell eingeben]</strong> </p> <p>Geben Sie im Feld [!UICONTROL Arbeitsmappen-ID] die ID der Arbeitsmappe ein, die die abzurufende Tabelle enthält, oder ordnen Sie sie zu.</p> <p>Geben Sie im Feld [!UICONTROL Tabellenname] den Namen der Tabelle ein, die Sie abrufen möchten, oder ordnen Sie ihn zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Aus der Liste auswählen]</strong> </p> <p>Wählen Sie die Arbeitsmappe und das Arbeitsblatt aus, die die abzurufende Tabelle enthalten, und wählen Sie dann die Tabelle aus.</p> </li> 
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
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Arbeitsmappe] </td> 
   <td> <p>Wählen Sie die Arbeitsmappe aus, die das Arbeitsblatt enthält, dem Sie eine Tabelle hinzufügen möchten.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL-Adresse]</p> </td> 
   <td> <p>Legen Sie die Größe der Tabelle fest, indem Sie die oberen linken und unteren rechten Zellen angeben. Beispiel: <code>A1:C10</code> erstellt eine Tabelle mit 3 Spalten und 10 Zeilen.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Arbeitsmappe] </td>
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Tabelle enthält, der Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Arbeitsblatt] </td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Tabelle enthält, der Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL-Tabelle]</td>
   <td>Wählen Sie die Tabelle aus, der Sie eine Zeile hinzufügen möchten.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Geben Sie für jede Spalte den Wert ein, den die Spalte in der neuen Zeile haben soll.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Row ID]</p> </td> 
   <td> <p>Um eine Zeile an einer bestimmten Position in der Tabelle hinzuzufügen, geben Sie eine Zeilennummer ein oder ordnen Sie sie zu. Das Modul fügt die neue Zeile nach dieser Zeile ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren einer Tabelle]

Dieses Aktionsmodul aktualisiert eine vorhandene Tabelle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle aktualisieren]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Tabelle identifizieren möchten, die Sie aktualisieren möchten.</p> 
    <ul> 
     <li> <p><strong>Manuell eingeben</strong> </p> <p>Geben Sie im Feld [!UICONTROL Arbeitsmappen-ID] die ID der Arbeitsmappe ein, die die Tabelle enthält, die Sie aktualisieren möchten, oder ordnen Sie sie zu.</p> <p>Geben Sie im Feld [!UICONTROL Tabellenname] den Namen der Tabelle ein, die Sie aktualisieren möchten, oder ordnen Sie ihn zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Aus der Liste auswählen]</strong> </p> <p>Wählen Sie die Arbeitsmappe und das Arbeitsblatt aus, die die zu aktualisierende Tabelle enthalten, und wählen Sie dann die Tabelle aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Tabelle] </td> 
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
   <td role="rowheader">[!UICONTROL Gesamtwerte anzeigen]</td> 
   <td>Aktivieren Sie diese Option, um die Gesamtwerte der Tabelle anzuzeigen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Stil]</td> 
   <td>Wählen Sie einen Stil für die neue Tabelle.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabelle löschen]

Dieses Aktionsmodul löscht die angegebene Tabelle aus einem [!DNL Excel].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL, Tabelle abrufen]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Tabelle identifizieren möchten, die Sie löschen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Manuell eingeben]</strong> </p> <p>Geben Sie im Feld [!UICONTROL Arbeitsmappen-ID] die ID der Arbeitsmappe ein, die die zu löschende Tabelle enthält, oder ordnen Sie sie zu.</p> <p>Geben Sie im Feld [!UICONTROL Tabellenname] den Namen der Tabelle ein, die Sie löschen möchten, oder ordnen Sie ihn zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Aus der Liste auswählen]</strong> </p> <p>Wählen Sie die Arbeitsmappe und das Arbeitsblatt aus, die die zu löschende Tabelle enthalten, und wählen Sie dann die Tabelle aus.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

* [[!UICONTROL Daten abrufen]](#retrieve-data)
* [[!UICONTROL Erstellen eines API-Aufrufs]](#make-an-api-call)

#### [!UICONTROL Daten abrufen]

Diese Aktion ruft Daten aus dem definierten Arbeitsblattbereich ab und gibt für jede Zeile ein Bundle zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Arbeitsmappe] </td> 
   <td> <p>Wählen Sie die Arbeitsmappe aus, die die Daten enthält, die Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitsblatt] </td> 
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die abzurufenden Daten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Bereich] </td> 
   <td> <p>Geben Sie den Bereich des Blatts an, aus dem Sie Daten abrufen möchten, indem Sie die oberen linken und unteren rechten Zellen angeben. Beispiel: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines API-Aufrufs]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten API-Aufruf durchführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://graph.microsoft.com</code> ein. Beispiel:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Methode]</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kopfzeilen]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL body]</td> 
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:   <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
