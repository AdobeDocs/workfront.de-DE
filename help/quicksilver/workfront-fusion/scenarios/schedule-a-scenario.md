---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Planen eines Szenarios in Adobe Workfront Fusion
description: Standardmäßig wird ein Szenario alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft ein aktiviertes Szenario ausgeführt wird.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# Planen eines Szenarios in [!DNL Adobe Workfront Fusion]

Standardmäßig wird ein Szenario alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft ein aktiviertes Szenario ausgeführt wird.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung] </p>  </td>    </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Planen eines Szenarios

1. Klicken Sie in der rechten oberen Ecke der Detailseite &quot;Szenario&quot;auf **[!UICONTROL Optionen]** > **[!UICONTROL Planung]**

   Oder

   Klicken Sie auf **[!UICONTROL Planung]** -Symbol (Uhr) auf dem Trigger-Modul des Szenarios angezeigt.

1. Geben Sie Informationen in die folgenden Felder ein:

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ausführungsszenario]</td> 
      <td> <p>Wählen Sie die Häufigkeit aus, mit der Sie das Szenario ausführen möchten, und wählen Sie dann das Intervall aus.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL in regelmäßigen Abständen]</strong> </p> <p>Geben Sie die Anzahl der Minuten zwischen den Ausführungen ein. Der Standardwert ist 15 Minuten.</p> </li> 
        <li> <p><strong>[!UICONTROL Einmal]</strong> </p> <p>Geben Sie das Datum und die Uhrzeit ein, zu dem das Szenario ausgeführt werden soll. Format verwenden <code>MM/DD/YYYY h:mm A</code>. Beispiel: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Jeden Tag]</strong> </p> <p>Geben Sie den Zeitpunkt ein, zu dem das Szenario ausgeführt werden soll. Format verwenden <code>h:mm A</code>. Beispiel: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Wochentage]</strong> </p> <p>Tage: Wählen Sie die Wochentage aus, an denen das Szenario ausgeführt werden soll. Sie können einen oder mehrere Tage auswählen.</p> <p>Zeit: Geben Sie die Zeit ein, zu der das Szenario an den ausgewählten Tagen ausgeführt werden soll. Format verwenden <code>h:mm A</code>. Beispiel: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Tage des Monats]</strong> </p> <p>Tage: Wählen Sie die Tage des Monats aus, an denen das Szenario ausgeführt werden soll. Sie können einen oder mehrere Tage auswählen.</p> <p>Zeit: Geben Sie die Zeit ein, zu der das Szenario an den ausgewählten Tagen ausgeführt werden soll. Format verwenden <code>h:mm A</code>. Beispiel: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Festgelegte Datumswerte]</strong> </p> <p>Monate: Wählen Sie die Monate aus, in denen das Szenario ausgeführt werden soll. Sie können einen oder mehrere Monate auswählen.</p> <p>Tage: Wählen Sie die Tage des Monats aus, an denen das Szenario ausgeführt werden soll. Sie können einen oder mehrere Tage auswählen.</p> <p>Zeit: Geben Sie die Zeit ein, zu der das Szenario an den ausgewählten Tagen ausgeführt werden soll. Format verwenden <code>h:mm A</code>. Beispiel: <code>11:00 PM</code></p> </li> 
       </ul> <p>Hinweis: Damit ein Szenario an diesem Datum ausgeführt werden kann, muss ein Datum vorhanden sein. Beispielsweise wird ein Szenario, das nur für den 31. des Monats geplant ist, nicht im Februar, April, Juni, September oder November ausgeführt, da diese Monate keinen 31. Tag haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Erweiterte Planung]</td> 
      <td>Sie können bestimmte Zeitintervalle definieren, in denen Ihr Szenario ausgeführt werden soll. Sie können Tageszeiträume, Wochentage oder Monate angeben. Klicken Sie für jedes Intervall auf <strong>[!UICONTROL Hinzufügen]</strong> und füllen Sie die Felder wie im Feld [!UICONTROL Run scenario] beschrieben aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Geben Sie das Datum und die Uhrzeit ein, nach denen das Szenario ausgeführt werden soll. Format verwenden <code>MM/DD/YYYY h:mm A</code>. Beispiel: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ende]</td> 
      <td>Geben Sie das Datum und die Uhrzeit ein, vor denen das Szenario ausgeführt werden soll. Format verwenden <code>MM/DD/YYYY h:mm A</code>. Beispiel: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL OK]** , um die Zeitplaneinstellungen zu speichern und zum Szenario zurückzukehren.
