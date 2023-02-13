---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]
description: Wenn Sie einen API-Aufruf in einem Modul konfigurieren, müssen Sie das Feld für die HTTP-Anforderungsmethode ausfüllen.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]

Wenn Sie einen API-Aufruf in einem Modul konfigurieren, müssen Sie das Feld für die HTTP-Anforderungsmethode ausfüllen.

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
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## HTTP-Methoden

Verwenden Sie eine der folgenden HTTP-Methoden.

* **[!UICONTROL GET]**: Ruft Daten von einem Webserver basierend auf Ihren Parametern ab. [!UICONTROL GET] fordert eine Darstellung der angegebenen Ressource an und erhält eine [!UICONTROL 200 OK] Antwortnachricht mit dem angeforderten Inhalt, falls erfolgreich.
* **[!UICONTROL POST]**: Sendet Daten basierend auf Ihren Parametern an einen Webserver. [!UICONTROL POST] -Anfragen umfassen Aktionen wie das Hochladen einer Datei. Mehrere [!UICONTROL POST]kann zu einem anderen Ergebnis führen als zu einem [!UICONTROL POST], also seien Sie vorsichtig, wenn Sie unbeabsichtigt mehrere [!UICONTROL POST]s. Wenn eine [!UICONTROL POST] erfolgreich ist, erhalten Sie eine [!UICONTROL 200 OK] Antwortmeldung.
* **[!UICONTROL PUT]**: Sendet Daten basierend auf Ihren Parametern an einen Speicherort auf dem Webserver. [!UICONTROL PUT] -Anfragen umfassen Aktionen wie das Hochladen einer Datei. Der Unterschied zwischen einem [!UICONTROL PUT] und [!UICONTROL POST] ist, dass PUT idempotent ist, was bedeutet, dass das Ergebnis eines einzelnen erfolgreichen [!UICONTROL PUT] ist identisch mit vielen [!UICONTROL PUT]s. Wenn eine PUT erfolgreich ist, erhalten Sie eine 200-Antwortnachricht (normalerweise 201 oder 204).
* **[!UICONTROL PATCH]**: (Bei einigen API-Aufrufmodulen nicht verfügbar) Wendet je nach Ihren Parametern partielle Änderungen an einer Ressource auf einem Webserver an. [!UICONTROL PATCH] ist nicht idempotent, d. h. das Ergebnis mehrerer [!UICONTROL PATCH]Wir könnten unbeabsichtigte Folgen haben. Wenn eine [!UICONTROL PATCH] erfolgreich ist, erhalten Sie eine 200-Antwort-Nachricht (in der Regel 204).
* **[!UICONTROL DELETE]**: Löscht die angegebene Ressource basierend auf Ihren Parametern aus dem Webserver (sofern die Ressource vorhanden ist). Wenn eine [!UICONTROL DELETE] erfolgreich ist, erhalten Sie eine 200 OK-Antwortmeldung.
