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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 1%

---

# Flusssteuerung in Adobe Workfront Fusion

Beim Erstellen oder Bearbeiten eines Szenarios können Sie Einstellungen konfigurieren, um den Datenfluss zu steuern.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Repeater

Sie können eine [!UICONTROL Repeater] -Modul, um eine Aufgabe eine bestimmte Anzahl von Malen zu wiederholen. A [!UICONTROL Repeater] -Modul generiert Pakete nacheinander.

Sie können beispielsweise eine [!UICONTROL Repeater] Modul zum Senden von fünf E-Mails mit den Betreffen &quot;Hello 1&quot;, &quot;Hello 2&quot;usw. durch Verbinden des **[!UICONTROL Email] >[!UICONTROL Senden Sie mir eine E-Mail]** -Modul [!UICONTROL Repeater] -Modul.

So verwenden Sie eine [!UICONTROL Repeater] -Modul:

1. Klicken Sie auf [!UICONTROL Flusssteuerung] icon ![](assets/flow-control-icon.gif) Klicken Sie unten im Bildschirm auf **[!UICONTROL Repeater]** im angezeigten Menü.
1. Klicken Sie auf [!UICONTROL Repeater] Bundle, und klicken Sie dann auf **[!UICONTROL Automatisch verbinden]** in dem Feld, das angezeigt wird.
1. Im [!UICONTROL Flusssteuerung] in das Feld eingeben, wie viele Wiederholungen (ausgegebene Bundles) Sie in das Feld **[!UICONTROL Wiederholungen]** ankreuzen.

   In unserem E-Mail-Beispiel würden Sie 5 eingeben.

   ![](assets/repeater-2-350x207.png)

   Der Wert des Elements erhöht sich bei jeder Wiederholung um den im Feld **[!UICONTROL Schritt]** -Feld, das Sie anzeigen können, indem Sie **[!UICONTROL Erweiterte Einstellungen anzeigen]**. Diese Zahl ist standardmäßig 1.

1. Klicken **[!UICONTROL OK]** zum Schließen der **[!UICONTROL Flusssteuerung]** ankreuzen.

1. Klicken Sie auf die App oder das Dienstmodul, die mit dem [!UICONTROL Repeater] -Modul.
1. Geben Sie in das Feld, das angezeigt wird, die Informationen ein, die Sie wiederholen möchten.

   In unserem E-Mail-Beispiel würden Sie &quot;Hello&quot;in die [!UICONTROL Betreff] Feld, dann Zuordnung `i` aus dem Repeater-Modul.

   ![](assets/repeater-3-350x207.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Anfangswert] | Geben Sie die Zahl ein oder ordnen Sie sie zu, die das Modul als `i` in der ersten Iteration. Der Standardwert ist 1. |
| [!UICONTROL Wiederholungen] | Geben Sie ein oder ordnen Sie die Anzahl der Wiederholungen des Moduls zu. Diese Zahl muss größer oder gleich 0 und kleiner oder gleich 10.000 sein. |
| [!UICONTROL Schritt] | Dies ist die Zahl, um die das Modul den Wert von `i`. Der Standardwert ist 1. |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>Die Anzahl der Wiederholungen wird nicht durch den Wert von `i`, da es sich in einer Schleife der Programmierung befindet. Das Modul wiederholt die in der Variablen [!UICONTROL Wiederholungen] -Feld. Der Wert `i` Änderungen bei jeder Iteration der [!DNL repeater] -Modul und können späteren Modulen zugeordnet werden. Das obige Beispiel ordnet den Wert von `i` in die Meldung &quot;Hallo&quot;ein, was zu Meldungen mit &quot;Hallo 1&quot;, &quot;Hallo 2&quot;usw. führt.

## [!UICONTROL Iterator]

Ein [!UICONTROL Iterator] ist ein spezieller Modultyp, der ein Array in eine Reihe von Bundles konvertiert. Jedes Array-Element ist ein separates Bundle im [!UICONTROL Iterator] -Modulausgabe. Weitere Informationen finden Sie unter [[!UICONTROL Iterator] -Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Array-Aggregator

Ein Array-Aggregator ist ein spezieller Modultyp, der es ermöglicht, mehrere Bundles zu einem Bundle zusammenzuführen. Weitere Informationen finden Sie unter [[!UICONTROL Aggregator] Modul in Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Router]

Die [!UICONTROL Router] ermöglicht es Ihnen, Ihren Fluss in mehrere Routen zu verzweigen und die Daten innerhalb der einzelnen Routen unterschiedlich zu verarbeiten. Einmal [!UICONTROL Router] -Modul ein Bundle erhält, es an jede verbundene Route weiterleitet, in der die Routen an die [!UICONTROL Router] -Modul. Weitere Informationen finden Sie unter [Router-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
