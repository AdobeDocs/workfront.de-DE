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
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Umgang mit Fehlern in [!DNL Adobe Workfront Fusion]

Wenn bei der Ausführung eines Szenarios Fehler auftreten, liegt der Grund normalerweise darin, dass ein Dienst aufgrund eines Fehlers nicht verfügbar ist, ein Dienst mit unerwarteten Daten antwortet oder die Validierung von Eingabedaten fehlschlägt.

>[!NOTE]
>
>Wenn ein Modul während der Ausführung des Szenarios einen Fehler auslöst und keine mit dem Modul verbundene Fehlerbearbeitungsroute vorhanden ist, wird eine standardmäßige Fehlerbearbeitungslogik ausgeführt, wie in [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Durch Hinzufügen einer Fehler-Handler-Route zu einem Modul können Sie die standardmäßige Fehlerbearbeitungslogik durch Ihre eigene ersetzen. [!DNL Adobe Workfront Fusion] bietet fünf verschiedene Direktiven, von denen jede am Ende Ihrer Fehler-Handler-Routen eingefügt werden kann. Weitere Informationen finden Sie unter [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Fehler-Handler-Route

Um eine Fehler-Handler-Route zu einem Modul hinzuzufügen (wir nennen es Modul X), klicken Sie mit der rechten Maustaste auf das Modul und wählen Sie **[!UICONTROL Fehler-Handler hinzufügen]**:

![](assets/error-handler-route.png)

Das -Modul zeigt eine Liste von Richtlinien sowie die in Ihrem Szenario verwendeten Apps an. Wenn Modul X das letzte Modul in Ihrer Route ist, müssen Sie eine der Anweisungen auswählen. Oder Sie können Ihrer Route ein oder mehrere Module hinzufügen. In diesem Fall wird die [!UICONTROL Ignorieren] wird standardmäßig auf Modul X angewendet und im Falle eines Fehlers werden die nachfolgenden Module auf dieser Route verarbeitet.

![](assets/directives-350x426.png)

Wie Sie unten sehen können, wenn beim Ausführen der [!UICONTROL Ordner erstellen] -Modul [!UICONTROL Ignorieren] wird automatisch angewendet und das Szenario wechselt zum nächsten Modul auf der Fehler-Handler-Route, wenn der Filter &quot;Datenfehler erfolgt&quot;ein oder mehrere Bundles zurückgibt.

Wenn jedoch kein Fehler vorliegt, wird das Szenario zum [!UICONTROL Alle Dateien in einem Ordnermodul auflisten] auf der regulären Route.

![](assets/if-there-is-no-error-350x234.png)

Um eine Fehler-Handler-Route von einer normalen Route zu unterscheiden, besteht die erste aus transparenten Kreisen, wie oben gezeigt.

## Richtlinien zur Fehlerbehebung

Die Richtlinien werden im Folgenden kurz erläutert. Weitere Informationen finden Sie unter [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Es gibt insgesamt fünf Direktiven, die in die folgenden Kategorien eingeteilt werden können, je nachdem, ob die Ausführung eines Szenarios fortgesetzt werden soll oder nicht:

Die folgenden Anweisungen stellen sicher, dass die Ausführung eines Szenarios fortgesetzt wird:

* **[!UICONTROL Fortsetzen]** ermöglicht es Ihnen, eine Ersatzausgabe für das Modul mit dem Fehler anzugeben und der Ausführungsstatus des Szenarios wird als erfolgreich markiert
* **[!UICONTROL Ignorieren]** ignoriert einfach den Fehler und der Ausführungsstatus des Szenarios wird als erfolgreich markiert
* **[!UICONTROL Break]** speichert die Eingabe in die Warteschlange unvollständiger Ausführungen und der Ausführungsstatus des Szenarios wird als Warnung markiert. Weitere Informationen finden Sie unter [Unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Wenn dagegen die Ausführung eines Szenarios angehalten werden soll, müssen Sie eine der folgenden Anweisungen verwenden:

* **[!UICONTROL Rollback]** stoppt die Ausführung des Szenarios sofort und markiert seinen Status als Fehler
* **[!UICONTROL Bestätigen]** stoppt die Ausführung des Szenarios sofort und markiert seinen Status als erfolgreich

## Zusätzliche Ressourcen

* [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Erweiterte Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) (umfasst die Einrichtung des oben genannten Szenarios für die Dropbox)
