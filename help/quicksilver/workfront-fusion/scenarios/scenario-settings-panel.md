---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Das Bedienfeld „Szenario-Einstellungen“ in Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1266'
ht-degree: 0%

---

# Das Bedienfeld „Szenario-Einstellungen“ in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Szenario-Einstellungen konfigurieren](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-scenario-settings/configure-scenario-settings.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Szenarioeinstellungen öffnen

1. Öffnen Sie den Szenario-Editor, wie in [Der Szenario-Editor in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md) beschrieben.
1. Klicken Sie unten links auf der Seite auf das Zahnradsymbol.

   ![](assets/scenario-settings-350x221.png)

   Im angezeigten Bedienfeld [!UICONTROL Szenarioeinstellungen] können Sie verschiedene erweiterte Einstellungen für das Szenario konfigurieren.

## [!UICONTROL Speichern unvollständiger Ausführungen zulassen]

Diese Option bestimmt, wie [!DNL Adobe Workfront Fusion] bei einem Fehler während der Ausführung eines Szenarios verfahren wird. Wenn diese Option aktiviert ist, wird das Szenario angehalten und in &quot;[ anzeigen und unvollständige Ausführungen in auflösen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) verschoben. Dadurch haben Sie die Möglichkeit, das Problem zu beheben und die Ausführung von dort fortzusetzen, wo das Szenario gestoppt wurde. Wenn diese Option deaktiviert ist, wird die Ausführung des Szenarios gestoppt und eine Rollback-Phase gestartet.

## [!UICONTROL Sequenzielle Verarbeitung]

Diese Option erzwingt, dass alle Ausführungen in der richtigen Reihenfolge erfolgen, und ist in erster Linie für Webhooks und für unvollständige Ausführungen relevant.

Wenn die sequenzielle Verarbeitung aktiviert ist, werden parallele Ausführungen des Szenarios deaktiviert.

### Sofortige Webhooks

Wenn ein Webhook-Trigger als `instant` konfiguriert und die „sequenzielle Verarbeitung“ aktiviert ist, werden alle sofortigen Webhook-Payloads in der Reihenfolge ihrer Ankunft in die Warteschlange gestellt und verarbeitet. Dies kann nützlich sein, wenn Ereignisse von externen Systemen in einer exakten Reihenfolge verarbeitet werden.

>[!NOTE]
>
>Es kommt zu automatischen Verarbeitungsverzögerungen, da jede Payload verarbeitet wird, bevor die nächste gestartet wird.

### Unvollständige Ausführungen

Wenn auch „Unvollständige Ausführungen“ aktiviert ist und bei der Ausführung eines Szenarios ein Fehler auftritt, wird das Szenario angehalten. Eine der folgenden Situationen tritt dann auf:

* Wenn die Option Sequenzielle Verarbeitung **aktiviert**, stoppt Workfront Fusion die Verarbeitung der bereits vorhandenen Sequenz, bis alle unvollständigen Ausführungen aufgelöst sind.
* Wenn die Option für die sequenzielle Verarbeitung **deaktiviert** ist, wird das Szenario weiterhin gemäß seinem Zeitplan ausgeführt, begleitet von wiederholten Versuchen, die unvollständigen Ausführungen erneut auszuführen.

Weitere Informationen zu unvollständigen Ausführungen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

<!--

This option determines how [!DNL Workfront Fusion] proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the [!UICONTROL Sequential processing] option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the [!UICONTROL Sequential processing] option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.-->

>[!NOTE]
>
>Die sequenzielle Verarbeitung kann die Ausführung eines Szenarios verzögern. Wenn sich noch unvollständige Ausführungen in der Warteschlange befinden, wenn die Ausführung eines Sofortszenarios oder eines geplanten Trigger festgelegt ist, wird dieses Szenario ausgeführt, nachdem alle Ausführungen abgeschlossen sind, bevor es in der Warteschlange abgeschlossen ist.
>
>Wenn der Anwendungsfall für Ihre Szenarien keine sequenzielle Verarbeitung erfordert, empfehlen wir, die Option für die sequenzielle Verarbeitung zu deaktivieren.

