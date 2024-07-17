---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google Forms-Module
description: Mit den [!DNL Adobe Workfront Fusion Google Forms] Modulen können Sie Antworten in Ihrer Google Forms überwachen, auswählen, hinzufügen, aktualisieren oder löschen.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 0%

---

# [!DNL Google Forms] Module

Mit den Modulen [!DNL Adobe Workfront Fusion] [!DNL Google Forms] können Sie Antworten auf Ihre [!DNL Google Forms] überwachen, auswählen, hinzufügen, aktualisieren oder löschen.

Um [!DNL Google Docs] mit [!DNL Adobe Workfront Fusion] zu verwenden, ist ein [!DNL Google] -Konto erforderlich. Wenn Sie noch kein [!DNL Google] -Konto haben, können Sie eines auf der Hilfeseite für das [!DNL Google] Konto erstellen.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Google Forms] -Module zu verwenden, müssen Sie über ein [!DNL Google] -Konto verfügen.

## Erstellen einer Tabelle aus dem Formular

Damit Sie mit Ihren Formulareinstellungen arbeiten können, muss die Tabelle aus Ihren Antworten erstellt werden.

1. Öffnen Sie Ihr Formular.
1. Gehen Sie zur Registerkarte **[!UICONTROL Antworten]** .
1. Klicken Sie auf das Symbol **[!UICONTROL Tabelle erstellen]** ![](assets/spreadsheet-icon.png).

1. Wählen Sie aus, ob Sie eine neue oder eine vorhandene Tabelle erstellen möchten
1. Klicken Sie auf **[!UICONTROL Erstellen]**.

## [!DNL Google Forms] Module und ihre Felder

Wenn Sie [!DNL Google Forms] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Google Forms] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td role="rowheader">Zeile mit Kopfzeilen</td> 
   <td>Geben Sie die Kopfzeile der Tabelle an. Die Standardzeile ist <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>Geben Sie an, wie die Werte in der Ausgabe gerendert werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formatierter Wert]</strong> </p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema des Arbeitsblatts, nicht auf dem Gebietsschema des anfordernden Benutzers. Wenn beispielsweise <code>A1</code> den Wert <code>1. 23</code> und <code>A2 </code>den Wert <code>=A1</code> aufweist und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>$1. 23</code> zurück.</p> </li> 
     <li> <p><strong>[!UICONTROL Unformatierter Wert]</strong> </p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn beispielsweise <code>A1</code> den Wert <code>1. 23</code> und <code>A2 </code>den Wert <code>=A1</code> aufweist und als Währung formatiert ist, gibt <code>A2</code> die Zahl <code>1. 23</code> zurück.</p> </li> 
     <li> <p><strong>[!UICONTROL Formel]</strong> </p> <p>Die Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn beispielsweise <code>A1</code> den Wert <code>1. 23</code> und <code>A2 </code>den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>=A1</code> zurück.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Renderoption für Datum und Uhrzeit</td> 
   <td>Wählen Sie aus, wie Datum, Uhrzeit und Dauer in der Ausgabe dargestellt werden sollen. Dieses Feld wird ignoriert, wenn [!UICONTROL Value Render Option] auf [!UICONTROL Formatierter Wert] gesetzt ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Antworten fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeitet.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Hinzufügen einer Antwort]](#add-a-response)
* [[!UICONTROL Aktualisieren einer Antwort]](#update-a-response)
* [[!UICONTROL Löschen einer Antwort]](#delete-a-response)

#### [!UICONTROL Hinzufügen einer Antwort]

Dieses Modul hängt eine neue Antwort an den unteren Rand des Formularkalkulationssatzes an.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Benutzer eingegeben]</strong></p> <p>Die Werte werden so analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, aber Zeichenfolgen können in Zahlen, Datumsangaben oder andere Formate konvertiert werden, die den gleichen Regeln entsprechen, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets] -Benutzeroberfläche angewendet werden.</p> </li> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
     <li> <p><strong>[!UICONTROL Benutzer eingegeben]</strong></p> <p>Die Werte werden so analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, aber Zeichenfolgen können in Zahlen, Datumsangaben oder andere Formate konvertiert werden, die den gleichen Regeln entsprechen, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets] -Benutzeroberfläche angewendet werden.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen einer Antwort]

Dieses Modul löscht eine ausgewählte Antwort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
* [[!UICONTROL Suchantworten (erweitert])](#search-responses-advanced)

#### [!UICONTROL Suchantworten]

Dieses Modul gibt Antworten zurück, die den angegebenen Kriterien entsprechen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Verbindung</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p> Wählen Sie den Spaltenbereich aus, den Sie suchen möchten.</p> </td> 
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
    <td>[!UICONTROL Bestellung nach]</td>
   <td> <p> Wählen Sie die Spalte aus, nach der die zurückgegebenen Antworten sortiert werden sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>Geben Sie an, wie die Werte in der Ausgabe gerendert werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formatierter Wert]</strong></p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema des Arbeitsblatts, nicht auf dem Gebietsschema des anfordernden Benutzers. Wenn beispielsweise <code>A1</code> den Wert <code>1. 23</code> und <code>A2 </code>den Wert <code>=A1</code> aufweist und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>$1. 23</code> zurück.</p> </li> 
     <li> <p><strong>[!UICONTROL Unformatierter Wert]</strong> </p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn beispielsweise <code>A1</code> den Wert <code>1. 23</code> und <code>A2 </code>den Wert <code>=A1</code> aufweist und als Währung formatiert ist, gibt <code>A2</code> die Zahl <code>1. 23</code> zurück.</p> </li> 
     <li> <p><strong>[!UICONTROL Formel]</strong> </p> <p>Die Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn beispielsweise <code>A1</code> den Wert <code>1. 23</code> und <code>A2 </code>den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>=A1</code> zurück.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Renderoption für Datum und Uhrzeit</td>
    <td>Wählen Sie aus, wie Datum, Uhrzeit und Dauer in der Ausgabe dargestellt werden sollen. Dieses Feld wird ignoriert, wenn die Option [!UICONTROL Value Render] auf "Formatierter Wert"gesetzt ist. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Maximale Anzahl zurückgegebener Antworten]</td>
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
    <td>[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>Definieren Sie die Suchabfrage mit dem Wert "<a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>".</p> <p>Beispiel: <code>select * where C = "John"</code> ruft alle Werte für die Zeile ab, in der die Spalte "C""John"ist.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Zeilen]</td>
   <td> <p> Legen Sie die maximale Anzahl von Antworten fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>
