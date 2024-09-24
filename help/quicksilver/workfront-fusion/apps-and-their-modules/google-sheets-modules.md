---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google Tabellen-Module
description: Um die Erweiterung [!DNL Google Sheets] mit der Erweiterung [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] zu verwenden (optional, aber für sofortige Trigger erforderlich).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 16cd5dee183153540bcccea8ce469a461d0e8562
workflow-type: tm+mt
source-wordcount: '4000'
ht-degree: 0%

---

# [!DNL Google Sheets] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Google Sheets] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung zu  [!DNL Adobe Workfront Fusion]  - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

Um die Module [!UICONTROL Google Tabellen] zu verwenden, müssen Sie über ein [!UICONTROL Google] -Konto verfügen.

## Trigger

### [!UICONTROL Zeilen ansehen]

Ruft Werte aus jeder neu hinzugefügten Zeile im Arbeitsblatt ab.

Das Modul ruft nur neue Zeilen ab, die noch nicht ausgefüllt wurden. Der Trigger verarbeitet keine überschriebene Zeile.

>[!IMPORTANT]
>
>Wenn das Arbeitsblatt eine leere Zeile enthält, werden keine Zeilen nach der leeren Zeile verarbeitet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle aus, die das zu überwachende Blatt enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Blatt aus, das Sie für eine neue Zeile sehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle enthält Kopfzeilen]</td> 
   <td> <p> Wählen Sie aus, ob das Arbeitsblatt die Kopfzeile enthält.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ja]</strong> </p> <p>Das Modul ruft die Kopfzeile nicht als Ausgabedaten ab. </p> <p>Variablennamen in der Ausgabe werden von den Kopfzeilen aufgerufen.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Das Modul ruft auch die erste Tabellenzeile ab</p> <p>Variablennamen in der Ausgabe werden als A, B, C, D usw. bezeichnet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zeile mit Kopfzeilen </td> 
   <td> <p>Geben Sie den Bereich der Kopfzeile ein. Beispiel: <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Erste Tabellenzeile]</td> 
   <td> <p>Geben Sie den Bereich der ersten Tabellenzeile ein. Beispiel: <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Wert-Renderoption]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatierter Wert]</p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema des Arbeitsblatts, nicht auf dem Gebietsschema des anfordernden Benutzers. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>"$1.23"</code> zurück.</p> <p style="font-weight: bold;">[!UICONTROL Unformatierter Wert]</p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> aufweist und als Währung formatiert ist, gibt <code>A2</code> die Zahl <code>"1.23"</code> zurück.</p> <p style="font-weight: bold;">[!UICONTROL Formel]</p> <p>Die Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>"=A1"</code> zurück.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Renderoption für Datum und Uhrzeit</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Seriennummer]</p> <p>Weist die Felder Datum, Uhrzeit, Datum und Dauer in Form von Dubletten im Format "Seriennummer"an, wie durch Lotus 1-2-3 bekannt. Der gesamte Zahlenteil des Werts (links vom Dezimalzeichen) zählt die Tage seit dem 30. Dezember 1899. Der Bruchteil (rechts von der Dezimalstelle) zählt die Zeit als Bruchteil des Tages. Zum Beispiel wäre der 1. Januar 1900 um 12 Uhr 2,5, 2, weil es 2 Tage nach dem 30. Dezember 1899 ist, und 0,5, weil die Mittagszeit ein halber Tag ist. Der 1. Februar 1900 um 15 Uhr wäre 33.625 Uhr. Damit wird das Jahr 1900 richtig als kein Schaltjahr behandelt.</p> <p style="font-weight: bold;">[!UICONTROL Formatierte Zeichenfolge]</p> <p>Weist die Felder Datum, Uhrzeit, Datum und Dauer als Zeichenfolgen im angegebenen Zahlenformat an (abhängig vom Gebietsschema des Arbeitsblatts).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Ausführungszyklus arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aktionen

