---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: Mit der XML-App können Sie einen im XML-Format formatierten Text über das XML &gt; Parse XML-Modul analysieren und in ein Bundle konvertieren, um die Daten für andere Module verfügbar zu machen. Sie können ein Bundle auch über das XML &gt; XML erstellen in einen XML-formatierten Text konvertieren
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 1%

---

# XML

Mit der App [!UICONTROL XML] können Sie einen XML-formatierten Text über das Modul [!UICONTROL XML] > [!UICONTROL XML analysieren] analysieren und in ein Bundle konvertieren, um die Daten für andere Module verfügbar zu machen. Sie können ein Bundle auch über das Modul [!UICONTROL XML] > [!UICONTROL XML erstellen] in einen XML-formatierten Text konvertieren

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
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Parse XML]

Das Modul [!UICONTROL XML] > [!UICONTROL XML analysieren] analysiert einen XML-formatierten Text und gibt ein einzelnes Bundle aus, das alle aus der XML extrahierten Informationen enthält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Datenstruktur]</p> </td> 
   <td> <p>Die Datenstruktur beschreibt die Struktur der XML, um die Ausgabe des Moduls im Zuordnungsbereich für die folgenden Module verfügbar zu machen.</p> <p>Wenn Sie über ein Beispiel der XML-Datei verfügen, die Sie analysieren möchten, können Sie damit die Datenstruktur generieren:</p> 
    <ol> 
     <li value="1">Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Add]</strong> .</li> 
     <li value="2">Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Generator]</strong> .</li> 
     <li value="3">Kopieren Sie das XML-Beispiel und fügen Sie es in das Feld <strong>[!UICONTROL Beispieldaten]</strong> ein.</li> 
     <li value="4">Klicken Sie auf <strong>[!UICONTROL Save]</strong>.</li> 
     <li value="5">Überprüfen Sie, ob die Datenstruktur erfolgreich generiert wurde.</li> 
     <li value="6"> <p>Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Speichern]</strong> , um die Datenstruktur zu speichern.</p> <p>Sie können die Schritte 2 bis 5 überspringen, um eine leere Datenstruktur bereitzustellen. Wenn die Datenstruktur leer ist, ist die Ausgabe des Moduls erst dann im Zuordnungsbereich verfügbar, wenn das Modul mindestens einmal ausgeführt wurde.</p> </li> 
    </ol> <p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Datenstrukturen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zahlen als Text beibehalten]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass Zahlen als Textwerte (Zeichenfolge) beibehalten werden. Andernfalls werden Zahlen in Zahlenwerte umgewandelt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Geben Sie den XML-formatierten Text ein oder ordnen Sie ihn zu, den Sie analysieren möchten.</p> <p>Wenn Sie eine Formel verwenden, stellen Sie sicher, dass der Ergebniswerttyp den Datentyp [!UICONTROL Text] ist (oder automatisch zu diesem Typ erzwungen werden kann). </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Wenn der Ergebniswerttyp [!UICONTROL Buffer] (Binärdaten) ist, konvertieren Sie ihn mit der Funktion <code>toString()</code> in den Datentyp Text . Weitere Informationen finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a> und <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Elementdatentypen in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** So laden Sie eine XML-Datei von einer URL herunter und analysieren ihren Inhalt:
