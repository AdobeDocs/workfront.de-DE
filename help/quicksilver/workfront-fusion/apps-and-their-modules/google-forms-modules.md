---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google Forms-Module
description: Die [!DNL Adobe Workfront Fusion Google Forms] -Module ermöglichen es Ihnen, Antworten in Ihrer Google Forms zu überwachen, auszuwählen, hinzuzufügen, zu aktualisieren oder zu löschen.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 0%

---

# [!DNL Google Forms]-Module

Die [!DNL Adobe Workfront Fusion] [!DNL Google Forms] -Module ermöglichen es Ihnen, Antworten auf Ihre [!DNL Google Forms].

Zur Verwendung [!DNL Google Docs] mit [!DNL Adobe Workfront Fusion], muss ein [!DNL Google] -Konto. Wenn Sie keine [!DNL Google] -Konto erstellen können, können Sie eines im [!DNL Google] Hilfeseite für Konten.

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Google Forms] -Module, müssen Sie über eine [!DNL Google] -Konto.

## Erstellen einer Tabelle aus dem Formular

Damit Sie mit Ihren Formulareinstellungen arbeiten können, muss die Tabelle aus Ihren Antworten erstellt werden.

1. Öffnen Sie Ihr Formular.
1. Navigieren Sie zu **[!UICONTROL Antworten]** Registerkarte.
1. Klicken Sie auf **[!UICONTROL Tabelle erstellen]** icon ![](assets/spreadsheet-icon.png).

1. Wählen Sie aus, ob Sie eine neue oder eine vorhandene Tabelle erstellen möchten
1. Klicken Sie auf **[!UICONTROL Erstellen]**.

## [!DNL Google Forms] Module und ihre Felder

Bei der Konfiguration [!DNL Google Forms] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Google Forms] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### [!UICONTROL Antworten ansehen]

Überprüft das Formular auf neue Antworten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Antworten aus dem Formular enthält, das Sie auf neue Antworten achten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zeile mit Kopfzeilen]</td> 
   <td>Geben Sie die Kopfzeile der Tabelle an. Die Standardzeile lautet <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>Geben Sie an, wie die Werte in der Ausgabe gerendert werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formatierter Wert]</strong> </p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema des Arbeitsblatts, nicht auf dem Gebietsschema des anfordernden Benutzers. Wenn beispielsweise <code>A1</code> is <code>1. 23</code> und <code>A2 </code>is <code>=A1</code> und als Währung formatiert, <code>A2</code> return <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Unformatierter Wert]</strong> </p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn beispielsweise <code>A1</code> is <code>1. 23</code> und <code>A2 </code>is <code>=A1</code> und als Währung formatiert, <code>A2</code> gibt die Zahl aus <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formel]</strong> </p> <p>Die Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn beispielsweise <code>A1</code> is <code>1. 23</code> und <code>A2 </code>is <code>=A1</code> und als Währung formatiert, <code>A2</code> return <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Renderoption für Datum und Uhrzeit</td> 
   <td>Wählen Sie aus, wie Datum, Uhrzeit und Dauer in der Ausgabe dargestellt werden sollen. Dieses Feld wird ignoriert, wenn [!UICONTROL Value Render Option] auf [!UICONTROL Formatierter Wert] gesetzt ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Antworten fest, die [!DNL Workfront Fusion] arbeitet mit während eines Zyklus zusammen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Eine Antwort hinzufügen]](#add-a-response)
* [[!UICONTROL Aktualisieren einer Antwort]](#update-a-response)
* [[!UICONTROL Antworten löschen]](#delete-a-response)

#### [!UICONTROL Eine Antwort hinzufügen]

Dieses Modul hängt eine neue Antwort an den unteren Rand des Formularkalkulationssatzes an.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p>Wählen Sie die Tabelle aus, die die Tabelle enthält, in der Sie eine Antwort hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Werte]</p> </td> 
   <td> <p>Geben Sie die gewünschten Werte in die Tabellenspalten ein.</p> <p>Verwenden Sie für die Spalte [!UICONTROL Timestamp] im richtigen Format den folgenden Wert:</p><pre>formatDate(now;DD/MM/JJJJ HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Werteingabe-Option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Die vom Benutzer eingegebenen Werte werden nicht analysiert und unverändert gespeichert. </p> </li> 
     <li> <p><strong>[!UICONTROL Benutzer eingegeben]</strong></p> <p>Die Werte werden so analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, aber Zeichenfolgen können in Zahlen, Datumsangaben oder andere Formate konvertiert werden, die den gleichen Regeln entsprechen, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets] Benutzeroberfläche.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Option "Daten einfügen"]</td> 
   <td> <p>Geben Sie an, wie vorhandene Daten geändert werden, wenn neue Daten eingegeben werden. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>Die neuen Daten überschreiben bestehende Daten in den Bereichen, in denen sie geschrieben wurden. Durch das Hinzufügen von Daten zum Ende des Arbeitsblatts werden neue Zeilen oder Spalten eingefügt, sodass die Daten geschrieben werden können.</p> </li> 
     <li> <p><strong>[!UICONTROL Zeilen einfügen]</strong></p> <p>Für die neuen Daten werden Zeilen eingefügt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren einer Antwort]

