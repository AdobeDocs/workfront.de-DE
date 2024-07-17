---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Planen eines Szenarios in Adobe Workfront Fusion
description: Standardmäßig wird ein Szenario alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft ein aktiviertes Szenario ausgeführt wird.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Ein Szenario in [!DNL Adobe Workfront Fusion] planen

Standardmäßig wird ein Szenario alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft ein aktiviertes Szenario ausgeführt wird. Fusionsszenarien können so oft wie alle 5 Minuten ausgeführt werden.

## Zugriffsanforderungen

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td>    </tr> 
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

## Planen eines Szenarios

1. Klicken Sie oben rechts auf der Detailseite &quot;Szenario&quot;auf **[!UICONTROL Optionen]** > **[!UICONTROL Zeitplan]** .

   Oder

   Klicken Sie auf das Symbol **[!UICONTROL Planung]** (Uhr) im Trigger-Modul des Szenarios.

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
        <li> <p><strong>[!UICONTROL Einmal]</strong> </p> <p>Geben Sie das Datum und die Uhrzeit ein, zu dem das Szenario ausgeführt werden soll. Verwenden Sie das Format <code>MM/DD/YYYY h:mm A</code>. Beispiel: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Jeden Tag]</strong> </p> <p>Geben Sie den Zeitpunkt ein, zu dem das Szenario ausgeführt werden soll. Verwenden Sie das Format <code>h:mm A</code>. Beispiel: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Wochentage]</strong> </p> <p>Tage: Wählen Sie die Wochentage aus, an denen das Szenario ausgeführt werden soll. Sie können einen oder mehrere Tage auswählen.</p> <p>Zeit: Geben Sie die Zeit ein, zu der das Szenario an den ausgewählten Tagen ausgeführt werden soll. Verwenden Sie das Format <code>h:mm A</code>. Beispiel: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Tage des Monats]</strong> </p> <p>Tage: Wählen Sie die Tage des Monats aus, an denen das Szenario ausgeführt werden soll. Sie können einen oder mehrere Tage auswählen.</p> <p>Zeit: Geben Sie die Zeit ein, zu der das Szenario an den ausgewählten Tagen ausgeführt werden soll. Verwenden Sie das Format <code>h:mm A</code>. Beispiel: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Angegebene Datumswerte]</strong> </p> <p>Monate: Wählen Sie die Monate aus, in denen das Szenario ausgeführt werden soll. Sie können einen oder mehrere Monate auswählen.</p> <p>Tage: Wählen Sie die Tage des Monats aus, an denen das Szenario ausgeführt werden soll. Sie können einen oder mehrere Tage auswählen.</p> <p>Zeit: Geben Sie die Zeit ein, zu der das Szenario an den ausgewählten Tagen ausgeführt werden soll. Verwenden Sie das Format <code>h:mm A</code>. Beispiel: <code>11:00 PM</code></p> </li> 
       </ul> <p>Hinweis: Ein Datum muss vorhanden sein, damit ein Szenario an diesem Datum ausgeführt werden kann. Beispielsweise wird ein Szenario, das nur für den 31. des Monats geplant ist, nicht im Februar, April, Juni, September oder November ausgeführt, da diese Monate keinen 31. Tag haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Erweiterte Planung]</td> 
      <td>Sie können bestimmte Zeitintervalle definieren, in denen Ihr Szenario ausgeführt werden soll. Sie können Tageszeiträume, Wochentage oder Monate angeben. Klicken Sie für jedes Intervall auf <strong>[!UICONTROL Add]</strong> und füllen Sie die Felder wie im Feld [!UICONTROL Run scenario] beschrieben aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Geben Sie das Datum und die Uhrzeit ein, nach denen das Szenario ausgeführt werden soll. Verwenden Sie das Format <code>MM/DD/YYYY h:mm A</code>. Beispiel: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ende]</td> 
      <td>Geben Sie das Datum und die Uhrzeit ein, vor denen das Szenario ausgeführt werden soll. Verwenden Sie das Format <code>MM/DD/YYYY h:mm A</code>. Beispiel: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL OK]** , um die Zeitplaneinstellungen zu speichern und zum Szenario zurückzukehren.
