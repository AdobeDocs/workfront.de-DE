---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ablauf der Szenario-Ausführung in Adobe Workfront Fusion
description: In diesem Artikel wird erläutert, wie ein Szenario ausgeführt wird und wie Daten durch es fließen. Außerdem wird erläutert, wo Sie Informationen zu Ihren verarbeiteten Daten finden und wie Sie diese lesen können.
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Ausführungsfluss des Szenarios in [!DNL Adobe Workfront Fusion]

In diesem Artikel wird erläutert, wie ein Szenario ausgeführt wird und wie Daten durch es fließen. Außerdem wird erläutert, wo Sie Informationen zu Ihren verarbeiteten Daten finden und wie Sie diese lesen können.

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
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

## Ausführungsprozess eines Szenarios

Nachdem ein Szenario korrekt eingerichtet und aktiviert wurde, wird es gemäß seinem definierten Zeitplan ausgeführt.

Bei Beginn des Szenarios antwortet das erste Modul auf ein Ereignis, auf das es überwacht werden soll. Wenn irgendwelche Bundles (Daten) zurückgegeben werden, werden sie an das nächste Modul übergeben und das Szenario wird fortgesetzt, wobei die Bundles jeweils einzeln über jedes aufeinander folgende Modul weitergegeben werden.

Wenn die Bundles in allen Modulen korrekt verarbeitet werden, wird das Szenario im Szenario-Detailbereich als erfolgreich markiert, wie hier beschrieben: [Details zum Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* Weitere Informationen zum Einrichten eines Szenarios finden Sie unter [Grundlegende Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* Weitere Informationen zum Aktivieren eines Szenarios finden Sie unter [Aktivieren oder deaktivieren Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* Weitere Informationen zum Planen eines Szenarios finden Sie unter [Planen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* Weitere Informationen zu Modulen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

### Beispiel: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]

>[!INFO]
>
>**Beispiel:** In einem Szenario, das nach eingehenden Anforderungen in überwacht [!DNL Workfront] und konvertiert sie dann in [!DNL Workfront] -Projekte würden die Daten wie folgt fließen.
>
>Der erste Schritt des Szenarios, der vom ersten Modul durchgeführt wird, besteht darin, nach Anforderungen zu suchen. Jede Anfrage, die eingeht, gilt als ein Bundle. Wenn das Modul ausgeführt wird, ohne Pakete zu finden, endet das Szenario nach dem ersten Modul.
>
>Wenn das erste Modul ein Bundle zurückgibt, durchläuft das Bundle den Rest des Szenarios. In diesem Beispiel besteht der Rest des Szenarios aus dem zweiten und letzten Modul, das die Anforderung in ein Projekt konvertiert.
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### Beispiel: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration]

>[!INFO]
>
>**Beispiel:** In einem Szenario, aus dem Dokumente heruntergeladen werden [!DNL Adobe Workfront] und sendet sie an einen Ordner in [!DNL Dropbox], würden die Daten wie folgt fließen.
>
>Der erste Schritt des Szenarios, der vom ersten Modul durchgeführt wird, besteht darin, nach Bundles (Dokumenten) zu suchen. In diesem Beispiel sucht das Modul nach Bundles in [!DNL Workfront]. Wenn kein Bundle zurückgegeben wird, endet das Szenario nach dem ersten Modul.
>
>Wenn ein Bundle zurückgegeben wird, durchläuft das Bundle den Rest des Szenarios. In diesem Beispiel besteht der Rest des Szenarios aus dem zweiten und letzten Modul, das das Bundle in den [!DNL Dropbox] Ordner.
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>Wenn das erste Modul mehrere Bundles zurückgibt, wird das erste Bundle in hochgeladen [!DNL Dropbox] bevor das zweite Bundle hochgeladen wird. Dann lädt das zweite Bundle hoch, dann das dritte usw.

## Informationen zu verarbeiteten Bundles

Für jedes Modul durchläuft das Bundle einen vierstufigen Prozess, bevor es zum nächsten Modul wechselt oder sein endgültiges Ziel erreicht. Der vierstufige Prozess ist die Initialisierung, der Vorgang, das Bestätigen/Zurücksetzen und die Fertigstellung. Dies wird als Transaktionsverarbeitung bezeichnet und hilft zu erklären, wie Daten in einem Modul verarbeitet wurden.

Sobald ein Szenario ausgeführt wurde, zeigt jedes Modul ein Symbol an, das die Anzahl der durchgeführten Vorgänge anzeigt. Sie können auf dieses Symbol klicken, um detaillierte Informationen zu den verarbeiteten Bundles im oben beschriebenen Format anzuzeigen. Sie können sehen, welche Moduleinstellungen verwendet wurden und welche Bundles von welchem Modul zurückgegeben wurden.

![](assets/info-processed-bundles-350x396.png)

Ein Modul erhielt Eingabedaten wie zum Beispiel:

* Konvertiertes Bild
* Ausgewählter Ordner, in den das Bild hochgeladen werden soll
* Ursprünglicher Name der [!DNL Facebook] image

Nach der Verarbeitung gab das Modul die folgenden Ausgabedaten zurück:

* Von [!DNL Dropbox]
* Vollständiger Pfad, in [!DNL Dropbox] [!DNL Workfront Fusion] Datei hochgeladen

Die oben genannten Informationen werden für jedes Bundle separat erfasst, wie durch die Dropdown-Felder gekennzeichnet [!UICONTROL Vorgang 1] und [!UICONTROL Vorgang 2] im Bild.

Weitere Informationen zur Transaktionsverarbeitung finden Sie unter [Ausführung des Szenarios, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Fehler beim Ausführen eines Szenarios

Während der Ausführung des Szenarios kann ein Fehler auftreten. Wenn Sie beispielsweise die [!DNL Dropbox] -Ordner, den Sie in der Moduleinstellung als Zielordner festgelegt haben, wird das Szenario mit einer Fehlermeldung beendet. Weitere Informationen zum Umgang mit Fehlern finden Sie unter [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