Dieses Modul aktualisiert die ausgewählte Antwort.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Tabelle enthält, in der Sie eine Antwort aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Zeilennummer]</p> </td> 
   <td> <p>Geben Sie die Nummer der Zeile ein, die Sie aktualisieren möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Werte]</p> </td> 
   <td> <p>Geben Sie die neuen Werte in die gewünschten Spalten ein.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Werteingabe-Option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Die vom Benutzer eingegebenen Werte werden nicht analysiert und unverändert gespeichert. </p> </li> 
     <li> <p><strong>[!UICONTROL Benutzer eingegeben]</strong></p> <p>Die Werte werden so analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, aber Zeichenfolgen können in Zahlen, Datumsangaben oder andere Formate konvertiert werden, die den gleichen Regeln entsprechen, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets] Benutzeroberfläche.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Antworten löschen]

Dieses Modul löscht eine ausgewählte Antwort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p>Wählen Sie das Arbeitsblatt aus, das die Tabelle enthält, in der Sie eine Antwort löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Zeilennummer]</p> </td> 
   <td> <p>Geben Sie die Nummer der Zeile ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Suchantworten]](#search-responses)
* [[!UICONTROL Suchantworten (erweitert)])](#search-responses-advanced)

#### [!UICONTROL Suchantworten]

Dieses Modul gibt Antworten zurück, die den angegebenen Kriterien entsprechen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Verbindung</td>
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Tabelle]</td>
   <td> <p>Wählen Sie das Formular aus, in dem Sie suchen möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Tabelle] </td>
   <td> <p>Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Spaltenbereich]</td>
   <td> <p> Wählen Sie den zu suchenden Spaltenbereich aus.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Definieren Sie den Filter, nach dem Sie Antworten suchen möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Sortierreihenfolge] </td>
   <td> <p>Wählen Sie aus, ob die zurückgegebenen Antworten in auf- oder absteigender Reihenfolge sortiert werden sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Sortierreihenfolge]</td>
   <td> <p> Wählen Sie die Spalte aus, nach der die zurückgegebenen Antworten sortiert werden sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>Geben Sie an, wie die Werte in der Ausgabe gerendert werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formatierter Wert]</strong></p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema des Arbeitsblatts, nicht auf dem Gebietsschema des anfordernden Benutzers. Wenn beispielsweise <code>A1</code> is <code>1. 23</code> und <code>A2 </code>is <code>=A1</code> und als Währung formatiert, <code>A2</code> return <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Unformatierter Wert]</strong> </p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn beispielsweise <code>A1</code> is <code>1. 23</code> und <code>A2 </code>is <code>=A1</code> und als Währung formatiert, <code>A2</code> gibt die Zahl aus <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formel]</strong> </p> <p>Die Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn beispielsweise <code>A1</code> is <code>1. 23</code> und <code>A2 </code>is <code>=A1</code> und als Währung formatiert, <code>A2</code> return <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Renderoption für Datum und Uhrzeit</td>
    <td>Wählen Sie aus, wie Datum, Uhrzeit und Dauer in der Ausgabe dargestellt werden sollen. Dieses Feld wird ignoriert, wenn die Option [!UICONTROL Value Render] auf "Formatierter Wert"gesetzt ist. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Maximale Anzahl zurückgegebener Antworten]</td>
   <td> <p> Legen Sie die maximale Anzahl von Antworten fest, die [!DNL Workfront Fusion] gibt während eines Zyklus zurück.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchantworten (erweitert)]

Dieses Modul führt eine Suche mithilfe der [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Dieses Modul gibt keine Zeilennummer zurück.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tabelle]</td>
   <td> <p>Wählen Sie die Tabelle aus, die das zu suchende Blatt enthält.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tabelle]</td>
   <td> <p> Wählen Sie das Blatt aus, das die Formularantworten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Definieren Sie die Suchabfrage mithilfe der <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Beispiel: <code>select * where C = "John"</code> ruft alle Werte für die Zeile ab, in der die Spalte C "John"lautet.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Zeilen]</td>
   <td> <p> Legen Sie die maximale Anzahl von Antworten fest, die [!DNL Workfront Fusion] gibt während eines Zyklus zurück.</p> </td> 
  </tr> 
 </tbody> 
</table>
