---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Das Bedienfeld "Szenario-Einstellungen"in Adobe Workfront Fusion
description: In diesem Artikel werden die Einstellungen beschrieben, die im Bedienfeld [!UICONTROL szenario settings] in Ihren [!DNL Adobe Workfront Fusion] Szenarien verfügbar sind.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 1b729960a23e43252bda16d9bfb7ca9656a115a1
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# Das Bedienfeld für die Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

## Öffnen Sie die Szenario-Einstellungen.

1. Öffnen Sie den Szeneneditor, wie in [Der Szeneneditor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md) beschrieben.
1. Klicken Sie auf das Zahnradsymbol unten links auf der Seite.

   ![](assets/scenario-settings-350x221.png)

   Im angezeigten Bedienfeld [!UICONTROL Szenario-Einstellungen] können Sie verschiedene erweiterte Einstellungen für das Szenario konfigurieren.

## [!UICONTROL Speichern unvollständiger Ausführungen zulassen]

Diese Option bestimmt, wie [!DNL Adobe Workfront Fusion] ausgeführt wird, wenn während der Ausführung eines Szenarios ein Fehler auftritt. Wenn diese Option aktiviert ist, wird das Szenario angehalten und in [Ansicht verschoben, um unvollständige Ausführungen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) aufzulösen. Dadurch haben Sie die Möglichkeit, das Problem zu beheben und die Ausführung dort fortzusetzen, wo das Szenario angehalten wurde. Wenn diese Option deaktiviert ist, wird das Szenario angehalten und eine Rollback-Phase gestartet.

## [!UICONTROL  Sequenzielle Verarbeitung]

Diese Option bestimmt, wie [!DNL Workfront Fusion] ausgeführt wird, wenn ein Fehler auftritt und die Ausführung eines Szenarios in die [Ansicht verschoben wird und unvollständige Ausführungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) aufgelöst werden. Wenn die Option [!UICONTROL Sequenzielle Verarbeitung] aktiviert ist, stoppt Workfront Fusion die Verarbeitung der Aufgabensequenz vollständig, bis alle unvollständigen Ausführungen abgeschlossen sind. Wenn die Option [!UICONTROL Sequenzielle Verarbeitung] deaktiviert ist, wird das Szenario weiterhin gemäß seinem Zeitplan ausgeführt, wobei wiederholte Versuche unternommen werden, die unvollständigen Ausführungen erneut auszuführen.

>[!NOTE]
>
>Die sequenzielle Verarbeitung kann die Ausführung eines Szenarios verzögern. Wenn sich noch unvollständige Ausführungen in der Warteschlange befinden, wenn ein Sofortszenario oder ein geplantes Szenario zur Ausführung bestimmt ist, wird dieses Szenario ausgeführt, nachdem alle Ausführungen abgeschlossen sind, bevor es in der Warteschlange ausgeführt wurde.
>
>Wenn der Anwendungsfall für Ihre Szenarien keine sequenzielle Verarbeitung erfordert, empfehlen wir, die Option für die sequenzielle Verarbeitung zu deaktivieren.

