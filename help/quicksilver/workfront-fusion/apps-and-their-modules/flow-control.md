---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Flusskontrolle in Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Flusskontrolle in Adobe Workfront Fusion

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Flusskontrolle](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/flow-control.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Beim Erstellen oder Bearbeiten eines Szenarios können Sie Einstellungen konfigurieren, um den Datenfluss zu steuern.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Repeater

Sie können ein [!UICONTROL Repeater]-Modul verwenden, um eine Aufgabe eine bestimmte Anzahl von Malen zu wiederholen. Ein [!UICONTROL Repeater]-Modul generiert Pakete nacheinander.

Sie können beispielsweise ein [!UICONTROL Repeater]-Modul verwenden, um fünf E-Mails mit den Betreffen „Hello 1“, „Hello 2“ usw. zu senden, indem Sie das Modul **[!UICONTROL E-Mail] > [!UICONTROL E-Mail senden]** mit dem Modul [!UICONTROL Repeater] verbinden.

So verwenden Sie ein [!UICONTROL Repeater]-Modul:

1. Klicken Sie auf [!UICONTROL  Symbol „Flusssteuerung] unten ![](assets/flow-control-icon.gif) auf dem Bildschirm und dann im angezeigten Menü auf **[!UICONTROL Repeater]**.
1. Klicken Sie auf das [!UICONTROL Repeater]-Bundle und dann in ]**angezeigten Feld auf**[!UICONTROL  Automatisch verbinden.
1. Geben [!UICONTROL  im daraufhin angezeigten Feld ]Fluss-Steuerung“ die gewünschte Anzahl von Wiederholungen (ausgegebenen Bundles) in das Feld **[!UICONTROL Wiederholungen]** ein.

   In unserem E-Mail-Beispiel würden Sie 5 eingeben.

   ![](assets/repeater-2-350x207.png)

   Der Wert des Elements erhöht sich bei jeder Wiederholung um diesen Wert, der im Feld **[!UICONTROL Schritt]** angegeben ist, das Sie durch Auswahl von **[!UICONTROL Erweiterte Einstellungen anzeigen]** anzeigen können. Diese Zahl ist standardmäßig 1.

1. Klicken Sie **[!UICONTROL OK]**, um das ]**&quot;**[!UICONTROL &quot; zu schließen.

1. Klicken Sie auf die App oder das Service-Modul, das mit dem [!UICONTROL Repeater]-Modul verbunden ist.
1. Geben Sie in das sich öffnende Feld die Informationen ein, die Sie wiederholen möchten.

   In unserem E-Mail-Beispiel geben Sie Hello in das Feld [!UICONTROL Subject] ein und ordnen dann `i` aus dem Repeater-Modul zu.

   ![](assets/repeater-3-350x207.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Ausgangswert] | Geben Sie die Zahl ein, die das Modul in der ersten Iteration als `i` festlegen soll, oder ordnen Sie sie zu. Der Standardwert ist 1. |
| [!UICONTROL Wiederholungen] | Geben Sie die Anzahl der Wiederholungen des Moduls ein oder mappen Sie sie. Diese Zahl muss größer oder gleich 0 und kleiner oder gleich 10.000 sein. |
| [!UICONTROL Schritt] | Dies ist die Zahl, um die das Modul den Wert von `i` erhöht. Der Standardwert ist 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>Die Anzahl der Wiederholungen wird nicht durch den Wert von `i` bestimmt, wie dies bei der Programmierung in einer Schleife der Fall wäre. Das Modul wiederholt die im Feld „Wiederholungen[!UICONTROL  angegebenen ]. Der Wert `i` ändert sich mit jeder Iteration des [!DNL repeater] Moduls und kann späteren Modulen zugeordnet werden. Im obigen Beispiel wird der Wert von `i` der „Hello“-Nachricht zugeordnet, was zu Meldungen mit dem Wert „Hello 1“, „Hello 2“ usw. führt.

## [!UICONTROL Iterator]

Ein [!UICONTROL Iterator] ist ein spezieller Modultyp, der ein Array in eine Reihe von Bundles konvertiert. Jedes Array-Element ist ein separates Bundle in der Ausgabe des [!UICONTROL Iterator]-Moduls. Weitere Informationen finden Sie unter [[!UICONTROL Iterator]-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Array-Aggregator

Ein Array-Aggregator ist ein spezieller Modultyp, mit dem mehrere Bundles zu einem Bundle zusammengeführt werden können. Weitere Informationen finden Sie unter [[!UICONTROL Aggregator]-Modul in Adobe Workfront ](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Router]

Das [!UICONTROL Router]-Modul ermöglicht es Ihnen, Ihren Fluss in mehrere Routen zu verzweigen und die Daten innerhalb jeder Route unterschiedlich zu verarbeiten. Sobald ein [!UICONTROL Router]-Modul ein Bundle erhält, leitet es es es an jede angeschlossene Route in der Reihenfolge weiter, in der die Routen an das [!UICONTROL Router]-Modul angehängt wurden. Weitere Informationen finden Sie unter [Router-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