Weitere Informationen zur Planung finden Sie unter [Planen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Daten sind vertraulich

Nachdem ein Szenario ausgeführt wurde, können Sie standardmäßig Informationen darüber anzeigen, welche Daten von Modulen im Szenario verarbeitet wurden. Wenn diese Informationen nicht gespeichert werden sollen, aktivieren Sie die Option [!UICONTROL Daten sind vertraulich].

Weitere Informationen zum Anzeigen von Informationen finden [ unter „Szenario-Ausführungsfluss in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Wenn Sie diese Option aktivieren, kann es schwierig sein, Fehler zu beheben, die während der Ausführung eines Szenarios auftreten können.

## Datenverlust aktivieren

Diese Option hat mit der Aktivierung von Datenverlust zu tun, wenn [!DNL Workfront Fusion] ein Bundle nicht in der Warteschlange von speichern [unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (z. B. aufgrund von fehlendem Speicherplatz). Wenn diese Option aktiviert ist, gehen die Daten verloren, um Unterbrechungen bei der Ausführung des Gesamtszenarios zu verhindern. Dies ist nützlich für Szenarien, in denen die höchste Priorität die kontinuierliche Ausführung ist und die eingehenden fehlerhaften Daten nicht so wichtig sind.

Darüber hinaus kann es beim Ausführen eines Szenarios vorkommen, dass ein Modul auf eine Datei trifft, die größer ist als die maximal zulässige Größe. In diesem Fall wird [!DNL Workfront Fusion] gemäß der Einstellung der Option [!UICONTROL Datenverlust aktivieren] fortgesetzt und eine Warnmeldung wird angezeigt.

Weitere Informationen zur maximalen Dateigröße finden Sie unter [Informationen zum Zuordnen von Dateien in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Weitere Informationen zu Warnungen finden Sie unter [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Automatische Bestätigung]

Die Einstellungen [!UICONTROL Automatische ]) gelten für Transaktionen und definieren die Verarbeitung eines Szenarios. Wenn die Option „Auto Commit“ aktiviert ist, beginnt die Commit-Phase für jedes Modul sofort nach Abschluss der Vorgangsphase. Bei deaktivierter Option „Automatisches Commit“ erfolgt kein Commit, bis Vorgänge für alle Module ausgeführt werden (dies ist der Standardmodus).

Weitere Informationen zu Transaktionen finden Sie unter [Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Maximale Zyklenanzahl

Das Festlegen weiterer Zyklen kann nützlich sein, wenn Sie eine Verbindungsunterbrechung zu einem Drittanbieterdienst verhindern und sicherstellen möchten, dass alle Datensätze innerhalb eines einzigen Szenarios verarbeitet werden.

* Wenn das Szenario mit einem Abrufintervall beginnt, definiert die Einstellung die maximale Anzahl von Triggern, die während der Ausführung des Szenarios zulässig ist.

  Weitere Informationen zum Abrufen von Trigger Triggern finden Sie unter [Abrufen von ](../../workfront-fusion/modules/module-types.md#polling)&quot; in [Modultypen](../../workfront-fusion/modules/module-types.md).

* Wenn das Szenario mit einem sofortigen Trigger beginnt, wird die Einstellung ignoriert und alle ausstehenden Ereignisse werden während einer einzigen Szenario-Ausführung verarbeitet, ein Ereignis pro Zyklus.

  Weitere Informationen zu Instant Triggern finden Sie unter [Instant Trigger ](../../workfront-fusion/modules/module-types.md#instant) unter [Modultypen](../../workfront-fusion/modules/module-types.md).

* Wenn das Szenario nicht mit einem Trigger beginnt (Sofort-/Abrufintervall), wird immer die angegebene maximale Anzahl von Zyklen ausgeführt.

>[!INFO]
>
>**Beispiele:** [!DNL Workfront] > [!UICONTROL Datensatz beobachten] überwacht neue Probleme, die auftreten, und [!DNL Workfront] >[!UICONTROL Objekt konvertieren] konvertiert die neue Anfrage in ein Projekt und weist ihr die entsprechende Vorlage zu.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>Eine Einstellung [!UICONTROL Weitere Zyklen] wird nur angewendet, wenn Sie die Ausführung des Szenarios planen. Wenn Sie die Schaltfläche [!UICONTROL Einmal ausführen] verwenden, werden die Zykluseinstellungen berücksichtigt.
>
>### Die maximale Anzahl von Zyklen ist auf 1 festgelegt (Standard)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>Die [!UICONTROL Maximale Anzahl zurückgegebener Dateien] im Modul [!UICONTROL Workfront] >[!UICONTROL Datensätze ] ist auf `10` festgelegt.
>Wenn 100 Anfragen an [!DNL Workfront] gesendet werden und das Feld [!UICONTROL Limit] auf 10 festgelegt ist, werden 90 Dateien nach einer Szenario-Ausführung nicht verarbeitet. Die nächsten 10 Dateien werden im nächsten geplanten Szenario verarbeitet.
>
>### Die maximale Anzahl von Zyklen ist auf 10 festgelegt.
>
>Die [!UICONTROL Maximale Anzahl zurückgegebener Dateien] im Modul [!UICONTROL Dropbox] >[!UICONTROL Dateien ] ist auf `10` festgelegt.
>
>Wenn dem Ordner &quot;Dropbox&quot; 100 Dateien hinzugefügt werden und die Option [!UICONTROL Maximale Anzahl zurückgegebener Dateien] auf 10 festgelegt ist, werden während des ersten Zyklus 10 Dateien, während des zweiten Zyklus die nächsten 10 Dateien, im dritten Zyklus die nächsten 10 Dateien usw. verarbeitet, bis alle Dateien verarbeitet sind.
>
>Alle Dateien werden innerhalb eines Szenario-Durchgangs verarbeitet.
>
>Die bereits ausgeführten Zyklen werden in den Details des Szenarios angezeigt:
>
>![](assets/scenario-detail-350x207.png)
>
>Weitere Informationen zu dieser Seite finden Sie unter [Szenariodetails in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Anzahl aufeinander folgender Fehler

Definiert die maximale Anzahl aufeinander folgender Ausführungsversuche, bevor die Ausführung eines Szenarios deaktiviert wird (außer [!UICONTROL DataError], [!UICONTROL DuplicateDataError] und [!UICONTROL ConnectionError]).

Weitere Informationen zu Fehlern finden Sie unter [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Wenn ein Szenario mit einem sofortigen Trigger beginnt, wird die Einstellung ignoriert und das Szenario wird sofort deaktiviert, wenn der erste Fehler aufgetreten ist.
