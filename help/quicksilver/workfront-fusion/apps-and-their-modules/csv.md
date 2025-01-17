---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# CSV

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [CSV](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/csv.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit [!DNL Adobe Workfront Fusion] [!UICONTROL CSV]-Modulen können Sie CSV-Dateien erstellen und CSV-Text aus einem empfangenen Textwert oder einer Datei analysieren.

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## [!UICONTROL CSV erstellen]

Mit [!UICONTROL  Aggregator „CSV erstellen] können Sie CSV-Text aus empfangenen Textwerten erstellen.

Weitere Informationen zu Aggregatoren finden Sie unter [Aggregator-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source-Modul]</td>
        <td>Wählen Sie das Modul aus, das Sie zum Aggregieren der benötigten Felder verwenden.</td>
    </tr>
    <tr>
        <td>[!UICONTROL aggregierte Felder]</td>
        <td>Wählen Sie die Felder, die Sie aggregieren möchten, aus der Liste der verfügbaren Felder aus.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Kopfzeilen in die erste Zeile einfügen]</td>
        <td>Wählen Sie diese Option, um die Kopfzeilen in das Ergebnis aufzunehmen.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Gruppieren nach]</td>
        <td>Geben Sie den Filter ein, um die Ergebnisse zu gruppieren. Geben Sie beispielsweise ein Datum ein.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Verarbeitung nach einer leeren Aggregation anhalten]</td>
        <td>Wählen Sie diese Option, um das Szenario anzuhalten, wenn keine Ergebnisse vorliegen.</td>
    </tr>
</table>

## [!UICONTROL CSV erstellen (erweitert)]

Mit [!UICONTROL  Aggregator CSV erstellen (erweitert] können Sie CSV-Text aus empfangenen Textwerten erstellen. Sie verwendet eine Datenstruktur, die die CSV-Spalten in der resultierenden CSV-Datei definiert. Nach der Definition erscheinen die Spalten als Felder bei der Einrichtung des CSV-Moduls und können einem späteren Modul im Szenario zugeordnet werden.

Weitere Informationen zu Aggregatoren finden Sie unter [Aggregator-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Modul]</td> 
   <td>Wählen Sie das App-Modul aus, das Sie verwenden, um die benötigten Felder zu aggregieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Datenstruktur]</td> 
   <td> <p>Wählen Sie die Datenstruktur aus, um die Felder wie gewünscht zu aggregieren. Nachdem Sie die Datenstruktur definiert haben, können Sie die Elemente den entsprechenden Feldern zuordnen.</p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Datenstrukturen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kopfzeilen in die erste Zeile einfügen] </td> 
   <td>Wählen Sie diese Option, um die Kopfzeilen in das Ergebnis aufzunehmen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gruppieren nach] </td> 
   <td>Geben Sie den Filter ein, um die Ergebnisse zu gruppieren. Geben Sie beispielsweise ein Datum ein. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verarbeitung nach einer leeren Aggregation anhalten] </td> 
   <td>Wählen Sie diese Option, um das Szenario anzuhalten, wenn keine Ergebnisse vorliegen. </td> 
  </tr> 
 </tbody> 
</table>


