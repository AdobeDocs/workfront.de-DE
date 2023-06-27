---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Umgang mit Fehlern in [!DNL Adobe Workfront Fusion]
description: Wenn bei der Ausführung eines Szenarios Fehler auftreten, liegt der Grund normalerweise darin, dass ein Dienst aufgrund eines Fehlers nicht verfügbar ist, ein Dienst mit unerwarteten Daten antwortet oder die Validierung von Eingabedaten fehlschlägt.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Umgang mit Fehlern in [!DNL Adobe Workfront Fusion]

Wenn bei der Ausführung eines Szenarios Fehler auftreten, liegt der Grund normalerweise darin, dass ein Dienst aufgrund eines Fehlers nicht verfügbar ist, ein Dienst mit unerwarteten Daten antwortet oder die Validierung von Eingabedaten fehlschlägt.

Wenn ein Modul während der Ausführung des Szenarios einen Fehler auslöst und keine mit dem Modul verbundene Fehlerbearbeitungsroute vorhanden ist, wird die standardmäßige Fehlerbearbeitungslogik ausgeführt, wie hier beschrieben: [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Durch Hinzufügen einer Fehler-Handler-Route zu einem Modul können Sie die standardmäßige Fehlerbearbeitungslogik durch Ihre eigene ersetzen. [!DNL Adobe Workfront Fusion] bietet fünf verschiedene Anweisungen, die am Ende Ihrer Fehler-Handler-Routen eingefügt werden können.

Weitere Informationen finden Sie unter [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Fehler-Handler-Route

So fügen Sie einem Modul eine Fehler-Handler-Route hinzu:

1. Klicken Sie mit der rechten Maustaste auf das Modul und wählen Sie **[!UICONTROL Fehler-Handler hinzufügen]**:

   ![](assets/error-handler-route.png)

   Das -Modul zeigt eine Liste von Richtlinien sowie die in Ihrem Szenario verwendeten Apps an.

1. Wenn das Modul, dem Sie einen Fehler-Handler hinzugefügt haben, das letzte Modul in Ihrer Route ist, wählen Sie eine der Anweisungen aus.

   Oder

   Fügen Sie der Fehler-Handler-Route ein oder mehrere Module hinzu.

   Wenn Sie der Route weitere Module hinzufügen, wird die [!UICONTROL Ignorieren] wird standardmäßig angewendet und im Falle eines Fehlers werden die nachfolgenden Module auf dieser Route verarbeitet.


>[!INFO]
>
>Wenn in diesem Beispiel beim Ausführen der [!UICONTROL Ordner erstellen] -Modul [!UICONTROL Ignorieren] wird automatisch angewendet und das Szenario wechselt zum nächsten Modul auf der Fehler-Handler-Route.
>
>Wenn jedoch kein Fehler vorliegt, wird das Szenario zum [!UICONTROL Alle Dateien in einem Ordnermodul auflisten] auf der regulären Route.
>
>![](assets/if-there-is-no-error-350x234.png)

Beachten Sie, dass eine Fehler-Handler-Route aus transparenten Kreisen besteht, während eine normale Route aus soliden Kreisen besteht.

## Richtlinien zur Fehlerbehebung

Die Richtlinien werden im Folgenden kurz erläutert. Weitere Informationen finden Sie unter [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Es gibt insgesamt fünf Direktiven, die in die folgenden Kategorien eingeteilt werden können, je nachdem, ob die Ausführung eines Szenarios fortgesetzt werden soll oder nicht.

Die folgenden Anweisungen stellen sicher, dass die Ausführung eines Szenarios fortgesetzt wird:

* **[!UICONTROL Fortsetzen]**: Ermöglicht die Angabe einer Ersatzausgabe für das Modul mit dem Fehler. Der Ausführungsstatus des Szenarios wird als erfolgreich markiert
* **[!UICONTROL Ignorieren]**: ignoriert den Fehler. Der Ausführungsstatus des Szenarios wird als erfolgreich markiert
* **[!UICONTROL Break]**: Speichert die Eingabe in die Warteschlange unvollständiger Ausführungen. Der Ausführungsstatus des Szenarios wird als Warnung markiert. Weitere Informationen finden Sie unter [Unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Wenn die Ausführung eines Szenarios bei Auftreten eines Fehlers beendet werden soll, verwenden Sie eine der folgenden Anweisungen:

* **[!UICONTROL Rollback]**: Stoppt die Ausführung des Szenarios sofort und markiert seinen Status als Fehler
* **[!UICONTROL Bestätigen]**: Stoppt die Ausführung des Szenarios sofort und markiert seinen Status als Erfolg

Weitere Informationen zur Fehlerbehebung finden Sie unter:

* [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Erweiterte Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)