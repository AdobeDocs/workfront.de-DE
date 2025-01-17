---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Zuordnen von Informationen von einem Modul zu einem anderen in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1628'
ht-degree: 0%

---

# Zuordnen von Informationen von einem Modul zu einem anderen in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Informationen von einem Modul einem anderen zuordnen](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-data-from-one-to-another.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Bei der Zuordnung werden die Ausgaben eines Moduls, strukturiert in Elemente, den Eingabefeldern eines anderen Moduls zugewiesen.

Das Zuordnungsbedienfeld wird angezeigt, wenn Sie auf ein Feld klicken, in das Sie einen Wert einfügen möchten, der von einem vorherigen Modul in einem Szenario ausgegeben wurde. Innerhalb eines Moduls können Sie in jedem Feld, das für die Zuordnung verfügbar ist, eine Formel erstellen, indem Sie eine beliebige Kombination aus Funktionen und zugeordneten Elementen aus dem Zuordnungsbereich mit von Ihnen eingegebenem statischem Text verwenden. Diese Elemente können ineinander geschachtelt werden.

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

## Bundles und Elemente

Der Betrieb eines Moduls erzeugt null, ein oder mehrere Bundles als Ausgabe. Ein Bundle besteht aus einem oder mehreren Elementen.

So untersuchen Sie die Ausgabe eines Moduls:

1. Klicken Sie auf **[!UICONTROL Einmal ausführen]**, um das Modul auszuführen.
1. Klicken Sie auf die Blase über dem Modul.

   Ein Protokoll mit allen Modulphasen wird angezeigt. Die von der Betriebsphase eines Moduls ausgegebenen Bundles finden Sie unter der Überschrift **[!UICONTROL Ausgabe]**. Jedes Bundle enthält seine Elemente und die Werte jedes Elements.

>[!INFO]
>
>**Beispiel:** Dieses Beispiel zeigt das Modul [!UICONTROL E-] > [!UICONTROL E-Mails ansehen]. Sie können sehen, dass 1 Vorgang ausgeführt wurde, bei dem ein einzelnes Bundle erstellt wurde, das verschiedene Elemente wie `Date`, `Email ID (UID)`, `size` usw. enthält.
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>Die Ausgaben von Modulen, die zwischen einem [!UICONTROL Iterator] und [!UICONTROL Aggregator] umschlossen sind, sind über das Modul [!UICONTROL Aggregator] hinaus nicht zugänglich.

## Zuordnen eines Elements

Nachdem Sie eine Sequenz von Modulen erstellt haben, indem Sie zwei oder mehr von ihnen verknüpft haben, kann jedes Modul Werte von Elementen verarbeiten, die von den Modulen ausgegeben werden, die ihm vorausgehen.

So weisen Sie die Elemente den Eingabefeldern eines Moduls zu:

1. Klicken Sie auf das Modul, das die Ausgabe des oder der vorhergehenden Module verarbeiten soll(en).
1. Klicken Sie im angezeigten Bedienfeld Moduleinstellungen auf ein Feld, in dem Sie den Wert eines Elements verwenden möchten, das von einem oder mehreren vorhergehenden Modulen ausgegeben wurde.

   Das Zuordnungsbedienfeld wird geöffnet.

1. Klicken Sie auf ein Element im Zuordnungsbereich, um es in das Feld einzufügen.
1. (Optional) Um nach einem bestimmten Feld im Zuordnungsbereich zu suchen, klicken Sie auf die Suchleiste des Zuordnungsbereichs und geben Sie den Begriff ein, nach dem Sie suchen möchten. Klicken Sie auf das Feld, wenn es in der Liste angezeigt wird.

   Suchergebnisse enthalten den Suchbegriff und unterscheiden nicht zwischen Groß- und Kleinschreibung.

