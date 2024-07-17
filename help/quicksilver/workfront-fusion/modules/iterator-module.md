---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Iteratormodul in Adobe Workfront Fusion
description: Ein Iterator-Modul ist ein spezielles Modul, das ein Array in eine Reihe von Bundles konvertiert. Jedes Array-Element wird als separates Bundle ausgegeben.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# [!UICONTROL Iterator]-Modul in [!DNL Adobe Workfront Fusion]

Ein [!UICONTROL Iterator] -Modul ist ein spezieller Modultyp, der ein Array in eine Reihe von Bundles konvertiert. Jedes Array-Element wird als separates Bundle ausgegeben.

Weitere Informationen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md) und [Zuordnen eines Arrays in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>Ihr Unternehmen muss Adobe Workfront Fusion sowie Adobe Workfront erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iterator] Modulkonfiguration

Sie richten ein [!UICONTROL Iterator]-Modul ein, das auch für andere Module gilt. Das Feld [!UICONTROL Array] enthält das Array, das in separate Bundles konvertiert oder aufgeteilt werden soll.

![](assets/set-up-iterator-350x190.jpg)

Weitere Informationen finden Sie unter [Einstellungen eines Moduls in Adobe Workfront Fusion konfigurieren](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Beispiele:**
>
>* Im folgenden Szenario erfahren Sie, wie Sie E-Mails mit Anhängen abrufen und die Anhänge als einzelne Dateien in einem ausgewählten [!DNL Dropbox] -Ordner speichern.
>
>   E-Mails können eine Reihe von Anhängen enthalten. Das Modul [!UICONTROL Iterator] , das nach dem ersten Modul eingefügt wurde, ermöglicht es Ihnen, jede Anlage separat zu handhaben. Das Modul [!UICONTROL Iterator] teilt das Array der Anlagen in einzelne Pakete auf. Jedes Bundle mit einer Anlage wird dann einzeln in einem ausgewählten [!DNL Dropbox] -Ordner gespeichert. Das Modul [!UICONTROL Iterator] wird oben gezeigt: Das Feld [!UICONTROL Array] sollte das Array `Attachments` enthalten.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Zur Vereinfachung bieten viele [!DNL Workfront Fusion] -Apps spezielle [!UICONTROL Iterator] -Module mit vereinfachtem Setup. Beispielsweise enthält die App [!UICONTROL E-Mail] das spezielle Modul [!UICONTROL Iterator] [!UICONTROL E-Mail] > [!UICONTROL Iterate attachments] , das dieselben Ergebnisse wie das allgemeine Modul [!UICONTROL Iterator] liefert.
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Fehlerbehebung: Zuordnungsbedienfeld zeigt keine zuordnbaren Elemente unter dem Modul [!UICONTROL Iterator] an

Wenn ein [!UICONTROL Iterator] -Modul keine Informationen über die Struktur der Elemente des Arrays enthält, zeigt das Zuordnungsbedienfeld in den Modulen, die auf das Modul [!UICONTROL Iterator] folgen, nur 2 Elemente unter dem Modul [!UICONTROL Iterator] an:`Total number of bundles` und `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Dies liegt daran, dass jedes Modul für die Bereitstellung von Informationen zu den von ihm ausgelieferten Elementen verantwortlich ist, damit diese Elemente in den nachfolgenden Modulen ordnungsgemäß im Zuordnungsbereich angezeigt werden können. Einige Module können diese Informationen jedoch in einigen Fällen nicht bereitstellen, z. B. [!UICONTROL JSON] > [!UICONTROL JSON analysieren] oder [!UICONTROL Webhooks] > [!UICONTROL Benutzerspezifischer Webhook] -Module mit fehlender Datenstruktur.

Die Lösung besteht darin, das Szenario manuell auszuführen, damit das Modul über die von ihm ausgegebenen Elemente informiert wird, damit es die Informationen an die folgenden Module weitergeben kann.

Beispiel: Sie verfügen über das Modul [!UICONTROL JSON] > [!UICONTROL JSON analysieren] ohne Datenstruktur wie folgt:

![](assets/json-parse-json-350x285.png)

Wenn Sie dann ein [!UICONTROL Iterator] -Modul damit verbinden, können Sie die Ausgabe des Moduls nicht dem Array-Feld im Setup-Bereich des [!UICONTROL Iterator] -Moduls zuordnen:

![](assets/connect-iterator-module-350x146.png)

Um dies zu beheben, starten Sie das Szenario manuell im Szenario-Editor. Sie können die Verknüpfung der Module nach dem Modul [!UICONTROL JSON] > [!UICONTROL JSON analysieren] aufheben, um zu verhindern, dass der Fluss weiter fortgesetzt wird. Alternativ können Sie mit der rechten Maustaste auf das Modul [!UICONTROL JSON] > [!UICONTROL JSON analysieren] klicken und im Kontextmenü die Option **[!UICONTROL Nur dieses Modul ausführen]** auswählen, um nur das Modul [!UICONTROL JSON] > [!UICONTROL JSON analysieren] auszuführen.

Wenn der Befehl [!UICONTROL JSON] > [!UICONTROL JSON analysieren] ausgeführt wird, lernt er von den Elementen, die er ausgibt, und stellt diese Informationen allen nachfolgenden Modulen einschließlich des Iterator-Moduls bereit. Im Zuordnungsbereich in der Einrichtung des Iterators werden dann die Elemente angezeigt:

![](assets/mapping-panel-displays-items-350x131.png)

Darüber hinaus zeigt das Zuordnungsbedienfeld in den Modulen, die nach dem Modul [!UICONTROL Iterator] verbunden sind, die Elemente an, die in den Elementen des Arrays enthalten sind:

![](assets/items-contained-in-array-350x156.png)

Wenn Sie einige Elemente im Zuordnungsbereich eines Moduls nicht sehen können, führen Sie das Szenario einmal aus, damit alle Module über die von ihnen ausgegebenen Elemente erfahren und diese Informationen den folgenden Modulen bereitstellen können.
