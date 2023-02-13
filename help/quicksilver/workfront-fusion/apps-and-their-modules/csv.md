---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Mit den Adobe Workfront Fusion CSV-Modulen können Sie CSV-Dateien erstellen und CSV-Text aus einem empfangenen Textwert oder einer Datei analysieren.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# CSV

Die [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] können Sie CSV-Dateien erstellen und CSV-Text aus einem empfangenen Textwert oder einer Datei analysieren.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL CSV erstellen]

Die [!UICONTROL CSV erstellen] Aggregator ermöglicht die Erstellung eines CSV-Textes aus empfangenen Textwerten.

Weitere Informationen zu Aggregatoren finden Sie unter [Aggregatormodul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Quellmodul]</td>
        <td>Wählen Sie das Modul aus, das Sie zum Aggregieren der benötigten Felder verwenden.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Aggregierte Felder]</td>
        <td>Wählen Sie aus der Liste der verfügbaren Felder die zu aggregierenden Felder aus.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Kopfzeilen in erste Zeile einschließen]</td>
        <td>Wählen Sie diese Option aus, um die Kopfzeilen in das Ergebnis einzuschließen.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Gruppe nach]</td>
        <td>Geben Sie den Filter ein, um die Ergebnisse zu gruppieren. Geben Sie beispielsweise ein Datum ein.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen]</td>
        <td>Wählen Sie diese Option, um das Szenario zu stoppen, wenn keine Ergebnisse vorliegen.</td>
    </tr>
</table>

## [!UICONTROL CSV erstellen (erweitert)]

Die [!UICONTROL CSV erstellen (erweitert)] Aggregator ermöglicht die Erstellung eines CSV-Textes aus empfangenen Textwerten. Es verwendet eine Datenstruktur, die die CSV-Spalten in der resultierenden CSV-Datei definiert. Nach der Definition erscheinen die Spalten als Felder in der CSV-Moduleinrichtung und können im Szenario einem späteren Modul zugeordnet werden.

Weitere Informationen zu Aggregatoren finden Sie unter [Aggregatormodul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quellmodul]</td> 
   <td>Wählen Sie das Anwendungsmodul aus, das Sie zum Aggregieren der benötigten Felder verwenden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datenstruktur]</td> 
   <td> <p>Wählen Sie die Datenstruktur aus, um die Felder nach Bedarf zu aggregieren. Nach der Definition der Datenstruktur können Sie die Elemente den entsprechenden Feldern zuordnen.</p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Datenstrukturen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kopfzeilen in erste Zeile einschließen] </td> 
   <td>Wählen Sie diese Option aus, um die Kopfzeilen in das Ergebnis einzuschließen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gruppe nach] </td> 
   <td>Geben Sie den Filter ein, um die Ergebnisse zu gruppieren. Geben Sie beispielsweise ein Datum ein. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen] </td> 
   <td>Wählen Sie diese Option, um das Szenario zu stoppen, wenn keine Ergebnisse vorliegen. </td> 
  </tr> 
 </tbody> 
</table>