Weitere Informationen finden Sie [Konfigurieren der Moduleinstellungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## Formeln

Sie können einem Feld mehrere Elemente zuordnen, sie mit Literalen (festen Werten) kombinieren und Operatoren und Funktionen verwenden, um komplexe Formeln zu erstellen:

![](assets/operators-and-functions.png)

Die Funktionen und Operatoren finden Sie im Bedienfeld Zuordnung auf einer der Registerkarten.

![](assets/functions-toolbar-350x189.png)

Die erste ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (die beim Öffnen des Bedienfelds angezeigt wird) zeigt die Elemente an, die Sie aus anderen Modulen zuordnen können.

Die anderen Registerkarten enthalten die folgenden Arten von Funktionen:

* **Allgemeine Funktionen** ![](assets/toolbar-icon-general-function.png) - Weitere Informationen finden [Allgemeine Funktionen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

* **Mathematische Funktionen** ![](assets/toolbar-icon-math-functions.png) - Weitere Informationen finden Sie [Mathematische Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md).

* **Text- und Binärfunktionen** ![](assets/toolbar-icon-text&binary-functions.png) - Weitere Informationen finden Sie unter [Zeichenfolgenfunktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md).

* **Datum und Uhrzeit** ![](assets/toolbar-icon-date&time-functions.png) - Weitere Informationen finden Sie [Datums- und  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) in und in den folgenden Artikeln.

   * [Token zur Formatierung von Datum und Uhrzeit in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token zum Analysieren von Datum und Uhrzeit in Adobe Workfront Fusion](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funktionen für die Arbeit mit Arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Weitere Informationen finden Sie unter [Array [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md)Funktionen in.

>[!TIP]
>
>Wenn Sie eine komplexe Formel erstellen, die Sie in einem anderen Feld wiederverwenden möchten, können Sie auf das Feld klicken, das die Kombination enthält, sie mit Befehl A oder Strg-A auswählen und dann kopieren und in das andere Feld einfügen.

Weitere Informationen zum Zuordnen von Elementen mithilfe von Funktionen finden Sie unter [Zuordnen von Elementen mithilfe von Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## Sammlungen

Einige Elemente können mehrere Werte verschiedener Typen enthalten. Hierbei handelt es sich um Sammlungstyp-Elemente.

Ein Element vom Typ [!UICONTROL Sammlung] können Sie anhand des kleinen schwarzen Rechtecks rechts neben der Beschriftung des Elements und seiner automatisch erweiterten Liste von Unterelementen identifizieren:

![](assets/collection.png)

>[!NOTE]
>
>In den meisten Fällen ordnen Sie die Unterelemente der Sammlung zu, anstatt das Element, das die gesamte Sammlung darstellt.

Weitere Informationen zu Sammlungen finden Sie unter [Elementdatentypen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

## Arrays

Einige Elemente können mehrere Elemente desselben Typs enthalten. Dies sind Elemente vom Typ Array.

Ein Element vom Typ Array kann durch die eckigen Klammern am Ende der Beschriftung des Elements identifiziert werden. Klicken Sie auf das kleine schwarze Rechteck rechts neben der Beschriftung des Elements, um die Elemente des Elements anzuzeigen:

![](assets/array.png)

Weitere Informationen zu Arrays finden Sie unter [Elementdatentypen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### Zuordnen des ersten Elements eines Arrays

Wenn Sie das `Recipient name` eines Arrays zuordnen, wird es wie folgt im Feld angezeigt:

![](assets/map-array-1st-element.png)

Die Zahl in den eckigen Klammern ist ein Index, der bestimmt, welches Element des Arrays verwendet wird. Standardmäßig ist dieser Wert auf 1 festgelegt.

### Zuordnen des n-ten Elements eines Arrays

Wenn Sie auf ein anderes Element zugreifen möchten, klicken Sie auf die eckigen Klammern und bearbeiten Sie den Indexwert:

![](assets/access-another-element.png)

### Ordnen Sie das Element eines Arrays einem bestimmten Schlüssel zu

Einige Arrays enthalten mehrere Sammlungen mit Schlüssel- und Wertelementen. Dabei handelt es sich normalerweise um verschiedene Metadaten, Attribute usw.

Das folgende Beispiel zeigt die Ausgabe der [!DNL Jira] App.

![](assets/output-of-jira-app-350x100.png)

In diesem Beispiel erhalten wir einen Dateinamen aus einem Array von Anlagen für den spezifischen Anhang mit der ID 10108.

Die Ausgabe von [!DNL Jira] sieht wie folgt aus:

![](assets/output-from-jira-350x261.png)

Die typische Anforderung besteht darin, ein Element anhand seines angegebenen Schlüsselwerts zu suchen und den entsprechenden Wert aus dem Wertelement abzurufen. Dies lässt sich durch eine Formel erreichen, die eine Kombination der `map()`- und `get()`-Funktionen verwendet.

Im Folgenden finden Sie eine detaillierte Aufschlüsselung der Formel:

1. Der erste Parameter der `map()` ist das gesamte Array-Element.
1. Der zweite Parameter ist der Rohname des Wertelements. Um den Rohnamen zu erhalten, bewegen Sie den Mauszeiger über das Element im Bedienfeld [!UICONTROL Zuordnung]:

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >Bei allen Parametern wird zwischen Groß- und Kleinschreibung unterschieden. Auch wenn sich die Beschriftung des Elements in diesem Beispiel nur in der Groß-/Kleinschreibung von seinem Rohnamen unterscheidet, muss der Rohname verwendet werden, bei dem es sich im Gegensatz zum Beschriftungswert um einen Wert in Kleinbuchstaben handelt.

1. Der dritte Parameter ist der Rohname des Schlüsselelements:

   ![](assets/3rd-parameter-350x166.png)

1. Der 4. Parameter ist der gegebene Schlüsselwert.

Da die Funktion `map()` ein Array zurückgibt (da mit dem angegebenen Schlüsselwert weitere Elemente vorhanden sein könnten), muss die Funktion `get()` angewendet werden, um das erste Element zu erhalten:

* Der 1. Parameter der `get()` ist das Ergebnis der `map()`.

* Der zweite Parameter ist der Index des Elements - eins.

Weitere Informationen zur `map()` finden Sie unter [Array-Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

Weitere Informationen zur `get()` finden Sie unter [Allgemeine Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## Konvertieren von Elementen in eine Reihe von Bundles

Arrays können mithilfe des Moduls [!UICONTROL Iterator“ in eine Reihe von Bundles ] werden. Weitere Informationen finden Sie [[!UICONTROL  Modul „Iterator] in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## Fehlerbehebung

### Fehlende Elemente im Zuordnungsbereich

Im Zuordnungsbereich werden für jedes Modul alle Ausgabeelemente angezeigt, die vom Autor des Moduls aufgelistet sind. In einigen Fällen kann diese Liste aus verschiedenen Gründen unvollständig sein, und einige Elemente fehlen möglicherweise. [!DNL Workfront Fusion] können die fehlenden Ausgabeelemente automatisch erkennen, wenn Sie das Modul im Szenario-Editor ausführen. Die genaue Vorgehensweise unterscheidet sich je nach Modultyp geringfügig:

#### Sofortiger Trigger

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie **[!UICONTROL Nur dieses Modul ausführen]** in dem angezeigten Menü.

   Wenn keine Webhooks in der Warteschlange vorhanden sind, wartet das Modul auf die Verarbeitung eines neuen Webhooks.

1. Erstellen eines Webhooks.

   Beispielsweise sendet das Webhook-Modul **[!DNL Slack]>[!UICONTROL Auf neue Ereignisse]** wartet auf neue Kanalnachrichten in einem Kanal) eine Nachricht an den Kanal.

1. Wenn das Modul fertig ausgeführt wird, klicken Sie auf die Blase über dem Modul, um die vollständige Ausgabe zu überprüfen.

   Das Zuordnungsbedienfeld enthält alle Elemente, die in der Modulausgabe gefunden wurden.

#### Trigger wird abgerufen

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie **[!UICONTROL Nur dieses Modul ausführen]** in dem angezeigten Menü.
1. Wenn keine Ausgabe vorhanden ist, klicken Sie auf **[!UICONTROL Startpunkt auswählen]** und passen Sie die Einstellungen an.
1. Wenn kein zu verarbeitendes Ereignis vorhanden ist, erstellen Sie ein Ereignis und fahren Sie mit Schritt 2 fort.

   Beispielsweise sendet das Webhook-Modul **[!UICONTROL Gmail] > [!UICONTROL E-Mails]**) eine E-Mail an den Ordner, den das Modul beobachtet.

1. Wenn das Modul fertig ausgeführt wird, klicken Sie auf die Blase über dem Modul, um die vollständige Ausgabe zu überprüfen.

   Das Zuordnungsbedienfeld enthält jetzt alle Elemente, die in der -Ausgabe des Moduls gefunden wurden.

#### Andere Module

Sie können Folgendes ausführen:

* Das gesamte Szenario (oder nur der Teil, der das Modul enthält)

  Wenn Ihr Szenario mit einem Trigger beginnt, lesen Sie den Abschnitt [Sofortiger Trigger ](#instant-trigger) oder [Abruf-Trigger ](#polling-trigger) weiter oben.

* Nur das einzelne Modul

Wenn Sie nur das einzelne Modul ausführen:

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie **[!UICONTROL Nur dieses Modul ausführen]** in dem angezeigten Menü auf..
1. Geben Sie Beispielwerte für die Eingabeelemente ein und klicken Sie dann auf **[!UICONTROL OK]** .
1. Wenn das Modul fertig ausgeführt wird, klicken Sie auf die Blase über dem Modul, um die vollständige Ausgabe zu überprüfen.

   Das Zuordnungsbedienfeld enthält jetzt alle Elemente, die in der -Ausgabe des Moduls gefunden wurden.
