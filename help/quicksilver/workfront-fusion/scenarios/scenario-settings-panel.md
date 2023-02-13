---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Das Bedienfeld "Szenario-Einstellungen"in Adobe Workfront Fusion
description: In diesem Artikel werden die Einstellungen beschrieben, die im [!UICONTROL Szenario-Einstellungen] -Bedienfeld in [!DNL Adobe Workfront Fusion] Szenarien.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 0%

---

# Das Bedienfeld für die Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Öffnen Sie die Szenario-Einstellungen.

1. Öffnen Sie den Szeneneditor, wie hier beschrieben: [Der Szenario-Editor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Klicken Sie auf das Zahnradsymbol unten links auf der Seite.

   ![](assets/scenario-settings-350x221.png)

   Im [!UICONTROL Szenario-Einstellungen] angezeigt werden, können Sie verschiedene erweiterte Einstellungen für das Szenario konfigurieren.

## [!UICONTROL Speichern unvollständiger Ausführungen zulassen]

Diese Option bestimmt, wie [!DNL Adobe Workfront Fusion] wird fortgesetzt, wenn während der Ausführung eines Szenarios ein Fehler auftritt. Wenn diese Option aktiviert ist, wird das Szenario angehalten und nach [Unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Dadurch haben Sie die Möglichkeit, das Problem zu beheben und die Ausführung dort fortzusetzen, wo das Szenario angehalten wurde. Wenn diese Option deaktiviert ist, wird das Szenario angehalten und eine Rollback-Phase gestartet.

## [!UICONTROL Sequenzielle Verarbeitung]

Diese Option bestimmt, wie [!DNL Workfront Fusion] wird fortgesetzt, wenn ein Fehler auftritt und die Ausführung eines Szenarios an die [Unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Wenn die Variable [!UICONTROL Sequenzielle Verarbeitung] aktiviert ist, stoppt Workfront Fusion die Verarbeitung der Aufgabensequenz, bis alle unvollständigen Ausführungen abgeschlossen sind. Wenn die Variable [!UICONTROL Sequenzielle Verarbeitung] deaktiviert ist, wird das Szenario weiterhin gemäß seinem Zeitplan ausgeführt und es werden wiederholt Versuche unternommen, die unvollständigen Ausführungen erneut auszuführen.

Weitere Informationen zur Planung finden Sie unter [Planen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Daten sind vertraulich

Sobald ein Szenario ausgeführt wurde, können Sie standardmäßig Informationen darüber anzeigen, welche Daten von Modulen im Szenario verarbeitet wurden. Wenn diese Informationen nicht gespeichert werden sollen, aktivieren Sie die [!UICONTROL Daten sind vertraulich] -Option.

Weitere Informationen zur Anzeige von Informationen finden Sie unter [Ausführungsfluss des Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Wenn Sie diese Option aktivieren, kann es schwierig sein, Fehler zu beheben, die während der Ausführung eines Szenarios auftreten können.

## Datenverlust aktivieren

Diese Option hat mit der Aktivierung des Datenverlusts zu tun, wenn [!DNL Workfront Fusion] das Speichern eines Bundles in der Warteschlange von [Unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (z. B. wegen fehlenden freien Speicherplatzes). Wenn diese Option aktiviert ist, gehen die Daten verloren, um Unterbrechungen bei der Ausführung des Szenarios insgesamt zu vermeiden. Dies ist für Szenarien nützlich, in denen die kontinuierliche Ausführung mit der höchsten Priorität erfolgt und die eingehenden fehlerhaften Daten nicht so wichtig sind.

Darüber hinaus kann ein Modul bei der Ausführung eines Szenarios auf eine Datei stoßen, die größer als die maximal zulässige Größe ist. In diesem Fall [!DNL Workfront Fusion] Erlöse gemäß der Festlegung der [!UICONTROL Datenverlust aktivieren] und eine Warnmeldung angezeigt.

Weitere Informationen zur maximalen Dateigröße finden Sie unter [Über die Zuordnung von Dateien in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Weitere Informationen zu Warnungen finden Sie unter [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Automatische Übertragung]

Die [!UICONTROL Automatische Übertragung] -Einstellungen gelten für Transaktionen und definieren die Methode zur Verarbeitung eines Szenarios. Wenn die Option Automatisches Übertragen aktiviert ist, beginnt die Commit-Phase in jedem Modul unmittelbar nach Abschluss der Betriebsphase. Wenn die Option Automatisches Übertragen deaktiviert ist, erfolgt keine Übertragung, bis Vorgänge für alle Module ausgeführt werden (dies ist der Standardmodus).

Weitere Informationen zu Transaktionen finden Sie unter [Ausführung des Szenarios, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Höchstzahl der Zyklen

Das Festlegen weiterer Zyklen kann nützlich sein, wenn Sie eine Unterbrechung der Verbindung zu einem Drittanbieterdienst verhindern und sicherstellen möchten, dass alle Datensätze innerhalb eines Szenarios verarbeitet werden.

* Beginnt das Szenario mit einem Abrufintereignis, wird in der Einstellung die maximale Anzahl von Triggern definiert, die während der Ausführung des Szenarios zulässig sind.

   Weitere Informationen zu Triggern in der Abfrage finden Sie unter [Abruf von Triggern](../../workfront-fusion/modules/module-types.md#polling) in [Modultypen](../../workfront-fusion/modules/module-types.md).

* Wenn das Szenario mit einem sofortigen Trigger beginnt, wird die Einstellung ignoriert und alle ausstehenden Ereignisse werden während der Ausführung eines einzigen Szenarios verarbeitet, d. h. ein Ereignis pro Zyklus.

   Weitere Informationen zu sofortigen Triggern finden Sie unter [Sofortige Trigger](../../workfront-fusion/modules/module-types.md#instant) in [Modultypen](../../workfront-fusion/modules/module-types.md).

* Wenn das Szenario nicht mit einem Trigger beginnt (Instant/Polling), wird immer die angegebene maximale Anzahl von Zyklen ausgeführt.

>[!INFO]
>
>**Beispiele:**  [!DNL Workfront] > [!UICONTROL Aufzeichnung ansehen] überwacht neue Probleme, die auftreten, und [!DNL Workfront] >[!UICONTROL Konvertierungsobjekt] konvertiert die neue Anforderung in ein Projekt und weist ihr die entsprechende Vorlage zu.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL mehr Zyklen] wird nur angewendet, wenn Sie die Ausführung des Szenarios planen. Wenn Sie [!UICONTROL Einmal ausführen] -Schaltfläche, werden die Zykluseinstellungen berücksichtigt.
>
>### Die maximale Anzahl von Zyklen ist auf 1 gesetzt (Standard)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>Die [!UICONTROL Maximale Anzahl an zurückgegebenen Dateien] im [!UICONTROL Dropbox] >[!UICONTROL Dateien überwachen] -Modul auf `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Wenn 100 Anfragen an [!DNL Workfront]und die [!UICONTROL Limit] auf 10 gesetzt ist, bleiben nach einem Szenario 90 Dateien nicht mehr verarbeitet. Die nächsten 10 Dateien werden bei der nächsten geplanten Ausführung des Szenarios verarbeitet.
>
>### Die maximale Anzahl von Zyklen ist auf 10 festgelegt.
>
>Die [!UICONTROL Maximale Anzahl an zurückgegebenen Dateien] im [!UICONTROL Dropbox] >[!UICONTROL Dateien überwachen] -Modul auf `10`.
>
>Wenn 100 Dateien zum Ordner &quot;Dropbox&quot;hinzugefügt werden und die [!UICONTROL Maximale Anzahl an zurückgegebenen Dateien] auf 10 gesetzt ist, werden im ersten Zyklus 10 Dateien verarbeitet, im nächsten Zyklus 10 Dateien, im zweiten Zyklus die nächsten 10 Dateien im dritten Zyklus usw., bis alle Dateien verarbeitet werden.
>
>Alle Dateien werden innerhalb eines Szenarios verarbeitet.
>
>Die bereits ausgeführten Zyklen werden in den Details des Szenarios angezeigt:
>
>![](assets/scenario-detail-350x207.png)
>
>Weitere Informationen zu dieser Seite finden Sie unter [Details zum Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Anzahl aufeinander folgender Fehler

Definiert die maximale Anzahl aufeinander folgender Ausführungsversuche, bevor die Ausführung eines Szenarios deaktiviert wird (außer [!UICONTROL DataError], [!UICONTROL DuplicateDataError] und [!UICONTROL ConnectionError]).

Weitere Informationen zu Fehlern finden Sie unter [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Wenn ein Szenario mit einem sofortigen Trigger beginnt, wird die Einstellung ignoriert und das Szenario sofort deaktiviert, nachdem der erste Fehler aufgetreten ist.
