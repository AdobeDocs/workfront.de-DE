---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Router-Modul in Adobe Workfront Fusion
description: Mit dem Router-Modul können Sie Ihren Fluss in mehrere Routen verzweigen und die Daten in den einzelnen Routen unterschiedlich verarbeiten. Sobald ein Router-Modul ein Bundle erhält, leitet es es an jede verbundene Route weiter in der Reihenfolge, in der die Routen an das Router-Modul angehängt wurden.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!UICONTROL Router] -Modul in [!DNL Adobe Workfront Fusion]

Die [!UICONTROL Router] ermöglicht es Ihnen, Ihren Fluss in mehrere Routen zu verzweigen und die Daten innerhalb der einzelnen Routen unterschiedlich zu verarbeiten. Einmal [!UICONTROL Router] -Modul ein Bundle erhält, es an jede verbundene Route weiterleitet, in der die Routen an die [!UICONTROL Router] -Modul.

>[!NOTE]
>
>* Um die Reihenfolge der Routen zu überprüfen, können Sie auf die [!UICONTROL Automatische Ausrichtung] -Symbol, über das die Routen entsprechend der Reihenfolge von oben nach unten angeordnet werden.
>
>  Um die Reihenfolge zu ändern, entfernen Sie die [!UICONTROL Router] und verbinden Sie die Routen in der gewünschten Reihenfolge neu.
>
>* Routen werden nacheinander, nicht parallel verarbeitet. Ein Bundle wird erst dann an die nächste Route gesendet, wenn es vollständig von der vorherigen Route verarbeitet wurde.
>



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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Hinzufügen einer [!UICONTROL Router] -Modul in ein Szenario

A [!UICONTROL Router] kann auf eine der folgenden Arten zu einem Szenario hinzugefügt werden:

* Wenn Sie die [!UICONTROL Router] -Modul nach einem Modul, klicken Sie auf den rechten Griff des Moduls und beginnen Sie mit der Eingabe **[!UICONTROL Router]** , um danach zu suchen, und wählen Sie **[!UICONTROL Flusssteuerung]** > **[!UICONTROL Router]** in der Liste der Module, die angezeigt werden.

  ![](assets/connect-the-router-350x108.png)

* Wenn Sie die [!UICONTROL Router] -Modul zwischen zwei Modulen, klicken Sie auf das Schraubenschlüsselsymbol unter der Route, die die beiden Module verbindet (oder klicken Sie mit der rechten Maustaste auf die Route) und wählen Sie **[!UICONTROL Router hinzufügen]** aus dem Menü.

  ![](assets/insert-router-350x191.png)

* Sie können eine [!UICONTROL Router] automatisch hinzugefügt. Um beispielsweise in der Abbildung unten das Modul in der unteren rechten Ecke mit dem Modul in der oberen linken Ecke zu verbinden (das bereits mit dem Modul in der oberen rechten Ecke verbunden ist), ziehen Sie den linken Ziehpunkt des unteren rechten Moduls und legen Sie es auf das Modul oben links ab.

  ![](assets/insert-router-automatically-350x379.png)

## Filter

Sie können einen Filter auf eine Route nach der [!UICONTROL Router] -Modul verwenden, um Bundles wie auf jeder anderen Route zu filtern:

1. Klicken Sie auf einen der Punkte in der Route.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. Im **[!UICONTROL Filter einrichten]** -Feld, das angezeigt wird, Bedingungen hinzufügen und dann auf **[!UICONTROL OK]** , um die Filtereinrichtung zu speichern.

   ![](assets/set-up-a-filter-2-350x242.png)

Weitere Informationen finden Sie unter [Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Die Ausweichroute

Die Filtereinrichtung auf einer Route nach einer [!UICONTROL Router] -Modul enthält eine spezielle Option: Die Ausweichroute:

![](assets/fallback-route-350x260.png)

Wenn diese Route aktiviert ist, wird sie verwendet, wenn ein Bundle nicht über die [!UICONTROL Router] -Modul über eine andere Route, da die Filter auf den anderen Routen es herausgefiltert haben.

Die Fallback-Route wird mit einem anderen Pfeilzeichen innerhalb der [!UICONTROL Router] -Modul:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Ein typischer Anwendungsfall der Ausweichroute besteht darin, den Fluss mit einer Route fortzusetzen, wenn die Bedingung erfüllt ist, und mit einer anderen Route, falls dies nicht der Fall ist, wie in den folgenden Schritten gezeigt:

1. Einfügen einer [!UICONTROL Router] -Modul in Ihrem Szenario.
1. Verbinden Sie beide Routen mit dem [!UICONTROL Router] Modul .
1. Klicken Sie auf die erste Route und geben Sie eine Bedingung an:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Klicken Sie auf die zweite Route und aktivieren Sie die [!UICONTROL Ausweichroute] Option:

   ![](assets/enable-fallback-route-option-350x238.png)
