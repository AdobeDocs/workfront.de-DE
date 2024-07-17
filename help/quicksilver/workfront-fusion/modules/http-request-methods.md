---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: HTTP-Anforderungsmethoden in  [!DNL Adobe Workfront Fusion]
description: Wenn Sie einen API-Aufruf in einem Modul konfigurieren, müssen Sie das Feld für die HTTP-Anforderungsmethode ausfüllen.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]

Wenn Sie einen API-Aufruf in einem Modul konfigurieren, müssen Sie das Feld für die HTTP-Anforderungsmethode ausfüllen.

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

## HTTP-Methoden

Verwenden Sie eine der folgenden HTTP-Methoden.

* **[!UICONTROL GET]**: Ruft Daten von einem Webserver basierend auf Ihren Parametern ab. [!UICONTROL GET] fordert eine Darstellung der angegebenen Ressource an und erhält eine Antwort-Meldung mit dem Wert [!UICONTROL 200 OK] mit dem angeforderten Inhalt, falls er erfolgreich ist.
* **[!UICONTROL POST]**: Sendet Daten basierend auf Ihren Parametern an einen Webserver. [!UICONTROL POST] -Anfragen umfassen Aktionen wie das Hochladen einer Datei. Mehrere [!UICONTROL POST]s können zu einem anderen Ergebnis führen als eine einzelne [!UICONTROL POST]. Seien Sie also vorsichtig, wenn Sie versehentlich mehrere [!UICONTROL POST]senden. Wenn eine [!UICONTROL POST] erfolgreich ist, erhalten Sie eine [!UICONTROL 200 OK] Antwortmeldung.
* **[!UICONTROL PUT]**: Sendet Daten basierend auf Ihren Parametern an einen Speicherort auf dem Webserver. [!UICONTROL PUT] -Anfragen umfassen Aktionen wie das Hochladen einer Datei. Der Unterschied zwischen einer [!UICONTROL PUT] und [!UICONTROL POST] besteht darin, dass PUT idempotent ist, d. h. das Ergebnis einer einzigen erfolgreichen [!UICONTROL PUT] entspricht vielen identischen [!UICONTROL PUT]s. Wenn eine PUT erfolgreich ist, erhalten Sie eine 200-Antwortnachricht (in der Regel 201 oder 204).
* **[!UICONTROL PATCH]**: (Bei einigen API-Aufrufmodulen nicht verfügbar) Wendet partielle Änderungen an einer Ressource auf einem Webserver an, die auf Ihren Parametern basiert. [!UICONTROL PATCH] ist nicht idempotent, d. h. das Ergebnis mehrerer [!UICONTROL PATCH]&#39;s kann unbeabsichtigte Folgen haben. Wenn eine [!UICONTROL PATCH] erfolgreich ist, erhalten Sie eine 200-Antwortmeldung (in der Regel 204).
* **[!UICONTROL DELETE]**: Löscht die angegebene Ressource aus dem Webserver entsprechend Ihren Parametern (sofern die Ressource vorhanden ist). Wenn ein [!UICONTROL DELETE] erfolgreich ist, erhalten Sie eine 200 OK-Antwortmeldung.
