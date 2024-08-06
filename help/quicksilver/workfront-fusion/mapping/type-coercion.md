---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Typenzwang in Adobe Workfront Fusion
description: In diesem Dokument wird beschrieben, wie sich [!DNL Adobe Workfront Fusion] in Situationen verhält, in denen Werte in erwarteten und unerwarteten Datenformaten empfangen werden.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: d09174b874ff59676a28881de02ae4e7196d0f80
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 3%

---

# Typerzwingung in [!DNL Adobe Workfront Fusion]

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

### Typerzwingung

In diesem Dokument wird beschrieben, wie sich [!DNL Adobe Workfront Fusion] in Situationen verhält, in denen Werte in erwarteten und unerwarteten Datenformaten empfangen werden.

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Erwartet</th> 
   <th>Erhalten</th> 
   <th> <p>Beschreibung</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>array </td> 
   <td>array </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>array </td> 
   <td>other </td> 
   <td> <p>Wenn der empfangene Wert nicht vom Array-Typ ist, erstellt [!DNL Workfront Fusion] ein Array und das erste (und einzige) Element ist der empfangene Wert.</p> </td> 
  </tr> 
  <tr> 
   <td>Boolescher Wert </td> 
   <td>Boolescher Wert </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>Boolescher Wert </td> 
   <td>number </td> 
   <td> <p>Der Wert wird in "Logisches Ja"konvertiert, auch wenn der Wert 0 beträgt.</p> </td> 
  </tr> 
  <tr> 
   <td>Boolescher Wert </td> 
   <td>text </td> 
   <td> <p>Wenn der Wert gleich false oder leer ist, wird er in logisches Nein konvertiert. Wenn nicht, wird sie in "logisches Ja"konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>Boolescher Wert </td> 
   <td>other </td> 
   <td> <p>Der Wert wird in "Logisches Ja"konvertiert, wenn der empfangene Wert vorhanden ist (nicht null ist).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>Der Wert wird nur dann unverändert übergeben, wenn die Codepage erwartungsgemäß ist. Wenn die Codepage unterschiedlich ist, versucht [!DNL Workfront Fusion], den empfangenen Wert in die angeforderte Codepage zu konvertieren. Wenn diese Konvertierung nicht unterstützt wird, gibt [!DNL Workfront Fusion] einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>Boolescher Wert </td> 
   <td> <p>Der Wert wird in Text (true/false) und dann in Binärdaten konvertiert, wie oben beschrieben, um in Text zu konvertieren.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>Datum </td> 
   <td> <p>Der Wert wird in ISO 8601-Text und dann in Binärdaten konvertiert, entsprechend den Schritten, die für die Konvertierung in Text angegeben wurden.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>number </td> 
   <td> <p>Der Wert wird in Text und anschließend in Binärdaten konvertiert, wie oben beschrieben, um ihn in Text zu konvertieren.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>text </td> 
   <td> <p>Der Wert wird in Binärdaten konvertiert und erwartungsgemäß kodiert. Wenn die erwartete Kodierung nicht angegeben ist, wird utf8-Kodierung verwendet.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>collection </td> 
   <td>collection </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>collection </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>Datum </td> 
   <td>Datum </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>Datum </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] versucht, den Text in ein Datum zu konvertieren. Wenn die Konvertierung fehlschlägt, wird ein Validierungsfehler zurückgegeben. Das Datum muss Tag, Monat und Jahr enthalten. Das Datum kann Uhrzeit und Zeitzone enthalten. Die Standardzeitzone basiert auf Ihren Einstellungen. Beispiele:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Datum </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>number </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] versucht, den Text in eine Zahl zu konvertieren. Wenn die Konvertierung fehlschlägt, wird ein Validierungsfehler zurückgegeben.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>text </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>array </td> 
   <td> <p>Wenn das angegebene Array die Konvertierung in Text unterstützt, wird der Wert konvertiert. Andernfalls gibt [!DNL Workfront Fusion] einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>Boolescher Wert </td> 
   <td> <p>Der Wert wird in Text umgewandelt (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffer </td> 
   <td> <p>Wenn für Binärdaten eine Textkodierung angegeben ist, wird der Wert in Text konvertiert. Andernfalls gibt [!DNL Workfront Fusion] einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>Datum </td> 
   <td> <p>Der Wert wird in ISO 8601-Text konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>number </td> 
   <td> <p>Der Wert wird in Text umgewandelt.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>Uhrzeit </td> 
   <td>Uhrzeit </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>Uhrzeit </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] versucht, die Zeit in das Stunden:minutes:Sekunden-Format zu konvertieren. Wenn die Konvertierung fehlschlägt, wird ein Validierungsfehler zurückgegeben.</p> </td> 
  </tr> 
  <tr> 
   <td>Uhrzeit </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
 </tbody> 
</table>
