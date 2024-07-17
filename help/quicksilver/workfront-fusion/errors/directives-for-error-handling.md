---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Richtlinien für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]
description: In diesem Artikel werden Richtlinien beschrieben, die Sie für die Fehlerbehandlung in Ihren [!DNL Adobe Workfront Fusion] Szenarien verwenden können.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 12%

---

# Richtlinien für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
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

## Richtlinien für die Fehlerbehandlung

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Rollback</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>Die Ausführung des Szenarios wird sofort angehalten und eine <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Rollback</a> -Phase wird für alle Module gestartet, um zu versuchen, alle Module wieder in ihren ursprünglichen Zustand zu versetzen. Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Außer einigen Fehlertypen wird das Szenario nach der Anzahl aufeinander folgender Fehler deaktiviert, die unter den Szenario-Einstellungen angegeben sind. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Anzahl aufeinander folgender Fehler</a>.</p> <p>Der Status der Szenarioausführung ist als „Fehler“ gekennzeichnet.</p> <p>Hinweis: Dies ist das Standardverhalten, wenn keine Fehler-Handler-Route an das Modul angehängt ist und die Einstellung <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Zulassen, dass unvollständige Ausführungen gespeichert werden]</a> unter [!UICONTROL Szenario-Einstellungen] nicht aktiviert ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zusichern</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>Die Ausführung des Szenarios wird sofort gestoppt und für alle Module wird eine Commit-Phase gestartet. Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Alle nicht verarbeiteten Bundles werden ignoriert.</p> <p>Der Ausführungsstatus des Szenarios wird als "Erfolg"markiert. Weitere Informationen zu Commitphasen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Bestätigen</a> im Artikel <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Ausführung, Zyklen und Phasen eines Szenarios in Adobe Workfront Fusion</a>.</p> </td> 
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
   <td> <p>Der Zustand der Szenarioausführung wird in der Warteschlange für unvollständige Ausführungen gespeichert, wo der Fehler manuell behoben werden kann. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Anzeigen und Auflösen unvollständiger Ausführungen in Adobe Workfront Fusion</a>. </p> <p>Es gibt jedoch einige Ausnahmen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Speichern unvollständiger Ausführungen zulassen</a> im Artikel <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Das Bedienfeld mit den Szenario-Einstellungen in Adobe Workfront Fusion zulassen</a>.</p> <p>Die nachfolgenden Module werden nicht verarbeitet.</p> <p>Wenn unbearbeitete Bündel vorhanden sind, wird die Ausführung des Szenarios normal fortgesetzt.</p> <p>Der Ausführungsstatus des Szenarios wird als "Warnung"markiert, wenn die Option [!UICONTROL Automatisch ausführen] deaktiviert ist.</p> <p>Weitere Informationen finden Sie unten im Abschnitt <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Erneut versuchen</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>In einigen Fällen kann es nützlich sein, ein fehlerhaftes Modul mehrmals erneut auszuführen, wenn die Wahrscheinlichkeit besteht, dass der Grund für den Fehler mit der Zeit vergeht.</p> <p>Workfront Fusion bietet derzeit keine Retry-Direktive, obwohl mehrere Workarounds verwendet werden können, um ihre Funktionalität zu imitieren. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Fehlerbehandlung in Adobe Workfront Fusion wiederholen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Derzeit können die Richtlinien zur Fehlerbehebung nicht außerhalb einer Fehlerbearbeitungsroute verwendet werden.
>
>   Weitere Informationen finden Sie unter [Fehler-Handler-Route](../../workfront-fusion/errors/error-handling.md#error) im Artikel [Umgang mit Fehlern in Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] bietet derzeit kein Throw-Modul, mit dem Sie einfach bedingt Fehler (Auswerfen) generieren können, obwohl eine Problemumgehung verwendet werden kann, um die Funktionalität zu imitieren.
>
>   Weitere Informationen finden Sie unter [Problemumgehung für Throw](../../workfront-fusion/errors/throw.md#workaround-for-throw) im Artikel [Umgang mit Throw-Fehlern in Adobe Workfront Fusion verarbeiten](../../workfront-fusion/errors/throw.md).

## Unterbrechen {#break}

Wenn ein Fehler von der Anweisung [!DNL Break] verarbeitet wird, wird ein Datensatz im Ordner Unvollständige Ausführungen erstellt. Dieser Datensatz speichert den Ausführungsstatus des Szenarios zusammen mit Daten aus den vorherigen Modulen. Der Datensatz verweist auf das Modul, in dem der Fehler aufgetreten ist, und enthält Informationen darüber, welche Daten vom Modul als Eingabe empfangen wurden. Für jedes Datenbündel, das den Fehler verursacht, wird ein separater Datensatz erstellt.

Weitere Informationen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Beheben von Fehlern, die aus der Break-Richtlinie resultieren

Sie können den Fehler manuell beheben, indem Sie das Szenario (bei Bedarf) aktualisieren und es einmal ausführen.

Sie können das Szenario auch so konfigurieren, dass eine unvollständige Ausführung automatisch verarbeitet wird, indem Sie das Szenario erneut ausführen. So konfigurieren Sie das Modul für die Verarbeitung unvollständiger Ausführungen:

1. Aktivieren Sie im Modul Umbruch die Option [!UICONTROL **Ausführung automatisch abschließen**] .
1. Geben Sie im Feld **Anzahl der Versuche** die maximale Anzahl von Versuchen ein, die das Modul zur erneuten Ausführung ausführen soll.

   Diese Zahl muss zwischen 1 und 100 liegen.
1. Geben Sie im Feld **Intervall zwischen Versuchen** die Anzahl der Minuten zwischen jedem Wiederholungsversuch ein oder ordnen Sie sie zu.

Wenn diese Option aktiviert ist, wird bei einem Fehler die unvollständige Ausführung abgerufen (nach der im Feld [!UICONTROL Intervall zwischen Versuchen] angegebenen Zeit) und mit den ursprünglichen Eingabedaten ausgeführt. Dieser Vorgang wiederholt sich, bis die Ausführung des Moduls ohne Fehler abgeschlossen ist oder die angegebene Anzahl von Versuchen erreicht ist.

>[!NOTE]
>
>Wenn der erste Wiederholungsversuch fehlschlägt, erhöht sich das Intervall zwischen Wiederholungen bei jedem zweiten Versuch exponentiell.


Wenn &quot;Ausführung automatisch abschließen&quot;aktiviert ist, wird die Ausführung des Szenarios als &quot;Erfolg&quot;markiert, da der automatische Wiederholungsversuch des Fehler-Handlers Break das Problem automatisch verarbeitet. In diesem Fall erhalten Benutzer keine E-Mail über die fehlgeschlagene Ausführung.

Wenn &quot;Ausführung automatisch abschließen&quot;deaktiviert ist, wird die Ausführung als &quot;Warnung&quot;markiert.

Es gibt einige Ausnahmen davon, dass Ausführungen unter &quot;Unvollständige Ausführungen&quot;gespeichert werden. Bei einigen Fehlertypen ist die automatische Wiederholung einer Szenario-Ausführung nicht möglich.

Weitere Informationen finden Sie unter [Speichern unvollständiger Ausführungen zulassen](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) im Artikel [Das Bedienfeld mit den Szenario-Einstellungen in Adobe Workfront Fusion zulassen](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Weitere Informationen finden Sie unter [Erweiterte Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
