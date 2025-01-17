---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Anweisungen für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 12%

---

# Anweisungen für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Anweisungen für die Fehlerbehandlung](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/directives-for-error-handling.html)
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

## Anweisungen für die Fehlerbehandlung

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Rollback</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>Die Ausführung des Szenarios wird sofort gestoppt und eine <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Rollback</a>-Phase wird für alle Module gestartet, um sie alle in den Ausgangszustand zurückzuversetzen. Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Abgesehen von einigen Fehlertypen wird das Szenario nach der in den Szenario-Einstellungen angegebenen Anzahl aufeinander folgender Fehler deaktiviert. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Anzahl aufeinander folgender Fehler</a>.</p> <p>Der Status der Szenarioausführung ist als „Fehler“ gekennzeichnet.</p> <p>Hinweis: Dies ist das Standardverhalten, wenn dem Modul keine Fehler-Handler-Route angehängt ist und die Einstellung <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Speichern unvollständiger Ausführungen zulassen]</a> unter [!UICONTROL Szenario-Einstellungen] nicht aktiviert ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zusichern</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>Die Ausführung des Szenarios wird sofort gestoppt und eine Commit-Phase wird für alle Module gestartet. Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Alle nicht verarbeiteten Pakete werden ignoriert.</p> <p>Der Ausführungsstatus des Szenarios wird als „Erfolg“ markiert. Informationen zu Commit-Phasen finden Sie <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Commit</a> im Artikel <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Szenario-Ausführung, -Zyklen und -Phasen in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Wieder aufnehmen</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Es wird eine Ersatzausgabe angegeben und an das Modul geliefert, bei dem ein Fehler auftritt.</p> <p>Die nachfolgenden Module werden verarbeitet.</p> <p>Der Status der Szenarioausführung wird als „erfolgreich“ gekennzeichnet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorieren</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>Der Fehler wird ignoriert und die nachfolgenden Module werden nicht verarbeitet.</p> <p>Wenn unbearbeitete Bündel vorhanden sind, wird die Ausführung des Szenarios normal fortgesetzt.</p> <p>Der Status der Szenarioausführung wird als „erfolgreich“ gekennzeichnet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Unterbrechen</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>Der Zustand der Szenarioausführung wird in der Warteschlange für unvollständige Ausführungen gespeichert, wo der Fehler manuell behoben werden kann. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Anzeigen und Beheben von unvollständigen Ausführungen in Adobe Workfront Fusion</a>. </p> <p>Es gibt jedoch einige Ausnahmen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Speichern unvollständiger Ausführungen zulassen</a> im Artikel <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Bedienfeld „Szenarioeinstellungen“ in Adobe Workfront Fusion</a>.</p> <p>Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Wenn unbearbeitete Bündel vorhanden sind, wird die Ausführung des Szenarios normal fortgesetzt.</p> <p>Der Ausführungsstatus des Szenarios wird als „Warnung“ markiert, wenn die Option [!UICONTROL Ausführung automatisch abschließen] deaktiviert ist.</p> <p>Weitere Informationen finden Sie im Abschnitt <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> weiter unten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Erneut versuchen</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>In einigen Fällen kann es nützlich sein, ein fehlerhaftes Modul einige Male erneut auszuführen, wenn die Wahrscheinlichkeit besteht, dass der Grund für den Fehler mit der Zeit vergeht.</p> <p>Workfront Fusion bietet derzeit keine Wiederholungsrichtlinie an, obwohl mehrere Problemumgehungen verwendet werden können, um die Funktionalität nachzuahmen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Fehlerbehandlung bei erneuten Versuchen in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Derzeit können die Anweisungen zur Fehlerbehandlung nicht außerhalb einer Route zur Fehlerbehandlung verwendet werden.
>
>   Weitere Informationen finden Sie unter [Fehler-Handler-Route](../../workfront-fusion/errors/error-handling.md#error) im Artikel [Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] bietet derzeit kein Throw-Modul, mit dem Sie einfach bedingt Fehler (Throw-Fehler) erzeugen können, obwohl eine Problemumgehung eingesetzt werden kann, um seine Funktionalität nachzuahmen.
>
>   Weitere Informationen finden Sie unter [Problemumgehung für ](../../workfront-fusion/errors/throw.md#workaround-for-throw)&quot; im Artikel [Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Unterbrechen {#break}

Wenn ein Fehler von der [!DNL Break]-Anweisung verarbeitet wird, wird im Ordner Unvollständige Ausführungen ein Datensatz erstellt. Dieser Datensatz speichert den Status der Szenario-Ausführung zusammen mit Daten aus den vorherigen Modulen. Der Datensatz verweist auf das Modul, von dem der Fehler stammt, und enthält Informationen darüber, welche Daten vom Modul als Eingabe empfangen wurden. Für jedes Datenbündel, das den Fehler verursacht, wird ein separater Datensatz erstellt.

Weitere Informationen finden Sie unter [Anzeigen und Beheben von unvollständigen Ausführungen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Beheben von Fehlern, die sich aus der Break-Direktive ergeben

Sie können den Fehler manuell beheben, indem Sie das Szenario (falls erforderlich) aktualisieren und es einmal ausführen.

Sie können das Szenario auch so konfigurieren, dass eine unvollständige Ausführung automatisch verarbeitet wird, indem Sie das Szenario erneut ausführen. So konfigurieren Sie das Modul für die Verarbeitung unvollständiger Ausführungen:

1. Aktivieren Sie innerhalb des Moduls break die Option [!UICONTROL **Ausführung automatisch abschließen**].
1. Geben **im Feld „Anzahl der**&quot; die maximale Anzahl der Versuche ein, für die das Modul die Ausführung wiederholen soll, oder mappen Sie sie

   Diese Zahl muss zwischen 1 und 100 liegen.
1. Geben **im Feld „Intervall zwischen**&quot; die Anzahl der Minuten zwischen den einzelnen Wiederholungsversuchen ein oder mappen Sie sie.

Wenn diese Option aktiviert ist, wird bei einem Fehler die unvollständige Ausführung abgerufen (nach der im Feld [!UICONTROL Intervall zwischen Versuchen] angegebenen Zeit) und mit den ursprünglichen Eingabedaten ausgeführt. Dies wird wiederholt, bis die Ausführung des Moduls fehlerfrei abgeschlossen wird oder die angegebene Anzahl von Versuchen erreicht ist.

>[!NOTE]
>
>Wenn der erste Wiederholungsversuch fehlschlägt, erhöht sich das Intervall zwischen den Wiederholungsversuchen exponentiell bei jedem zweiten Versuch.


Wenn „Ausführung automatisch abschließen“ aktiviert ist, wird die Ausführung des Szenarios als „Erfolg“ markiert, da das Problem durch den automatischen Wiederholungsversuch des Fehler-Handlers automatisch behoben wird. In diesem Fall erhalten Benutzerinnen und Benutzer keine E-Mail über die fehlgeschlagene Ausführung.

Wenn „Automatische Ausführung abschließen“ deaktiviert ist, wird der Durchlauf als „Warnung“ markiert.

Es gibt einige Ausnahmen davon, dass Ausführungen unter Unvollständige Ausführungen gespeichert werden. Bei einigen Fehlertypen ist der automatische erneute Versuch einer Szenarioausführung nicht möglich.

Weitere Informationen finden Sie unter [Speichern unvollständiger Ausführungen zulassen](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) im Artikel [Bedienfeld „Szenarioeinstellungen“ in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Weitere Informationen finden Sie unter [Erweiterte Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
