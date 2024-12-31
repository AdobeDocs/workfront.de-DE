---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Router-Modul in Adobe Workfront Fusion
description: Mit dem Router-Modul können Sie Ihren Fluss in mehrere Routen verzweigen und die Daten innerhalb jeder Route unterschiedlich verarbeiten. Sobald ein Router-Modul ein Bundle erhält, leitet es es es an jede angeschlossene Route in der Reihenfolge weiter, in der die Routen an das Router-Modul angehängt wurden.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!UICONTROL Router]-Modul in [!DNL Adobe Workfront Fusion]

Das [!UICONTROL Router]-Modul ermöglicht es Ihnen, Ihren Fluss in mehrere Routen zu verzweigen und die Daten innerhalb jeder Route unterschiedlich zu verarbeiten. Sobald ein [!UICONTROL Router]-Modul ein Bundle erhält, leitet es es es an jede angeschlossene Route in der Reihenfolge weiter, in der die Routen an das [!UICONTROL Router]-Modul angehängt wurden.

>[!NOTE]
>
>* Um die Reihenfolge der Routen zu überprüfen, können Sie auf das Symbol [!UICONTROL Automatische Ausrichtung] klicken, wodurch die Routen entsprechend der Reihenfolge von oben nach unten angeordnet werden.
>
>  Um die Reihenfolge zu ändern, entfernen Sie das Modul [!UICONTROL Router] und verbinden Sie die Routen wieder in der gewünschten Reihenfolge.
>
>* Routen werden sequenziell verarbeitet, nicht parallel. Ein Bundle wird erst dann an die nächste Route gesendet, wenn es von der vorherigen Route vollständig verarbeitet wurde.
>



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

## Hinzufügen eines [!UICONTROL Router]-Moduls zu einem Szenario

Ein [!UICONTROL Router] kann einem Szenario auf eine der folgenden Arten hinzugefügt werden:

* Wenn Sie das Modul [!UICONTROL Router] nach einem Modul verbinden möchten, klicken Sie auf den rechten Griff des Moduls, beginnen Sie mit der Eingabe **[!UICONTROL Router]**, um danach zu suchen, wählen Sie dann **[!UICONTROL Flusssteuerung]** > **[!UICONTROL Router]** in der angezeigten Modulliste.

  ![](assets/connect-the-router-350x108.png)

* Wenn Sie das Modul [!UICONTROL Router] zwischen zwei Modulen einfügen möchten, klicken Sie auf das Schraubenschlüsselsymbol unter der Route, die die beiden Module verbindet (oder klicken Sie mit der rechten Maustaste auf die Route) und wählen Sie **[!UICONTROL Router hinzufügen]** aus dem Menü.

  ![](assets/insert-router-350x191.png)

* Sie können ein [!UICONTROL Router]-Modul automatisch einfügen. Um beispielsweise im folgenden Bild das Modul in der unteren rechten Ecke mit dem Modul in der oberen linken Ecke zu verbinden (das bereits mit dem Modul in der oberen rechten Ecke verbunden ist), ziehen Sie den linken Griff des Moduls in der unteren rechten Ecke und legen Sie es auf dem Modul in der oberen linken Ecke ab.

  ![](assets/insert-router-automatically-350x379.png)

## Filter

Sie können einen Filter auf eine Route nach dem Modul [!UICONTROL Router] einfügen, um Bundles wie bei jeder anderen Route zu filtern:

1. Klicken Sie auf einen der Punkte in der Route.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. Fügen Sie im angezeigten Feld **[!UICONTROL Filter einrichten]** Bedingungen hinzu und klicken Sie dann auf **[!UICONTROL OK]**, um die Filtereinstellungen zu speichern.

   ![](assets/set-up-a-filter-2-350x242.png)

Weitere Informationen finden Sie unter [Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## Die Fallback-Route

Die Filtereinrichtung auf einer Route nach einem [!UICONTROL Router]-Modul enthält eine spezielle Option: Die Ausweichroute:

![](assets/fallback-route-350x260.png)

Wenn diese Option aktiviert ist, wird diese Route verwendet, wenn ein Bundle nicht über eine andere Route vom [!UICONTROL Router]-Modul weitergeleitet werden kann, da die Filter auf den anderen Routen sie herausgefiltert haben.

Die Ausweichroute wird durch ein anderes Pfeilzeichen im Modul [!UICONTROL Router] gekennzeichnet:

![](assets/arrow-sign-in-router-module-350x361.png)

## if/else

Ein typischer Anwendungsfall der Ausweichroute besteht darin, den Fluss mit einer Route fortzusetzen, wenn die Bedingung erfüllt ist, und mit einer anderen Route, wenn dies nicht der Fall ist, wie in den folgenden Schritten beschrieben:

1. Fügen Sie ein [!UICONTROL Router]-Modul in Ihr Szenario ein.
1. Verbinden Sie beide Routen mit dem Modul [!UICONTROL Router] .
1. Klicken Sie auf die erste Route und geben Sie eine Bedingung an:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Klicken Sie auf die zweite Route und aktivieren Sie die Option [!UICONTROL Ausweichroute]:

   ![](assets/enable-fallback-route-option-350x238.png)
