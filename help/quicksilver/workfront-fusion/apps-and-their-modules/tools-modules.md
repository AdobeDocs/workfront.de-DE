---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Instrumente
description: Die [!DNL Adobe Workfront Fusion Tools] enthält mehrere nützliche Module, die Ihr Szenario verbessern können.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2290'
ht-degree: 0%

---

# [!UICONTROL Instrumente]

Die [!DNL Adobe Workfront Fusion Tools] enthält mehrere nützliche Module, die Ihr Szenario verbessern können.

[!UICONTROL Instrumente] -Module sind in der Liste der Apps verfügbar oder über die [!UICONTROL Instrumente] icon ![](assets/tools-icon-small.png) unten auf dem Bildschirm.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
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

## [!UICONTROL Instrumente] und ihre Felder

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Aggregatoren](#aggregators)
* [Transformatoren](#transformers)

### Trigger

#### [!UICONTROL Grundlegender Trigger]

Mit diesem Modul können Sie einen benutzerdefinierten Trigger erstellen und dessen Eingabepakete definieren.

Sie können dieses Modul beispielsweise für Kontakte oder andere Listen verwenden, die an eine bestimmte E-Mail-Adresse gesendet werden sollen (z. B. [!UICONTROL Email] >[!UICONTROL E-Mail senden]oder [!DNL Gmail] >[!UICONTROL E-Mail senden] -Module) oder als einfache Erinnerung, die ausgelöst werden soll, wann immer Sie möchten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>Erstellen Sie benutzerdefinierte Bundles, indem Sie Array-Elemente hinzufügen. Das Array besteht aus den Paaren name - Wert .</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Abrufen mehrerer Variablen]](#get-multiple-variables)
* [[!UICONTROL Variable abrufen]](#get-variable)
* [[!UICONTROL Inkrementierungsfunktion]](#increment-function)
* [[!UICONTROL Mehrere Variablen festlegen]](#set-multiple-variables)
* [[!UICONTROL Variable festlegen]](#set-variable)
* [[!UICONTROL Schlafen]](#sleep)

#### [!UICONTROL Abrufen mehrerer Variablen]

Dieses Modul ruft Werte ab, die zuvor von der [!UICONTROL Variable festlegen] oder [!UICONTROL Mehrere Variablen festlegen] -Modul.

Dieses Modul kann Variablen lesen, die an einer beliebigen Stelle im Szenario festgelegt wurden, selbst wenn die Variable auf einer anderen Route als der festgelegt wurde, auf der die [!UICONTROL Abrufen mehrerer Variablen] -Modul befindet. Die einzige Voraussetzung ist, dass die [!UICONTROL Instrumente] > [!UICONTROL Variable festlegen] oder [!UICONTROL Instrumente] > [!UICONTROL Mehrere Variablen festlegen] -Modul vor dem [!UICONTROL Instrumente] > [!UICONTROL Abrufen mehrerer Variablen] -Modul. Weitere Informationen zur Reihenfolge, in der Module ausgeführt werden, finden Sie unter [Router-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variablen]</td>
        <td>Fügen Sie die Variablen hinzu, die das Modul abrufen soll.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Variablenname]</td>
        <td>Ordnen Sie für jede hinzugefügte Variable den Namen der Variablen zu, die Sie abrufen möchten.</td>
    </tr>
</table>

>[!INFO]
>
>**Beispiele:**  Die folgenden Verwendungsmöglichkeiten sind möglich: [!UICONTROL Satz]/[!UICONTROL Abrufen (mehrerer) Variablen] -Module:
>
>* So speichern Sie einen berechneten Wert für die spätere Verwendung, auch in einer anderen Route. Dies ist in Fällen nützlich, in denen der Wert in mehreren Modulen verwendet wird und die Formel zur Berechnung des Werts zu komplex ist.
>* So debuggen Sie eine Formel. Wenn eine in einem Modul verwendete Formel anscheinend kein korrektes Ergebnis liefert, kopieren Sie die Formel und fügen Sie sie in ein [!UICONTROL Variable festlegen] -Modul, das Sie vor dem entsprechenden Modul einfügen. Trennen Sie die Module nach der [!UICONTROL Variable festlegen] und führen Sie das Szenario aus. Überprüfen Sie die [!UICONTROL Variable festlegen] die Ausgabe, Anpassung oder Vereinfachung der Formel des Moduls, wiederholte Ausführung des Szenarios und Fortsetzung des Vorgangs, bis das Problem behoben wurde.


#### [!UICONTROL Variable abrufen]

Dieses Modul ruft einen Wert ab, der zuvor vom [!UICONTROL Variable festlegen] oder [!UICONTROL Mehrere Variablen festlegen] -Modul.

Dieses Modul kann Variablen lesen, die an einer beliebigen Stelle im Szenario festgelegt wurden, selbst wenn die Variable auf einer anderen Route als der festgelegt wurde, auf der die [!UICONTROL Variable abrufen] -Modul befindet. Die einzige Voraussetzung ist, dass die [!UICONTROL Instrumente] > [!UICONTROL Variable festlegen] oder [!UICONTROL Instrumente] > [!UICONTROL Mehrere Variablen festlegen] -Modul vor dem [!UICONTROL Instrumente] > [!UICONTROL Variable abrufen] -Modul. Weitere Informationen zur Reihenfolge, in der Module ausgeführt werden, finden Sie unter [Router-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variablenname]</td> 
   <td> <p>Ordnen Sie den Namen der Variablen zu, die das Modul abrufen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inkrementierungsfunktion]

Dieses Modul gibt einen Wert zurück, der nach dem Vorgang jedes Moduls um 1 inkrementiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wert zurücksetzen]</td> 
   <td> <p>Wählen Sie aus, wann das Modul den Wert erhöhen soll. </p> 
    <ul> 
     <li>[!UICONTROL Nach einem Zyklus]</li> 
     <li>[!UICONTROL Nach einem Szenario ausführen]</li> 
     <li>[!UICONTROL Nie]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:**
>
>Eine der Verwendungsmöglichkeiten des Moduls besteht darin, eine &quot;Round Robin&quot;-Zuweisung von Aufgaben, Leads, E-Mails usw. zu Benutzern in einer Gruppe zu implementieren. Der Algorithmus wählt die Bevollmächtigten einer Gruppe in einer rationalen Reihenfolge aus, die normalerweise von oben nach unten verläuft. Wenn der Algorithmus das Ende der Liste erreicht, wird dem Benutzer die nächste Zuweisung dann oben in der Liste zugewiesen und die Zuweisungen in der Liste fortgesetzt.
>
>Im folgenden Szenario wird nach jedem ungeraden Szenario eine E-Mail an den ersten Empfänger und nach jedem geraden Szenario an den zweiten Empfänger gesendet.
>
>![](assets/example-email-350x246.gif)
>
>1. So erstellen Sie dieses Szenario:
>1. Legen Sie die **[!UICONTROL Wert zurücksetzen]** auf &quot;Nie&quot;gesetzt.
>1. Legen Sie die Route für ungerade Werte fest. Legen Sie den Filter für diese Route mithilfe der Modulus-Mathematikfunktion fest, die `1`:
>
>   ![](assets/odd-350x459.png)
>
>  **Hinweis**: Vergessen Sie nicht, die [!UICONTROL Gleich] -Operator aus der Standardeinstellung [!UICONTROL Text] dem [!UICONTROL Numerisch] Operator.
>
>1. Legen Sie die Route für Gleichheitswerte mit der Modulus-mathematischen Funktion fest, die gleich `0`:
>
>Die inkrementelle Funktion fügt jedes Mal, wenn das Szenario ausgeführt wird, einmal hinzu. Die Filter prüfen die Inkrementierung und beeinflussen den Wert, sodass E-Mails gleichmäßig verteilt werden.

#### [!UICONTROL Mehrere Variablen festlegen]

Dieses Modul erstellt Variablen, die von anderen Modulen in der Route zugeordnet werden können. Die Variable kann auch der Variablen [!UICONTROL Variable abrufen] oder [!UICONTROL Abrufen mehrerer Variablen] -Module für jede Route im Szenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variablen]</td> 
   <td>Fügen Sie die Variablen hinzu, die das Modul festlegen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variablenname] </td> 
   <td>Geben Sie für jede Variable den Variablennamen ein. Dieser Name wird angezeigt, wenn die Variable in anderen Modulen zugeordnet wird. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variablenwert] </td> 
   <td>Geben Sie für jede Variable den Wert für die Variable ein. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variablenlebensdauer] </td> 
   <td> <p>Wählen Sie aus, wie lange die Variablen gültig bleiben sollen (den gleichen Wert beibehalten).</p> 
    <ul> 
     <li><strong>[!UICONTROL Ein Zyklus]</strong>: Die Variable ist für einen Zyklus gültig. Nützlich, wenn mehrere Webhooks in einem Szenario empfangen werden (mehr Webhooks = mehr Zyklen). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: Die -Variable ist für die Ausführung eines Szenarios gültig. Eine Ausführung kann einen oder mehrere Zyklen enthalten.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Variable festlegen]