<p>Angenommen, Sie möchten Ihre Google-Kontakte in eine CSV-Datei mit zwei Spalten "Vollständiger Name"und "E-Mail"exportieren. Das Ausgabebundle aus dem Modul [!UICONTROL Google Contacts] &gt;[!UICONTROL Kontakte von einer Gruppe abrufen] weist die folgende Struktur auf. Die E-Mail-Adressen werden im <code>[!UICONTROL Emails[]]</code> -Element ein Array von Sammlungen ist, wobei jede Sammlung zwei Elemente enthält: <code>Label</code> und <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Wenn Sie die einfache [!DNL Create CSV] -Modul, wird Ihnen eine Liste von Kontrollkästchen angeboten, die den Elementen der obersten Ebene eines Bundles entsprechen. Wenn Sie versuchen, <code>Full name</code> und <code>Emails</code> -Elemente enthält, erzeugt das Modul [!UICONTROL CSV] erstellen die folgende Ausgabe, was wahrscheinlich nicht Ihre Aufgabe ist:</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Shon Winer"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[object Object]","Abby Eisenbarth"</p>
<p>Seit dem Element <code>Full Name</code> von einfachem Typ Text ist, wird es nur gut exportiert. Aber das Element <code>Emails</code>, das ein komplexes Array von Sammlungen ist, wird als [Objektobjekt] exportiert. So werden Sammlungen und Arrays standardmäßig in Text umgewandelt. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Elementdatentypen in Adobe Workfront Fusion</a>.</p>
<p>So exportieren Sie den Inhalt der <code>Email </code>Element der ersten Kollektion der <code>Emails[]</code> stattdessen das Modul [!UICONTROL CSV (erweitert) erstellen verwenden. Mit dem -Modul können Sie einzelne Spalten Ihrer CSV-Datei definieren und ihnen Elemente zuordnen, einschließlich verschachtelter Spalten.</p>
<ol>
<li value="1">Fügen Sie das Modul [!UICONTROL CSV (erweitert) erstellen in ein Szenario ein und öffnen Sie seine Konfiguration.</li>
<li value="2">Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> neben dem Feld [!UICONTROL Datenstruktur] , um eine neue Datenstruktur zu erstellen.</li>
<li value="3"> <p>Schreiben Sie einen Namen für die Datenstruktur und klicken Sie auf die Schaltfläche <strong>[!UICONTROL Element hinzufügen]</strong> -Schaltfläche, um die einzelnen Spalten hinzuzufügen. Wenn Sie zwei Spalten exportieren möchten: "Vollständiger Name"und "E-Mail", würde die resultierende Datenstruktur wie folgt aussehen:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Sobald Sie die Datenstruktur erfolgreich definiert haben, sollten die Felder, die jeder einzelnen Spalte entsprechen, in der Konfiguration des Moduls [!UICONTROL CSV erstellen (erweitert)] angezeigt werden, damit Sie die Elemente zuordnen können. Nehmen Sie den ersten Artikel aus dem <code>[!UICONTROL Emails[]]</code> Array und Zuordnen des Elements <code>Email </code>zum Feld/Spalte E-Mail:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Führen Sie das Szenario aus. Seit dem Element <code>Emails[1]: Email</code> der Spalte "E-Mail"zugeordnet ist, ist vom einfachen Typ Text und exportiert jetzt korrekt:</p> <p>"Full Name","Email"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL CSV analysieren]

Die [!UICONTROL CSV analysieren] Mit transformer können Sie CSV-Text aus einem empfangenen Textwert oder einer Datei analysieren.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzahl der Spalten]</td> 
   <td>Geben Sie die Anzahl der Spalten in der CSV-Datei an.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV enthält Kopfzeilen]</td> 
   <td> <p>Wählen Sie diese Option aus, wenn die erste Zeile des CSV-Texts Kopfzeilen enthält.</p> <p>Hinweis: Das Modul verwendet diese Header nicht, um die Spalten in der Ausgabe zu beschriften. Stattdessen stellt dieses Feld sicher, dass die Kopfzeilen nicht in die Ausgabedaten eingeschlossen sind.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Wählen Sie das Trennzeichen für die CSV-Datei aus. Das Trennzeichen ist das Textzeichen, das die Grenze zwischen separaten Werten oder Feldern anzeigt.</p> 
    <ul> 
     <li>[!UICONTROL Komma]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Sonstige]</p> <p>Wenn Sie [!UICONTROL Sonstige] auswählen, geben Sie das Trennzeichen ein, das die CSV-Datei zum Trennen von Werten verwendet. Sie müssen nur genau ein Zeichen eingeben.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beibehalten von Anführungszeichen innerhalb eines nicht in Anführungszeichen gesetzten Felds]</td> 
   <td>Aktivieren Sie diese Option, um Anführungszeichen beizubehalten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Geben Sie die CSV-Datei ein oder ordnen Sie sie zu, die Sie analysieren möchten.<p>Notiz: <p>Wenn Ihre Daten in Binärform vorliegen (normalerweise aus einer Datei), müssen Sie die Funktion "toString()" verwenden, um die Binärdaten in [!UICONTROL String] zu konvertieren:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
