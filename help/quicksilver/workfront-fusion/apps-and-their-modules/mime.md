---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: MIME-Module
description: Sie können MIME-Typen in Adobe Workfront Fusion verwenden. MIME-Typen (Multizweck Internet Mail Extension) sind Bezeichnungen, mit denen Software verschiedene Arten von im Internet freigegebenen Daten identifizieren kann. Webserver und Browser verwenden den MIME-Typ, um zu bestimmen, was mit einer Datei gemacht werden soll. Beispielsweise wird eine Datei mit dem MIME-Typ text/html in einem Browser anders verarbeitet als eine Datei mit dem MIME-Typ image/jpeg. MIME-Typen funktionieren unabhängig von Betriebssystem und Hardware.
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# [!UICONTROL MIME] Module

Sie können MIME-Typen in Adobe Workfront Fusion verwenden. MIME-Typen (Multizweck Internet Mail Extension) sind Bezeichnungen, mit denen Software verschiedene Arten von im Internet freigegebenen Daten identifizieren kann. Webserver und Browser verwenden den MIME-Typ, um zu bestimmen, was mit einer Datei gemacht werden soll. Beispiel: eine Datei mit dem MIME-Typ `text/html` wird in einem Browser anders verarbeitet als in einer Datei mit dem MIME-Typ. `image/jpeg`. MIME-Typen funktionieren unabhängig von Betriebssystem und Hardware.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> <p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL MIME] Module und ihre Felder

### [!UICONTROL Abrufen eines MIME-Typs]

Dieses Transformatormodul gibt den MIME-Typ zurück, der mit einem bestimmten Namen, Pfad oder einer Erweiterung verknüpft ist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei]</td> 
   <td> <p>Geben Sie die Datei ein oder ordnen Sie sie zu, für die Sie den MIME-Typ bestimmen möchten. </p> <p>Sie können die Datei wie folgt eingeben:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Dateipfad]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Dateiname]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL Dateierweiterung]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Dateierweiterung abrufen]

Dieses Transformatormodul gibt die ursprüngliche Dateierweiterung für einen bestimmten MIME-Typ zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME type]</td> 
   <td> <p>Geben Sie den MIME-Typ ein oder ordnen Sie ihn zu, für den Sie die Dateierweiterung bestimmen möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>