Dieses Modul erstellt eine Variable, die von anderen Modulen in der Route zugeordnet werden kann. Die Variable kann auch der Variablen [!UICONTROL Variable abrufen] oder [!UICONTROL Abrufen mehrerer Variablen] -Module für jede Route im Szenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variablenname] </td> 
   <td>Geben Sie den Variablennamen ein. Dieser Name wird angezeigt, wenn die Variable in anderen Modulen zugeordnet wird. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variablenlebensdauer] </td> 
   <td> <p>Wählen Sie aus, wie lange die Variablen gültig bleiben sollen (den gleichen Wert beibehalten).</p> 
    <ul> 
     <li><strong>[!UICONTROL Ein Zyklus]</strong>: Die Variable ist für einen Zyklus gültig. Nützlich, wenn mehrere Webhooks in einem Szenario empfangen werden (mehr Webhooks = mehr Zyklen). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: Die -Variable ist für die Ausführung eines Szenarios gültig. Eine Ausführung kann einen oder mehrere Zyklen enthalten.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variablenwert] </td> 
   <td>Geben Sie den Wert für die Variable ein oder ordnen Sie ihn zu. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Schlafen]

Mit diesem Modul können Sie den Szenario-Fluss für bis zu 300 Sekunden (5 Minuten) verzögern.