<p>Angenommen, Sie möchten Ihre Google-Kontakte in eine CSV-Datei mit zwei Spalten „Vollständiger Name“ und „E-Mail“ exportieren. Das Ausgabepaket vom Modul [!UICONTROL Google-Kontakte] &gt;[!UICONTROL Kontakte aus einer Gruppe abrufen] hat die folgende Struktur. Die E-Mail-Adressen werden im <code>[!UICONTROL Emails[]]</code> gespeichert, einem Array von Sammlungen, wobei jede Sammlung zwei Elemente enthält: <code>Label</code> und <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Wenn Sie das Modul Einfache [!DNL Create CSV] verwenden, erhalten Sie eine Liste von Kontrollkästchen, die den Elementen auf oberster Ebene eines Pakets entsprechen. Wenn Sie versuchen, <code>Full name</code> und <code>Emails</code> Elemente zu markieren, erzeugt das [!UICONTROL CSV erstellen]-Modul die folgende Ausgabe, die wahrscheinlich nicht das ist, was Sie möchten:</p>
<p>„emails“,„fullName“</p>
<p>"[Objekt]",„Gewinner anzeigen“</p>
<p>"[Objekt]",„Lizeth Fulmore“</p>
<p>"[Objekt]",„Hilario Gullatt“</p>
<p>"[Objekt]",„Abby Eisenbarth“</p>
<p>Da das Element <code>Full Name</code> vom einfachen Typ Text ist, wird es problemlos exportiert. Das Element "<code>Emails</code>", das ein komplexes Array von Sammlungen ist, wird jedoch als [Object Object] exportiert, d. h. wie Sammlungen und Arrays standardmäßig in Text umgewandelt werden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Elementdatentypen in Adobe Workfront Fusion</a>.</p>
<p>Um stattdessen den Inhalt des <code>Email </code>Elements der ersten Sammlung des <code>Emails[]</code>-Arrays zu exportieren, muss das Modul [!UICONTROL CSV erstellen (erweitert)] verwendet werden. Mit dem Modul können Sie einzelne Spalten Ihrer CSV-Datei definieren und ihnen Elemente zuordnen, einschließlich der verschachtelten.</p>
<ol>
<li value="1">Fügen Sie das Modul [!UICONTROL CSV erstellen (erweitert)] in ein Szenario ein und öffnen Sie seine Konfiguration.</li>
<li value="2">Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Hinzufügen]</strong> neben dem Feld [!UICONTROL Datenstruktur], um eine neue Datenstruktur zu erstellen.</li>
<li value="3"> <p>Schreiben Sie einen Namen für die Datenstruktur ein und klicken Sie auf die Schaltfläche <strong>[!UICONTROL Element hinzufügen</strong>, um die einzelnen Spalten hinzuzufügen. Wenn Sie zwei Spalten exportieren möchten: „Vollständiger Name“ und „E-Mail“, würde die resultierende Datenstruktur wie folgt aussehen:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>Nachdem Sie die Datenstruktur erfolgreich definiert haben, sollten die Felder, die jeder einzelnen Spalte entsprechen, in der Konfiguration des Moduls [!UICONTROL CSV erstellen (erweitert)] angezeigt werden, damit Sie die Elemente zuordnen können. Nehmen Sie das erste Element aus dem <code>[!UICONTROL Emails[]]</code>-Array und ordnen Sie sein Element <code>Email </code>dem Feld/der Spalte E-Mail zu:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Führen Sie das Szenario aus. Da das Element der Spalte „E-Mail“ zugeordnet <code>Emails[1]: Email</code>, vom einfachen Typ „Text“ ist, wird es jetzt korrekt exportiert:</p> <p>„Vollständiger Name“,„E-Mail“</p> <p>„Shon Winer“,“Shon@Winer.com"</p> <p>„Lizeth Fulmore“,“Lizeth@Fulmore.com"</p> <p>„Hilario Gullatt“,“Hilario@Gullatt.com"</p> <p>„Abby Eisenbarth“,“Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL CSV analysieren]

Der [!UICONTROL CSV parsen]-Transformer ermöglicht das Analysieren von CSV-Text aus einem empfangenen Textwert oder einer Datei.

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
   <td> <p>Wählen Sie diese Option, wenn die erste Zeile des CSV-Texts Kopfzeilen enthält.</p> <p>Hinweis: Das Modul verwendet diese Kopfzeilen nicht zur Beschriftung der Spalten in der Ausgabe. Stattdessen stellt dieses Feld sicher, dass die -Kopfzeilen nicht in den Ausgabedaten enthalten sind.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Trennzeichen für die CSV-Datei auswählen. Das Trennzeichen ist das Textzeichen, das die Grenze zwischen separaten Werten oder Feldern angibt.</p> 
    <ul> 
     <li>[!UICONTROL Komma]</li> 
     <li>[!UICONTROL tab]</li> 
     <li> <p>[!UICONTROL Sonstige]</p> <p>Wenn Sie [!UICONTROL Other] auswählen, geben Sie das Trennzeichen ein, das die CSV-Datei zum Trennen der Werte verwendet. Sie müssen genau ein Zeichen eingeben.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anführungszeichen in nicht angeführten Feldern beibehalten]</td> 
   <td>Aktivieren Sie diese Option, um Anführungszeichen beizubehalten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Geben Sie die CSV-Datei ein, die Sie parsen möchten, oder mappen Sie sie.<p>Hinweis: <p>Wenn Ihre Daten in binärer Form vorliegen (normalerweise aus einer Datei), müssen Sie die Funktion „toString()“ verwenden, um die Binärdaten in [!UICONTROL String] zu konvertieren:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
