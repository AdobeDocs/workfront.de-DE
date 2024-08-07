---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Ordnen Sie Informationen von einem Modul zum anderen in [!DNL Adobe Workfront Fusion] zu.
description: Bei der Zuordnung werden die Ausgaben eines Moduls, strukturiert in Elemente, den Eingabefeldern eines anderen Moduls zugewiesen.
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 3772223938008e3a54ce0a48aaae1f3edb5bf252
workflow-type: tm+mt
source-wordcount: '1567'
ht-degree: 0%

---

# Informationen von einem Modul in [!DNL Adobe Workfront Fusion] einem anderen zuordnen

Bei der Zuordnung werden die Ausgaben eines Moduls, strukturiert in Elemente, den Eingabefeldern eines anderen Moduls zugewiesen.

Das Zuordnungsbedienfeld wird angezeigt, wenn Sie auf ein Feld klicken, in das Sie einen aus einem vorherigen Modul ausgegebenen Wert in ein Szenario einfügen möchten. Innerhalb eines Moduls können Sie in jedem Feld, das für die Zuordnung verfügbar ist, eine Formel erstellen, indem Sie eine beliebige Kombination von Funktionen und zugeordneten Elementen aus dem Zuordnungsbereich mit statischem Text verwenden, den Sie eingeben. Diese Elemente können ineinander verschachtelt werden.

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

## Bundles und Artikel

Der Betrieb eines Moduls erzeugt null, eins oder mehrere Pakete als Ausgabe. Ein Bundle besteht aus einem oder mehreren Elementen.

So untersuchen Sie die Ausgabe eines Moduls:

1. Klicken Sie auf **[!UICONTROL Einmal ausführen]** , um das Modul auszuführen.
1. Klicken Sie auf die Blase über dem Modul.

   Ein Protokoll mit allen Modulphasen wird angezeigt. Sie finden das von der Betriebsphase eines Moduls ausgegebene Bundle oder Bundles unter der Überschrift **[!UICONTROL Ausgabe]** . Jedes Bundle enthält seine Elemente und die Werte jedes Elements.

>[!INFO]
>
>**Beispiel:** Dieses Beispiel zeigt das Modul [!UICONTROL E-Mail] > [!UICONTROL E-Mails ansehen]. Sie können sehen, dass es einen Vorgang ausgeführt hat, der ein einzelnes Bundle generiert hat, das verschiedene Elemente wie `Date`, `Email ID (UID)`, `size` usw. enthält.
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>Die Ausgaben aus Modulen, die zwischen einem [!UICONTROL Iterator] und [!UICONTROL Aggregator] eingeschlossen sind, sind über das Modul [!UICONTROL Aggregator] hinaus nicht zugänglich.

## Element zuordnen

Nachdem Sie eine Folge von Modulen erstellt haben, indem Sie zwei oder mehr von ihnen verknüpft haben, kann jedes Modul Werte von Elementen verarbeiten, die von den davor stehenden Modulen ausgegeben werden.

So weisen Sie die Elemente den Eingabefeldern eines Moduls zu:

1. Klicken Sie auf das Modul, das die Ausgabe des vorherigen Moduls bzw. der vorherigen Module verarbeiten soll.
1. Klicken Sie im angezeigten Bedienfeld Moduleinstellungen auf ein Feld, in dem Sie den Wert eines Elements verwenden möchten, das aus einem oder mehreren vorhergehenden Modul(en) ausgegeben wurde.

   Das Zuordnungsfenster wird geöffnet.

1. Klicken Sie auf ein Element im Zuordnungsbereich, um es in das Feld einzufügen.
1. (Optional) Um im Zuordnungsbereich nach einem bestimmten Feld zu suchen, klicken Sie auf die Suchleiste des Zuordnungsbereichs und geben Sie den Begriff ein, nach dem Sie suchen möchten. Klicken Sie auf das Feld, wenn es in der Liste angezeigt wird.

   Suchergebnisse enthalten den Suchbegriff und unterscheiden nicht zwischen Groß- und Kleinschreibung.

