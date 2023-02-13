---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Aggregatormodul in Adobe Workfront Fusion
description: Ein Aggregatormodul ist ein Modultyp, der dazu dient, mehrere Datenbündel in einem Bundle zusammenzuführen.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# [!UICONTROL Aggregator] -Modul in [!DNL Adobe Workfront Fusion]

Ein Aggregatormodul ist ein Modultyp, der dazu dient, mehrere Datenbündel in einem Bundle zusammenzuführen.

Weitere Informationen zu Modultypen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
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

## [!UICONTROL Aggregator] Modul

Wenn ein [!UICONTROL Aggregator] -Modul ausgeführt wird, wird Folgendes ausgeführt:

* Akkumuliert alle Bundles, die es während des Vorgangs eines einzelnen Quellmoduls erhält.
* Gibt ein einzelnes Bundle mit einem Array aus, das pro akkumuliertem Bundle ein Element enthält. Der Inhalt der Elemente des Arrays hängt von einem bestimmten [!UICONTROL Aggregator] -Modul und dessen Einrichtung.

Die folgende Abbildung zeigt eine typische Einrichtung der [!UICONTROL Aggregator] module :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Quellmodul]</p> </td> 
   <td> <p>Das Modul, von dem aus die Bundle-Aggregation gestartet wird. Das Quellmodul ist normalerweise ein Iterator oder ein Suchmodul, das eine Reihe von Bundles ausgibt. Wenn Sie das Quellmodul des Aggregators einrichten (und die Einrichtung des Aggregators schließen), wird die Route zwischen dem Quellmodul und dem Aggregatormodul in einen grauen Bereich eingeschlossen, sodass Sie den Beginn und das Ende der Aggregation deutlich sehen können. 
   </p> <p>Weitere Informationen zu Iteratoren finden Sie unter <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator]-Modul in [!DNL Adobe Workfront Fusion]</a></p> <p>Weitere Informationen zu Suchmodulen finden Sie unter Suchmodule in <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Modultypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target-Strukturtyp]</p> </td> 
   <td> <p>(Gilt nur für das [!UICONTROL Array Aggregator]-Modul.) Zielstruktur, in die die Daten aggregiert werden. Mit der Standardoption [!UICONTROL Benutzerdefiniert] können Sie Elemente auswählen, die im Ausgabepaket des A[!UICONTROL Array Aggregators] aggregiert werden sollen <code>Array </code>item:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Sobald Sie weitere Module nach dem [!UICONTROL Array Aggregator]-Modul verbinden und zum Setup des Moduls zurückkehren, enthält das Dropdown-Menü vom Strukturtyp [!UICONTROL Target] alle folgenden Module und deren Felder, die vom Typ Array of Collections sind, wie im Feld [!UICONTROL Attachments] des Felds [!DNL Slack] &gt;[!UICONTROL Nachrichtenmodul erstellen:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregierte Felder]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Aggregatormodulausgabe einbeziehen möchten.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Gruppe nach]</p> </td> 
   <td> <p>Die Ausgabe des Aggregators kann mithilfe des Felds [!UICONTROL Group by] in mehrere Gruppen aufgeteilt werden. Das Feld [!UICONTROL Gruppe nach] kann eine Formel enthalten, die für das Eingabepaket jedes Aggregators ausgewertet wird. Der Aggregator gibt dann ein Bundle pro Wert jeder einzelnen Formel aus. Jedes Bundle enthält zwei Elemente:</p> 
    <ul> 
     <li><code>Key </code>enthält den eindeutigen Wert.</li> 
     <li><code>Array </code>enthält die aggregierten Daten aus den Bundles, für die die Formel zur <code>Key </code>-Wert.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Verarbeitung nach einer leeren Aggregation stoppen</p> </td> 
   <td> <p>Standardmäßig gibt das Modul [!UICONTROL Aggregator] das Ergebnis der Aggregation aus, selbst wenn keine Pakete das [!UICONTROL Aggregator]-Modul erreicht haben (z. B. weil sie alle auf ihrem Weg herausgefiltert wurden). Wenn die Option [!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen] aktiviert ist, erzeugt das Modul [!UICONTROL Aggregator] in diesem Fall kein Ausgabebundle und der Fluss stoppt.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Bundles, die von Modulen zwischen dem Quellmodul und dem [!UICONTROL Aggregator] -Modul nicht von der [!UICONTROL Aggregator] -Modul, sodass sie für die Module im Fluss nach dem [!UICONTROL Aggregator]. Wenn Sie Daten aus einem Bundle benötigen, das von einem Modul zwischen dem Quellmodul und dem [!UICONTROL Aggregator] -Modul, stellen Sie sicher, dass das angegebene Element in die [!UICONTROL Aggregator] -Moduleinrichtung (wie im [!UICONTROL Aggregierte Felder] -Feld in der Einrichtung der [!UICONTROL Array-Aggregator] -Modul).


>[!INFO]
>
>**Beispiel:** Anwendungsbeispiel: Alle E-Mail-Anhänge komprimieren und die ZIP-Datei in hochladen [!DNL Dropbox]
>
>Das folgende Szenario zeigt, wie:
>
>* Postfach auf eingehende E-Mails achten: [!UICONTROL Email] >[!UICONTROL E-Mails ansehen] Trigger gibt ein Bundle mit Element aus `Attachments[]`: Array, das alle Anlagen der E-Mail enthält.
>
>* Iterate the email&#39;s attachments: [!UICONTROL Email] >[!UICONTROL Anhänge itterieren] Der Iterator nimmt die Elemente aus der `Attachments[]` -Array nach dem anderen und sendet sie als separate Bundles weiter.
>
>* Aggregieren Sie die von der [!UICONTROL Email] >[!UICONTROL Anhänge itterieren] -Modul: [!UICONTROL Archivieren] >[!UICONTROL Erstellen eines Archiv-Aggregators] sammelt alle Bundles, die es empfängt, und gibt ein einzelnes Bundle aus, das die ZIP-Datei enthält.
>
>* Laden Sie die resultierende ZIP-Datei in [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Datei hochladen] ruft die ZIP-Datei von der [!UICONTROL Archivieren] > [!UICONTROL Erstellen eines Archivs] -Modul und lädt es in [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>Nachfolgend finden Sie ein Beispiel für die Einrichtung der [!UICONTROL Archivieren] > [!UICONTROL Erstellen eines Archivs] Aggregator:
>
>![](assets/archive-create-an-archive-350x484.png)
