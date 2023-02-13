---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Typenzwang in Adobe Workfront Fusion
description: In diesem Dokument wird beschrieben, wie [!DNL Adobe Workfront Fusion] verhält sich in Situationen, in denen Werte in erwarteten und unerwarteten Datenformaten empfangen werden.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 1%

---

# Typenkonvertierung in [!DNL Adobe Workfront Fusion]

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

### Typerzwingung

In diesem Dokument wird beschrieben, wie [!DNL Adobe Workfront Fusion] verhält sich in Situationen, in denen Werte in erwarteten und unerwarteten Datenformaten empfangen werden.

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
   <td> <p>Wenn der empfangene Wert nicht vom Array-Typ ist, [!DNL Workfront Fusion] erstellt ein Array und das erste (und einzige) Element ist der empfangene Wert.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>boolean </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>number </td> 
   <td> <p>Der Wert wird in "Logisches Ja"konvertiert, auch wenn der Wert 0 beträgt.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>text </td> 
   <td> <p>Wenn der Wert gleich false oder leer ist, wird er in logisches Nein konvertiert. Wenn nicht, wird sie in "logisches Ja"konvertiert.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>other </td> 
   <td> <p>Der Wert wird in "Logisches Ja"konvertiert, wenn der empfangene Wert vorhanden ist (nicht null ist).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>Der Wert wird nur dann unverändert übergeben, wenn die Codepage erwartungsgemäß ist. Wenn sich die Codepage unterscheidet, [!DNL Workfront Fusion] versucht, den empfangenen Wert in die angeforderte Codepage zu konvertieren. Wenn diese Konvertierung nicht unterstützt wird, [!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>boolean </td> 
   <td> <p>Der Wert wird in Text (true/false) und dann in Binärdaten konvertiert, wie oben beschrieben, um in Text zu konvertieren.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>date </td> 
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
   <td>date </td> 
   <td>date </td> 
   <td> <p>Der Wert wird unverändert übergeben.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] versucht, den Text in ein Datum zu konvertieren. Wenn die Konvertierung fehlschlägt, wird ein Validierungsfehler zurückgegeben. Das Datum muss Tag, Monat und Jahr enthalten. Das Datum kann Uhrzeit und Zeitzone enthalten. Die Standardzeitzone basiert auf Ihren Einstellungen. Beispiele:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
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
   <td> <p>Wenn das angegebene Array die Konvertierung in Text unterstützt, wird der Wert konvertiert. Wenn nicht, [!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>boolean </td> 
   <td> <p>Der Wert wird in Text umgewandelt (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffer </td> 
   <td> <p>Wenn für Binärdaten eine Textkodierung angegeben ist, wird der Wert in Text konvertiert. Wenn nicht, [!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>date </td> 
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
   <td> <p>[!DNL Workfront Fusion] versucht, die Zeit in Stunden umzurechnen:minutes:Sekunden-Format. Wenn die Konvertierung fehlschlägt, wird ein Validierungsfehler zurückgegeben.</p> </td> 
  </tr> 
  <tr> 
   <td>Uhrzeit </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] gibt einen Validierungsfehler zurück.</p> </td> 
  </tr> 
 </tbody> 
</table>