* [[!UICONTROL Eine Zeile hinzufügen]](#add-a-row)
* [[!UICONTROL Eine Zeile aktualisieren]](#update-a-row)
* [[!UICONTROL Löschen einer Zeile]](#clear-a-row)
* [[!UICONTROL Eine Zeile löschen]](#delete-a-row)
* [[!UICONTROL Abrufen einer Zelle]](#get-a-cell)
* [[!UICONTROL Zelle aktualisieren]](#update-a-cell)
* [[!UICONTROL Zelle löschen]](#clear-a-cell)
* [[!UICONTROL Blatt hinzufügen]](#add-a-sheet)
* [[!UICONTROL Erstellen einer Tabelle]](#create-a-spreadsheet)
* [[!UICONTROL Eine Tabelle löschen]](#delete-a-sheet)
* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)

### [!UICONTROL Eine Zeile hinzufügen]

Dieses Modul hängt eine Zeile an ein Blatt an.

Wenn Sie [!DNL Google Sheets] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Google Sheets] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modus]</td> 
   <td> <p>Wählen Sie aus, ob Sie die Tabelle und das Blatt manuell oder durch Zuordnung auswählen möchten.</p> <p>Hinweis: Die manuelle Zuordnung ist beispielsweise dann nützlich, wenn eine neue Tabelle in einem [!DNL Workfront Fusion] -Szenario erstellt wird und Sie Daten in der neu erstellten Tabelle direkt im Szenario hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle [!DNL Google] aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Blatt aus, dem Sie eine Zeile hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spaltenbereich]</td> 
   <td>Wählen Sie den Spaltenbereich aus, mit dem Sie arbeiten möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle enthält Kopfzeilen]</td> 
   <td> <p> Wählen Sie aus, ob das Arbeitsblatt die Kopfzeile enthält.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ja]</strong> </p> <p>Das Modul ruft die Kopfzeile nicht als Ausgabedaten ab. </p> <p>Variablennamen in der Ausgabe werden von den Kopfzeilen aufgerufen.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Das Modul ruft auch die erste Tabellenzeile ab</p> <p>Variablennamen in der Ausgabe werden als A, B, C, D usw. bezeichnet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Werte] </td> 
   <td> <p>Geben Sie die gewünschten Zellen der Zeile ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Werteingabe-Option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Benutzer eingegeben]</strong></p> <p>Die Werte werden so analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, aber Zeichenfolgen können in Zahlen, Datumsangaben oder andere Formate konvertiert werden, die den gleichen Regeln entsprechen, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets] -Benutzeroberfläche angewendet werden.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Die vom Benutzer eingegebenen Werte werden nicht analysiert und unverändert gespeichert. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Option "Daten einfügen"]</td> 
   <td> <p>Geben Sie an, wie vorhandene Daten geändert werden, wenn neue Daten eingegeben werden. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Zeilen einfügen]</strong></p> <p>Für die neuen Daten werden Zeilen eingefügt.</p> </li> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>Die neuen Daten überschreiben bestehende Daten in den Bereichen, in denen sie geschrieben wurden. Durch das Hinzufügen von Daten zum Ende des Arbeitsblatts werden neue Zeilen oder Spalten eingefügt, sodass die Daten geschrieben werden können.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eine Zeile aktualisieren]

