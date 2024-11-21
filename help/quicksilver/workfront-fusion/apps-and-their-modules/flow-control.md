---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Flusssteuerung in Adobe Workfront Fusion
description: Beim Erstellen oder Bearbeiten eines Szenarios können Sie Einstellungen konfigurieren, um den Datenfluss zu steuern.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Flusssteuerung in Adobe Workfront Fusion

Beim Erstellen oder Bearbeiten eines Szenarios können Sie Einstellungen konfigurieren, um den Datenfluss zu steuern.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Repeater

Sie können ein [!UICONTROL Repeater]-Modul verwenden, um eine Aufgabe eine bestimmte Anzahl von Malen zu wiederholen. Ein [!UICONTROL Repeater]-Modul generiert Bundles, eines nach dem anderen.

Sie können beispielsweise das Modul [!UICONTROL Repeater] verwenden, um fünf E-Mails mit den Betreffen &quot;Hello 1&quot;, &quot;Hello 2&quot;usw. zu senden, indem Sie das Modul **[!UICONTROL E-Mail] >[!UICONTROL E-Mail senden]** an das Modul [!UICONTROL Repeater] anschließen.

So verwenden Sie ein [!UICONTROL Repeater]-Modul:

1. Klicken Sie unten im Bildschirm auf das Symbol [!UICONTROL Flusssteuerung] ![](assets/flow-control-icon.gif) und klicken Sie dann im angezeigten Menü auf **[!UICONTROL Repeater]** .
1. Klicken Sie auf das Bundle [!UICONTROL Repeater] und dann im angezeigten Feld auf **[!UICONTROL Automatisch verbinden]** .
1. Geben Sie im angezeigten Feld [!UICONTROL Flusssteuerung] die Anzahl der Wiederholungen (ausgegebene Bundles) ein, die Sie in das Feld **[!UICONTROL Wiederholungen]** aufnehmen möchten.

   In unserem E-Mail-Beispiel würden Sie 5 eingeben.

   ![](assets/repeater-2-350x207.png)

   Der Wert des Elements erhöht sich bei jeder Wiederholung um den im Feld **[!UICONTROL Schritt]** angegebenen Wert, den Sie durch Auswahl von **[!UICONTROL Erweiterte Einstellungen anzeigen]** anzeigen können. Diese Zahl ist standardmäßig 1.

1. Klicken Sie auf **[!UICONTROL OK]** , um das Feld **[!UICONTROL Flusssteuerung]** zu schließen.

1. Klicken Sie auf die App oder das Dienstmodul, die mit dem Modul [!UICONTROL Repeater] verbunden ist.
1. Geben Sie in das Feld, das angezeigt wird, die Informationen ein, die Sie wiederholen möchten.

   In unserem E-Mail-Beispiel würden Sie &quot;Hello&quot;in das Feld [!UICONTROL Betreff] eingeben und dann `i` aus dem Repeater-Modul zuordnen.

   ![](assets/repeater-3-350x207.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Anfangswert] | Geben Sie die Zahl ein oder ordnen Sie sie zu, die das Modul in der ersten Iteration als `i` festlegen soll. Der Standardwert ist 1. |
| [!UICONTROL Wiederholungen] | Geben Sie ein oder ordnen Sie die Häufigkeit zu, mit der das Modul wiederholt werden soll. Diese Zahl muss größer oder gleich 0 und kleiner oder gleich 10.000 sein. |
| [!UICONTROL Schritt] | Dies ist die Zahl, um die das Modul den Wert von `i` erhöht. Der Standardwert ist 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>Die Anzahl der Wiederholungen wird nicht durch den Wert von `i` bestimmt, da es sich bei der Programmierung um eine Schleife handelt. Das Modul wiederholt die im Feld [!UICONTROL Wiederholungen] angegebene Anzahl von Wiederholungen. Der Wert `i` ändert sich bei jeder Iteration des Moduls [!DNL repeater] und kann späteren Modulen zugeordnet werden. Das obige Beispiel ordnet den Wert von `i` der Meldung &quot;Hello&quot;zu, was zu Meldungen mit dem Wortlaut &quot;Hello 1, Hello 2&quot;usw. führt.

## [!UICONTROL Iterator]

Ein [!UICONTROL Iterator] ist ein spezieller Modultyp, der ein Array in eine Reihe von Bundles konvertiert. Jedes Array-Element ist ein separates Bundle in der Ausgabe des [!UICONTROL Iterator]-Moduls. Weitere Informationen finden Sie unter [[!UICONTROL Iterator] -Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Array-Aggregator

Ein Array-Aggregator ist ein spezieller Modultyp, der es ermöglicht, mehrere Bundles zu einem Bundle zusammenzuführen. Weitere Informationen finden Sie unter [[!UICONTROL Aggregator]-Modul in Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Router]

Mit dem Modul [!UICONTROL Router] können Sie Ihren Fluss in mehrere Routen verzweigen und die Daten in den einzelnen Routen unterschiedlich verarbeiten. Sobald ein Modul vom Typ [!UICONTROL Router] ein Bundle erhält, leitet es es an jede verbundene Route weiter, in der Reihenfolge, in der die Routen mit dem Modul [!UICONTROL Router] verbunden waren. Weitere Informationen finden Sie unter [Router-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
