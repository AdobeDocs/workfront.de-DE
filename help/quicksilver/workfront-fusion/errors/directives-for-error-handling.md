---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]
description: In diesem Artikel werden Richtlinien beschrieben, die Sie für die Fehlerbehandlung in Ihrem [!DNL Adobe Workfront Fusion] Szenarien.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: f4e43d34068c987755559573b4ecd618ff710686
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---

# Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Richtlinien für die Fehlerbehandlung

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Rollback</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>Die Ausführung des Szenarios wird sofort angehalten und eine <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Rollback</a> -Phase wird auf allen Modulen gestartet, um zu versuchen, alle Module in ihren ursprünglichen Zustand zurückzuversetzen. Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Außer einigen Fehlertypen wird das Szenario nach der Anzahl aufeinander folgender Fehler deaktiviert, die unter den Szenario-Einstellungen angegeben sind. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Anzahl aufeinander folgender Fehler</a>.</p> <p>Der Ausführungsstatus des Szenarios wird als "Fehler"markiert.</p> <p>Hinweis: Dies ist das Standardverhalten, wenn keine Fehler-Handler-Route an das -Modul und die <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Zulassen der Speicherung unvollständiger Ausführungen]</a> nicht unter [!UICONTROL Szenario-Einstellungen] aktiviert ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zusichern</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>Die Ausführung des Szenarios wird sofort gestoppt und für alle Module wird eine Commit-Phase gestartet. Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Alle nicht verarbeiteten Bundles werden ignoriert.</p> <p>Der Ausführungsstatus des Szenarios wird als "Erfolg"markiert. Weitere Informationen zu Commit-Phasen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Bestätigen</a> im Artikel <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Ausführung, Zyklen und Phasen eines Szenarios in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Fortsetzen</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Eine Ersatzausgabe wird angegeben und an das Modul geliefert, bei dem ein Fehler auftritt.</p> <p>Die nachfolgenden Module werden verarbeitet.</p> <p>Der Ausführungsstatus des Szenarios wird als "Erfolg"markiert.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorieren</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>Der Fehler wird ignoriert und die nachfolgenden Module werden nicht verarbeitet.</p> <p>Wenn es nicht verarbeitete Bundles gibt, wird das Szenario normal ausgeführt.</p> <p>Der Ausführungsstatus des Szenarios wird als "Erfolg"markiert.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Break</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>Der Ausführungsstatus des Szenarios wird in der Warteschlange unvollständiger Ausführungen gespeichert, wo der Fehler manuell behoben werden kann. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Unvollständige Ausführungen in Adobe Workfront Fusion anzeigen und auflösen</a>. </p> <p>Es gibt jedoch einige Ausnahmen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Speichern unvollständiger Ausführungen zulassen</a> im Artikel <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Das Bedienfeld "Szenario-Einstellungen"in Adobe Workfront Fusion</a>.</p> <p>Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Wenn es nicht verarbeitete Bundles gibt, wird das Szenario normal ausgeführt.</p> <p>Der Ausführungsstatus des Szenarios wird als "Warnung"markiert, wenn die Option [!UICONTROL Automatisch ausführen] deaktiviert ist.</p> <p>Siehe <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> für weitere Informationen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Erneut versuchen</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>In einigen Fällen kann es nützlich sein, ein fehlerhaftes Modul mehrmals erneut auszuführen, wenn die Wahrscheinlichkeit besteht, dass der Grund für den Fehler mit der Zeit vergeht.</p> <p>Workfront Fusion bietet derzeit keine Retry-Direktive, obwohl mehrere Workarounds verwendet werden können, um ihre Funktionalität zu imitieren. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Wiederholen der Fehlerbehandlung in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Derzeit können die Richtlinien zur Fehlerbehebung nicht außerhalb einer Fehlerbearbeitungsroute verwendet werden.
   >
   >   Weitere Informationen finden Sie unter [Fehler-Handler-Route](../../workfront-fusion/errors/error-handling.md#error) im Artikel [Umgang mit Fehlern in Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] bietet derzeit kein Throw-Modul an, mit dem Sie einfach bedingt Fehler (Auswerfen) generieren können, obwohl eine Problemumgehung verwendet werden kann, um die Funktionalität zu imitieren.
   >
   >   Weitere Informationen finden Sie unter [Problemumgehung für Throw](../../workfront-fusion/errors/throw.md#workaround-for-throw) im Artikel [Umgang mit Throw-Fehlern in Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).


## Break {#break}

Wenn ein Fehler von der [!DNL Break] -Anweisung, wird ein Datensatz im Ordner Unvollständige Ausführungen erstellt. Dieser Datensatz speichert den Ausführungsstatus des Szenarios zusammen mit Daten aus den vorherigen Modulen. Der Datensatz verweist auf das Modul, in dem der Fehler aufgetreten ist, und enthält Informationen darüber, welche Daten vom Modul als Eingabe empfangen wurden. Für jedes Datenbündel, das den Fehler verursacht, wird ein separater Datensatz erstellt.

Weitere Informationen finden Sie unter [Unvollständige Ausführungen in Adobe Workfront Fusion anzeigen und auflösen](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Beheben von Fehlern, die aus der Break-Richtlinie resultieren

Sie können den Fehler manuell beheben, indem Sie das Szenario (bei Bedarf) aktualisieren und es einmal ausführen.

Sie können das Szenario auch so konfigurieren, dass eine unvollständige Ausführung automatisch verarbeitet wird, indem Sie das Szenario erneut ausführen. So konfigurieren Sie das Modul für die Verarbeitung unvollständiger Ausführungen:

1. Aktivieren Sie innerhalb des Moduls Umbruch die [!UICONTROL **Automatische Ausführung**] -Option.
1. Im **Anzahl der Versuche** -Feld die maximale Anzahl von Versuchen eingeben oder zuordnen, bei denen das Modul die Ausführung erneut versuchen soll

   Diese Zahl muss zwischen 1 und 100 liegen.
1. Im **Intervall zwischen Versuchen** eingeben oder die Anzahl der Minuten zwischen den einzelnen Wiederholungsversuchen zuordnen.

Wenn diese Option aktiviert ist, wird bei einem Fehler die unvollständige Ausführung abgerufen (nach der in der Variablen [!UICONTROL Intervall zwischen Versuchen] -Feld) und mit den ursprünglichen Eingabedaten ausgeführt werden. Dieser Vorgang wiederholt sich, bis die Ausführung des Moduls ohne Fehler abgeschlossen ist oder die angegebene Anzahl von Versuchen erreicht ist.

>[!NOTE]
>
>Wenn der erste Wiederholungsversuch fehlschlägt, erhöht sich das Intervall zwischen Wiederholungen bei jedem zweiten Versuch exponentiell.


Wenn &quot;Ausführung automatisch abschließen&quot;aktiviert ist, wird die Ausführung des Szenarios als &quot;Erfolg&quot;markiert, da der automatische Wiederholungsversuch des Fehler-Handlers Break das Problem automatisch verarbeitet. In diesem Fall erhalten Benutzer keine E-Mail über die fehlgeschlagene Ausführung.

Wenn &quot;Ausführung automatisch abschließen&quot;deaktiviert ist, wird die Ausführung als &quot;Warnung&quot;markiert.

Es gibt einige Ausnahmen davon, dass Ausführungen unter &quot;Unvollständige Ausführungen&quot;gespeichert werden. Bei einigen Fehlertypen ist die automatische Wiederholung einer Szenario-Ausführung nicht möglich.

Weitere Informationen finden Sie unter [Speichern unvollständiger Ausführungen zulassen](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) im Artikel [Das Bedienfeld &quot;Szenario-Einstellungen&quot;in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Weitere Informationen finden Sie unter [Erweiterte Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