Mit diesem Modul können Sie den Zelleninhalt in einer ausgewählten Zeile ändern.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modus]</td> 
   <td> <p>Wählen Sie aus, ob Sie die Tabelle und das Blatt manuell oder durch Zuordnung auswählen möchten.</p> <p>Hinweis: Die manuelle Zuordnung ist beispielsweise dann nützlich, wenn eine neue Tabelle im [!UICONTROL Workfront Fusion]-Szenario erstellt wird und Sie dem neu erstellten Arbeitsblatt Daten direkt im Szenario hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle [!DNL Google] aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Blatt aus, in dem Sie eine Zeile aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeilennummer]</td> 
   <td> <p> Geben Sie die Nummer der Zeile ein, die Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle enthält Kopfzeilen]</td> 
   <td> <p> Wählen Sie aus, ob das Arbeitsblatt die Kopfzeile enthält.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ja]</strong> </p> <p>Das Modul ruft die Kopfzeile nicht als Ausgabedaten ab. </p> <p>Variablennamen in der Ausgabe werden von den Kopfzeilen aufgerufen.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>Das Modul ruft auch die erste Tabellenzeile ab</p> <p>Variablennamen in der Ausgabe werden als A, B, C, D usw. bezeichnet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Werte] </td> 
   <td> <p>Geben Sie die Werte ein oder ordnen Sie sie den gewünschten Zellen der Zeile zu, die Sie ändern (aktualisieren) möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Werteingabe-Option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Benutzer eingegeben]</strong></p> <p>Die Werte werden so analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, aber Zeichenfolgen können in Zahlen, Datumsangaben oder andere Formate konvertiert werden, die den gleichen Regeln entsprechen, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets] -Benutzeroberfläche angewendet werden.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Die vom Benutzer eingegebenen Werte werden nicht analysiert und unverändert gespeichert. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Löschen einer Zeile]

Löscht Werte aus einer angegebenen Zeile.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die [!DNL Google] -Tabelle aus, die das Blatt enthält, aus dem Sie eine Zeile löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p> Wählen Sie das Blatt aus, aus dem Sie Daten löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeilennummer]</td> 
   <td> <p>Geben Sie die Nummer der Zeile ein, aus der die Daten gelöscht werden sollen. Beispiel: <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eine Zeile löschen]

Löscht eine angegebene Zeile.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Google-Arbeitsblatt aus, das das Arbeitsblatt enthält, aus dem Sie eine Zeile löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Arbeitsblatt </td> 
   <td> <p>Wählen Sie das Blatt aus, aus dem Sie eine Zeile löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Zeilennummer</td> 
   <td> <p>Geben Sie die Nummer der Zeile ein, die Sie löschen möchten. Beispiel: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Abrufen einer Zelle]

Ruft einen Wert aus einer ausgewählten Zelle ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle [!DNL Google] aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Blatt aus, das die Zelle enthält, aus der Sie Daten abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Geben Sie die Kennung der Zelle ein, aus der Sie Daten abrufen möchten. Beispiel: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Wert-Renderoption]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatierter Wert]</p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema des Arbeitsblatts, nicht auf dem Gebietsschema des anfordernden Benutzers. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>"$1.23"</code> zurück.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> aufweist und als Währung formatiert ist, gibt <code>A2</code> die Zahl <code>"1.23"</code> zurück.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>Die Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>"=A1"</code> zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Weist die Felder Datum, Uhrzeit, Datum und Dauer in Form von Dubletten im Format "Seriennummer"an, wie durch Lotus 1-2-3 bekannt. Der gesamte Zahlenteil des Werts (links vom Dezimalzeichen) zählt die Tage seit dem 30. Dezember 1899. Der Bruchteil (rechts von der Dezimalstelle) zählt die Zeit als Bruchteil des Tages. Zum Beispiel wäre der 1. Januar 1900 um 12 Uhr 2,5, 2, weil es 2 Tage nach dem 30. Dezember 1899 ist, und 0,5, weil die Mittagszeit ein halber Tag ist. Der 1. Februar 1900 um 15 Uhr wäre 33.625 Uhr. Damit wird das Jahr 1900 richtig als kein Schaltjahr behandelt.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Weist die Felder Datum, Uhrzeit, Datum und Dauer als Zeichenfolgen im angegebenen Zahlenformat an (abhängig vom Gebietsschema des Arbeitsblatts).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Zelle aktualisieren]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle [!DNL Google] aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Geben Sie die Kennung der Zelle ein, die Sie aktualisieren möchten. Beispiel: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Wert]</td> 
   <td> <p>Geben Sie den neuen Wert für die Zelle ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Werteingabe-Option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Benutzer eingegeben]</strong></p> <p>Die Werte werden so analysiert, als ob der Benutzer sie in die Benutzeroberfläche eingegeben hätte. Zahlen bleiben Zahlen, aber Zeichenfolgen können in Zahlen, Datumsangaben oder andere Formate konvertiert werden, die den gleichen Regeln entsprechen, die bei der Eingabe von Text in eine Zelle über die [!DNL Google Sheets] -Benutzeroberfläche angewendet werden.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Die vom Benutzer eingegebenen Werte werden nicht analysiert und unverändert gespeichert. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Zelle löschen]