Weitere Informationen zur Planung finden Sie unter [Planen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Daten sind vertraulich

Sobald ein Szenario ausgeführt wurde, können Sie standardmäßig Informationen darüber anzeigen, welche Daten von Modulen im Szenario verarbeitet wurden. Wenn diese Informationen nicht gespeichert werden sollen, aktivieren Sie die Option [!UICONTROL Daten sind vertraulich] .

Weitere Informationen zur Anzeige von Informationen finden Sie unter [Ausführungsfluss eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Wenn Sie diese Option aktivieren, kann es schwierig sein, Fehler zu beheben, die während der Ausführung eines Szenarios auftreten können.

## Datenverlust aktivieren

Diese Option hat mit der Aktivierung des Datenverlusts zu tun, wenn [!DNL Workfront Fusion] ein Bundle nicht in der Warteschlange von [Anzeigen und Auflösen unvollständiger Ausführungen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) speichern kann (z. B. weil kein freier Speicherplatz vorhanden ist). Wenn diese Option aktiviert ist, gehen die Daten verloren, um Unterbrechungen bei der Ausführung des Szenarios insgesamt zu vermeiden. Dies ist für Szenarien nützlich, in denen die kontinuierliche Ausführung mit der höchsten Priorität erfolgt und die eingehenden fehlerhaften Daten nicht so wichtig sind.

Darüber hinaus kann ein Modul bei der Ausführung eines Szenarios auf eine Datei stoßen, die größer als die maximal zulässige Größe ist. In diesem Fall wird [!DNL Workfront Fusion] entsprechend der Einstellung der Option [!UICONTROL Datenverlust aktivieren] fortgesetzt und es wird eine Warnmeldung angezeigt.

Weitere Informationen zur maximalen Dateigröße finden Sie unter [Über die Zuordnung von Dateien in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Weitere Informationen zu Warnungen finden Sie unter [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Auto commit]

Die Einstellungen für [!UICONTROL Automatisches Übertragen] gelten für Transaktionen und definieren die Methode zur Verarbeitung eines Szenarios. Wenn die Option Automatisches Übertragen aktiviert ist, beginnt die Commit-Phase in jedem Modul unmittelbar nach Abschluss der Betriebsphase. Wenn die Option Automatisches Übertragen deaktiviert ist, erfolgt keine Übertragung, bis Vorgänge für alle Module ausgeführt werden (dies ist der Standardmodus).

Weitere Informationen zu Transaktionen finden Sie unter [Ausführung, Zyklen und Phasen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Höchstzahl der Zyklen

Das Festlegen weiterer Zyklen kann nützlich sein, wenn Sie eine Unterbrechung der Verbindung zu einem Drittanbieterdienst verhindern und sicherstellen möchten, dass alle Datensätze innerhalb des einen Szenario verarbeitet werden.

* Beginnt das Szenario mit einem Abrufintereignis, wird in der Einstellung die maximale Anzahl von Triggern definiert, die während der Ausführung des Szenarios zulässig sind.

  Weitere Informationen zu Triggern zum Abruf finden Sie unter [Abrufen von Triggern](../../workfront-fusion/modules/module-types.md#polling) in [Modultypen](../../workfront-fusion/modules/module-types.md).

* Wenn das Szenario mit einem sofortigen Trigger beginnt, wird die Einstellung ignoriert und alle ausstehenden Ereignisse werden während der Ausführung eines einzigen Szenarios verarbeitet, d. h. ein Ereignis pro Zyklus.

  Weitere Informationen zu sofortigen Triggern finden Sie unter [Instant Trigger](../../workfront-fusion/modules/module-types.md#instant) in [Modultypen](../../workfront-fusion/modules/module-types.md).

* Wenn das Szenario nicht mit einem Trigger beginnt (Instant/Polling), wird immer die angegebene maximale Anzahl von Zyklen ausgeführt.

>[!INFO]
>
>**Beispiele:** [!DNL Workfront] > [!UICONTROL Datensatz überwachen] überwacht neue Probleme, die auftreten, und [!DNL Workfront] >[!UICONTROL Objekt konvertieren] konvertiert die neue Anforderung in ein Projekt und weist ihr die entsprechende Vorlage zu.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>Die Einstellung [!UICONTROL Mehr Zyklen] wird nur angewendet, wenn Sie die Ausführung des Szenarios planen. Wenn Sie die Schaltfläche [!UICONTROL Einmal ausführen] verwenden, werden die Zykluseinstellungen berücksichtigt.
>
>### Die maximale Anzahl von Zyklen ist auf 1 gesetzt (Standard).
>
>![](assets/max-number-cycles-1-350x201.png)
>
>Die [!UICONTROL Maximale Anzahl der zurückgegebenen Dateien] im Modul [!UICONTROL Workfront] >[!UICONTROL Datensätze überwachen] ist auf `10` eingestellt.
>Wenn 100 Anfragen an [!DNL Workfront] gesendet werden und das Feld [!UICONTROL Limit] auf 10 gesetzt ist, werden nach einem Szenario 90 Dateien nicht mehr verarbeitet. Die nächsten 10 Dateien werden bei der nächsten geplanten Ausführung des Szenarios verarbeitet.
>
>### Die maximale Anzahl von Zyklen ist auf 10 festgelegt.
>
>Die [!UICONTROL maximale Anzahl der zurückgegebenen Dateien] im Modul [!UICONTROL Dropbox] >[!UICONTROL Dateien ansehen] ist auf `10` eingestellt.
>
>Wenn 100 Dateien zum Dropbox-Ordner hinzugefügt werden und die Option [!UICONTROL Maximale Anzahl an zurückgegebenen Dateien] auf 10 festgelegt ist, werden während des ersten Zyklus, der nächsten 10 Dateien im zweiten Zyklus, der nächsten 10 Dateien im dritten Zyklus usw. verarbeitet, bis alle Dateien verarbeitet werden.
>
>Alle Dateien werden innerhalb eines Szenarios verarbeitet.
>
>Die bereits ausgeführten Zyklen werden in den Details des Szenarios angezeigt:
>
>![](assets/scenario-detail-350x207.png)
>
>Weitere Informationen zu dieser Seite finden Sie unter [Details zum Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Anzahl aufeinander folgender Fehler

Definiert die maximale Anzahl aufeinander folgender Ausführungsversuche, bevor die Ausführung eines Szenarios deaktiviert wird (ausgenommen [!UICONTROL DataError], [!UICONTROL DuplicateDataError] und [!UICONTROL ConnectionError]).

Weitere Informationen zu Fehlern finden Sie unter [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Wenn ein Szenario mit einem sofortigen Trigger beginnt, wird die Einstellung ignoriert und das Szenario sofort deaktiviert, nachdem der erste Fehler aufgetreten ist.
