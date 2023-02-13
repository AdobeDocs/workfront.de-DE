---
navigation-topic: search
title: Suchen [!DNL Adobe Workfront]
description: Sie können Elemente einfach in [!DNL Adobe Workfront] , indem Sie nach ihnen suchen, wenn Sie sich nicht an ihren genauen Standort erinnern können.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 1%

---

# Suchen [!DNL Adobe Workfront]

Sie können Elemente einfach in [!DNL Adobe Workfront] , indem Sie nach ihnen suchen, wenn Sie sich nicht an ihren genauen Standort erinnern können.

Sie können die [!UICONTROL Suche] in der oberen rechten Ecke einer beliebigen Seite in [!DNL Workfront].

![](assets/search-globalnavigationbar-350x62.png)

Sie müssen über die Berechtigungen zum Anzeigen eines Objekts verfügen, bevor Sie es in einer Suche finden können. Aus diesem Grund variieren die Suchergebnisse von Benutzer zu Benutzer.

## Zugriffsanforderungen

+++ Erweitern Sie diesen Abschnitt, um den Zugriff anzuzeigen, der zur Durchführung der Schritte in diesem Artikel erforderlich ist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Ansicht] Zugriff auf den Objekttyp </p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Sie müssen über die Berechtigungen zum Anzeigen eines Objekts verfügen, bevor Sie es in einer Suche finden können.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

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
* Benutzer
* Vorlagen
* Dokumente
* Portfolios
* Programme
* Dashboards
* Firmen
* Notizen

### Für die Suche verfügbare Felder

Die für die Suche verfügbaren Felder basieren auf dem Suchtyp: Einfach oder [!UICONTROL Erweiterte Suche].