Löscht einen Wert aus einer angegebenen Zelle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Google-Arbeitsblatt aus, das das Arbeitsblatt enthält, aus dem Sie eine Zelle löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Blatt aus, aus dem Sie eine Zelle löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Geben Sie die Kennung der Zelle ein, die Sie löschen möchten. Beispiel: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Blatt hinzufügen]

Erstellt ein neues Arbeitsblatt in einer ausgewählten Tabelle.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Google-Tabelle aus, der Sie ein Blatt hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Eigenschaften]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Titel]</p> <p>Geben Sie den Namen des neuen Arbeitsblatts ein.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Index]</p> <p>Geben Sie die Tabellenposition ein. Der Standardwert ist 0 (platziert das Blatt an erster Stelle).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Erstellen einer Tabelle]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Titel] </td> 
   <td> <p>Geben Sie den Namen eines neuen Arbeitsblatts ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Locale]</td> 
   <td> <p>Geben Sie das Gebietsschema des Arbeitsblatts in eines der folgenden Formate ein:</p> 
    <ul> 
     <li>einen Sprachcode nach ISO 639-1, z. B. <code>en</code></li> 
     <li>einen Sprachcode nach ISO 639-2, z. B. <code>haw</code>, wenn kein 639-1-Code vorhanden ist</li> 
     <li>eine Kombination des ISO-Sprachencodes und des Ländercodes, z. B. <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Neuberechnungsintervall]</td> 
   <td> <p>Die Wartezeit bis zur Neuberechnung von flüchtigen Funktionen:</p> <p style="font-weight: bold;">[!UICONTROL On change]</p> <p>Volatile Funktionen werden bei jeder Änderung aktualisiert.</p> <p style="font-weight: bold;">[!UICONTROL Änderungen und jede Minute]</p> <p>Volatile Funktionen werden bei jeder Änderung und jede Minute aktualisiert.</p> <p style="font-weight: bold;">[!UICONTROL Bei Änderung und stündlicher Ausführung]</p> <p>Volatile Funktionen werden bei jeder Änderung und stündlich aktualisiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zeitzone]</td> 
   <td> <p> Wählen Sie die Zeitzone des Arbeitsblatts aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zahlenformat]</td> 
   <td> <p>Wählen Sie das Standardformat aller Zellen des Arbeitsblatts aus.</p> <p><strong>[!UICONTROL Text]</strong>: Textformatierung. Beispiel: <code>1000. 12</code></p> <p><strong>[!UICONTROL Number]</strong>: Zahlenformatierung. Beispiel: <code>1,000.12</code></p> <p><strong>[!UICONTROL Prozent]</strong>: Prozentformatierung. Beispiel: <code>10. 12%</code></p> <p><strong>[!UICONTROL Währung]</strong>: Währungsformatierung. Beispiel: <code>$1,000.12</code></p> <p><strong>[!UICONTROL Date]</strong>: Datumsformatierung. Beispiel: <code>9/26/2008</code></p> <p><strong>[!UICONTROL Time]</strong>: Zeitformatierung. Beispiel: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Datum/Uhrzeit]</strong>: Formatierung von Datum und Uhrzeit. Beispiel: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientific]</strong>Wissenschaftliche Zahlenformatierung. Beispiel: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabellen] </td> 
   <td> <p>Klicken Sie auf <strong>[!UICONTROL Add]</strong> , um dem Arbeitsblatt ein Blatt hinzuzufügen. Geben Sie für jedes Blatt einen Titel für das Blatt und den Index des Blatts ein oder ordnen Sie ihn zu. Der Index 0 steht für das erste Blatt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eine Tabelle löschen]

