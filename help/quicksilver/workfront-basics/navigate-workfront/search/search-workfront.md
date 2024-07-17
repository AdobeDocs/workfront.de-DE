---
navigation-topic: search
title: Suche [!DNL Adobe Workfront]
description: Sie können Elemente in [!DNL Adobe Workfront] einfach finden, indem Sie nach ihnen suchen, wenn Sie sich nicht an deren genauen Speicherort erinnern können.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1668'
ht-degree: 1%

---

# [!DNL Adobe Workfront] suchen

Sie können Elemente in [!DNL Adobe Workfront] einfach finden, indem Sie nach ihnen suchen, wenn Sie sich nicht an deren genauen Speicherort erinnern können.

Sie können das Feld [!UICONTROL Suche] in der oberen rechten Ecke einer beliebigen Seite in [!DNL Workfront] sehen.

![](assets/search-globalnavigationbar-350x62.png)

Sie müssen über die Berechtigungen zum Anzeigen eines Objekts verfügen, bevor Sie es in einer Suche finden können. Aus diesem Grund variieren die Suchergebnisse von Benutzer zu Benutzer.

## Zugriffsanforderungen

+++ Erweitern Sie diesen Abschnitt, um den Zugriff anzuzeigen, der zur Durchführung der Schritte in diesem Artikel erforderlich ist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf den Objekttyp in der [!UICONTROL Ansicht] </p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Sie müssen über die Berechtigungen zum Anzeigen eines Objekts verfügen, bevor Sie es in einer Suche finden können.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Suche verstehen

