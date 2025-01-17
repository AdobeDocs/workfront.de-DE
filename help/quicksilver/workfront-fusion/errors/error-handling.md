---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fehlerbehandlung in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Fehlerbehandlung in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Fehlerbehandlung hinzufügen](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/error-handling.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Wenn bei der Ausführung eines Szenarios Fehler auftreten, liegt dies in der Regel daran, dass ein Service aufgrund eines Fehlers nicht verfügbar ist, ein Service mit unerwarteten Daten antwortet oder die Validierung der Eingabedaten fehlschlägt.

Wenn ein Modul während der Ausführung des Szenarios einen Fehler ausgibt und dem Modul keine Route zur Fehlerbehandlung angehängt ist, wird die standardmäßige Logik zur Fehlerbehandlung ausgeführt, wie unter [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) beschrieben.

Durch Hinzufügen einer Fehler-Handler-Route zu einem Modul können Sie die standardmäßige Fehlerbehandlungslogik durch Ihre eigene ersetzen. [!DNL Adobe Workfront Fusion] bietet fünf verschiedene Anweisungen, die am Ende Ihrer Fehler-Handler-Routen eingefügt werden können.

Weitere Informationen finden Sie unter [Anweisungen für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Route des Fehler-Handlers

So fügen Sie einem Modul eine Fehler-Handler-Route hinzu:

1. Klicken Sie mit der rechten Maustaste auf das Modul und wählen **[!UICONTROL Fehler-Handler hinzufügen]**:

   ![](assets/error-handler-route.png)

   Das Modul zeigt eine Liste der Anweisungen sowie der in Ihrem Szenario verwendeten Apps an.

1. Wenn das Modul, dem Sie einen Fehler-Handler hinzugefügt haben, das letzte Modul in Ihrer Route ist, wählen Sie eine der Anweisungen aus.

   Oder

   Fügen Sie ein oder mehrere Module zur Fehler-Handler-Route hinzu.

   Wenn Sie der Route weitere Module hinzufügen, wird [!UICONTROL Ignore]-Direktive angewendet, und im Falle eines Fehlers werden die nachfolgenden Module auf dieser Route verarbeitet.


>[!INFO]
>
>Wenn in diesem Beispiel während der Ausführung des Moduls [!UICONTROL Ordner erstellen] ein Fehler auftritt, wird die [!UICONTROL Ignorieren]-Direktive automatisch angewendet und das Szenario wechselt zum nächsten Modul auf der Route des Fehler-Handlers.
>
>Wenn jedoch kein Fehler auftritt, wird das Szenario auf der regulären Route in die [!UICONTROL Alle Dateien in einem ] auflisten) verschoben.
>
>![](assets/if-there-is-no-error-350x234.png)

Eine Route für Fehler-Handler besteht aus transparenten Kreisen, während eine reguläre Route aus durchgezogenen Kreisen besteht.

## Anweisungen zur Fehlerbehandlung

Die Richtlinien werden im Folgenden kurz erläutert. Weitere Informationen finden Sie unter [Anweisungen für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Es gibt insgesamt fünf Direktiven, die sich in die folgenden Kategorien unterteilen lassen, je nachdem, ob die Ausführung eines Szenarios fortgesetzt werden soll oder nicht.

Die folgenden Anweisungen stellen sicher, dass ein Szenario weiterhin ausgeführt wird:

* **[!UICONTROL Fortsetzen]**: Ermöglicht die Angabe einer Ersatzausgabe für das Modul mit dem Fehler. Der Ausführungsstatus des Szenarios wird als erfolgreich markiert
* **[!UICONTROL Ignorieren]**: Ignoriert den Fehler. Der Ausführungsstatus des Szenarios wird als erfolgreich markiert
* **[!UICONTROL break]**: Speichert die Eingabe bei unvollständigen Ausführungen in die Warteschlange. Der Ausführungsstatus des Szenarios wird als Warnung gekennzeichnet. Weitere Informationen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Wenn die Ausführung eines Szenarios bei einem Fehler beendet werden soll, verwenden Sie eine der folgenden Anweisungen:

* **[!UICONTROL Rollback]**: Hält die Ausführung des Szenarios sofort an und markiert seinen Status als Fehler
* **[!UICONTROL Bestätigen]**: Hält die Ausführung des Szenarios sofort an und markiert seinen Status als Erfolg

Weitere Informationen zur Fehlerbehandlung finden Sie unter:

* [Anweisungen für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Erweiterte Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)