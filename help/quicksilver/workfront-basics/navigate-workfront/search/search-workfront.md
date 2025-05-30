---
navigation-topic: search
title: Suche [!DNL Adobe Workfront]
description: Sie können Elemente in leicht finden [!DNL Adobe Workfront]  indem Sie nach ihnen suchen, wenn Sie sich nicht an ihre genaue Position erinnern können.
feature: Get Started with Workfront
author: Lisa
exl-id: 7c856349-c79f-40d8-9c96-b32bfb6d5417
source-git-commit: a9dbfe21337be9cd9929f4e982e4979265ca14e1
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 1%

---

# [!DNL Adobe Workfront] suchen

<!-- Audited: 5/2025 -->

Sie können Elemente in [!DNL Adobe Workfront] leicht finden, indem Sie nach ihnen suchen, wenn Sie sich nicht an ihre genaue Position erinnern können.

Das Feld [!UICONTROL Suche] wird oben rechts auf jeder Seite in [!DNL Workfront] angezeigt.

![Suchsymbol in der Navigationsleiste](assets/search-globalnavigationbar-350x62.png)

Sie müssen über die Berechtigung zum Anzeigen eines Objekts verfügen, bevor Sie es bei einer Suche finden können. Aus diesem Grund variieren die Suchergebnisse von Benutzer zu Benutzer.

## Zugriffsanforderungen

+++ Erweitern Sie diesen Abschnitt, um den Zugriff anzuzeigen, der zum Ausführen der Schritte in diesem Artikel erforderlich ist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: Mitwirkender oder höher<p>
   <p>Oder</p>
   <p>Aktuell: Anforderung oder höher </p>


</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL View]-Zugriff auf den Objekttyp </p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie müssen über die Berechtigung zum Anzeigen eines Objekts verfügen, bevor Sie es bei einer Suche finden können.</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Suche verstehen

### Für die Suche verfügbare Objekte

Sie können in Workfront nach folgenden Objekten suchen:

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

Die für die Suche verfügbaren Felder basieren auf dem Typ der Suche: Einfache oder [!UICONTROL Erweiterte Suche].