Diese Funktion kann nützlich sein, wenn Sie beispielsweise die Variable [!DNL target] Laden des Dienstservers oder , um menschliches Verhalten beim Senden von Massen-SMS oder E-Mails zu imitieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Verzögerung]</p> </td> 
   <td> <p>Geben Sie an, wie viele Sekunden das Szenario angehalten werden soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Wenn Sie den Fluss für längere Zeiträume anhalten möchten, empfehlen wir, Ihr Szenario in zwei Szenarien zu unterteilen:
>
>* Das erste Szenario würde den Teil vor der Pause enthalten.
>* Das zweite Szenario würde den folgenden Teil enthalten.
>
>Das erste Szenario führt dazu, dass alle erforderlichen Informationen zusammen mit dem aktuellen Zeitstempel in einem Datenspeicher gespeichert werden. Das zweite Szenario würde den Datenspeicher regelmäßig auf Datensätze mit einem Zeitstempel überprüfen, der der vorgesehenen Verzögerung entspricht, die Datensätze abrufen, die Datenverarbeitung abschließen und die Datensätze aus dem Datenspeicher entfernen.
>
>Weitere Informationen zu Datenspeichern finden Sie unter [Datenspeicher in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>Weitere Informationen zu bestimmten Datenspeichermodulen finden Sie unter [[!UICONTROL Datenspeicher] Module](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Aggregatoren

* [[!UICONTROL Numerischer Aggregator]](#numeric-aggregator)
* [[!UICONTROL Tabellenaggregator]](#table-aggregator)
* [[!UICONTROL Textaggregator]](#text-aggregator)

#### [!UICONTROL Numerischer Aggregator]

Mit diesem Modul können Sie numerische Werte abrufen, dann eine der ausgewählten Funktionen (SUM, AVG, COUNT, MAX, MIN) anwenden und das Ergebnis in einem Bundle zurückgeben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Quellmodul]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, aus dem die Felder aggregiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Aggregate function]</p> </td> 
   <td> <p>Wählen Sie die Funktion aus, mit der die Werte aggregiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Gruppe nach]</p> </td> 
   <td> <p>Definieren Sie einen Ausdruck, nach dem Sie die aggregierte Ausgabe gruppieren möchten. Dieser Ausdruck kann ein oder mehrere zugeordnete Elemente enthalten. Die aggregierten Daten werden dann mithilfe des Werts dieses Ausdrucks in Gruppen unterteilt. Jede Gruppe gibt als separates Bundle mit einem Schlüssel (dem ausgewerteten Ausdruck) und einem Wert (dem aggregierten Wert) aus. Sie können den Schlüssel als Filter in nachfolgenden Modulen verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen]</td> 
   <td>Aktivieren Sie diese Option, um das Szenario zu stoppen, wenn keine Ergebnisse vorliegen.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Wert]</p> </td> 
   <td> <p>Geben Sie den zu aggregierenden Wert ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tabellenaggregator]

