---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: Mit der XML-App können Sie einen im XML-Format formatierten Text über XML &gt analysieren. Analysieren Sie das XML-Modul und konvertieren Sie es in ein Bundle, um die Daten für andere Module verfügbar zu machen. Sie können ein Bundle auch über XML &gt in einen XML-formatierten Text konvertieren. XML-Modul erstellen
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 1%

---

# XML

Die [!UICONTROL XML] Mit dem Programm können Sie einen XML-formatierten Text über die [!UICONTROL XML] > [!UICONTROL Parse XML] und konvertieren Sie es in ein Bundle, um die Daten für andere Module verfügbar zu machen. Sie können ein Bundle auch über die [!UICONTROL XML] > [!UICONTROL XML erstellen] Modul

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

## [!UICONTROL Parse XML]

Die [!UICONTROL XML] > [!UICONTROL Parse XML] analysiert einen XML-formatierten Text und gibt ein einzelnes Bundle aus, das alle aus der XML extrahierten Informationen enthält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Datenstruktur]</p> </td> 
   <td> <p>Die Datenstruktur beschreibt die Struktur der XML, um die Ausgabe des Moduls im Zuordnungsbereich für die folgenden Module verfügbar zu machen.</p> <p>Wenn Sie über ein Beispiel der XML-Datei verfügen, die Sie analysieren möchten, können Sie damit die Datenstruktur generieren:</p> 
    <ol> 
     <li value="1">Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> Schaltfläche.</li> 
     <li value="2">Klicken Sie auf <strong>[!UICONTROL Generator]</strong> Schaltfläche.</li> 
     <li value="3">Kopieren Sie das XML-Beispiel und fügen Sie es in das <strong>[!UICONTROL Beispieldaten]</strong> -Feld.</li> 
     <li value="4">Klicken <strong>[!UICONTROL Save]</strong>.</li> 
     <li value="5">Überprüfen Sie, ob die Datenstruktur erfolgreich generiert wurde.</li> 
     <li value="6"> <p>Klicken Sie auf <strong>[!UICONTROL Save]</strong> zum Speichern der Datenstruktur.</p> <p>Sie können die Schritte 2 bis 5 überspringen, um eine leere Datenstruktur bereitzustellen. Wenn die Datenstruktur leer ist, ist die Ausgabe des Moduls erst dann im Zuordnungsbereich verfügbar, wenn das Modul mindestens einmal ausgeführt wurde.</p> </li> 
    </ol> <p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Datenstrukturen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zahlen als Text beibehalten]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass Zahlen als Textwerte (Zeichenfolge) beibehalten werden. Andernfalls werden Zahlen in Zahlenwerte umgewandelt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Geben Sie den XML-formatierten Text ein oder ordnen Sie ihn zu, den Sie analysieren möchten.</p> <p>Wenn Sie eine Formel verwenden, stellen Sie sicher, dass der Ergebniswerttyp den Datentyp [!UICONTROL Text] ist (oder automatisch zu diesem Typ erzwungen werden kann). </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Wenn der Ergebniswerttyp [!UICONTROL Buffer] (Binärdaten) ist, verwenden Sie die <code>toString()</code> -Funktion, um sie in den Datentyp Text zu konvertieren. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typenkonvertierung in [!DNL Adobe Workfront Fusion]</a> und <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Elementdatentypen in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** So laden Sie eine XML-Datei von einer URL herunter und analysieren ihren Inhalt:
