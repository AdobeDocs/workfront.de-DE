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
source-git-commit: 948fe5fc249e0dcb04655f015c8e46493159c3ed
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# [!UICONTROL Aggregator]-Modul in [!DNL Adobe Workfront Fusion]

Ein Aggregatormodul ist ein Modultyp, der dazu dient, mehrere Datenbündel in einem Bundle zusammenzuführen.

Weitere Informationen zu Modultypen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
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

+++

## Überblick über das Modul [!UICONTROL Aggregator]

Wenn ein [!UICONTROL Aggregator] -Modul ausgeführt wird, wird Folgendes ausgeführt:

* Akkumuliert alle Bundles, die es während des Vorgangs eines einzelnen Quellmoduls erhält.
* Gibt ein einzelnes Bundle mit einem Array aus, das pro akkumuliertem Bundle ein Element enthält. Der Inhalt der Elemente des Arrays hängt von dem jeweiligen [!UICONTROL Aggregator]-Modul und dessen Einrichtung ab.

Die folgende Abbildung zeigt eine typische Einrichtung des Moduls [!UICONTROL Aggregator] :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>Das Modul, in dem die Bundle-Aggregation beginnt. Das Quellmodul ist normalerweise ein Iterator oder ein Suchmodul, das eine Reihe von Bundles ausgibt.</p><p>Wenn Sie das Quellmodul des Aggregators einrichten (und die Einrichtung des Aggregators schließen), wird die Route zwischen dem Quellmodul und dem Aggregatormodul in einen grauen Bereich eingeschlossen, sodass Sie den Beginn und das Ende der Aggregation deutlich sehen können. 
   </p> <p>Weitere Informationen zu Iteratoren finden Sie unter <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator]-Modul in [!DNL Adobe Workfront Fusion]</a></p> <p>Weitere Informationen zu Suchmodulen finden Sie unter Suchmodule in <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Modultypen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target-Strukturtyp]</p> </td> 
   <td> <p>(Gilt nur für das [!UICONTROL Array Aggregator]-Modul.) Die Zielstruktur, in der die Daten aggregiert werden. Mit der Standardoption [!UICONTROL Benutzerdefiniert] können Sie Elemente auswählen, die im <code>Array </code> -Element des Ausgabebundles des [!UICONTROL Array Aggregators] aggregiert werden sollen:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Sobald Sie weitere Module nach dem [!UICONTROL Array Aggregator]-Modul verbinden und zum Setup des Moduls zurückkehren, enthält das Dropdown-Menü vom Strukturtyp [!UICONTROL Target] alle folgenden Module und deren Felder vom Typ "Array of Collections", wie im Feld [!UICONTROL Attachments] des Moduls [!DNL Slack] &gt;[!UICONTROL Nachricht erstellen] dargestellt:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregierte Felder]</td> 
   <td>Die Felder, die Sie in die Aggregatormodulausgabe einbeziehen möchten.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Gruppe nach]</p> </td> 
   <td> <p>Die Ausgabe des Aggregators kann mithilfe des Felds [!UICONTROL Group by] in mehrere Gruppen aufgeteilt werden. Das Feld [!UICONTROL Gruppe nach] kann eine Formel enthalten, die für das Eingabepaket jedes Aggregators ausgewertet wird. Der Aggregator gibt dann ein Bundle pro Wert jeder einzelnen Formel aus. Jedes Bundle enthält zwei Elemente:</p> 
    <ul> 
     <li><code>Key </code>enthält den eindeutigen Wert.</li> 
     <li><code>Array </code>enthält die aggregierten Daten aus den Bundles, für die die Formel zum <code>Key </code>Wert ausgewertet wurde.</li> 
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
>Bundles, die von Modulen zwischen dem Quellmodul und dem Modul [!UICONTROL Aggregator] generiert wurden, werden nicht vom Modul [!UICONTROL Aggregator] ausgegeben, sodass sie für die Module im Fluss nach dem Modul [!UICONTROL Aggregator] nicht zugänglich sind. Wenn Sie Daten aus einem von einem Modul zwischen dem Quellmodul und dem Modul [!UICONTROL Aggregator] ausgegebenen Bundle benötigen, stellen Sie sicher, dass Sie das angegebene Element in die Einrichtung des Moduls [!UICONTROL Aggregator] einbeziehen (wie im Feld [!UICONTROL Aggregierte Felder] bei der Einrichtung des Moduls [!UICONTROL Array Aggregator] ).


## Beispielszenario der Funktionsweise von Aggregatoren

Dieses Beispielszenario zeigt, wie Sie alle E-Mail-Anhänge komprimieren und die ZIP-Datei auf [!DNL Dropbox] hochladen.

![](assets/dropbox-archive-350x87.png)

Das folgende Szenario zeigt, wie:

* Das erste Modul überwacht ein Postfach auf eingehende E-Mails: Der Trigger [!UICONTROL E-Mail] >[!UICONTROL E-Mails ansehen] gibt ein Bundle mit dem Element `Attachments[]` aus, wobei es sich um ein Array mit allen Anhängen der E-Mail handelt.

* Das zweite Modell iteriert die Anlagen der E-Mail: [!UICONTROL E-Mail] >[!UICONTROL Iterate attachments] iterator übernimmt die Elemente aus dem `Attachments[]` -Array nacheinander und sendet sie als separate Bundles weiter.

* Das dritte Modul aggregiert die Bundles, die vom Modul [!UICONTROL E-Mail] >[!UICONTROL Anlagen durchsuchen] ausgegeben werden: [!UICONTROL Archiv] >[!UICONTROL Erstellen eines Archiv-Aggregators] sammelt alle Bundles, die es empfängt, und gibt ein einzelnes Bundle aus, das die ZIP-Datei enthält.

* Das letzte Modul lädt die resultierende ZIP-Datei in [!DNL Dropbox] hoch: [!DNL Dropbox] > [!UICONTROL Eine Datei hochladen] ruft die ZIP-Datei aus dem Modul [!UICONTROL Archiv] > [!UICONTROL Archiv erstellen] auf und lädt sie in [!DNL Dropbox] hoch.



Nachfolgend finden Sie ein Beispiel für die Einrichtung des Aggregators [!UICONTROL Archiv] > [!UICONTROL Archiv erstellen] :

![](assets/archive-create-an-archive-350x484.png)