* **Einfache Suche**: Bei der Suche nach Objekten in einer Einfache Suche sucht [!DNL Workfront] in den folgenden Feldern nach Text, der Ihre Keywords enthalten könnte:

   * Objektnamen
   * Beschreibungen
   * Benutzerdefinierte Datenfelder
   * Updates
   * Dokumentnamen (bei bestimmten Dokumentsuchen und bei einer einfachen Suche)

  Weitere Informationen zur einfachen Suche in [!DNL Workfront] finden Sie im folgenden Abschnitt in diesem Artikel: [Einfache Suche](#basic-search).

* **[!UICONTROL Erweiterte Suche]**: In einer [!UICONTROL Erweiterten Suche] können Sie Filter einrichten, um Suchfelder zu suchen, die in der einfachen Suche nicht verfügbar sind. Daher ermöglicht [!UICONTROL Erweiterte Suche] die Suche nach beliebigen Feldern im Objekt.

  Weitere Informationen zur [!UICONTROL erweiterten Suche] finden Sie im folgenden Abschnitt in diesem Artikel: [Erweiterte Suche](#advanced-search).

>[!NOTE]
>
>Um eine [!UICONTROL erweiterte Suche] durchzuführen, müssen Sie die Option [!UICONTROL Erweiterte Suche] auswählen, wenn Sie Ihre Suche starten. Sie können eine einfache Suche nicht in eine [!UICONTROL erweiterte Suche“ &#x200B;].

## Verstehen der Einschränkungen [!DNL Workfront] Suchvorgänge

Beachten Sie die folgenden Einschränkungen bei der Verwendung von [!UICONTROL Suche] in [!DNL Workfront]:

* Bei Suchen wird nicht zwischen Groß- und Kleinschreibung unterschieden.
* [!DNL Workfront] korrigiert oder versteht keinen Tippfehler.
* Die Suche in [!DNL Workfront] unterstützt keine Platzhalter.
* Die Suche in [!DNL Workfront] unterstützt die Suche nach Wortteilen, unterstützt jedoch nicht die Suche nach Teilzeichenfolgen.\
   Beispielsweise würde das Suchbegriff „stand“ Ergebnisse zurückgeben, die das Wort „standard“ enthalten, aber keine Ergebnisse zurückgeben, die das Wort „verstehen“ enthalten.

## Nach mehreren Wörtern suchen

Wenn Sie mehrere Wörter in eine Suche einbeziehen und nur Objekte finden möchten, die mit allen Wörtern im Suchfeld übereinstimmen, können Sie die Wörter in beliebiger Reihenfolge eingeben.

Wenn Sie beispielsweise nach „Marketing-Demo“ (ohne Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:

* Marketing-Demo
* Demo-Marketing
* Demo zur Marktanalyse im Januar

Außerdem werden Objekte gefunden, die „Marketing“ im Namen und „Demo“ in der Beschreibung enthalten können.

Sie können jedoch Folgendes im Feld [!UICONTROL Suche] tun, um die angezeigten Suchergebnisse anzupassen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Anführungszeichen einschließen</td> 
   <td> <p>Wenn Sie Wörter in der richtigen Reihenfolge in doppelten Anführungszeichen eingeben, können Sie nur Objekte finden, die genau übereinstimmen.<br>Wenn Sie beispielsweise nach „Marketing-Demo“ (mit Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:</p> 
    <ul> 
     <li> Marketing-Demo</li> 
     <li> Januar-Marketing-Demo</li> 
     <li>Marketing-Demoplan</li> 
    </ul> <p>Bei dieser Suche wurde jedoch kein Objekt mit dem Namen „Demo Marketing“ gefunden.</p> </td> 
  </tr> 
  <tr> 
   <td>ODER einschließen</td> 
   <td> <p>Durch Verbinden von Wörtern mit „OR“ (ohne Anführungszeichen) können Sie nur Objekte finden, die mit mindestens einem der Wörter im Feld [!UICONTROL Search] übereinstimmen. Die Wörter können in beliebiger Reihenfolge eingegeben werden.<br>Wenn Sie beispielsweise nach „Marketing ODER Demo“ (ohne Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:</p> 
    <ul> 
     <li> Demo zur Marktanalyse</li> 
     <li>Demo zur Marktanalyse im Januar</li> 
     <li>Demo</li> 
     <li>Marktanalyse</li> 
    </ul> <p>Hinweis: „OR“ muss in Großbuchstaben angegeben werden. Andernfalls wird es als ein weiteres Wort in der Phrase interpretiert, nach der Sie suchen.</p> </td> 
  </tr> 
  <tr> 
   <td>UND einschließen</td> 
   <td> <p>Das Verbinden von Wörtern mit „AND“ (ohne Anführungszeichen) ermöglicht es, nur Objekte zu finden, die mit allen Wörtern im Feld [!UICONTROL Search] übereinstimmen. Die Wörter können in beliebiger Reihenfolge eingegeben werden.<br>Wenn Sie beispielsweise nach „Marketing UND Demo“ (ohne Anführungszeichen) suchen, werden Objekte mit den folgenden Namen gefunden:</p> 
    <ul> 
     <li>Marketing-Demo</li> 
     <li>Demo-Marketing</li> 
     <li>Demo zur Marktanalyse im Januar</li> 
    </ul> <p>Hinweis: „UND“ muss in Großbuchstaben angegeben werden. Andernfalls wird es als ein weiteres Wort in der Phrase interpretiert, nach der Sie suchen. Gleichermaßen sucht das Einschließen von "&amp;" (ohne Anführungszeichen) nur nach Objekten, die das kaufmännische Und-Zeichen enthalten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verwenden der Suche in [!DNL Workfront]

[!DNL Workfront] bietet zwei Arten von Suchvorgängen: Einfach und Erweitert. Verwenden Sie die einfache Suche, wenn Sie Keywords in allgemeinen Objektfeldern wie Name oder Beschreibung finden möchten. Verwenden [!UICONTROL Erweiterte Suche] wenn Sie Filter verwenden möchten, um andere Objektfelder zu suchen.

* [Einfache Suche](#basic-search)
* [Erweiterte Suche](#advanced-search)

### Einfache Suche

Mit einer einfachen Suche können Sie nach Keywords für alle Objekte im System oder nur für jeweils ein Objekt (z. B. Projekte) suchen. [!DNL Workfront] sucht dann in einigen spezifischen Feldern nach diesen Keywords. Anschließend können Sie Ihre Suchergebnisse verfeinern, basierend auf anderen objektspezifischen Feldern, die von [!DNL Workfront] ausgewählt wurden.

Eine Liste der spezifischen Felder, nach denen in der Standardsuche gesucht wird, finden Sie im folgenden Abschnitt in diesem Artikel: [Felder für die Suche](#fields-available-for-search).

>[!NOTE]
>
>Um eine [!UICONTROL erweiterte Suche] durchzuführen, müssen Sie die Option [!UICONTROL Erweiterte Suche] auswählen, wenn Sie Ihre Suche starten. Sie können eine einfache Suche nicht in eine [!UICONTROL erweiterte Suche“ &#x200B;].

* [Durchführen einer einfachen Suche](#perform-a-basic-search)
* [Einfache Suche verfeinern](#refine-a-basic-search)

#### Durchführen einer einfachen Suche

Sie können eine einfache Suche auf eine der folgenden Arten durchführen:

* Über alle Objekte im System hinweg (allgemeine Suche).
* Jeweils nur ein Objekt (objektspezifische Suche).

So führen Sie eine einfache Suche durch:

1. Klicken Sie auf die Lupe ![Suchsymbol](assets/search-icon.png) in der oberen rechten Ecke der Seite.

1. (Optional) Um nach einem bestimmten Objekt zu suchen, klicken Sie auf das **[!UICONTROL Alle]** Dropdown-Menü und wählen Sie das Objekt aus, nach dem Sie suchen möchten.

   ![Suche nach Objekttyp](assets/search-objecttype.png)

1. Beginnen Sie **[!UICONTROL Feld]**&#x200B;Suchen“ mit der Eingabe der gesuchten Informationen.
Informationen dazu, welche Felder in [!DNL Workfront] durchsucht werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Suche verstehen](#understand-search).
   ![Dropdown-Liste „Suche“](assets/qs-search-drop-down-highlighted-350x234.png)

   Wenn Sie mit der Eingabe in die Suchleiste beginnen, gibt [!DNL Workfront] Empfehlungen, die auf Ihrem Ansichtsverlauf basieren, und es wird das gesuchte Keyword in Blau hervorgehoben.

1. Wenn das gesuchte Element im Menü [!UICONTROL mit automatischer Textvervollständigung] angezeigt wird, klicken Sie darauf.

   Oder

   Drücken Sie die Eingabetaste (Mac[!UICONTROL &#x200B; oder &#x200B;]Eingabetaste) auf der Tastatur, um eine umfassende Suche durchzuführen. Diese Suche fragt die gesamte Datenbank anstelle der zuletzt angezeigten Elemente ab und öffnet die Seite **Suche**.

   Wenn Sie eine allgemeine Suche durchgeführt haben, gibt [!DNL Workfront] Ergebnisse für alle Objekte zurück, die dem Suchbegriff in einem der Suchfelder entsprechen, wie in [Suchen verstehen](#understand-search) beschrieben. Die Objekte, die Ihrer Suche entsprechen, werden in einer Liste angezeigt.

   >[!NOTE]
   >
   >Manchmal werden Varianten eines Wortes in der Liste der gefundenen Elemente angezeigt.\
   >Wenn Sie beispielsweise nach „Marketing“ suchen, werden Objekte angezeigt, die im Namen entweder „Marketing“ oder „Markt“ enthalten.

1. (Optional) Wenn Ihre Suche zu viele Ergebnisse generiert hat, verfeinern Sie Ihre Suche wie in [Einfache Suche verfeinern](#refine-a-basic-search) beschrieben.

#### Einfache Suche verfeinern

Nachdem Sie eine einfache Suche durchgeführt haben, können Sie die Suche verfeinern.

Verwenden Sie die Symbolleiste links neben Ihren Suchergebnissen, um die gesuchten Informationen einzugrenzen.

So verfeinern Sie eine Suche:

1. (Bedingt) Wenn Sie eine allgemeine Suche durchgeführt haben, wählen Sie das gesuchte Objekt in der Liste der Objekte oben links in den Ergebnissen aus.
1. Suchen Sie die Felder, die für die Objekte verfügbar sind, die bei der Suche angezeigt werden, in der Symbolleiste links neben den Ergebnissen. Die Werte der einzelnen Felder werden, sortiert nach Anzahl, für jedes Feld bis zu 10 Werte angezeigt.
1. Klicken Sie in eines der verfügbaren Felder, um die Ergebnisliste zu verkürzen. Die von Ihnen vorgenommenen Auswahlen werden blau hervorgehoben und die nicht ausgewählten Feldwerte sind ausgeblendet.
Nachdem Sie jeden neuen Wert ausgewählt haben, werden die Ergebnisse auf der rechten Seite dynamisch aktualisiert.

   ![Registerkarte „Einfache Suche“](assets/basic-search.png)

1. (Optional) Klicken Sie auf die ausgewählten Werte, um die Auswahl aufzuheben und alle Werte für jedes Feld erneut anzuzeigen.

### [!UICONTROL Erweiterte Suche]

[!UICONTROL Erweiterte Suche] ermöglicht die Suche mithilfe von Feldern und Filtern, die für die einfache Suche nicht verfügbar sind. Sie können beispielsweise nach Projekten mit einer bestimmten Priorität oder einem bestimmten Dokumentbesitzernamen suchen.

>[!NOTE]
>
>Um eine [!UICONTROL erweiterte Suche] durchzuführen, müssen Sie die Option [!UICONTROL Erweiterte Suche] auswählen, wenn Sie Ihre Suche starten. Sie können eine einfache Suche nicht in eine [!UICONTROL erweiterte Suche“ &#x200B;].

* [Verwenden [!UICONTROL erweiterten Suche]](#use-advanced-search)

#### Verwenden [!UICONTROL erweiterten Suche]

Sie können die [!UICONTROL Erweiterte Suche] verwenden, um Ihre Suche nach bestimmten Kriterien zu filtern.\
Diese Art der Suche ist hilfreich, wenn Sie sich ein Keyword, das mit einem Objekt verknüpft ist, nicht merken können, aber bestimmte Informationen zu diesem Objekt kennen (Beispiel: Projektpriorität, Name des Dokumentbesitzers usw.).

So führen Sie eine erweiterte Suche durch:

1. Klicken Sie oben rechts auf einer beliebigen Seite in [!DNL Workfront] auf das Symbol **[!UICONTROL Suchen]** (![) ](assets/search-icon.png). Das Menü **Suche** wird angezeigt.

1. Klicken Sie unten im Menü **Suche** auf **[!UICONTROL Erweiterte Suche]**. Die **Suche** wird geöffnet, wobei die Registerkarte **Erweiterte Suche** standardmäßig ausgewählt ist.
   ![Erweiterte Suche](assets/qs-advanced-search-350x224.png)


1. Wählen Sie den Typ des Objekts aus, nach dem Sie suchen. **[!UICONTROL Aufgaben]** ist standardmäßig ausgewählt.

   ![Erweiterte Suchobjekte](assets/advanced-search.png)

1. (Optional) Geben Sie ein Keyword in das Feld oben in der Liste ein.
1. (Optional) Schalten Sie **[!UICONTROL Ergebnisse filtern]** auf **Ein** um, um einen Filter zur Verfeinerung Ihrer Suche zu erstellen. Klicken Sie **Abschluss auf**&#x200B;Übernehmen“.

1. Klicken Sie auf **[!UICONTROL Suchen]**. Rechts neben der Symbolleiste **[!UICONTROL Erweiterte Suche“ wird eine Liste mit Elementen]**, die Ihrer Suche entsprechen.
