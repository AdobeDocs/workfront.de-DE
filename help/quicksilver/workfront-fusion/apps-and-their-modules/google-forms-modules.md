---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Google Forms-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 0%

---

# [!DNL Google Forms]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Google Forms-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-forms-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit den [!DNL Adobe Workfront Fusion] [!DNL Google Forms] können Sie Antworten auf Ihre [!DNL Google Forms] überwachen, auswählen, hinzufügen, aktualisieren oder löschen.

Um [!DNL Google Docs] mit [!DNL Adobe Workfront Fusion] verwenden zu können, muss ein [!DNL Google] Konto vorhanden sein. Wenn Sie noch kein [!DNL Google] Konto haben, können Sie eines auf der Hilfeseite zum [!DNL Google] Konto erstellen.

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

Um [!DNL Google Forms]-Module verwenden zu können, müssen Sie über ein [!DNL Google]-Konto verfügen.

## Google Forms API-Informationen

Der Google Forms-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>2,0,10</td> 
  </tr>
 </tbody> 
 </table>

## Erstellen einer Tabelle aus dem Formular

Damit Sie mit Ihren Formularantworten arbeiten können, muss eine Tabelle aus Ihren Antworten erstellt werden.

1. Öffnen Sie das Formular.
1. Navigieren Sie zur Registerkarte **[!UICONTROL Antworten]** .
1. Klicken Sie auf **[!UICONTROL Symbol]** Tabelle erstellen![](assets/spreadsheet-icon.png).

1. Wählen Sie aus, ob Sie eine neue Tabelle oder eine vorhandene Tabelle erstellen möchten
1. Klicken Sie auf **[!UICONTROL Erstellen]**.

## [!DNL Google Forms] Module und ihre Felder

Beim Konfigurieren [!DNL Google Forms] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Google Forms] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### [!UICONTROL Antworten ansehen]

Überwacht das Formular auf neue Antworten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Tabelle]</td> 
   <td> <p>Wählen Sie die Tabelle aus, die die Antworten aus dem Formular enthält, auf das Sie auf neue Antworten achten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zeile mit Überschriften]</td> 
   <td>Geben Sie die Kopfzeile der Tabelle an. Die Standardzeile lautet <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wert rendern option]</td> 
   <td> <p>Geben Sie an, wie die Werte in der Ausgabe gerendert werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL formatierter Wert]</strong> </p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema der Tabelle, nicht auf dem Gebietsschema des anfragenden Benutzers. Wenn <code>A1</code> beispielsweise <code>1. 23</code> und <code>A2 </code>als Währung <code>=A1</code> und formatiert ist, gibt <code>A2</code> <code>$1. 23</code> zurück.</p> </li> 
     <li> <p><strong>[!UICONTROL Unformatted value]</strong> </p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn <code>A1</code> beispielsweise <code>1. 23</code> und <code>A2 </code>als Währung <code>=A1</code> und formatiert ist, gibt <code>A2</code> die Zahl <code>1. 23</code> zurück.</p> </li> 
     <li> <p><strong>[!UICONTROL-Formel]</strong> </p> <p>Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn <code>A1</code> beispielsweise <code>1. 23</code> und <code>A2 </code>als Währung <code>=A1</code> und formatiert ist, gibt <code>A2</code> <code>=A1</code> zurück.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Render-Option Datum und Uhrzeit]</td> 
   <td>Wählen Sie aus, wie Datum, Uhrzeit und Dauer in der Ausgabe dargestellt werden sollen. Dieses Feld wird ignoriert, wenn [!UICONTROL Value Render Option] auf [!UICONTROL Formatted Value] gesetzt ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Antworten fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeitet.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Antwort hinzufügen]](#add-a-response)
* [[!UICONTROL Aktualisieren einer Antwort]](#update-a-response)
* [[!UICONTROL Antwort löschen]](#delete-a-response)

#### [!UICONTROL Antwort hinzufügen]

Dieses Modul fügt eine neue Antwort an das untere Ende der Tabelle des Formulars an.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Tabelle]</td> 
   <td> <p>Wählen Sie das Arbeitsblatt aus, das das Arbeitsblatt enthält, dem Sie eine Antwort hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL-Werte]</p> </td> 
   <td> <p>Geben Sie die gewünschten Werte in die Tabellenspalten ein.</p> <p>Verwenden Sie für die Spalte [!UICONTROL Timestamp] im richtigen Format den folgenden Wert:</p><pre>formatDate(now;TT/MM/JJJJ hh:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL-Werteingabeoption]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL RAW]</strong> </p> <p> Die vom Benutzer eingegebenen Werte werden nicht geparst und unverändert gespeichert. </p> </li> 
     <li> <p><strong>[!UICONTROL Benutzer entered]</strong></p> <p>Die Werte werden analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, Zeichenfolgen können jedoch nach denselben Regeln, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets]-Benutzeroberfläche angewendet werden, in Zahlen, Daten oder andere Formate konvertiert werden.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Option zum Einfügen von Daten]</td> 
   <td> <p>Geben Sie an, wie vorhandene Daten bei der Eingabe neuer Daten geändert werden. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>Die neuen Daten überschreiben vorhandene Daten in den Bereichen, in denen sie geschrieben werden. Durch Hinzufügen von Daten am Ende des Arbeitsblatts werden neue Zeilen oder Spalten eingefügt, damit die Daten geschrieben werden können.</p> </li> 
     <li> <p><strong>[!UICONTROL Zeilen einfügen]</strong></p> <p>Für die neuen Daten werden Zeilen eingefügt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren einer Antwort]