* **Grundlegende Suche**: Bei der Suche nach Objekten in einer einfachen Suche [!DNL Workfront] sucht nach Text, der möglicherweise Ihre Suchbegriffe in den folgenden Feldern enthält:

   * Objektnamen
   * Beschreibungen
   * Benutzerdefinierte Datenfelder
   * Updates
   * Dokumentnamen (in bestimmten Dokumentsuchvorgängen und in einer einfachen Suche)

   Weitere Informationen zur grundlegenden Suche in [!DNL Workfront], siehe [Grundlegende Suche](#basic-search) in diesem Artikel.

* **[!UICONTROL Erweiterte Suche]**: In einer [!UICONTROL Erweiterte Suche]können Sie Filter einrichten, um Felder zu suchen, die in der einfachen Suche nicht verfügbar sind. Daher [!UICONTROL Erweiterte Suche] können Sie jedes Feld im Objekt durchsuchen.

   Weitere Informationen finden Sie unter [!UICONTROL Erweiterte Suche], siehe [Erweiterte Suche](#advanced-search) in diesem Artikel.

>[!NOTE]
>
>So führen Sie eine [!UICONTROL Erweiterte Suche], müssen Sie die [!UICONTROL Erweiterte Suche] -Option beim Starten der Suche. Sie können die einfache Suche nicht in eine [!UICONTROL Erweiterte Suche].

## Erläuterung der Einschränkungen [!DNL Workfront] Suchvorgänge

Beachten Sie bei der Verwendung von [!UICONTROL Suche] in [!DNL Workfront]:

* Bei Suchvorgängen wird nicht zwischen Groß- und Kleinschreibung unterschieden
* [!DNL Workfront] Tippfehler nicht korrigieren oder verstehen
* Suchen in [!DNL Workfront] unterstützt keine Platzhalter
* Suchen in [!DNL Workfront] unterstützt Teilsuchvorgänge nach Wörtern, unterstützt jedoch keine Suchvorgänge nach Unterzeichenfolgen.\
   Beispielsweise gibt der Suchbegriff &quot;Stand&quot;Ergebnisse zurück, einschließlich des Wortes &quot;Standard&quot;, gibt jedoch keine Ergebnisse zurück, einschließlich des Wortes &quot;Verstehen&quot;.

## Suchen nach mehreren Wörtern

Wenn Sie mehrere Wörter in eine Suche einschließen und nur Objekte finden möchten, die mit allen Wörtern im Suchfeld übereinstimmen, können Sie die Wörter in beliebiger Reihenfolge eingeben.

Wenn Sie beispielsweise nach &quot;Marketing Demo&quot;(ohne Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:

* Marketing-Demo
* Demo-Marketing
* Demo zur Marktanalyse im Januar

Außerdem werden Objekte gefunden, die im Namen möglicherweise &quot;Marketing&quot;und in der Beschreibung &quot;Demo&quot;enthalten.

Sie können jedoch Folgendes im [!UICONTROL Suche] , um die angezeigten Suchergebnisse anzupassen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Anführungszeichen einschließen</td> 
   <td> <p>Wenn Sie Wörter in der richtigen Reihenfolge innerhalb doppelter Anführungszeichen eingeben, können Sie nur Objekte finden, die exakt übereinstimmen.<br>Wenn Sie beispielsweise nach "Marketing Demo"(mit Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:</p> 
    <ul> 
     <li> Marketing-Demo</li> 
     <li> Januar-Marketing-Demo</li> 
     <li>Marketingdemo-Plan</li> 
    </ul> <p>Bei dieser Suche wurde jedoch kein Objekt mit dem Namen "Demo Marketing"gefunden.</p> </td> 
  </tr> 
  <tr> 
   <td>ODER einschließen</td> 
   <td> <p>Wenn Sie Wörter mit "OR"(ohne Anführungszeichen) verbinden, können Sie nur Objekte finden, die mindestens einem der Wörter im Feld [!UICONTROL Suche] entsprechen. Diese Wörter können in beliebiger Reihenfolge eingegeben werden.<br>Wenn Sie beispielsweise nach "Marketing ODER Demo"(ohne Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:</p> 
    <ul> 
     <li> Demo zur Marktanalyse</li> 
     <li>Demo zur Marktanalyse im Januar</li> 
     <li>Demo</li> 
     <li>Marktanalyse</li> 
    </ul> <p>Hinweis: "OR"muss in Großbuchstaben sein. Andernfalls wird es in der gesuchten Wortgruppe als ein anderes Wort interpretiert.</p> </td> 
  </tr> 
  <tr> 
   <td>UND einschließen</td> 
   <td> <p>Wenn Sie Wörter mit "AND"(ohne Anführungszeichen) verbinden, können Sie nur Objekte finden, die mit allen Wörtern im Feld [!UICONTROL Suche] übereinstimmen. Diese Wörter können in beliebiger Reihenfolge eingegeben werden.<br>Wenn Sie beispielsweise nach "Marketing AND Demo"(ohne Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:</p> 
    <ul> 
     <li>Marketing-Demo</li> 
     <li>Demo-Marketing</li> 
     <li>Demo zur Marktanalyse im Januar</li> 
    </ul> <p>Hinweis: "AND"muss in jeder Hinsicht vorhanden sein. Andernfalls wird es in der gesuchten Wortgruppe als ein anderes Wort interpretiert. Ebenso sucht die Verwendung von "&amp;"(ohne Anführungszeichen) nur nach Objekten, die das kaufmännische Und-Zeichen enthalten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verwenden Sie die Suche in [!DNL Workfront]

[!DNL Workfront] bietet zwei Arten von Suchen: Einfach und erweitert. Verwenden Sie die einfache Suche, wenn Sie Suchbegriffe in gängigen Objektfeldern wie Name oder Beschreibung suchen möchten. Verwendung [!UICONTROL Erweiterte Suche] , wenn Sie Filter verwenden möchten, um andere Objektfelder zu durchsuchen.

* [Einfache Suche](#basic-search)
* [Erweiterte Suche](#advanced-search)

### Einfache Suche

Eine einfache Suche ermöglicht die Suche nach Suchbegriffen für alle Objekte im System oder nur für ein Objekt auf einmal (z. B. Projekte). [!DNL Workfront] sucht dann in einigen bestimmten Feldern nach diesen Schlüsselwörtern. Anschließend können Sie die Suchergebnisse anhand anderer objektspezifischer Felder einschränken, die von [!DNL Workfront].

Eine Liste der Felder, die bei der einfachen Suche gesucht werden, finden Sie unter [Für die Suche verfügbare Felder](#fields-available-for-search) in diesem Artikel.

>[!NOTE]
>
>So führen Sie eine [!UICONTROL Erweiterte Suche], müssen Sie die [!UICONTROL Erweiterte Suche] -Option beim Starten der Suche. Sie können die einfache Suche nicht in eine [!UICONTROL Erweiterte Suche].

* [Grundlegende Suche durchführen](#perform-a-basic-search)
* [Einfache Suche verfeinern](#refine-a-basic-search)

#### Grundlegende Suche durchführen

Sie können eine einfache Suche auf eine der folgenden Arten durchführen:

* Alle Objekte im System (allgemeine Suche).
* Bei jeweils nur einem Objekt (objektspezifische Suche).

So führen Sie eine einfache Suche durch:

1. Klicken Sie auf die Lupe ![](assets/search-icon.png) in der oberen rechten Ecke der Seite. Sie können auch **[!UICONTROL ALT + /]** oder **[!UICONTROL Option + /]** , um [!UICONTROL Suche] Menü.

1. (Optional) Um nach einem bestimmten Objekt zu suchen, klicken Sie auf das **[!UICONTROL Alle]** und wählen Sie das Objekt aus, nach dem Sie suchen möchten.

   ![](assets/search-objecttype.png)

1. Im **[!UICONTROL Suche]** eingeben.\
   Informationen dazu, welche Felder gesucht werden [!DNL Workfront], siehe [Suche verstehen](#understand-search).\
   ![](assets/qs-search-drop-down-highlighted-350x234.png)\
   Wenn Sie mit der Eingabe in die Suchleiste beginnen, [!DNL Workfront] erstellt Empfehlungen basierend auf Ihrem Anzeigeverlauf und markiert den gesuchten Suchbegriff in Blau.

1. Wenn das gesuchte Element im [!UICONTROL typeahead] und klicken Sie darauf.

   Oder

   Presse **[!UICONTROL Eingabe]** , um eine umfassende Suche durchzuführen. Bei dieser Suche wird die gesamte Datenbank anstelle der zuletzt angezeigten Elemente abgerufen.

   Die [!UICONTROL Suchergebnisse] Seitenfolien werden von links geöffnet und decken den Großteil der vorherigen Seite ab.

   Wenn Sie eine allgemeine Suche durchgeführt haben, [!DNL Workfront] gibt Ergebnisse für jedes Objekt zurück, das dem Suchbegriff in einem der durchsuchten Felder entspricht, wie unter [Suche verstehen](#understand-search). Die Objekte, die Ihrer Suche entsprechen, werden in einer Liste angezeigt.

   >[!NOTE]
   >
   >Manchmal werden Varianten eines Wortes in der Liste der gefundenen Elemente angezeigt.\
   >Die Suche nach &quot;marketing&quot;zeigt beispielsweise Objekte an, die entweder &quot;marketing&quot;oder &quot;market&quot;im Namen enthalten.

1. (Optional) Wenn Ihre Suche zu viele Ergebnisse generiert hat, verfeinern Sie Ihre Suche wie in [Einfache Suche verfeinern](#refine-a-basic-search).
1. (Optional) Um zur Seite zurückzukehren, auf der Sie sich vor der Suche befanden, klicken Sie auf **[!UICONTROL Schließen]** in der oberen rechten Ecke.

>[!NOTE]
>
>Die [!UICONTROL Suchergebnisse] Seite bleibt nur geöffnet, wenn sie im Fokus ist. Wenn Sie von der Seite weg klicken oder eine andere Seite öffnen, wird der [!UICONTROL Suchergebnisse] Seite.

#### Einfache Suche verfeinern

Nach der Durchführung einer einfachen Suche, wie unter [[!UICONTROL Grundlegende Suche durchführen]](#perform-a-basic-search)- Sie können die Suche verfeinern.

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

[!UICONTROL Erweiterte Suche] ermöglicht die Suche mithilfe von Feldern und Filtern, die nicht für die einfache Suche verfügbar sind. Sie können beispielsweise nach Projekten mit einer bestimmten Priorität oder einem bestimmten Dokumentbesitzernamen suchen.

>[!NOTE]
>
>So führen Sie eine [!UICONTROL Erweiterte Suche], müssen Sie die [!UICONTROL Erweiterte Suche] -Option beim Starten der Suche. Sie können die einfache Suche nicht in eine [!UICONTROL Erweiterte Suche].

* [Verwenden Sie die [!UICONTROL erweiterte Suche]](#use-advanced-search)

#### Verwenden Sie die [!UICONTROL erweiterte Suche]

Sie können [!UICONTROL Erweiterte Suche] , um Ihre Suche nach bestimmten Kriterien zu filtern.\
Diese Art der Suche ist hilfreich, wenn Sie sich einen Suchbegriff, der mit einem Objekt verknüpft ist, nicht merken können, aber einige spezifische Informationen über dieses Objekt kennen (Beispiel: Projektpriorität, Name des Dokumenteneigentümers usw.).

So führen Sie eine erweiterte Suche durch:

1. In der rechten oberen Ecke einer beliebigen Seite in [!DNL Workfront], klicken Sie auf die **[!UICONTROL Suche]** icon ![](assets/search-icon.png). Die [!DNL Search] angezeigt.

1. Am unteren Rand des [!UICONTROL Suche] Menü, klicken Sie **[!UICONTROL Erweiterte Suche]**.\
   ![](assets/qs-advanced-search-350x224.png)\
   Die [!UICONTROL Erweiterte Suche] Seitenfolien werden von rechts geöffnet und decken den Großteil der vorherigen Seite ab.

1. Wählen Sie den Typ des gesuchten Objekts aus.\
   **[!UICONTROL Projekte]** ist standardmäßig ausgewählt.

   ![](assets/advanced-search-objects-qs-remove-after-prod-release.png)

1. (Optional) Geben Sie einen Suchbegriff in das Feld am Anfang der Liste ein.
1. (Optional) Klicken Sie auf **[!UICONTROL Ergebnisse filtern]** , um Ihre Suchergebnisse nach bestimmten Feldtypen zu filtern, und wählen Sie dann ein Feld aus der Liste aus. Wählen Sie ggf. auch einen Wert für das Feld aus.\
   Oder\
   Fügen Sie einen neuen Filter hinzu.

1. Klicken **[!UICONTROL Suche]**.\
   Eine Liste der Elemente, die Ihrer Suche entsprechen, wird rechts neben der [!UICONTROL Erweiterte Suche] Symbolleiste.

1. (Optional) Um zur Seite zurückzukehren, auf der Sie sich vor der Suche befanden, klicken Sie auf **[!UICONTROL Schließen]** in der oberen rechten Ecke.

>[!NOTE]
>
>Die [!UICONTROL Suchergebnisse] Seite bleibt nur geöffnet, wenn sie im Fokus ist. Wenn Sie von der Seite weg klicken oder eine andere Seite öffnen, wird der [!UICONTROL Suchergebnisse] Seite.