* [[!UICONTROL Für die Suche verfügbare Objekte]](#objects-available-for-search)
* [[!UICONTROL Für die Suche verfügbare Felder]](#fields-available-for-search)

### Für die Suche verfügbare Objekte

Sie können in Workfront nach den folgenden Objekten suchen:

* Projekte
* Aufgaben
* Probleme
* Berichte
* Benutzende
* Vorlagen
* Dokumente
* Portfolios
* Programme
* Dashboards
* Firmen
* Notizen

### Für die Suche verfügbare Felder

Die für die Suche verfügbaren Felder basieren auf dem Typ der Suche: Einfach oder [!UICONTROL Erweiterte Suche].

* **Grundlegende Suche**: Bei der Suche nach Objekten in einer einfachen Suche sucht [!DNL Workfront] nach Text, der möglicherweise Ihre Suchbegriffe in den folgenden Feldern enthält:

   * Objektnamen
   * Beschreibungen
   * Benutzerdefinierte Datenfelder
   * Updates
   * Dokumentnamen (in bestimmten Dokumentsuchvorgängen und in einer einfachen Suche)

  Weitere Informationen zur grundlegenden Suche in [!DNL Workfront] finden Sie unter [Grundlegende Suche](#basic-search) in diesem Artikel.

* **[!UICONTROL Erweiterte Suche]**: In einer [!UICONTROL erweiterten Suche] können Sie Filter einrichten, um Suchfelder einzurichten, die in der einfachen Suche nicht verfügbar sind. Daher können Sie mit der [!UICONTROL erweiterten Suche] nach jedem Feld im Objekt suchen.

  Weitere Informationen zu [!UICONTROL Erweiterte Suche] finden Sie unter [Erweiterte Suche](#advanced-search) in diesem Artikel.

>[!NOTE]
>
>Um eine [!UICONTROL erweiterte Suche] durchzuführen, müssen Sie beim Starten Ihrer Suche die Option [!UICONTROL Erweiterte Suche] auswählen. Sie können eine einfache Suche nicht in eine [!UICONTROL erweiterte Suche] verfeinern.

## Grundlegendes zu den Einschränkungen von [!DNL Workfront] Suchvorgängen

Beachten Sie bei Verwendung von [!UICONTROL Suche] in [!DNL Workfront] die folgenden Einschränkungen:

* Bei Suchen wird nicht zwischen Groß- und Kleinschreibung unterschieden
* [!DNL Workfront] korrigiert Tippfehler nicht oder versteht sie nicht
* Die Suche in [!DNL Workfront] unterstützt keine Platzhalter.
* Die Suche in [!DNL Workfront] unterstützt Teilsuchvorgänge nach Wörtern, unterstützt jedoch keine Suchvorgänge nach Unterzeichenfolgen.\
   Beispielsweise gibt der Suchbegriff &quot;Stand&quot;Ergebnisse zurück, einschließlich des Wortes &quot;Standard&quot;, gibt jedoch keine Ergebnisse zurück, einschließlich des Wortes &quot;Verstehen&quot;.

## Suchen nach mehreren Wörtern

Wenn Sie mehrere Wörter in eine Suche einschließen und nur Objekte finden möchten, die mit allen Wörtern im Suchfeld übereinstimmen, können Sie die Wörter in beliebiger Reihenfolge eingeben.

Wenn Sie beispielsweise nach &quot;Marketing Demo&quot;(ohne Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:

* Marketing-Demo
* Demo-Marketing
* Demo zur Marktanalyse Januar

Außerdem werden Objekte gefunden, die im Namen möglicherweise &quot;Marketing&quot;und in der Beschreibung &quot;Demo&quot;enthalten.

Sie können jedoch Folgendes im Feld [!UICONTROL Suche] tun, um die angezeigten Suchergebnisse anzupassen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Anführungszeichen einschließen</td> 
   <td> <p>Wenn Sie Wörter in der richtigen Reihenfolge innerhalb doppelter Anführungszeichen eingeben, können Sie nur Objekte finden, die exakt übereinstimmen.<br>Die Suche nach "Marketing Demo"(mit Anführungszeichen) findet beispielsweise Objekte mit den folgenden Namen:</p> 
    <ul> 
     <li> Marketing-Demo</li> 
     <li> Januar-Marketing-Demo</li> 
     <li>Marketingdemo-Plan</li> 
    </ul> <p>Bei dieser Suche wurde jedoch kein Objekt mit dem Namen "Demo Marketing"gefunden.</p> </td> 
  </tr> 
  <tr> 
   <td>ODER einschließen</td> 
   <td> <p>Wenn Sie Wörter mit "OR"(ohne Anführungszeichen) verbinden, können Sie nur Objekte finden, die mindestens einem der Wörter im Feld [!UICONTROL Suche] entsprechen. Diese Wörter können in beliebiger Reihenfolge eingegeben werden.<br>Die Suche nach "Marketing ODER Demo"(ohne Anführungszeichen) findet beispielsweise Objekte mit den folgenden Namen:</p> 
    <ul> 
     <li> Demo zur Marktanalyse</li> 
     <li>Demo zur Marktanalyse Januar</li> 
     <li>Demo</li> 
     <li>Marktanalyse</li> 
    </ul> <p>Hinweis: "OR"muss in Großbuchstaben angegeben werden. Andernfalls wird es in der gesuchten Wortgruppe als ein anderes Wort interpretiert.</p> </td> 
  </tr> 
  <tr> 
   <td>UND einschließen</td> 
   <td> <p>Wenn Sie Wörter mit "AND"(ohne Anführungszeichen) verbinden, können Sie nur Objekte finden, die mit allen Wörtern im Feld [!UICONTROL Suche] übereinstimmen. Diese Wörter können in beliebiger Reihenfolge eingegeben werden.<br>Die Suche nach "Marketing UND Demo"(ohne Anführungszeichen) findet beispielsweise Objekte mit den folgenden Namen:</p> 
    <ul> 
     <li>Marketing-Demo</li> 
     <li>Demo-Marketing</li> 
     <li>Demo zur Marktanalyse Januar</li> 
    </ul> <p>Hinweis: "AND"muss in Großbuchstaben angegeben werden. Andernfalls wird es in der gesuchten Wortgruppe als ein anderes Wort interpretiert. Ebenso sucht die Verwendung von "&amp;"(ohne Anführungszeichen) nur nach Objekten, die das kaufmännische Und-Zeichen enthalten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Suche in [!DNL Workfront] verwenden

[!DNL Workfront] bietet zwei Arten von Suchen: Einfach und erweitert. Verwenden Sie die einfache Suche, wenn Sie Suchbegriffe in gängigen Objektfeldern wie Name oder Beschreibung suchen möchten. Verwenden Sie [!UICONTROL Erweiterte Suche] , wenn Sie Filter verwenden möchten, um andere Objektfelder zu durchsuchen.

* [Einfache Suche](#basic-search)
* [Erweiterte Suche](#advanced-search)

### Einfache Suche

Eine einfache Suche ermöglicht die Suche nach Suchbegriffen für alle Objekte im System oder nur für ein Objekt auf einmal (z. B. Projekte). [!DNL Workfront] und sucht dann in einigen bestimmten Feldern nach diesen Suchbegriffen. Anschließend können Sie die Suchergebnisse auf der Grundlage anderer objektspezifischer Felder einschränken, die von [!DNL Workfront] ausgewählt wurden.

Eine Liste der spezifischen Felder, die bei der einfachen Suche durchsucht werden, finden Sie in diesem Artikel unter [Für die Suche verfügbare Felder](#fields-available-for-search) .

>[!NOTE]
>
>Um eine [!UICONTROL erweiterte Suche] durchzuführen, müssen Sie beim Starten Ihrer Suche die Option [!UICONTROL Erweiterte Suche] auswählen. Sie können eine einfache Suche nicht in eine [!UICONTROL erweiterte Suche] verfeinern.

* [Grundlegende Suche durchführen](#perform-a-basic-search)
* [Einfache Suche verfeinern](#refine-a-basic-search)

#### Grundlegende Suche durchführen

Sie können eine einfache Suche auf eine der folgenden Arten durchführen:

* Alle Objekte im System (allgemeine Suche).
* Bei jeweils nur einem Objekt (objektspezifische Suche).

So führen Sie eine einfache Suche durch:

1. Klicken Sie auf das Lupensymbol ![](assets/search-icon.png) in der oberen rechten Ecke der Seite. Sie können auch **[!UICONTROL ALT + /]** oder **[!UICONTROL Option + /]** eingeben, um das Menü [!UICONTROL Suche] zu öffnen.

1. (Optional) Um nach einem bestimmten Objekt zu suchen, klicken Sie auf das Dropdown-Menü **[!UICONTROL Alle]** und wählen Sie das Objekt aus, nach dem Sie suchen möchten.

   ![](assets/search-objecttype.png)

1. Geben Sie im Feld **[!UICONTROL Suchen]** die gesuchten Informationen ein.\
   Informationen dazu, welche Felder in [!DNL Workfront] gesucht werden, finden Sie unter [Suche verstehen](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   Wenn Sie mit der Eingabe in die Suchleiste beginnen, formuliert [!DNL Workfront] Empfehlungen basierend auf Ihrem Anzeigeverlauf und markiert den gesuchten Suchbegriff in Blau.

1. Wenn das gesuchte Element im Menü [!UICONTROL typeahead] angezeigt wird, klicken Sie darauf.

   Oder

   Drücken Sie **[!UICONTROL die Eingabetaste]**, um eine umfassende Suche durchzuführen. Bei dieser Suche wird die gesamte Datenbank anstelle der zuletzt angezeigten Elemente abgerufen.

   Die Seite [!UICONTROL Suchergebnisse] wird von links aus geöffnet und deckt den Großteil der vorherigen Seite ab.

   Wenn Sie eine allgemeine Suche durchgeführt haben, gibt [!DNL Workfront] Ergebnisse für jedes Objekt zurück, das dem Suchbegriff in einem der durchsuchten Felder entspricht, wie in [Suche verstehen](#understand-search) beschrieben. Die Objekte, die Ihrer Suche entsprechen, werden in einer Liste angezeigt.

   >[!NOTE]
   >
   >Manchmal werden Varianten eines Wortes in der Liste der gefundenen Elemente angezeigt.\
   >Die Suche nach &quot;marketing&quot;zeigt beispielsweise Objekte an, die entweder &quot;marketing&quot;oder &quot;market&quot;im Namen enthalten.

1. (Optional) Wenn Ihre Suche zu viele Ergebnisse generiert hat, verfeinern Sie Ihre Suche wie in [Einfache Suche verfeinern](#refine-a-basic-search) beschrieben.
1. (Optional) Um zur Seite zurückzukehren, auf der Sie sich vor der Suche befanden, klicken Sie oben rechts auf **[!UICONTROL Schließen]** .

>[!NOTE]
>
>Die Seite [!UICONTROL Suchergebnisse] bleibt nur geöffnet, wenn sie im Fokus ist. Wenn Sie von der Seite weg klicken oder eine andere Seite öffnen, wird die Seite [!UICONTROL Suchergebnisse] geschlossen.

#### Einfache Suche verfeinern

Nachdem Sie eine einfache Suche durchgeführt haben, wie unter [[!UICONTROL Grundlegende Suche durchführen]](#perform-a-basic-search) beschrieben, können Sie die Suche verfeinern.

Verwenden Sie die Symbolleiste links neben den Suchergebnissen, um die gesuchten Informationen einzuschränken.

So verfeinern Sie eine Suche:

1. (Bedingt) Wenn Sie eine allgemeine Suche durchgeführt haben, wählen Sie in der Liste der Objekte oben links in den Ergebnissen das gesuchte Objekt aus.
1. Suchen Sie in der Symbolleiste links neben den Ergebnissen nach den Feldern, die für die in der Suche angezeigten Objekte verfügbar sind.\
   Die Werte der einzelnen Felder zeigen für jedes Feld bis zu 10 Werte an, sortiert nach Anzahl.
1. Klicken Sie in eines der verfügbaren Felder, um die Ergebnisliste zu verkürzen.\
   Die von Ihnen gewählten Optionen werden blau hervorgehoben und die nicht ausgewählten Feldwerte werden ausgeblendet.\
   Nachdem Sie jeden neuen Wert ausgewählt haben, werden die Ergebnisse auf der rechten Seite dynamisch aktualisiert.\
   ![](assets/qs-refine-search-350x175.png)

1. (Optional) Klicken Sie auf die ausgewählten Werte, um deren Auswahl aufzuheben und alle Werte für jedes Feld erneut anzuzeigen.

### [!UICONTROL Erweiterte Suche]

[!UICONTROL Erweiterte Suche] ermöglicht die Suche anhand von Feldern und Filtern, die nicht für die einfache Suche verfügbar sind. Sie können beispielsweise nach Projekten mit einer bestimmten Priorität oder einem bestimmten Dokumentbesitzernamen suchen.

>[!NOTE]
>
>Um eine [!UICONTROL erweiterte Suche] durchzuführen, müssen Sie beim Starten Ihrer Suche die Option [!UICONTROL Erweiterte Suche] auswählen. Sie können eine einfache Suche nicht in eine [!UICONTROL erweiterte Suche] verfeinern.

* [Verwenden Sie [!UICONTROL Erweiterte Suche]](#use-advanced-search)

#### Verwenden Sie [!UICONTROL Erweiterte Suche]

Sie können [!UICONTROL Erweiterte Suche] verwenden, um Ihre Suche nach bestimmten Kriterien zu filtern.\
Diese Art der Suche ist hilfreich, wenn Sie sich einen mit einem Objekt verknüpften Suchbegriff nicht merken können, aber einige spezifische Informationen zu diesem Objekt kennen (z. B. Projektpriorität, Dokumenteigentümername usw.).

So führen Sie eine erweiterte Suche durch:

1. Klicken Sie oben rechts auf einer beliebigen Seite in [!DNL Workfront] auf das Symbol **[!UICONTROL Suchen]** ![](assets/search-icon.png). Das Menü [!DNL Search] wird angezeigt.

1. Klicken Sie unten im Menü [!UICONTROL Suchen] auf **[!UICONTROL Erweiterte Suche]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   Die Seite [!UICONTROL Erweiterte Suche] wird von rechts aus geöffnet und deckt den Großteil der vorherigen Seite ab.

1. Wählen Sie den Typ des gesuchten Objekts aus.\
   **[!UICONTROL Projekte]** ist standardmäßig ausgewählt.

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. (Optional) Geben Sie einen Suchbegriff in das Feld am Anfang der Liste ein.
1. (Optional) Klicken Sie auf **[!UICONTROL Ergebnisse filtern]** , um Ihre Suchergebnisse nach bestimmten Feldtypen zu filtern, und wählen Sie dann ein Feld aus der Liste aus. Wählen Sie ggf. auch einen Wert für das Feld aus.\
   Oder\
   Hinzufügen eines neuen Filters.

1. Klicken Sie auf **[!UICONTROL Suchen]**.\
   Eine Liste der Elemente, die Ihrer Suche entsprechen, wird rechts neben der Symbolleiste [!UICONTROL Erweiterte Suche] angezeigt.

1. (Optional) Um zur Seite zurückzukehren, auf der Sie sich vor der Suche befanden, klicken Sie oben rechts auf **[!UICONTROL Schließen]** .

>[!NOTE]
>
>Die Seite [!UICONTROL Suchergebnisse] bleibt nur geöffnet, wenn sie im Fokus ist. Wenn Sie von der Seite weg klicken oder eine andere Seite öffnen, wird die Seite [!UICONTROL Suchergebnisse] geschlossen.