Löscht ein bestimmtes Blatt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle [!DNL Google] aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Blatt aus, das Sie löschen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API-Aufruf durchführen]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten API-Aufruf ausführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [Fusion App]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://sheets.googleapis.com/v4/</code> ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu, z. B. <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:   <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Suchvorgänge

* [[!UICONTROL Suchzeilen]](#search-rows)
* [[!UICONTROL Suchzeilen (erweitert)]](#search-rows-advanced)
* [[!UICONTROL Bereichswerte abrufen]](#get-range-values)
* [[!UICONTROL Listenblätter]](#list-sheets)

### [!UICONTROL Suchzeilen]

Sucht Zeilen mithilfe der Filteroptionen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [Fusion App]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung mit [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle [!DNL Google] aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Blatt aus, in dem Sie die Zeilen suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle enthält Kopfzeilen]</td> 
   <td> <p> Wählen Sie aus, ob das Arbeitsblatt die Kopfzeile enthält. Wenn die Option [!UICONTROL Ja] ausgewählt ist, ruft das Modul die Kopfzeile nicht ab, da die Ausgabedaten und Variablennamen in der Ausgabe von den Kopfzeilen aufgerufen werden. Wenn die Option [!UICONTROL Nein] ausgewählt ist, ruft das Modul auch die erste Tabellenzeile ab und die Variablennamen in der Ausgabe werden dann nur als A, B, C, D usw. bezeichnet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spaltenbereich]</td> 
   <td>Wählen Sie den Spaltenbereich aus, mit dem Sie arbeiten möchten. Beispiel: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Legen Sie den Filter für die Zeile fest, nach der gesucht werden soll.</p> <p>Weitere Informationen zu Filtern finden Sie unter <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Hinzufügen eines Filters zu einem Szenario in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sortierreihenfolge]</td> 
   <td>Wählen Sie aus, ob Sie eine aufsteigende oder absteigende Sortierung vornehmen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reihenfolge nach]</td> 
   <td>Wählen Sie die Spalte aus, nach der Sie sortieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Wert-Renderoption]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatierter Wert]</p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema des Arbeitsblatts, nicht auf dem Gebietsschema des anfordernden Benutzers. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>"$1.23"</code> zurück.</p> <p style="font-weight: bold;">[!UICONTROL Unformatierter Wert]</p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> aufweist und als Währung formatiert ist, gibt <code>A2</code> die Zahl <code>"1.23"</code> zurück.</p> <p style="font-weight: bold;">[!UICONTROL Formel]</p> <p>Die Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>"=A1"</code> zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Renderoption für Datum und Uhrzeit</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Seriennummer]</p> <p>Weist die Ausgabe der Felder Datum, Uhrzeit, Datum und Dauer im Format "Seriennummer"an, wie durch Lotus 1-2-3 bekannt. Der gesamte Zahlenteil des Werts (links vom Dezimalzeichen) zählt die Tage seit dem 30. Dezember 1899. Der Bruchteil (rechts von der Dezimalstelle) zählt die Zeit als Bruchteil des Tages. Zum Beispiel wäre der 1. Januar 1900 um 12 Uhr 2,5, 2, weil es 2 Tage nach dem 30. Dezember 1899 ist, und 0,5, weil die Mittagszeit ein halber Tag ist. Der 1. Februar 1900 um 15 Uhr wäre 33.625 Uhr. Damit wird das Jahr 1900 richtig als kein Schaltjahr behandelt.</p> <p style="font-weight: bold;">[!UICONTROL Formatierte Zeichenfolge]</p> <p>Weist die Felder Datum, Uhrzeit, Datum und Dauer als Zeichenfolgen im angegebenen Zahlenformat an (abhängig vom Gebietsschema des Arbeitsblatts).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Zeilen]</td> 
   <td>Legen Sie die maximale Anzahl von Zeilen fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Suchzeilen (erweitert)]

