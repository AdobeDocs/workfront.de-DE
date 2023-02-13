---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Fehlerbehebung bei Text-Parsern in [!DNL Adobe Workfront Fusion]
description: Verwenden Sie diese Informationen, wenn Sie keinen Text-Parser zur Ausgabe erhalten können.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Fehlerbehebung bei Text-Parsern in [!DNL Adobe Workfront Fusion]

Verwenden Sie diese Informationen, wenn Sie keinen Text-Parser erhalten können, um eine Ausgabe zu erzeugen.

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

## Fehlerbehebung

Im Beispielszenario möchten Sie den Dateityp eines Dateidokuments &quot;filename.docx&quot;analysieren und die Erweiterung des Dateinamens variiert immer von DOCX über PDF bis CSV.

Der Ausdruck, den Sie in diesem Fall verwenden können, lautet [!DNL \..+]

Wenn Sie dies auf Regex-Ausdruck auf regex101.com verwenden würden, erhalten Sie eine vollständige Übereinstimmung.

![](assets/regex-expression-350x130.png)

Auf dem Bild oben wurde die Dateierweiterung korrekt zugeordnet. Wenn Sie dies vornehmen und versuchen, es in Ihrem Text-Parser zu implementieren:

![](assets/text-parser-350x602.png)

Sie erhalten keine Übereinstimmung:

![](assets/text-parser-you-dont-get-a-match-350x365.png)

Der Grund dafür ist, dass das &quot;i&quot;nur die Anzahl der Übereinstimmungen pro Übereinstimmung anzeigt. In diesem Fall haben wir also 2 Übereinstimmungen, daher gibt es nach dem &quot;i&quot;einen numerischen Wert 1 und 2. Der Anwendungsfall dafür besteht darin, dass Sie, wenn Sie Daten je nur über den zweiten übereinstimmenden Wert über einen Filter abgleichen oder weitergeben müssen, den Wert angeben können, der durch den numerischen Wert dargestellt wird.

![](assets/text-parser-matches-350x355.png)

Um die Übereinstimmungswerte abzurufen, die Sie benötigen, um dem Teil, den Sie analysieren möchten (z. B. um aus &quot;filename.docx&quot;- nur &quot;docx&quot; zu extrahieren), sollten die Klammern gemäß dem für dieses Szenario verwendeten Regex-Ausdruck auf \ angewendet werden.(.+)

Dadurch wird das DOCX erfasst, in eine Gruppe eingefügt und der &quot;&quot;.&quot; aus.

![](assets/text-parser-get-matches-350x592.png)

In der Ausgabe, die im folgenden Bild gezeigt wird, stimmt die Erfassungsgruppe mit jedem Zeichen überein (mit Ausnahme der Zeilenenden).

![](assets/text-parser-output-350x389.png)

Eine weitere Problemumgehung, die auch regex enthält, ist die Verwendung der Funktion replace .

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

Dann ersetzen `abcdefghijklmno pqr stuvw xyz.docx` mit Ihrer eigentlichen Dateinamenvariable.
