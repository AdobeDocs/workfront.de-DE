---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Fehlerbehebung beim Text-Parser in [!DNL Adobe Workfront Fusion]
description: Verwenden Sie diese Informationen, wenn Sie keinen Text-Parser erhalten können, um eine Ausgabe zu erzeugen.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Fehlerbehebung beim Text-Parser in [!DNL Adobe Workfront Fusion]

Verwenden Sie diese Informationen, wenn Sie keinen Text-Parser erhalten können, um eine Ausgabe zu erzeugen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
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

## Fehlerbehebung

Im vorliegenden Beispiel soll der Dateityp des Dateidokuments „filename.docx“ analysiert werden. Die Dateinamenerweiterung variiert dabei von DOCX zu PDF zu CSV.

Der Ausdruck, den Sie in diesem Fall verwenden können, lautet [!DNL \..+]

Wenn Sie dies für den Regex-Ausdruck auf regex101.com verwenden, erhalten Sie eine vollständige Übereinstimmung.

![](assets/regex-expression-350x130.png)

Auf der Abbildung oben wurde die Dateierweiterung korrekt zugeordnet. Wenn Sie dies verwenden und versuchen, es in Ihrem Text-Parser zu implementieren:

![](assets/text-parser-350x602.png)

Sie erhalten keine Übereinstimmung:

![](assets/text-parser-you-dont-get-a-match-350x365.png)

Der Grund dafür ist, dass das „i“ nur die Anzahl der Übereinstimmungen pro Übereinstimmung anzeigt. In diesem Fall haben wir also 2 Übereinstimmungen, daher gibt es nach dem „i“ einen numerischen Wert 1 und 2. Der Anwendungsfall hierfür besteht darin, dass Sie, falls Sie Daten jemals mit dem zweiten übereinstimmenden Wert abgleichen oder durch einen Filter übergeben müssen, angeben können, welcher Wert durch den numerischen Wert dargestellt wird.

![](assets/text-parser-matches-350x355.png)

Um die Übereinstimmungswerte abzurufen, die Sie benötigen, um dem zu analysierenden Teil Klammern hinzuzufügen (z. B. um nur aus „filename.docx“ - „docx“ zu extrahieren), sollten die Klammern gemäß dem Regex-Ausdruck, den wir für dieses Szenario verwenden, auf \ angewendet werden.(.+)

Erfasst das DOCX, platziert es in einer Gruppe und lässt das &quot;.“ Raus damit.

![](assets/text-parser-get-matches-350x592.png)

In der im folgenden Bild gezeigten Ausgabe entspricht die Erfassungsgruppe einem beliebigen Zeichen (mit Ausnahme der Zeilenumbrüche).

![](assets/text-parser-output-350x389.png)

Eine weitere Problemumgehung, die auch Regex enthält, ist die Verwendung der Funktion Ersetzen .

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

Ersetzen Sie dann `abcdefghijklmno pqr stuvw xyz.docx` durch die eigentliche Dateinamenvariable .