Gibt Ergebnisse zurück, die den angegebenen Kriterien entsprechen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Google-Tabelle aus, die das zu durchsuchende Blatt enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie das Blatt aus, das die Zeilen enthält, die Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abfrage]</td> 
   <td> <p>Verwenden Sie den [!DNL Google Charts Query Language]. Beispiel: <code>select * where B = "John"</code></p> <p>Weitere Informationen zu [!DNL Google Charts Query Language] finden Sie unter <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Query Language Reference</a> in der Dokumentation zu [!DNL Google].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Bereichswerte abrufen]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle [!DNL Google] aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die Tabelle aus, aus der Sie den Bereichsinhalt abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Bereich] </td> 
   <td> <p>Geben Sie den Bereich ein, den Sie erhalten möchten. Beispiel: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle enthält Kopfzeilen]</td> 
   <td> <p>Aktivieren Sie dieses Kontrollkästchen, wenn das Blatt eine Kopfzeile enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>Zeile mit Kopfzeilen</td> 
   <td>Geben Sie den Bereich der Tabellenüberschriften ein. Beispiel <code>A1:F1</code>. Wenn Sie das Feld leer lassen, geht [!DNL Workfront Fusion] davon aus, dass sich die Kopfzeile in der ersten Zeile des angegebenen Bereichs befindet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Wert-Renderoption]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatierter Wert]</p> <p>Die Werte werden in der Antwort entsprechend der Zellenformatierung berechnet und formatiert. Die Formatierung basiert auf dem Gebietsschema des Arbeitsblatts, nicht auf dem Gebietsschema des anfordernden Benutzers. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>"$1.23"</code> zurück.</p> <p style="font-weight: bold;">[!UICONTROL Unformatierter Wert]</p> <p>Die Werte werden berechnet, aber in der Antwort nicht formatiert. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> aufweist und als Währung formatiert ist, gibt <code>A2</code> die Zahl <code>"1.23"</code> zurück.</p> <p style="font-weight: bold;">[!UICONTROL Formel]</p> <p>Die Werte werden nicht berechnet. Die Antwort enthält die Formeln. Wenn beispielsweise <code>A1</code> den Wert <code>1.23</code> und <code>A2</code> den Wert <code>=A1</code> hat und als Währung formatiert ist, gibt <code>A2</code> den Wert <code>"=A1"</code> zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Renderoption für Datum und Uhrzeit</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Seriennummer]</p> <p>Weist die Ausgabe der Felder Datum, Uhrzeit, Datum und Dauer im Format "Seriennummer"an, wie durch Lotus 1-2-3 bekannt. Der gesamte Zahlenteil des Werts (links vom Dezimalzeichen) zählt die Tage seit dem 30. Dezember 1899. Der Bruchteil (rechts von der Dezimalstelle) zählt die Zeit als Bruchteil des Tages. Zum Beispiel wäre der 1. Januar 1900 um 12 Uhr 2,5, 2, weil es 2 Tage nach dem 30. Dezember 1899 ist, und 0,5, weil die Mittagszeit ein halber Tag ist. Der 1. Februar 1900 um 15 Uhr wäre 33.625 Uhr. Damit wird das Jahr 1900 richtig als kein Schaltjahr behandelt.</p> <p style="font-weight: bold;">[!UICONTROL Formatierte Zeichenfolge]</p> <p>Weist die Felder Datum, Uhrzeit, Datum und Dauer als Zeichenfolgen im angegebenen Zahlenformat an (abhängig vom Gebietsschema des Arbeitsblatts).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Listenblätter]

