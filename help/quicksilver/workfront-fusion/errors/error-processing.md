---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fehler bei der Verarbeitung in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 1%

---

# Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Fehlertypen](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/error-processing.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Manchmal kann während der Ausführung eines Szenarios ein Fehler auftreten. Dies geschieht in der Regel, wenn ein Service aufgrund eines Fehlers bei der Verbindung zu einem Service nicht verfügbar ist oder wenn eine Validierung fehlschlägt. In diesem Artikel werden die häufigsten Fehler beschrieben, auf die Sie stoßen können.

[!DNL Adobe Workfront Fusion] unterscheidet zwischen mehreren grundlegenden Fehlertypen. Die Reaktion variiert je nach Art des aufgetretenen Fehlers.

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

## Verbindungsfehler

`ConnectionError`

Verbindungsfehler ist einer der häufigsten Fehler, der normalerweise durch die Nichtverfügbarkeit des Drittanbieterdienstes aus verschiedenen Gründen (Überlastung, Wartung, Ausfall usw.) verursacht wird. Die standardmäßige Behandlung dieses Fehlers hängt davon ab, bei welchem Modul er aufgetreten ist:

* Tritt der Fehler im ersten Modul auf, wird die Ausführung des Szenarios mit einer Warnmeldung beendet. [!DNL Workfront Fusion] versucht dann wiederholt, das Szenario in zunehmenden Zeitintervallen erneut auszuführen (diese werden unten erläutert). Wenn alle Versuche fehlschlagen, deaktiviert [!DNL Workfront Fusion] das Szenario.
* Wenn der Verbindungsfehler auf einem anderen Modul als dem ersten auftritt, hängen die nachfolgenden Schritte von der Option [Speichern unvollständiger Ausführungen zulassen](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) in den erweiterten Einstellungen des Szenarios ab:

   * Wenn diese Option aktiviert ist, wird die Ausführung des Szenarios in den Ordner [!UICONTROL Unvollständige Ausführungen] verschoben, wo [!DNL Workfront Fusion] wiederholt versucht, das Szenario in zunehmenden Zeitintervallen erneut auszuführen. Wenn alle Versuche fehlschlagen, verbleibt die Ausführung im Ordner Unvollständige Ausführungen, bis sie vom Benutzer manuell behoben wird.

     Weitere Informationen zu unvollständigen Ausführungen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Wenn diese Option deaktiviert ist, endet die Ausführung des Szenarios mit einem Fehler und einer darauf folgenden Rollback-Phase. [!DNL Workfront Fusion] versucht dann wiederholt, das Szenario in zunehmenden Zeitintervallen erneut auszuführen. Wenn alle Versuche fehlschlagen, deaktiviert [!DNL Workfront Fusion] das Szenario.

### Zunehmende Zeitintervalle

Der Algorithmus der multiplikativ steigenden Zeitintervalle zwischen Versuchen, wenn ein Fehler auftritt, wird als exponentieller Backoff bezeichnet. Die zunehmenden Zeitintervalle werden wie folgt festgelegt:

1. 10 Minuten
1. 1 Stunde
1. 3 Stunden
1. 12 Stunden
1. 24 Stunden

Der Hauptgrund für den Einsatz der zunehmenden Zeitintervalle in [!DNL Workfront Fusion] besteht darin, zu verhindern, dass häufig ausgeführte Szenarien Vorgänge bei wiederholt fehlgeschlagenen Versuchen beanspruchen.

>[!INFO]
>
>**Beispiel:**
>
>Ein Szenario enthält den [!DNL Google Sheets] Trigger [!UICONTROL Zeilen ]. [!DNL Google Sheets] ist beim Starten des Szenarios aufgrund von Wartungsarbeiten 30 Minuten lang nicht verfügbar [!DNL Workfront Fusion] kann daher keine neuen Zeilen abrufen. Das Szenario stoppt und versucht es in 10 Minuten erneut. Da [!DNL Google Sheets] immer noch nicht verfügbar ist, können [!DNL Workfront Fusion] nach wie vor keine Informationen zu neuen Zeilen abrufen. Die nächste Ausführung des Szenarios ist in 1 Stunde geplant. [!DNL Google Sheets] ist derzeit wieder verfügbar und das Szenario wird erfolgreich ausgeführt.

## Datenfehler

`DataError`

Ein Datenfehler wird erzeugt, wenn ein Element falsch zugeordnet wird und die auf der [!DNL Workfront Fusion] Seite oder auf der Seite des verwendeten Drittanbieter-Services durchgeführte Validierung nicht besteht.

Tritt dieser Fehler auf, wird das Szenario, bis zu dem das Modul fehlgeschlagen ist, in den Ordner „Unvollständige Ausführungen“ verschoben, wo Sie das Problem beheben können. Das Szenario wird jedoch nicht angehalten und wird weiterhin gemäß seinem Zeitplan ausgeführt. Um die Ausführung des Szenarios zu stoppen, wenn ein Datenfehler angezeigt wird, aktivieren Sie die Option Sequenzielle Verarbeitung im Bedienfeld „Szenario-Einstellungen“.

Wenn Sie die Option [!UICONTROL Speichern unvollständiger Ausführungen zulassen] in den Szenario-Einstellungen nicht aktiviert haben, wird die Ausführung des Szenarios mit dem Fehler beendet und ein Rollback wird durchgeführt.

