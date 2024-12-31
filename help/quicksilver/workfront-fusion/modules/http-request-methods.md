---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]
description: Wenn Sie einen API-Aufruf in einem Modul konfigurieren, müssen Sie das Feld für die HTTP-Anfragemethode ausfüllen.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]

Wenn Sie einen API-Aufruf in einem Modul konfigurieren, müssen Sie das Feld für die HTTP-Anfragemethode ausfüllen.

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

## HTTP-Methoden

Verwenden Sie eine der folgenden HTTP-Methoden.

* **[!UICONTROL GET]**: Ruft Daten von einem Webserver basierend auf Ihren Parametern ab. [!UICONTROL GET] fordert eine Darstellung der angegebenen Ressource an und erhält bei Erfolg eine [!UICONTROL 200 OK]-Antwortnachricht mit dem angeforderten Inhalt.
* **[!UICONTROL POST]**: Sendet Daten basierend auf Ihren Parametern an einen Webserver. [!UICONTROL POST ] -Anfragen enthalten Aktionen wie das Hochladen einer Datei. Mehrere [!UICONTROL POST ] zu einem anderen Ergebnis führen als eine einzelne [!UICONTROL POST ]. Seien Sie also vorsichtig, wenn Sie versehentlich mehrere [!UICONTROL POST ]. Wenn eine [!UICONTROL POST ] erfolgreich ist, erhalten Sie eine [!UICONTROL 200 OK]-Antwortnachricht.
* **[!UICONTROL PUT]**: Sendet Daten basierend auf Ihren Parametern an einen Speicherort im Webserver. [!UICONTROL PUT]-Anfragen enthalten Aktionen wie das Hochladen einer Datei. Der Unterschied zwischen einer [!UICONTROL PUT] und [!UICONTROL POST ] besteht darin, dass PUT idempotent ist, d. h., dass das Ergebnis einer erfolgreichen [!UICONTROL PUT] mit vielen identischen [!UICONTROL PUT] übereinstimmt. Bei erfolgreicher PUT erhalten Sie eine 200-fache Antwortnachricht (normalerweise 201 oder 204).
* **[!UICONTROL PATCH]**: (Für einige API-Aufrufmodule nicht verfügbar) Wendet basierend auf Ihren Parametern partielle Änderungen an einer Ressource auf einem Webserver an. [!UICONTROL PATCH] ist nicht idempotent, was bedeutet, dass das Ergebnis mehrerer [!UICONTROL PATCH]s unbeabsichtigte Folgen haben kann. Wenn eine [!UICONTROL PATCH] erfolgreich ist, erhalten Sie eine Antwortnachricht von 200 (normalerweise 204).
* **[!UICONTROL DELETE]**: Löscht die angegebene Ressource vom Webserver basierend auf Ihren Parametern (wenn die Ressource vorhanden ist). Wenn ein [!UICONTROL DELETE ] erfolgreich ist, erhalten Sie eine Antwort von 200 OK.