Dieses Modul gibt eine Liste aller Arbeitsblätter in einem Arbeitsblatt zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Sheets]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tabelle] </td> 
   <td> <p>Wählen Sie die [!DNL Google] -Tabelle aus, die die Tabellen enthält, die Sie auflisten möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Nutzungsbeschränkungen

Wenn der Fehler `429: RESOURCE_EXHAUSTED` auftritt, haben Sie das Limit der API-Rate überschritten.

Die [!DNL Google Sheets] -API erlaubt maximal 500 Anfragen pro 100 Sekunden pro Projekt und 100 Anfragen pro 100 Sekunden pro Benutzer. Beschränkungen für Lese- und Schreibvorgänge werden separat verfolgt. Es gibt keine tägliche Nutzungsbegrenzung.

Weitere Informationen finden Sie unter [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Tipps und Tricks

* [Abrufen leerer Zellen aus einem [!DNL Google] Blatt](#how-to-get-empty-cells-from-a-google-sheet)
* [Hinzufügen einer Schaltfläche in einem Arbeitsblatt zur Ausführung eines Szenarios](#add-a-button-in-a-sheet-to-run-a-scenario)

### Abrufen leerer Zellen von einem [!DNL Google Sheet]

Verwenden Sie das Modul [!UICONTROL Suchzeilen (erweitert)] und rufen Sie mit dieser Formel die leeren Spalten ab.
<pre>select * where E is null</pre>Hier ist "E"die Spalte und "ist null"die Bedingung. Sie können eine erweiterte Abfrage mit [Google Query Lang](https://developers.google.com/chart/interactive/docs/querylanguage) erstellen.

### Hinzufügen einer Schaltfläche in einem Arbeitsblatt zur Ausführung eines Szenarios

1. Fügen Sie in [!DNL Workfront Fusion] das Modul/den Trigger **[!UICONTROL Webhook]** > **[!UICONTROL Benutzerdefinierte Webhooks]** in das Szenario ein und konfigurieren Sie ihn (siehe [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Kopieren Sie die URL des Webhooks.
1. Führen Sie das Szenario aus.
1. Wählen Sie in Google Tabellen **[!UICONTROL Einfügen]** > **[!UICONTROL Zeichnen]**... aus der Hauptmenüleiste.

1. Klicken Sie im Fenster [!UICONTROL Zeichnen] auf das Symbol **[!UICONTROL Textfeld]** oben im Fenster ![](assets/text-box.png).
1. Erstellen Sie eine Schaltfläche und klicken Sie oben rechts auf die Schaltfläche **[!UICONTROL Speichern und schließen]** :
1. Die Schaltfläche wird in Ihr Arbeitsblatt eingefügt. Klicken Sie auf die drei vertikalen Punkte in der oberen rechten Ecke der Schaltfläche:
1. Wählen Sie &quot;**[!UICONTROL Skript zuweisen&quot;aus.].** aus dem Menü.
1. Geben Sie den Namen Ihres Skripts (Funktion) ein, z. B. `runScenario`, und klicken Sie auf **[!UICONTROL OK]**:
1. Wählen Sie in der Hauptmenüleiste **[!UICONTROL Tools]** > **[!UICONTROL Skript-Editor]** aus.

1. Fügen Sie den folgenden Code ein:

   * Der Name der Funktion muss dem in Schritt 9 angegebenen Namen entsprechen.
   * Ersetzen Sie die URL durch die URL des Webhooks, den Sie in Schritt 2 kopiert haben.

     <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("<webhook you copied>");</pre><pre>}</pre>

1. Drücken Sie **[!UICONTROL Strg+S]**, um die Skriptdatei zu speichern, geben Sie einen Projektnamen ein und klicken Sie auf **[!UICONTROL OK]**.

1. Wechseln Sie zurück zu [!DNL Google Sheets] und klicken Sie auf Ihre neue Schaltfläche.
1. Erteilen Sie dem Skript die erforderliche Autorisierung:
1. Überprüfen Sie in [!DNL Workfront Fusion], ob das Szenario erfolgreich ausgeführt wurde.

## Datum in einer Tabelle speichern

Wenn Sie einen Datumswert in einer Tabelle ohne Formatierung speichern, wird dieser im Arbeitsblatt als Text im ISO 8601-Format angezeigt. [!DNL Google Sheets] Formeln oder Funktionen, die mit Datumsangaben arbeiten, die diesen Text nicht verstehen (Beispiel: Formel `=A1+10`), zeigen jedoch den folgenden Fehler an:

![](assets/mceclip6-350x87.png)

Damit [!DNL Google Sheets] das Datum besser verstehen kann, formatieren Sie es mit der Funktion [[!UICONTROL formatDate] (date; format; [timezone])](../../workfront-fusion/functions/date-and-time-functions.md#formatda). Das richtige Format, das an die Funktion übergeben wird, da das zweite Argument von den Gebietsschemaeinstellungen des Arbeitsblatts abhängt.

So bestimmen Sie das richtige Format:

1. Wählen Sie im Hauptmenü die Einstellungen **[!UICONTROL Datei]** > **[!UICONTROL Tabellenblatt]** aus, um das Gebietsschema zu überprüfen/festzulegen.

1. Nachdem Sie das richtige Gebietsschema überprüft/festgelegt haben, bestimmen Sie das entsprechende Datums- und Uhrzeitformat, indem Sie im Hauptmenü die Option **[!UICONTROL Format]** > **[!UICONTROL Nummer]** auswählen. Das Format wird neben dem Menüelement Datum/Uhrzeit angezeigt:

1. Um das richtige Format zu erstellen, das an die Funktion [!UICONTROL formatDate()] übergeben werden soll, lesen Sie die Liste der [Token für die Formatierung von Datum und Uhrzeit in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Beispiel:** Die Verwendung des `MM/DD/YYYY HH:mm:ss` -Formats für das Gebietsschema USA:

![](assets/locale-time-350x83.png)

## Funktionen von [!DNL Google Sheets] nutzen

Wenn Sie eine integrierte Funktion vermissen, diese jedoch durch [!DNL Google Sheets] gekennzeichnet ist, können Sie sie nutzen. Weitere Informationen finden Sie unter [Verwenden von [!DNL Google Sheets] Funktionen](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [Ordnen Sie Elemente mithilfe von Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) zu.

## Vermeiden Sie es von [!DNL Google Sheets], Zahlen in Daten zu ändern

Möglicherweise wird eine Zeichenfolge mit Zahlen, die Sie als Text verwenden, als Datum in einem [!DNL Google] -Arbeitsblatt interpretiert. Sie geben beispielsweise 1-2019 ein, beabsichtigen es als Text, aber Google interpretiert es als Datum. Sie können die Zahl als Text vorformatieren, um dies zu verhindern.

1. Markieren Sie in [!DNL Google Sheets] die Spalte oder Zelle, die die Zahl oder die Zahlen enthält.
1. Klicken Sie auf **[!UICONTROL Format]** > **[!UICONTROL Zahl]** > **[!UICONTROL Klartext]**.

Eine weitere Problemumgehung in [!DNL Workfront Fusion] besteht darin, vor einer Zahl ein Apostroph (&#39;) einzugeben, z. B. &quot;1-2019&quot;oder &quot;1/47&quot;. Der Apostroph wird nicht in der Zelle angezeigt, nachdem die Daten von [!DNL Workfront Fusion] gesendet wurden.