Dieses Modul aktualisiert die ausgewählte Antwort.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Tabelle]</td> 
   <td> <p>Wählen Sie die Tabelle aus, die das Blatt enthält, in dem Sie eine Antwort aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Zeilennummer]</p> </td> 
   <td> <p>Geben Sie die Nummer der Zeile ein, die Sie aktualisieren möchten, oder mappen Sie sie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Werte]</p> </td> 
   <td> <p>Geben Sie die neuen Werte in die gewünschten Spalten ein.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL-Werteingabeoption]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL RAW]</strong> </p> <p> Die vom Benutzer eingegebenen Werte werden nicht geparst und unverändert gespeichert. </p> </li> 
     <li> <p><strong>[!UICONTROL Benutzer entered]</strong></p> <p>Die Werte werden analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, Zeichenfolgen können jedoch nach denselben Regeln, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets]-Benutzeroberfläche angewendet werden, in Zahlen, Daten oder andere Formate konvertiert werden.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Antwort löschen]

Dieses Modul löscht eine ausgewählte Antwort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Tabelle]</td> 
   <td> <p>Wählen Sie das Arbeitsblatt aus, das das Arbeitsblatt enthält, in dem Sie eine Antwort löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Zeilennummer]</p> </td> 
   <td> <p>Geben Sie die Nummer der Zeile ein, die Sie löschen möchten, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Suchantworten]](#search-responses)
* [[!UICONTROL Suchantworten (Erweitert])](#search-responses-advanced)

#### [!UICONTROL Suchantworten]

Dieses Modul gibt Antworten zurück, die den angegebenen Kriterien entsprechen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Verbindung</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL-Tabelle]</td>
   <td> <p>Wählen Sie das Formular aus, in dem Sie suchen möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Sheet] </td>
   <td> <p>Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Spaltenbereich]</td>
   <td> <p> Wählen Sie den Spaltenbereich aus, den Sie suchen möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL filter]</td> 
   <td> <p>Definieren Sie den Filter, nach dem Sie Antworten suchen möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Sortierreihenfolge] </td>
   <td> <p>Wählen Sie aus, ob die zurückgegebenen Antworten in auf- oder absteigender Reihenfolge sortiert werden sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Sortieren nach]</td>
   <td> <p> Wählen Sie die Spalte aus, nach der die zurückgegebenen Antworten sortiert werden sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Wert rendern option]</td> 
   <td> <p>Geben Sie an, wie die Werte in der Ausgabe gerendert werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL formatierter Wert]</strong></p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema der Tabelle, nicht auf dem Gebietsschema des anfragenden Benutzers. Wenn <code>A1</code> beispielsweise <code>1. 23</code> und <code>A2 </code>als Währung <code>=A1</code> und formatiert ist, gibt <code>A2</code> <code>$1. 23</code> zurück.</p> </li> 
     <li> <p><strong>[!UICONTROL Unformatted value]</strong> </p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn <code>A1</code> beispielsweise <code>1. 23</code> und <code>A2 </code>als Währung <code>=A1</code> und formatiert ist, gibt <code>A2</code> die Zahl <code>1. 23</code> zurück.</p> </li> 
     <li> <p><strong>[!UICONTROL-Formel]</strong> </p> <p>Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn <code>A1</code> beispielsweise <code>1. 23</code> und <code>A2 </code>als Währung <code>=A1</code> und formatiert ist, gibt <code>A2</code> <code>=A1</code> zurück.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Render-Option Datum und Uhrzeit]</td>
    <td>Wählen Sie aus, wie Datum, Uhrzeit und Dauer in der Ausgabe dargestellt werden sollen. Dieses Feld wird ignoriert, wenn die Option [!UICONTROL Value Render] auf Formatierter Wert gesetzt ist. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Maximale Anzahl der zurückgegebenen Antworten]</td>
   <td> <p> Legen Sie die maximale Anzahl von Antworten fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchantworten (erweitert)]

Dieses Modul führt eine Suche mit dem [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage) durch. Dieses Modul gibt keine Zeilennummer zurück.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL-Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL-Tabelle]</td>
   <td> <p>Wählen Sie das Arbeitsblatt aus, das das zu durchsuchende Arbeitsblatt enthält.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Sheet]</td>
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL filter]</td> 
   <td> <p>Definieren Sie die Suchabfrage mithilfe der <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Beispiel: <code>select * where C = "John"</code> ruft alle Werte für die Zeile ab, in der die Spalte C „John“ lautet.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Zeilen]</td>
   <td> <p> Legen Sie die maximale Anzahl von Antworten fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>