Weitere Informationen zur Zuordnung finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Informationen zu unvollständigen Ausführungen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Weitere Informationen zum Bedienfeld „Szenarioeinstellungen“ finden Sie unter [Bedienfeld „Szenarioeinstellungen“ in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Weitere Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Fehler beim Duplizieren von Daten

`DuplicateDataError`

Wenn [!DNL Workfront Fusion] versucht, dasselbe Bundle zweimal in einen Service einzufügen, der keine doppelten Daten zulässt, wird ein Fehler mit doppelten Daten erzeugt. Tritt dieser Fehler auf, wird der [!DNL Workfront Fusion] auf die gleiche Weise fortgesetzt wie beim Datenfehler.

## Fehler wegen ungültigem Zugriffs-Token

`InvalidAccessTokenError`

Ein Fehler mit einem ungültigen Zugriffstoken tritt auf, wenn [!DNL Workfront Fusion] nicht auf Ihr Konto zugreifen können, das bei einem Drittanbieterdienst registriert ist. Dies geschieht normalerweise, wenn Sie Zugriffsrechte für [!DNL Workfront Fusion] in der Verwaltung eines bestimmten Services widerrufen, aber die zugehörigen Szenarien werden weiterhin gemäß dem Zeitplan ausgeführt.

Tritt dieser Fehler auf, wird die Ausführung eines Szenarios sofort angehalten. Der Rest des Szenarios, das mit dem Modul beginnt, in dem der Fehler aufgetreten ist, wird in den Ordner „Unvollständige Ausführungen“ verschoben.

Informationen zu unvollständigen Ausführungen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Fehler bei der Ratenbegrenzung

`RateLimitError`

Wenn ein von einem bestimmten Service festgelegtes Limit überschritten wird, wird ein Fehler bei der Ratenbeschränkung generiert. Tritt dieser Fehler auf, wird der [!DNL Workfront Fusion] auf die gleiche Weise fortgesetzt wie beim Verbindungsfehler.

Weitere Informationen finden Sie unter [Verbindungsfehler](#connection-error).

## Unvollständiger Datenfehler

`IncompleteDataError`

Ein unvollständiger Datenfehler tritt nur bei Triggern auf. Dieser Fehler wird generiert, wenn ein Trigger die erforderlichen Daten nicht von einem bestimmten Service herunterladen kann.

Wenn ein Szenario mit dem `IncompleteDataError` beendet wird, hängt sein weiteres Verhalten von der Einstellung [!UICONTROL Maximale Anzahl aufeinander folgender Fehler] ab.

Weitere Informationen finden Sie unter [Anzahl aufeinander folgender Fehler](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) im Artikel [Bedienfeld Szenarioeinstellungen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Beispiel:**
>
>In einem Szenario ist der [!DNL Workfront] Trigger [!UICONTROL Datensatz ], um auf Dokumente zu achten. Das Szenario wird ausgeführt, während Sie ein großes Dokument hochladen, z. B. ein langes Video. Da [!UICONTROL Workfront Fusion] versucht, das Video herunterzuladen, während es noch auf Workfront hochgeladen wird, endet das Szenario mit der `IncompleteDataError`.

## Laufzeitfehler

`RuntimeError`

Wenn während der Ausführung des Szenarios ein anderer (oben nicht erwähnter) Fehler auftritt, wird dies als `RunTimeError` gemeldet.

Wenn ein Szenario mit dem `RuntimeError` beendet wird, hängt sein weiteres Verhalten von der Einstellung [!UICONTROL Maximale Anzahl aufeinander folgender Fehler] ab. Weitere Informationen finden Sie unter [Anzahl aufeinander folgender Fehler](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) im Artikel [Bedienfeld Szenarioeinstellungen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Wenn ein Szenario mit einem sofortigen Trigger beginnt, wird die Einstellung [!UICONTROL Maximale Anzahl aufeinander folgender Fehler] ignoriert und das Szenario wird sofort deaktiviert, wenn der erste Fehler aufgetreten ist. Weitere Informationen finden Sie unter [Instant Trigger](../../workfront-fusion/modules/module-types.md#instant) im Artikel [Modultypen](../../workfront-fusion/modules/module-types.md).

## Inkonsistenzfehler

`InconsistencyError`

Wenn ein oben beschriebener Fehler während der Commit- oder Rollback-Phase auftritt, wird ein Szenario mit einem Inkonsistenzfehler beendet. Weitere Informationen finden Sie unter [Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Wenn dieser Fehler in einem Szenario auftritt, wird die Ausführung des Szenarios sofort angehalten.

## Warnung

Während der Ausführung eines Szenarios erhalten Sie möglicherweise eine Warnung, die Sie über ein Problem informiert. Dies verhindert jedoch nicht, dass das Szenario erfolgreich abgeschlossen wird.

Beispielsweise kann eine Warnung angezeigt werden, wenn die maximal zulässige Dateigröße überschritten wird und die Option [!UICONTROL Datenverlust aktivieren] deaktiviert ist. Weitere Informationen finden Sie unter [Datenverlust aktivieren](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) im Artikel [Bedienfeld „Szenarioeinstellungen“ in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