>
>1. Erstellen Sie ein neues Szenario.
>1. Einfügen [!UICONTROL HTTP] > [!UICONTROL Datei abrufen] Modul
>1. Öffnen Sie die Konfiguration des Moduls und konfigurieren Sie sie wie folgt:
>
>   **URL**: URL der XML-Datei (z. B. `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Klicken **[!UICONTROL OK]**&#x200B;, um die Konfiguration des Moduls zu speichern und zu schließen.
>1. Hinzufügen [!UICONTROL XML] > [!UICONTROL Parse XML] -Modul, verbinden Sie es nach dem [!UICONTROL HTTP] > [!UICONTROL Datei abrufen] und konfigurieren Sie es wie folgt:
>
>   <table style="table-layout:auto"> 
>    <col> 
>    <col> 
>    <tbody> 
>     <tr> 
>      <td role="rowheader">[!UICONTROL Datenstruktur]</td> 
>      <td> 
>       <ol> 
>        <li value="1">Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> Schaltfläche.</li> 
>        <li value="2">Klicken Sie auf <strong>[!UICONTROL Generator]</strong> Schaltfläche.</li> 
>        <li value="3">Öffnen Sie in Ihrem Webbrowser eine neue Registerkarte oder ein neues Fenster.</li> 
>        <li value="4">Geben Sie die URL, die Sie im dritten Schritt verwendet haben, in die Adressleiste ein und rufen Sie die XML-Datei ab.</li> 
>        <li value="5">Wählen Sie den gesamten XML-Text aus und kopieren Sie ihn in die Zwischenablage.</li> 
>        <li value="6">Schließen Sie die Registerkarte oder das Fenster und kehren Sie zu Ihrem Szenario zurück.</li> 
>        <li value="7">Fügen Sie den kopierten XML-Text in das Feld Beispieldaten ein.</li> 
>        <li value="8">Klicken <strong>[!UICONTROL Save]</strong>.</li> 
>        <li value="9">Überprüfen Sie, ob die Datenstruktur erfolgreich generiert wurde.</li> 
>        <li value="10">Klicken <strong>[!UICONTROL Save]</strong> , um die Datenstruktur zu speichern.</li> 
>       </ol> <p>Sie können die Schritte 2 bis 9 überspringen, um eine leere Datenstruktur bereitzustellen. Wenn die Datenstruktur leer ist, ist die Ausgabe des Moduls erst dann im Zuordnungsbereich verfügbar, wenn das Modul mindestens einmal ausgeführt wurde.</p> </td> 
>     </tr> 
>     <tr> 
>      <td role="rowheader">[!UICONTROL XML]</td> 
>      <td> <p>Ordnen Sie die <code>Data </code>-Element aus der Ausgabe des Moduls [!UICONTROL HTTP] &gt; [!UICONTROL Laden Sie eine Datei] in das Feld. Verwenden Sie die <code>toString()</code> -Funktion, um den Wert aus dem Datentyp [!UICONTROL Buffer] (Binärdaten) in den Datentyp [!UICONTROL Text] zu konvertieren.</p> <p>Sie können den Code der Formel kopieren und in das Feld einfügen: <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Weitere Informationen zu den Datentypen "Puffer"und "Text"finden Sie unter <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Elementdatentypen in Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
>     </tr> 
>    </tbody> 
>   </table>


## [!UICONTROL XML-Attribute analysieren]

Standardmäßig wird die [!UICONTROL XML] > [!UICONTROL Parse XML] -Modul fügt Attribute in eine spezielle Sammlung ein `_attributes` als untergeordnetes Element des Knotens, der über diese Attribute verfügt. Wenn der Knoten ein Textknoten ist und über Attribute verfügt, werden zwei spezielle Eigenschaften hinzugefügt: `_attributes` für Attribute und `_value` für den Textinhalt des Knotens.

>[!INFO]
**Beispiel:** Diese XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

wird in dieses Bundle konvertiert:

![](assets/xml-converted-to-bundle.png)

## XML erstellen

Die [!UICONTROL XML] > [!UICONTROL XML erstellen] -Modul konvertiert ein Bundle in einen XML-formatierten Text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Datenstruktur]</p> </td> 
   <td> <p>Die Datenstruktur beschreibt die Struktur der resultierenden XML. Wenn Sie über ein Beispiel der XML-Datei verfügen, die Sie erstellen möchten, können Sie damit die Datenstruktur generieren:</p> 
    <ol> 
     <li value="1">Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> Schaltfläche.</li> 
     <li value="2">Klicken Sie auf <strong>[!UICONTROL Generator]</strong> Schaltfläche.</li> 
     <li value="3">Kopieren Sie das XML-Beispiel und fügen Sie es in das Feld Beispieldaten ein.</li> 
     <li value="4">Klicken Sie auf <strong>[!UICONTROL Save]</strong> Schaltfläche.</li> 
     <li value="5">Überprüfen Sie, ob die Datenstruktur erfolgreich generiert wurde.</li> 
     <li value="6">Klicken <strong>[!UICONTROL Save]</strong> , um die Datenstruktur zu speichern.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stammelementname]</td> 
   <td>Geben Sie den Namen des Stammelements der XML ein. Der Standardwert ist <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>Geben Sie den Dateinamen ein, der im<code> !DOCTYPE SYSTEM</code> Erklärung</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>Geben Sie den Dateinamen ein, der im<code> !DOCTYPE PUBLIC</code> Erklärung</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL XML-Deklaration löschen]</td> 
   <td>Aktivieren Sie diese Option, um die XML-Deklaration zu entfernen <code>&lt;?xml ... ?&gt;</code> und <code>&lt;!DOCTYPE ... &gt;</code>und lassen Sie nur das XML-Stammelement und seinen Inhalt.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:**
>
>Ein typischer Anwendungsfall besteht darin, Daten aus einem [!DNL Google] >Tabelle in XML.
>
>1. Platzieren Sie die [!DNL Google Sheets] > [!UICONTROL Zeilen auswählen] -Modul in Ihrem Szenario verwenden, um die Daten abzurufen. Richten Sie das Modul ein, um Zeilen aus Ihrem [!DNL Google] Tabelle. Festlegen des &#x200B;**[!UICONTROL Maximale Anzahl an zurückgegebenen Zeilen]** auf eine kleine Zahl, jedoch zu Testzwecken größer als 1 (Beispiel: 3). Führen Sie die [!DNL Google Sheets] -Modul durch Rechtsklick darauf und Auswahl von &quot;**[!UICONTROL Nur dieses Modul ausführen]**.&quot; Überprüfen Sie die Ausgabe des Moduls.
>1. Verbinden Sie die [!UICONTROL Array-Aggregator] -Modul nach [!DNL Google Sheets] -Modul. Wählen Sie in der Moduleinrichtung die [!DNL Google Sheets] -Modul im **[!UICONTROL Quellknoten]** -Feld. Lassen Sie die anderen Felder unverändert.
>1. Verbinden Sie die [!UICONTROL XML] > [!UICONTROL XML erstellen] -Modul nach [!UICONTROL Array-Aggregator] -Modul.
>
>   Die Einrichtung des Moduls erfordert eine Datenstruktur, die die Struktur der XML-Ausgabe beschreibt. Klicken Sie auf **[!UICONTROL Hinzufügen]** -Schaltfläche, um die Einrichtung der Datenstruktur zu öffnen. Die einfachste Möglichkeit, diese Datenstruktur zu erstellen, besteht darin, sie automatisch aus einem XML-Beispiel zu generieren.
>   
>1. Klicken Sie auf **[!UICONTROL Generator]** und fügen Sie Ihr XML-Beispiel in die [!UICONTROL Beispieldaten] -Feld:
>
>   ![](assets/sample-data-field-350x146.png)
>   
>1. Klicken Sie auf **[!UICONTROL Speichern]**. Das Feld Spezifikation in der Datenstruktur enthält nun die generierte Struktur.
>1. Ändern Sie den Namen Ihrer Datenstruktur in einen spezifischeren Namen und klicken Sie auf **[!UICONTROL Speichern]**. Ein Feld, das dem Root-Array-Attribut entspricht, wird als zuordnbares Feld in der Einrichtung des JSON-Moduls angezeigt.
>1. Klicken Sie auf **[!UICONTROL Zuordnung]** neben dem Feld klicken und die `Array[]` -Element [!UICONTROL Array-Aggregator] Ausgabe an sie:
>1. Klicken **[!UICONTROL OK]** , um das Setup des XML-Moduls zu schließen.
>1. Öffnen Sie die Einrichtung der [!UICONTROL Array-Aggregator] -Modul. Ändern Sie die **[!UICONTROL Zielstruktur]** von &quot;Benutzerdefiniert&quot;in das Feld eines XML-Moduls, das dem übergeordneten XML-Element entspricht.Zuordnen von Elementen aus dem [!DNL Google Sheets] in die entsprechenden Felder ein.
>1. Klicken **[!UICONTROL OK]** , um das Setup des Array Aggregator-Moduls zu schließen.
>1. Führen Sie das Szenario aus.
>
>   Das XML-Modul gibt die richtige XML-Datei aus.
>   
>1. Öffnen Sie die Einrichtung der [!DNL Google Sheets] und erhöhen Sie die [!UICONTROL Maximale Anzahl an zurückgegebenen Zeilen] -Zahl größer als die Anzahl der Zeilen in Ihrem Arbeitsblatt sein, um alle Daten zu verarbeiten.
>
>   Die resultierende XML-Datei kann in [!DNL Dropbox], als Anhang per E-Mail gesendet, über FTP auf einen Server hochgeladen usw.


## Hinzufügen von XML-Attributen

Wenn Sie einem komplexen Knoten (einem Knoten, der andere Knoten enthalten wird) Attribute hinzufügen möchten, müssen Sie eine Sammlung mit dem Namen hinzufügen `_attributes` für den komplexen Hinweis in Ihrer benutzerdefinierten Datenstruktur. Diese Sammlung wird Knotenattributen zugeordnet. Wenn Sie einem Textknoten Attribute hinzufügen möchten (z. B.: `<node attr="1">abc</node>`), müssen Sie eine Sammlung hinzufügen `_attributes` für Attribute und eine Texteigenschaft `_value` für den Knotenwert für diesen Knoten in Ihrer benutzerdefinierten Datenstruktur.

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## Fehlerbehebung: Es können keine Daten aus dem [!UICONTROL Parse XML] Modul

Stellen Sie sicher, dass die Datenstruktur korrekt definiert ist. Alternativ können Sie eine leere Datenstruktur verwenden und das Modul mindestens einmal ausführen, um eine XML-Eingabe zu verarbeiten.
