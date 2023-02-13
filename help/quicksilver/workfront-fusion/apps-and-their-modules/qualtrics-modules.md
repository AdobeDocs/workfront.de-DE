---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Qualtrics-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Qualtrics verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Qualtrics-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Qualtrics], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Qualtrics] -Module, müssen Sie über eine [!UICONTROL Qualtrics] -Konto.

## Verbinden [!DNL Qualtrics] nach [!DNL Workfront Fusion]

Sie können eine Verbindung zu Ihrem [!DNL Qualtrics] direkt in einer [!UICONTROL Qualtrics] -Modul.

1. In jeder [!UICONTROL Qualtrics] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] -Feld.
1. Geben Sie die folgenden Informationen ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Verbindungsname]</p> </td> 
      <td> <p>Geben Sie einen Namen für die neue Verbindung ein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Data Center ID] </td> 
      <td>Format verwenden <code>&lt;Data Center ID>.qualtrics.com</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API-Schlüssel]</td> 
      <td>Informationen zum Auffinden Ihres API-Schlüssels finden Sie unter <a href="https://api.qualtrics.com/instructions/docs/Instructions/api-key-authentication.md">API-Token-Authentifizierung</a> im [!DNL Qualtrics] Dokumentation.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Qualtrics] Module und ihre Felder

Die folgenden Module stehen für die [!DNL Qualtrics] connector:

* [!UICONTROL Neue Umfrageantwort ansehen]
* [!UICONTROL Einen Verzeichniskontakt erstellen]
* [!UICONTROL Einen Verzeichniskontakt löschen]
* [!UICONTROL Verzeichniskontakt abrufen]
* [!UICONTROL Aktualisieren eines Verzeichniskontakts]
* [!UICONTROL Erstellen einer neuen Umfrageverteilung per SMS]
* [!UICONTROL Verteilen einer Umfrage per E-Mail]
* [!UICONTROL API-Aufruf]
* [!UICONTROL Verzeichniskontakte auflisten]