>
>1. Erstellen Sie ein neues Szenario.
>1. Fügen Sie [!UICONTROL HTTP] > [!UICONTROL Dateimodul abrufen] ein.
>1. Öffnen Sie die Konfiguration des Moduls und konfigurieren Sie sie wie folgt:
>
>   **URL**: URL der XML-Datei (z. B. `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Klicken Sie auf **[!UICONTROL OK]** &#x200B;, um die Konfiguration des Moduls zu speichern und zu schließen.
1. Fügen Sie das Modul [!UICONTROL XML] > [!UICONTROL Parse XML] hinzu, verbinden Sie es nach dem Modul [!UICONTROL HTTP] > [!UICONTROL Get a file] und konfigurieren Sie es wie folgt:
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Datenstruktur]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Add]</strong> .</li> 
&gt;        <li value="2">Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Generator]</strong> .</li> 
&gt;        <li value="3">Öffnen Sie in Ihrem Webbrowser eine neue Registerkarte oder ein neues Fenster.</li> 
&gt;        <li value="4">Geben Sie die URL, die Sie im dritten Schritt verwendet haben, in die Adressleiste ein und rufen Sie die XML-Datei ab.</li> 
&gt;        <li value="5">Wählen Sie den gesamten XML-Text aus und kopieren Sie ihn in die Zwischenablage.</li> 
&gt;        <li value="6">Schließen Sie die Registerkarte oder das Fenster und kehren Sie zu Ihrem Szenario zurück.</li> 
&gt;        <li value="7">Fügen Sie den kopierten XML-Text in das Feld Beispieldaten ein.</li> 
&gt;        <li value="8">Klicken Sie auf <strong>[!UICONTROL Save]</strong>.</li> 
&gt;        <li value="9">Überprüfen Sie, ob die Datenstruktur erfolgreich generiert wurde.</li> 
&gt;        <li value="10">Klicken Sie auf <strong>[!UICONTROL Save]</strong> , um die Datenstruktur zu speichern.</li> 
&gt;       </ol> <p>Sie können die Schritte 2 bis 9 überspringen, um eine leere Datenstruktur bereitzustellen. Wenn die Datenstruktur leer ist, ist die Ausgabe des Moduls erst dann im Zuordnungsbereich verfügbar, wenn das Modul mindestens einmal ausgeführt wurde.</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>Ordnen Sie das Element <code>Data </code>aus der Ausgabe des Moduls [!UICONTROL HTTP] &gt; [!UICONTROL Datei abrufen] in das Feld ein. Verwenden Sie die Funktion <code>toString()</code> , um den zugehörigen Wert vom Datentyp [!UICONTROL Buffer] (Binärdaten) in [!UICONTROL Text] zu konvertieren.</p> <p>Sie können den Code der Formel kopieren und in das Feld einfügen: <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Weitere Informationen zu den Datentypen "Puffer"und "Text"finden Sie unter <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Elementdatentypen in Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL Parsen von XML-Attributen]

Standardmäßig legt das Modul [!UICONTROL XML] > [!UICONTROL XML analysieren] Attribute in eine spezielle Sammlung `_attributes` als untergeordnetes Element des Knotens mit diesen Attributen ab. Wenn der Knoten ein Textknoten ist und über Attribute verfügt, werden zwei spezielle Eigenschaften hinzugefügt: `_attributes` für Attribute und `_value` für den Textinhalt des Knotens.

>[!INFO]
>
**Beispiel:** Diese XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

wird in dieses Bundle konvertiert:

![](assets/xml-converted-to-bundle.png)

## XML erstellen

Das Modul [!UICONTROL XML] > [!UICONTROL XML erstellen] konvertiert ein Bundle in einen XML-formatierten Text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Datenstruktur]</p> </td> 
   <td> <p>Die Datenstruktur beschreibt die Struktur der resultierenden XML. Wenn Sie über ein Beispiel der XML-Datei verfügen, die Sie erstellen möchten, können Sie damit die Datenstruktur generieren:</p> 
    <ol> 
     <li value="1">Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Add]</strong> .</li> 
     <li value="2">Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Generator]</strong> .</li> 
     <li value="3">Kopieren Sie das XML-Beispiel und fügen Sie es in das Feld Beispieldaten ein.</li> 
     <li value="4">Klicken Sie auf die Schaltfläche <strong>[!UICONTROL Speichern]</strong> .</li> 
     <li value="5">Überprüfen Sie, ob die Datenstruktur erfolgreich generiert wurde.</li> 
     <li value="6">Klicken Sie auf <strong>[!UICONTROL Save]</strong> , um die Datenstruktur zu speichern.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stammelementname]</td> 
   <td>Geben Sie den Namen des Stammelements der XML-Datei ein. Der Standardwert ist <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>Geben Sie den Dateinamen ein, der in der <code> !DOCTYPE SYSTEM</code> -Deklaration verwendet werden soll</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>Geben Sie den Dateinamen ein, der in der <code> !DOCTYPE PUBLIC</code> -Deklaration verwendet werden soll</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL XML-Deklaration löschen]</td> 
   <td>Aktivieren Sie diese Option, um die XML-Deklaration <code>&lt;?xml ... ?&gt;</code> und <code>&lt;!DOCTYPE ... &gt;</code> zu entfernen und nur das XML-Stammelement und dessen Inhalt zu belassen.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**Beispiel:**
>
Ein typischer Anwendungsfall besteht darin, Daten aus einem [!DNL Google] > Arbeitsblatt in XML umzuwandeln.
>
1. Platzieren Sie das Modul [!DNL Google Sheets] > [!UICONTROL Zeilen auswählen] in Ihrem Szenario, um die Daten abzurufen. Richten Sie das -Modul ein, um Zeilen aus Ihrer [!DNL Google] -Tabelle abzurufen. Stellen Sie die &#x200B;**[!UICONTROL Maximale Anzahl der zurückgegebenen Zeilen]** auf eine kleine Zahl ein, die zu Testzwecken jedoch größer als eine ist (Beispiel: 3). Führen Sie das Modul [!DNL Google Sheets] aus, indem Sie mit der rechten Maustaste darauf klicken und &quot;**[!UICONTROL Nur dieses Modul ausführen]**&quot;auswählen. Überprüfen Sie die Ausgabe des Moduls.
1. Verbinden Sie das Modul [!UICONTROL Array Aggregator] nach dem Modul [!DNL Google Sheets] . Wählen Sie im Setup des Moduls das Modul [!DNL Google Sheets] im Feld **[!UICONTROL Source node]** aus. Lassen Sie die anderen Felder unverändert.
1. Verbinden Sie das Modul [!UICONTROL XML] > [!UICONTROL XML] erstellen nach dem Modul [!UICONTROL Array Aggregator] .
>
Die Einrichtung des Moduls erfordert eine Datenstruktur, die die Struktur der XML-Ausgabe beschreibt. Klicken Sie auf die Schaltfläche **[!UICONTROL Hinzufügen]** , um die Einrichtung der Datenstruktur zu öffnen. Die einfachste Möglichkeit, diese Datenstruktur zu erstellen, besteht darin, sie automatisch aus einem XML-Beispiel zu generieren.
>
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Generator]** und fügen Sie Ihr XML-Beispiel in das Feld [!UICONTROL Beispieldaten] ein:
>
![](assets/sample-data-field-350x146.png)
>
1. Klicken Sie auf **[!UICONTROL Speichern]**. Das Feld Spezifikation in der Datenstruktur enthält nun die generierte Struktur.
1. Ändern Sie den Namen Ihrer Datenstruktur in etwas spezifischeres und klicken Sie auf **[!UICONTROL Speichern]**. Ein Feld, das dem Root-Array-Attribut entspricht, wird als zuordnbares Feld in der Einrichtung des JSON-Moduls angezeigt.
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Zuordnung]** neben dem Feld und ordnen Sie ihm das Element `Array[]` aus der Ausgabe des [!UICONTROL Array-Aggregators] zu:
1. Klicken Sie auf **[!UICONTROL OK]** , um das Setup des XML-Moduls zu schließen.
1. Öffnen Sie die Einrichtung des Moduls [!UICONTROL Array Aggregator] . Ändern Sie die **[!UICONTROL Zielstruktur]** von &quot;Benutzerdefiniert&quot;in das Feld eines XML-Moduls, das dem übergeordneten XML-Element entspricht. Ordnen Sie Elemente aus dem [!DNL Google Sheets] -Modul den entsprechenden Feldern zu.
1. Klicken Sie auf **[!UICONTROL OK]** , um das Setup des Array Aggregator-Moduls zu schließen.
1. Führen Sie das Szenario aus.
>
Das XML-Modul gibt die richtige XML-Datei aus.
>
1. Öffnen Sie die Einrichtung des Moduls [!DNL Google Sheets] und erhöhen Sie die Zahl der maximal zurückgegebenen Zeilen] auf die Anzahl der Zeilen in Ihrer Tabelle, um alle Daten zu verarbeiten.[!UICONTROL 
>
Die resultierende XML-Datei kann in [!DNL Dropbox] gespeichert, als Anhang per E-Mail gesendet, über FTP auf einen Server hochgeladen usw.

## Hinzufügen von XML-Attributen

Wenn Sie einem komplexen Knoten Attribute hinzufügen möchten (einem Knoten, der andere Knoten enthalten wird), müssen Sie eine Sammlung mit dem Namen `_attributes` für den komplexen Hinweis in Ihrer benutzerdefinierten Datenstruktur hinzufügen. Diese Sammlung wird Knotenattributen zugeordnet. Wenn Sie einem Textknoten Attribute hinzufügen möchten (z. B. `<node attr="1">abc</node>`), müssen Sie in Ihrer benutzerdefinierten Datenstruktur eine Sammlung `_attributes` für Attribute und eine Texteigenschaft `_value` für den Knotenwert für diesen Knoten hinzufügen.

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

## Fehlerbehebung: Es können keine Daten aus dem Modul [!UICONTROL Parse XML] zugeordnet werden

Stellen Sie sicher, dass die Datenstruktur korrekt definiert ist. Alternativ können Sie eine leere Datenstruktur verwenden und das Modul mindestens einmal ausführen, um eine XML-Eingabe zu verarbeiten.