Weitere Informationen finden Sie unter [Konfigurieren der Einstellungen eines Moduls in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## Formeln

Sie können mehrere Elemente in einem Feld zuordnen, sie mit Literalen (festen Werten) kombinieren und mithilfe von Operatoren und Funktionen komplexe Formeln erstellen:

![](assets/operators-and-functions.png)

Die Funktionen und Operatoren finden Sie im Zuordnungsfenster unter einem seiner Registerkarten.

![](assets/functions-toolbar-350x189.png)

Auf der ersten Registerkarte ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (die beim Öffnen des Bedienfelds angezeigt wird) werden die Elemente angezeigt, die Sie aus anderen Modulen zuordnen können.

Die anderen Registerkarten enthalten die folgenden Funktionstypen:

* **Allgemeine Funktionen** ![](assets/toolbar-icon-general-function.png) - Weitere Informationen finden Sie unter [Allgemeine Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) .

* **Math-Funktionen** ![](assets/toolbar-icon-math-functions.png) - Weitere Informationen finden Sie unter [Math-Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) .

* **Text- und Binärfunktionen** ![](assets/toolbar-icon-text&binary-functions.png) - Weitere Informationen finden Sie unter [Zeichenfolgenfunktionen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) .

* **Datum und Uhrzeit** ![](assets/toolbar-icon-date&time-functions.png) - Weitere Informationen finden Sie unter [Datums- und Uhrzeitfunktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) und in den unten stehenden Artikeln.

   * [Token für die Datums- und Uhrzeitformatierung in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token für Datums- und Uhrzeitanalyse in Adobe Workfront Fusion](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funktionen für die Arbeit mit Arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Weitere Informationen finden Sie unter [Array-Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) .

>[!TIP]
>
>Wenn Sie eine komplexe Formel erstellen, die Sie in einem anderen Feld wiederverwenden möchten, können Sie auf das Feld klicken, das die Kombination enthält, die Kombination mit Befehl-A oder Strg-A auswählen und sie dann kopieren und in das andere Feld einfügen.

Weitere Informationen zum Zuordnen von Elementen mithilfe von Funktionen finden Sie unter [Elemente mithilfe von Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) zuordnen.

## Sammlungen

Einige Elemente können mehrere Werte verschiedener Typen enthalten. Dies sind Sammlungstypelemente.

Sie können ein Element vom Typ [!UICONTROL Sammlung] anhand des kleinen schwarzen Rechtecks identifizieren, das rechts neben dem Titel des Elements und seiner automatisch erweiterten Liste von Unterelementen angezeigt wird:

![](assets/collection.png)

>[!NOTE]
>
>In den meisten Fällen ordnen Sie die Unterelemente der Sammlung anstelle des Elements an, das die gesamte Sammlung darstellt.

Weitere Informationen zu Sammlungen finden Sie unter [Elementdatentypen in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

## Arrays

Einige Elemente können mehrere Elemente desselben Typs enthalten. Dies sind Elemente vom Typ Array.

Sie können ein Element vom Typ Array anhand der eckigen Klammern am Ende der Bezeichnung des Elements identifizieren. Klicken Sie auf das kleine schwarze Rechteck rechts neben dem Titel des Elements, um die Elemente anzuzeigen:

![](assets/array.png)

Weitere Informationen zu Arrays finden Sie unter [Elementdatentypen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### Zuordnen des ersten Elements eines Arrays

Wenn Sie das Element &quot;`Recipient name`&quot;eines Arrays zuordnen, wird es im Feld wie folgt angezeigt:

![](assets/map-array-1st-element.png)

Die Zahl in den eckigen Klammern ist ein Index, der bestimmt, welches Element des Arrays verwendet wird. Er ist standardmäßig auf 1 gesetzt.

### n-tes Element eines Arrays zuordnen

Wenn Sie auf ein anderes Element zugreifen möchten, klicken Sie auf die eckigen Klammern und bearbeiten Sie den Indexwert:

![](assets/access-another-element.png)

### Element eines Arrays mit einem bestimmten Schlüssel zuordnen

Einige Arrays enthalten mehrere Sammlungen mit Schlüssel- und Wertelementen. Dabei handelt es sich normalerweise um verschiedene Metadaten, Attribute usw.

Das folgende Beispiel zeigt die Ausgabe der [!DNL Jira]-App.

![](assets/output-of-jira-app-350x100.png)

In diesem Beispiel erhalten wir einen Dateinamen aus einem Array von Anlagen für den spezifischen Anhang mit der ID 10108.

Die Ausgabe von [!DNL Jira] sieht wie folgt aus:

![](assets/output-from-jira-350x261.png)

Die typische Anforderung besteht darin, ein Element anhand des angegebenen Schlüsselwerts zu suchen und den entsprechenden Wert aus dem Werteelement zu erhalten. Dies kann mit einer Formel erreicht werden, die eine Kombination der Funktionen `map()` und `get()` verwendet.

Im Folgenden wird die Formel detailliert aufgeschlüsselt:

1. Der erste Parameter der Funktion `map()` ist das gesamte Array-Element.
1. Der zweite Parameter ist der Rohname des Wertelements. Um den Rohnamen abzurufen, bewegen Sie den Mauszeiger über das Element im Bedienfeld [!UICONTROL mapping] :

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >Bei allen Parametern wird zwischen Groß- und Kleinschreibung unterschieden. Auch wenn sich in diesem speziellen Beispiel die Beschriftung des Elements nur in Großbuchstaben von seinem Rohnamen unterscheidet, muss der Rohname verwendet werden, der im Gegensatz zum Beschriftungswert ausschließlich aus Kleinbuchstaben besteht.

1. Der dritte Parameter ist der Rohname des Schlüsselelements:

   ![](assets/3rd-parameter-350x166.png)

1. Der vierte Parameter ist der angegebene Schlüsselwert.

Da die Funktion `map()` ein Array zurückgibt (da es mehr Elemente mit dem angegebenen Schlüsselwert geben kann), muss die Funktion `get()` angewendet werden, um das erste Element zu erhalten:

* Der erste Parameter der Funktion `get()` ist das Ergebnis der Funktion `map()`.

* Der zweite Parameter ist der Index des Elements - einer.

Weitere Informationen zur Funktion `map()` finden Sie unter [Array-Funktionen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

Weitere Informationen zur Funktion `get()` finden Sie unter [Allgemeine Funktionen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## Elemente in eine Reihe von Bundles konvertieren

Arrays können mithilfe des Moduls [!UICONTROL Iterator] in eine Reihe von Bundles konvertiert werden. Weitere Informationen finden Sie unter [[!UICONTROL Iterator]-Modul in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## Fehlerbehebung

### Fehlende Elemente im Zuordnungsbereich

Für jedes Modul zeigt das Zuordnungsbedienfeld alle Ausgabeelemente an, die vom Autor des Moduls aufgelistet werden. In einigen Fällen ist diese Liste möglicherweise aus verschiedenen Gründen unvollständig und einige Elemente fehlen möglicherweise. [!DNL Workfront Fusion] kann die fehlenden Ausgabeelemente automatisch erkennen, wenn Sie das Modul im Szenario-Editor ausführen. Das genaue Verfahren unterscheidet sich geringfügig je nach Modultyp:

#### Sofortiger Trigger

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie dann im angezeigten Menü auf **[!UICONTROL Nur dieses Modul ausführen]** .

   Wenn keine Webhooks in der Warteschlange vorhanden sind, wartet das Modul auf die Verarbeitung eines neuen Webhooks.

1. Erstellen Sie einen Webhook.

   Beispielsweise sendet das Webhook-Modul **[!DNL Slack]>[!UICONTROL Suchen nach neuen Ereignissen]** (das in einem Kanal nach neuen Kanalmeldungen sucht) eine Nachricht an den Kanal.

1. Wenn das Modul ausgeführt wird, klicken Sie auf die Blase über dem Modul, um die vollständige Ausgabe zu untersuchen.

   Das Zuordnungsbedienfeld enthält alle Elemente, die in der Ausgabe des Moduls gefunden wurden.

#### Abruf-Trigger

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie dann im angezeigten Menü auf **[!UICONTROL Nur dieses Modul ausführen]** .
1. Wenn keine Ausgabe vorhanden ist, klicken Sie auf **[!UICONTROL Auswählen, wo]** gestartet werden soll, und passen Sie die Einstellungen an.
1. Wenn kein Ereignis verarbeitet werden soll, erstellen Sie eines und gehen Sie zurück zu Schritt 2.

   Beispielsweise sendet das Webhook-Modul **[!UICONTROL Gmail] >[!UICONTROL E-Mails ansehen]** eine E-Mail an den Ordner, den das Modul überwacht.

1. Wenn das Modul ausgeführt wird, klicken Sie auf die Blase über dem Modul, um die vollständige Ausgabe zu untersuchen.

   Das Zuordnungsbedienfeld enthält jetzt alle Elemente, die in der Ausgabe des Moduls gefunden wurden.

#### Sonstige Module

Sie können Folgendes ausführen:

* Das gesamte Szenario (oder nur der Teil, der das Modul enthält)

  Wenn Ihr Szenario mit einem Trigger beginnt, lesen Sie den Abschnitt [Instant Trigger](#instant-trigger) oder [Polling Trigger](#polling-trigger) weiter oben.

* Nur das einzelne Modul

Wenn Sie nur das einzelne Modul ausführen möchten:

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie dann im angezeigten Menü auf **[!UICONTROL Nur dieses Modul ausführen]** .
1. Geben Sie Beispielwerte für die Eingabeelemente ein und klicken Sie dann auf **[!UICONTROL OK]** .
1. Wenn das Modul ausgeführt wird, klicken Sie auf die Blase über dem Modul, um die vollständige Ausgabe zu untersuchen.

   Das Zuordnungsbedienfeld enthält jetzt alle Elemente, die in der Ausgabe des Moduls gefunden wurden.