Dieses Modul führt Werte aus den ausgewählten Feldern empfangener Bundles mithilfe einer angegebenen Spalten- und Zeilentrennzeichen in einem Bundle zusammen (mit dem Sie eine Tabelle erstellen können).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Quellmodul]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, aus dem die Felder aggregiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregierte Felder]</td> 
   <td> <p> Wählen Sie die Felder aus dem oben ausgewählten Modul aus, die die Werte enthalten, die Sie in einem Bundle aggregieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Spaltentrennzeichen]</p> </td> 
   <td> <p>Wählen Sie den Trennzeichentyp aus oder geben Sie ihn ein, der die Feldwertspalten im resultierenden Bundle trennt. Wenn Sie [!UICONTROL Sonstige] auswählen, geben Sie das Zeichen ein, das Sie zum Trennen von Werten in das Trennzeichenfeld verwenden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Zeilentrennzeichen]</p> </td> 
   <td> <p>Wählen Sie den Trennzeichentyp aus oder geben Sie ihn ein, der die Feldwertzeilen im resultierenden Bundle trennt. Wenn Sie [!UICONTROL Sonstige] auswählen, geben Sie das Zeichen ein, das Sie zum Trennen von Werten in das Trennzeichenfeld verwenden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Gruppe nach]</p> </td> 
   <td> <p>Definieren Sie einen Ausdruck, nach dem Sie die aggregierte Ausgabe gruppieren möchten. Dieser Ausdruck kann ein oder mehrere zugeordnete Elemente enthalten. Die aggregierten Daten werden dann mithilfe des Werts dieses Ausdrucks in Gruppen unterteilt. Jede Gruppe gibt als separates Bundle mit einem Schlüssel (dem ausgewerteten Ausdruck) und einem Wert (dem aggregierten Wert) aus. Sie können den Schlüssel als Filter in nachfolgenden Modulen verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen]</td> 
   <td>Wählen Sie diese Option, um das Szenario zu stoppen, wenn keine Ergebnisse vorliegen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Textaggregator]

Dieses Modul führt Werte aus den ausgewählten Feldern empfangener Bundles zu einem Bundle zusammen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Quellmodul]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, aus dem die Felder aggregiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Zeilentrennzeichen]</p> </td> 
   <td> <p>Wählen Sie den Trennzeichentyp aus oder geben Sie ihn ein, der die Feldwertzeilen im resultierenden Bundle trennt. Wenn Sie [!UICONTROL Sonstige] auswählen, geben Sie das Zeichen ein, das Sie zum Trennen von Werten in das Trennzeichenfeld verwenden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Gruppe nach]</p> </td> 
   <td> <p>Definieren Sie einen Ausdruck, der ein oder mehrere zugeordnete Elemente enthält. Die aggregierten Daten werden unter Gruppen mit demselben Ausdruckswert getrennt. Jede Gruppe gibt als separates Bundle aus, das einen Schlüssel mit dem ausgewerteten Ausdruck und dem aggregierten Text enthält. Auf diese Weise können Sie den Schlüssel als Filter in nachfolgenden Modulen verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text]</td> 
   <td> <p> Geben Sie den Text ein oder ordnen Sie ihn zu, den das Modul aggregieren soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verarbeitung nach einer leeren Aggregation stoppen]</td> 
   <td>Wählen Sie diese Option, um das Szenario zu stoppen, wenn keine Ergebnisse vorliegen.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Sie können den Text-Aggregator verwenden, um weitere Werte (z. B. Kundennamen oder Hinweise) in ein einzelnes Bundle einzufügen und eine E-Mail mit allen Werten im E-Mail-Textkörper oder im E-Mail-Betreff zu senden.

