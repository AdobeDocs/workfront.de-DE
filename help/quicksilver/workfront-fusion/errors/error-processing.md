---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]
description: Manchmal kann während der Ausführung eines Szenarios ein Fehler auftreten. Dies geschieht normalerweise, wenn ein Dienst aufgrund eines Fehlers der Verbindung zu einem Dienst nicht verfügbar ist oder wenn eine Überprüfung fehlschlägt. In diesem Artikel werden die häufigen Fehler erläutert, auf die Sie stoßen können.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 184033c8957e955b3011f7e0845a73029f6b7aba
workflow-type: tm+mt
source-wordcount: '1194'
ht-degree: 0%

---

# Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]

Manchmal kann während der Ausführung eines Szenarios ein Fehler auftreten. Dies geschieht normalerweise, wenn ein Dienst aufgrund eines Fehlers der Verbindung zu einem Dienst nicht verfügbar ist oder wenn eine Überprüfung fehlschlägt. In diesem Artikel werden die häufigen Fehler erläutert, auf die Sie stoßen können.

[!DNL Adobe Workfront Fusion] unterscheidet zwischen mehreren grundlegenden Fehlertypen. Je nach Typ des aufgetretenen Fehlers reagiert sie unterschiedlich.

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

## Verbindungsfehler

`ConnectionError`

Verbindungsfehler sind einer der häufigsten Fehler, der normalerweise durch die Nichtverfügbarkeit des Drittanbieterdienstes aus verschiedenen Gründen (Überlastung, Wartung, Ausfall usw.) verursacht wird. Die standardmäßige Handhabung dieses Fehlers hängt davon ab, auf welchem Modul er gefunden wurde:

* Tritt der Fehler beim ersten Modul auf, wird die Ausführung des Szenarios mit einer Warnmeldung beendet. [!DNL Workfront Fusion] wiederholt versucht, das Szenario in zunehmendem Zeitintervall erneut auszuführen (diese werden unten erläutert). Wenn alle Versuche fehlschlagen, [!DNL Workfront Fusion] deaktiviert das Szenario.
* Wenn der Verbindungsfehler bei einem anderen Modul als dem ersten auftritt, hängen die nachfolgenden Schritte von der [Speichern unvollständiger Ausführungen zulassen](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) in den erweiterten Einstellungen des Szenarios:

   * Wenn diese Option aktiviert ist, wird die Ausführung des Szenarios an die [!UICONTROL Unvollständige Ausführungen] Ordner, [!DNL Workfront Fusion] wiederholt versucht, das Szenario in zunehmenden Zeitintervallen erneut auszuführen. Wenn alle Versuche fehlschlagen, bleibt die Ausführung im Ordner Unvollständige Ausführungen und wartet auf eine manuelle Auflösung durch den Benutzer.

      Weitere Informationen zu unvollständigen Ausführungen finden Sie unter [Unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Wenn diese Option deaktiviert ist, endet die Ausführung des Szenarios mit einem Fehler, gefolgt von einer Rollback-Phase. [!DNL Workfront Fusion] wiederholt versucht, das Szenario in zunehmenden Zeitintervallen erneut auszuführen. Wenn alle Versuche fehlschlagen, [!DNL Workfront Fusion] deaktiviert das Szenario.

### Erhöhen der Zeitintervalle

Der Algorithmus der multiplikativ steigenden Zeitintervalle zwischen Versuchen, wenn ein Fehler auftritt, wird als exponentieller Backoff bezeichnet. Die steigenden Zeitintervalle werden wie folgt festgelegt:

1. 10 Minuten
1. 1 Stunde
1. 3 Stunden
1. 12 Stunden
1. 24 Stunden

Hauptgrund für die Verwendung der zunehmenden Zeitintervalle in [!DNL Workfront Fusion] verhindert, dass häufig ausgeführte Szenarien Vorgänge bei wiederholten fehlgeschlagenen Versuchen verbrauchen.

>[!INFO]
>
>**Beispiel:**
>
>Ein Szenario enthält die [!DNL Google Sheets] Trigger [!UICONTROL Zeilen ansehen]. [!DNL Google Sheets] 30 Minuten lang nicht verfügbar ist, da es aufgrund von Wartungsarbeiten nicht möglich ist, [!DNL Workfront Fusion] startet das Szenario, sodass keine neuen Zeilen abgerufen werden können. Das Szenario stoppt und versucht es in 10 Minuten erneut. weil [!DNL Google Sheets] noch nicht verfügbar ist, [!DNL Workfront Fusion] kann immer noch keine Informationen zu neuen Zeilen abrufen. Die nächste Ausführung des Szenarios ist in einer Stunde geplant. [!DNL Google Sheets] ist jetzt wieder verfügbar und das Szenario wird erfolgreich ausgeführt.

## Datenfehler

`DataError`

Ein Datenfehler wird erzeugt, wenn ein Element falsch zugeordnet ist und die für die [!DNL Workfront Fusion] Seite oder auf der Seite des zu verwendenden Drittanbieterdienstes.

Tritt dieser Fehler auf, wird das Szenario, bis zu dem das Modul fehlschlug, in den Ordner mit unvollständigen Ausführungen verschoben, in dem Sie das Problem beheben können. Das Szenario wird jedoch nicht angehalten und läuft weiterhin gemäß seinem Zeitplan. Um die Ausführung des Szenarios beim Anzeigen des Datenfehlers zu stoppen, aktivieren Sie die Option Sequenzielle Verarbeitung im Bereich Szenario-Einstellungen .

Wenn Sie die Funktion [!UICONTROL Speichern unvollständiger Ausführungen zulassen] -Option in den Szenario-Einstellungen wird die Ausführung des Szenarios mit dem Fehler beendet und es wird ein Rollback durchgeführt.

Weitere Informationen zur Zuordnung finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Informationen zu unvollständigen Ausführungen finden Sie unter [Unvollständige Ausführungen in Adobe Workfront Fusion anzeigen und auflösen](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Weitere Informationen zum Bereich für die Szenario-Einstellung finden Sie unter [Das Bedienfeld &quot;Szenario-Einstellungen&quot;in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Weitere Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Datenfehler duplizieren

`DuplicateDataError`

Wenn [!DNL Workfront Fusion] versucht, dasselbe Bundle zweimal in einen Dienst einzufügen, der keine doppelten Daten zulässt, wird ein doppelter Datenfehler erzeugt. Tritt dieser Fehler auf, [!DNL Workfront Fusion] läuft genauso wie beim Datenfehler.

## Fehler bei ungültigem Zugriffstoken

`InvalidAccessTokenError`

Ein Fehler wegen eines ungültigen Zugriffstokens tritt auf, wenn [!DNL Workfront Fusion] kann nicht auf Ihr Konto zugreifen, das bei einem Drittanbieterdienst registriert ist. Dies geschieht normalerweise, wenn Sie Zugriffsberechtigungen für [!DNL Workfront Fusion] in der Verwaltung eines bestimmten Dienstes, aber die damit verbundenen Szenarien werden weiterhin planmäßig ausgeführt.

Tritt dieser Fehler auf, wird die Ausführung eines Szenarios sofort angehalten. Der Rest des Szenarios, beginnend mit dem -Modul, in dem der Fehler aufgetreten ist, wird in den Ordner für unvollständige Ausführungen verschoben.

Informationen zu unvollständigen Ausführungen finden Sie unter [Unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Fehler bei Ratenbeschränkung

`RateLimitError`

Wenn eine von einem bestimmten Dienst festgelegte Grenze überschritten wird, wird ein Fehler wegen einer Ratenbegrenzung erzeugt. Wenn dieser Fehler auftritt, [!DNL Workfront Fusion] läuft genauso wie beim Verbindungsfehler.

Weitere Informationen finden Sie unter [Verbindungsfehler](#connection-error).

## Fehler bei unvollständigen Daten

`IncompleteDataError`

Ein unvollständiger Datenfehler tritt nur bei Triggern auf. Dieser Fehler wird erzeugt, wenn ein Trigger die erforderlichen Daten von einem bestimmten Dienst nicht herunterladen kann.

Wenn ein Szenario mit der `IncompleteDataError`, hängt sein weiteres Verhalten von der Festlegung der [!UICONTROL Maximale Anzahl aufeinander folgender Fehler].

Weitere Informationen finden Sie unter [Anzahl aufeinander folgender Fehler](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) im Artikel [Das Bedienfeld &quot;Szenario-Einstellungen&quot;in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Beispiel:**
>
>Ein Szenario enthält die [!DNL Workfront] Trigger [!UICONTROL Aufzeichnen von Aufnahmen] Legen Sie fest, um nach Dokumenten zu suchen. Das Szenario wird beim Hochladen eines großen Dokuments, z. B. eines langen Videos, ausgeführt. weil [!UICONTROL Workfront Fusion] versucht, das Video herunterzuladen, während es noch auf Workfront hochgeladen wird, wird das Szenario mit der `IncompleteDataError`.

## Laufzeitfehler

`RuntimeError`

Wenn während der Ausführung des Szenarios ein anderer (oben nicht genannter) Fehler auftritt, wird er als `RunTimeError`.

Wenn ein Szenario mit der `RuntimeError`, hängt sein weiteres Verhalten von der Festlegung der [!UICONTROL Maximale Anzahl aufeinander folgender Fehler]. Weitere Informationen finden Sie unter [Anzahl aufeinander folgender Fehler](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) im Artikel [Das Bedienfeld &quot;Szenario-Einstellungen&quot;in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Wenn ein Szenario mit einem sofortigen Trigger beginnt, wird die Einstellung [!UICONTROL Maximale Anzahl aufeinander folgender Fehler] wird ignoriert und das Szenario wird sofort deaktiviert, nachdem der erste Fehler aufgetreten ist. Weitere Informationen finden Sie unter [Sofortige Trigger](../../workfront-fusion/modules/module-types.md#instant) im Artikel [Modultypen](../../workfront-fusion/modules/module-types.md).

## Inkonsistenzfehler

`InconsistencyError`

Wenn ein oben genannter Fehler während der Commit- oder Rollback-Phase auftritt, wird ein Szenario mit Inkonsistenzfehler beendet. Weitere Informationen finden Sie unter [Ausführung des Szenarios, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Wenn dieser Fehler in einem Szenario auftritt, wird die Ausführung des Szenarios sofort angehalten.

## Warnung

Beim Ausführen eines Szenarios erhalten Sie möglicherweise eine Warnung, die Sie über ein Problem informiert. Es verhindert jedoch nicht, dass das Szenario erfolgreich abgeschlossen wurde.

Beispielsweise kann eine Warnung angezeigt werden, wenn die maximal zulässige Dateigröße überschritten wird und die [!UICONTROL Datenverlust aktivieren] deaktiviert ist. Weitere Informationen finden Sie unter [Datenverlust aktivieren](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) im Artikel [Das Bedienfeld &quot;Szenario-Einstellungen&quot;in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
