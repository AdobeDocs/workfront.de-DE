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
source-git-commit: a2060e7179f2295bfd42da84bd7bca9862ad0a17
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!UICONTROL Iterator] -Modul in [!DNL Adobe Workfront Fusion]

Ein [!UICONTROL Iterator] -Modul ist ein spezieller Modultyp, der ein Array in eine Reihe von Bundles konvertiert. Jedes Array-Element wird als separates Bundle ausgegeben.

Weitere Informationen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md) und [Array in Adobe Workfront Fusion zuordnen](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>Ihr Unternehmen muss Adobe Workfront Fusion sowie Adobe Workfront erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iterator] Modulkonfiguration

Sie richten eine [!UICONTROL Iterator] -Modul identisch, wie Sie ein anderes Modul einrichten. Die [!UICONTROL Array] -Feld enthält das Array, das konvertiert oder in separate Bundles aufgeteilt werden soll.

![](assets/set-up-iterator-350x190.jpg)

Weitere Informationen finden Sie unter [Moduleinstellungen in Adobe Workfront Fusion konfigurieren](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Beispiele:**
>
>* Das folgende Szenario zeigt, wie E-Mails mit Anhängen abgerufen und als einzelne Dateien in einer ausgewählten Datei gespeichert werden [!DNL Dropbox] Ordner.
   >
   >   E-Mails können eine Reihe von Anhängen enthalten. Die [!UICONTROL Iterator] -Modul, das nach dem ersten Modul eingefügt wird, ermöglicht es Ihnen, jede Anlage separat zu handhaben. Die [!UICONTROL Iterator] -Modul teilt das Array der Anlagen in einzelne Bundles auf. Jedes Bundle mit einer Anlage wird dann nacheinander in einem ausgewählten [!DNL Dropbox] Ordner. Die [!UICONTROL Iterator] Die Moduleinrichtung ist oben dargestellt: die [!UICONTROL Array] -Feld sollte enthalten `Attachments` Array.
   >
   >   ![](assets/attachments-array-350x154.jpg)
>
>* Für Ihre Bequemlichkeit bieten viele [!DNL Workfront Fusion] Apps-Angebot spezialisiert [!UICONTROL Iterator] -Module mit einer vereinfachten Einrichtung. Beispiel: die [!UICONTROL Email] Die App enthält das spezielle [!UICONTROL Iterator] Modul [!UICONTROL Email] > [!UICONTROL Anhänge itterieren] die dieselben Ergebnisse wie im Allgemeinen [!UICONTROL Iterator] -Modul.
   >
   >   ![](assets/specialized-iterators-350x135.jpg)



## Fehlerbehebung: Zuordnungsbereich zeigt keine zuordnbaren Elemente unter [!UICONTROL Iterator] Modul

Wenn ein [!UICONTROL Iterator] -Modul keine Informationen über die Struktur der Elemente des Arrays hat, das Zuordnungsbedienfeld in den Modulen, die auf die [!UICONTROL Iterator] -Modul nur 2 Elemente unter [!UICONTROL Iterator] module :`Total number of bundles` und `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Dies liegt daran, dass jedes Modul für die Bereitstellung von Informationen über die von ihm ausgelieferten Elemente verantwortlich ist, sodass diese Elemente in den nachfolgenden Modulen ordnungsgemäß im Zuordnungsbereich angezeigt werden können. In einigen Fällen sind jedoch möglicherweise mehrere Module nicht in der Lage, diese Informationen bereitzustellen. Beispiel: [!UICONTROL JSON] > [!UICONTROL Parse JSON] oder [!UICONTROL Webhooks] > [!UICONTROL Benutzerspezifischer Webhook] -Module mit fehlender Datenstruktur.

Die Lösung besteht darin, das Szenario manuell auszuführen, damit das Modul über die von ihm ausgegebenen Elemente informiert wird, damit es die Informationen an die folgenden Module weitergeben kann.

Wenn Sie beispielsweise eine [!UICONTROL JSON] > [!UICONTROL Parse JSON] -Modul ohne Datenstruktur wie folgt:

![](assets/json-parse-json-350x285.png)

Und wenn Sie dann eine [!UICONTROL Iterator] -Modul hinzugefügt haben, können Sie die Ausgabe des Moduls nicht dem Feld Array im Setup-Bereich des [!UICONTROL Iterator] module :

![](assets/connect-iterator-module-350x146.png)

Um dies zu beheben, starten Sie das Szenario manuell im Szenario-Editor. Sie können die Verknüpfung der Module nach der [!UICONTROL JSON] > [!UICONTROL Parse JSON] -Modul, um zu verhindern, dass der Fluss weiter fortgesetzt wird. Oder Sie können mit der rechten Maustaste auf die [!UICONTROL JSON] > [!UICONTROL Parse JSON] -Modul und wählen Sie **[!UICONTROL Nur dieses Modul ausführen]** aus dem Kontextmenü, um nur die [!UICONTROL JSON] > [!UICONTROL Parse JSON] -Modul.

Wenn die [!UICONTROL JSON] > [!UICONTROL Parse JSON] führt aus, lernt er über die Elemente, die er ausgibt, und stellt diese Informationen für alle nachfolgenden Module bereit, einschließlich des Iterator-Moduls. Im Zuordnungsbereich in der Einrichtung des Iterators werden dann die Elemente angezeigt:

![](assets/mapping-panel-displays-items-350x131.png)

Darüber hinaus wird das Zuordnungsbedienfeld in den Modulen angezeigt, die nach dem [!UICONTROL Iterator] -Modul zeigen die Elemente an, die in den Elementen des Arrays enthalten sind:

![](assets/items-contained-in-array-350x156.png)

Wenn Sie einige Elemente im Zuordnungsbereich eines Moduls nicht sehen können, führen Sie das Szenario einmal aus, damit alle Module über die von ihnen ausgegebenen Elemente erfahren und diese Informationen den folgenden Modulen bereitstellen können.
