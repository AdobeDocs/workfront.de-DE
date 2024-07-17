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

# Modul [!UICONTROL Router] in [!DNL Adobe Workfront Fusion]

Mit dem Modul [!UICONTROL Router] können Sie Ihren Fluss in mehrere Routen verzweigen und die Daten in den einzelnen Routen unterschiedlich verarbeiten. Sobald ein Modul vom Typ [!UICONTROL Router] ein Bundle erhält, leitet es es an jede verbundene Route weiter, in der Reihenfolge, in der die Routen mit dem Modul [!UICONTROL Router] verbunden waren.

>[!NOTE]
>
>* Um die Reihenfolge der Routen zu überprüfen, können Sie auf das Symbol [!UICONTROL Automatische Ausrichtung] klicken, mit dem die Routen entsprechend der Reihenfolge von oben nach unten angeordnet werden.
>
>  Um die Reihenfolge zu ändern, entfernen Sie das Modul [!UICONTROL Router] und verbinden Sie die Routen in der gewünschten Reihenfolge erneut.
>
>* Routen werden nacheinander, nicht parallel verarbeitet. Ein Bundle wird erst dann an die nächste Route gesendet, wenn es vollständig von der vorherigen Route verarbeitet wurde.
>



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

## Hinzufügen eines [!UICONTROL Router]-Moduls zu einem Szenario

Ein [!UICONTROL Router] kann einem Szenario auf eine der folgenden Arten hinzugefügt werden:

* Wenn Sie das Modul [!UICONTROL Router] nach einem Modul verbinden möchten, klicken Sie auf den rechten Griff des Moduls. Geben Sie dann **[!UICONTROL Router]** ein, um danach zu suchen. Wählen Sie dann **[!UICONTROL Flusssteuerung]** > **[!UICONTROL Router]** in der Liste der angezeigten Module.

  ![](assets/connect-the-router-350x108.png)

* Wenn Sie das Modul [!UICONTROL Router] zwischen zwei Modulen einfügen möchten, klicken Sie auf das Schraubenschlüsselsymbol unter der Route, die die beiden Module verbindet (oder klicken Sie mit der rechten Maustaste auf die Route) und wählen Sie im Menü die Option **[!UICONTROL Router hinzufügen]** aus.

  ![](assets/insert-router-350x191.png)

* Sie können ein Modul [!UICONTROL Router] automatisch einfügen. Um beispielsweise in der Abbildung unten das Modul in der unteren rechten Ecke mit dem Modul in der oberen linken Ecke zu verbinden (das bereits mit dem Modul in der oberen rechten Ecke verbunden ist), ziehen Sie den linken Ziehpunkt des unteren rechten Moduls und legen Sie es auf das Modul oben links ab.

  ![](assets/insert-router-automatically-350x379.png)

## Filter

Sie können einen Filter auf eine Route nach dem Modul [!UICONTROL Router] platzieren, um Bundles wie auf jeder anderen Route zu filtern:

1. Klicken Sie auf einen der Punkte in der Route.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. Fügen Sie im angezeigten Feld **[!UICONTROL Filter einrichten]** Bedingungen hinzu und klicken Sie auf **[!UICONTROL OK]** , um die Filtereinrichtung zu speichern.

   ![](assets/set-up-a-filter-2-350x242.png)

Weitere Informationen finden Sie unter [Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Die Ausweichroute

Die Filtereinrichtung auf einer Route nach einem Modul [!UICONTROL Router] enthält eine spezielle Option: Die Ausweichroute:

![](assets/fallback-route-350x260.png)

Wenn diese Route aktiviert ist, wird sie verwendet, wenn ein Bundle nicht über eine andere Route über das Modul [!UICONTROL Router] fortfahren kann, da die Filter auf den anderen Routen es herausgefiltert haben.

Die Fallback-Route wird mit einem anderen Pfeilzeichen innerhalb des Moduls [!UICONTROL Router] unterschieden:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Ein typischer Anwendungsfall der Ausweichroute besteht darin, den Fluss mit einer Route fortzusetzen, wenn die Bedingung erfüllt ist, und mit einer anderen Route, falls dies nicht der Fall ist, wie in den folgenden Schritten gezeigt:

1. Fügen Sie ein [!UICONTROL Router] -Modul in Ihr Szenario ein.
1. Verbinden Sie beide Routen mit dem Modul [!UICONTROL Router] .
1. Klicken Sie auf die erste Route und geben Sie eine Bedingung an:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Klicken Sie auf die zweite Route und aktivieren Sie die Option [!UICONTROL Ausweichroute] :

   ![](assets/enable-fallback-route-option-350x238.png)