### Transformatoren

* [[!UICONTROL Erstellen einer Zeichenfolge]](#compose-a-string)
* [[!UICONTROL Konvertieren der Textkodierung]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Switch]](#switch)

#### [!UICONTROL Erstellen einer Zeichenfolge]

Konvertiert einen beliebigen Wert in einen String-Datentyp (Text). Dies erleichtert die Zuordnung, beispielsweise Binärdaten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p>Geben Sie die Daten ein oder ordnen Sie sie zu, die in Text konvertiert werden sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Konvertieren der Textkodierung]

Konvertiert eingegebenen Text (oder Binärdaten) in die ausgewählte Kodierung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Eingabedaten]</p> </td> 
   <td> <p>Geben Sie den zu konvertierenden Inhalt ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Input data codepage]</td> 
   <td> <p>Wählen Sie den Kodierungstyp der Eingabedaten aus. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Output data codepage]</p> </td> 
   <td> <p>Wählen Sie den Kodierungstyp Ihrer Zieldaten (Ausgabedaten) aus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Switch]

Überprüft den Eingabewert auf Übereinstimmung mit der bereitgestellten Werteliste. Gibt die Ausgabe basierend auf dem Ergebnis zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>Geben Sie den auszuwertenden Ausdruck ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verwenden regulärer Ausdrücke zur Übereinstimmung]</td> 
   <td> <p>Aktivieren Sie diese Option, um reguläre Ausdrücke zu verwenden. Das Modul bestimmt die Fälle anhand des regulären Ausdrucks und nicht anhand einer exakten Übereinstimmung.</p> 
    <div> 
     <p>Ein regulärer Ausdruck ist eine Folge von Zeichen, bei denen jedes Zeichen ein Metazeichen mit einer besonderen Bedeutung oder ein reguläres Zeichen mit einer literalen Bedeutung ist. Diese Zeichen und Metazeichen identifizieren ein Muster, das für die Suche nach Text verwendet werden kann. Wenn Sie beispielsweise nach Namen suchen möchten, können Sie einen regulären Ausdruck einrichten, um nach einem Muster zu suchen, das aus zwei aufeinander folgenden Wörtern besteht, die mit Großbuchstaben beginnen. Reguläre Ausdrücke sind ein leistungsstarkes Werkzeug zum Durchsuchen und Bearbeiten von Text.</p> 
     <p>Eine Diskussion über reguläre Ausdrücke geht über den Rahmen dieses Artikels hinaus. Wir empfehlen die folgenden Ressourcen:</p> 
     <ul> 
      <li>Eine vollständige Liste der Metazeichen finden Sie unter <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Reguläre Ausdrücke</a> in MDN-Webdocs.</li> 
      <li>Für ein Tutorial zum Erstellen regulärer Ausdrücke empfehlen wir, <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>Für das Experimentieren mit regulären Ausdrücken empfehlen wir die <a href="https://regex101.com/">Reguläre Ausdrücke 101</a> Website. Wählen Sie im linken Bereich den ECMAScript (JavaScript)-FLAVOR aus.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fälle] </td> 
   <td> <p>Wenn die Eingabe einen im Feld [!UICONTROL Pattern] eingegebenen Wert enthält, wird der im Feld [!UICONTROL Output] eingegebene Wert zurückgegeben.</p> <p>Wenn die Eingabe keinem der Werte entspricht, die Sie in einem [!UICONTROL Muster]-Feld festgelegt haben, tritt einer der folgenden Fälle auf:</p> 
    <ul> 
     <li>Der Wert aus dem Feld [!UICONTROL Else] wird zurückgegeben</li> 
     <li>Wenn im Feld [!UICONTROL Else] kein Wert vorhanden ist, wird keine Ausgabe zurückgegeben.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Geben Sie den Wert ein, der zurückgegeben wird, wenn die im Feld Fälle festgelegten Kriterien nicht erfüllt sind. </p> </td> 
  </tr> 
 </tbody> 
</table>
