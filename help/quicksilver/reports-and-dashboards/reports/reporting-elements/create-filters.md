---
product-area: reporting
navigation-topic: reporting-elements
title: Filter in Adobe Workfront erstellen oder bearbeiten
description: Mit einem Filter können Sie die Anzahl der angezeigten Informationen in einer Liste von Elementen einschränken. Sie können bestimmte Kriterien basierend auf bestimmten Informationen über ein Objekt definieren und nur die Objekte anzeigen, die diesen Kriterien entsprechen.
author: Nolan
feature: Reports and Dashboards
exl-id: 2e912e32-7924-418d-9d55-ce3c09f67d3e
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '2419'
ht-degree: 1%

---

# Filter in Adobe Workfront erstellen oder bearbeiten

<!-- Audited: 11/2024 -->

Mit einem Filter können Sie die Anzahl der angezeigten Informationen in einer Liste von Elementen einschränken. Sie können bestimmte Kriterien basierend auf bestimmten Informationen über ein Objekt definieren und nur die Objekte anzeigen, die diesen Kriterien entsprechen.

Sie können die folgenden Filtertypen in Adobe Workfront anwenden:

* Schnellfilter in einer Objektliste, um ein Element mithilfe eines Suchbegriffs zu finden. Hierbei handelt es sich um temporäre Filter, die Sie nicht für die zukünftige Verwendung speichern können.

  Informationen zu Schnellfiltern finden Sie unter [Anwenden des Schnellfilters auf eine Liste](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

* Ständige Filter, die Sie speichern und in mehreren Listen und Berichten mehrmals verwenden können. In diesem Artikel wird beschrieben, wie Sie einen permanenten Filter erstellen oder einen vorhandenen Filter in einer Liste oder einem Bericht bearbeiten.

* Filter in anderen Bereichen von Workfront außerhalb von Listen und Berichten.

  Eine Liste aller Filter in Workfront und der Bereiche, in denen Sie sie anwenden können, finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Mitwirkende bei der Änderung eines Filters</p></li>
         <li><p>Standard zum Ändern eines Filters in einem Bericht</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Filteranforderung</p></li>
         <li><p>Filter in einem Bericht ändern</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <ul><li><p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten</p></li></ul>

Um einen Filter in einem Bericht zu bearbeiten, müssen Sie über die folgende Konfiguration auf Zugriffsebene verfügen, zusätzlich zum Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten:

<ul><li><p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p></li></ul>   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen*</strong></td> 
   <td> <p>Berechtigungen für Filter verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Typen von Filteraufbauschnittstellen

Sie können Filter anhand der in der folgenden Tabelle beschriebenen Typen von Filtergenerator erstellen:

<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Builder-Typ</strong></td>
<td><strong>Filterobjekt</strong></td>
<td><strong>soweit verfügbar</strong></td>
</tr>
<tr>
<td>Standardaufbau</td>
<td>
<ul>
<li> <p>Projekte</p> </li>
<li> <p>Aufgaben </p> </li>
<li> <p>Probleme</p> </li>
<li> <p>Portfolios</p> </li>
<li> <p>Programme</p> </li>
<li> <p>Benutzende</p> </li>
<li> <p>Vorlagen</p> </li>
<li> <p>Gruppen</p> </li>
</ul>
</td>
<td>
<ul>
<li> <p>Listen </p> </li>
</ul>
<ul>
<li> <p>Die Liste "Projekte"im Szenario-Planer</p> <p>Für den Szenario-Planer ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter <a href="../../../scenario-planner/scenario-planner-overview.md">Überblick über den Szenario-Planer</a>. </p> </li>
</ul>
<p><b>NOTE:</b></p> <p>Standardgenerator für Filter sind in Berichten nicht verfügbar.
</td>
</tr>
<tr>
<td>Legacy-Builder</td>
<td>Alle Objekte </td>
<td>Listen und Berichte</td>
</tr>
</tbody>
</table>

Weitere Informationen zu Workfront-Objekten finden Sie unter [Grundlegendes zu Objekten in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Beachten Sie beim Erstellen von Filtern mit den verschiedenen Schnittstellen Folgendes:

* Sie finden den Standard-Builder an denselben Stellen wie die alte Filterschnittstelle für die in der obigen Tabelle aufgelisteten Bereiche.
* Der Standard-Builder ist das Standarderlebnis für alle Bereiche, in denen er verfügbar ist. Um zum alten Filtergenerator zu wechseln, klicken Sie auf das Menü **Mehr** neben [!UICONTROL **Filter**] und wählen Sie [!UICONTROL **Zurück zu Legacy-Filtern**].

  ![Zurück zu alten Filtern](assets/use-legacy-filters.png)

* Gespeicherte Filter sind in beiden Buildern verfügbar, unabhängig davon, welches Erlebnis Sie ursprünglich erstellt haben. Wenn Sie beispielsweise einen Filter mit dem Legacy-Builder erstellt haben, können Sie ihn auch in der Standard-Builder-Oberfläche finden und ändern.

  >[!TIP]
  >
  >Der Standard-Builder enthält keinen Filter &quot;Alle&quot;, da alle Listenelemente angezeigt werden, wenn keine Filter angewendet werden. Klicken Sie oben rechts im Builder auf [!UICONTROL **Alle löschen**] , um alle aktiven Filter zu löschen und alle Elemente anzuzeigen. Wenn [!UICONTROL **Alle löschen**] abgeblendet ist, werden keine Filter angewendet.

* Die Standard- und Legacy-Builder haben beim Erstellen von Filtern mit mehreren Aussagen, die die UND- und ODER-Operatoren kombinieren, eine etwas andere Syntax. Daher können diese Filter beim Wechsel von einem Builder zu einem anderen unterschiedlich angezeigt werden.

  >[!INFO]
  >
  >Das folgende Szenario ist vorhanden:
  >
  >1. Verwenden Sie den Standard-Builder, um einen Filter mit der folgenden Syntax zu erstellen:
  >
  >      `(A OR B) AND C`
  >
  >1. Wechseln Sie zum Legacy-Builder und bearbeiten Sie den Filter mithilfe der Syntax des Legacy-Builders, wie im Abschnitt [Erstellen oder Bearbeiten eines Filters im Legacy-Builder](#create-filter-in-legacy-builder) in diesem Artikel beschrieben. Die Syntax für den Legacy-Builder zeigt die Filteranweisungen wie folgt an:
  >
  >      `A AND C`
  >      `OR`
  >      `B AND C`
  >
  >1. Ändern Sie den Filter in der alten Benutzeroberfläche.
  >1. Wechseln Sie zurück zum Standard-Builder. Die Filteranweisung wird entsprechend der Logik angezeigt, die im Legacy-Builder unterstützt wird, wie oben beschrieben.
  >
  >      Der Filter wird in der Standard-Builder-Oberfläche wie folgt angezeigt:
  >  
  >      `A AND C`
  >      `OR`
  >      `B AND C`
  > 
  >      Dies geschieht, weil der Filter in der alten Benutzeroberfläche geändert wurde.

## Erstellen oder Bearbeiten von Filtern im Standard-Builder

Sie können Filter auf folgende Weise mithilfe der Standard-Builder-Oberfläche erstellen:

* Neu
* Vorhandenen Filter bearbeiten
* Vorhandenen Filter duplizieren
* Existierenden Filter duplizieren, bearbeiten und als neuen Filter speichern

Erstellen Sie einen Filter mit der Standard-Builder-Oberfläche:

1. Rufen Sie eine Liste auf, in der Sie einen Filter erstellen möchten oder der den anzupassenden Filter enthält.
1. Klicken Sie auf das Symbol **Filter** ![Filtersymbol](assets/filter-nwepng.png), um die Builder-Oberfläche zu öffnen.

   ![Standardfilter-Builder](assets/new-filters-all-filter-types.png)

1. Überprüfen Sie die folgenden Filterlisten:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Favorit</strong></td>
   <td>Filter, die Sie als Favoriten gekennzeichnet haben. Wenn Sie einen Filter bevorzugen, wird seine ursprüngliche Position unter dem Filternamen angezeigt und er wird aus der ursprünglichen Liste ausgeblendet, es sei denn, Sie entfernen ihn als Favoriten.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Gespeichert</strong></td>
   <td>Filter, die Sie selbst erstellt und gespeichert haben. Standardmäßig werden in dieser Liste gespeicherte Filter in der Reihenfolge angezeigt, in der sie zuletzt gespeichert wurden. Die Filternamen können jedoch per Drag-and-Drop manuell neu angeordnet werden.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Standardeinstellungen für das System</strong></td>
   <td>Standardfilter und Filter des Workfront-Systems, die der Workfront-Administrator Ihrer Filterliste entweder auf Systemebene oder in Ihrer Layoutvorlage hinzugefügt hat.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Für mich freigegeben</strong></td>
   <td>Filter, die von anderen erstellt und für Sie freigegeben wurden oder die systemweit freigegeben sind.</td>
   </tr>
   </tbody>
   </table>

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Neuer Filter** , um einen neuen Filter zu erstellen.
   * Bewegen Sie den Mauszeiger über einen vorhandenen Filter, den Sie verwalten dürfen, und klicken Sie auf das Symbol **Bearbeiten** ![Bearbeiten-Symbol](assets/edit-icon.png) , um ihn zu bearbeiten.

     Oder

     Bewegen Sie den Mauszeiger über einen vorhandenen Filter, den Sie anzeigen können, klicken Sie auf das Menü **Mehr** ![Mehr Menü](assets/more-icon-spectrum.png) und klicken Sie auf **Duplizieren** , um den vorhandenen Filter zu kopieren und eine Kopie zu bearbeiten.

   ![Weitere Menüoptionen](assets/new-filters-more-menu-options-with-delete.png)

1. (Bedingt) Je nachdem, ob Sie Objekte suchen möchten, die mit allen oder einer der Anweisungen in einer Filtergruppe übereinstimmen, wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Einschließen, wenn alle wahr sind</strong></td>
   <td>Die vom Filter gefundenen Objekte müssen allen Filterkriterien einer Filtergruppe entsprechen. In diesem Fall werden die Filteranweisungen durch den UND-Operator verbunden. Dies ist die Standardauswahl.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Einschließen, wenn eins davon wahr ist</strong></td>
   <td>Die vom Filter gefundenen Objekte müssen allen Filterkriterien einer Filtergruppe entsprechen. In diesem Fall werden die Filteranweisungen durch den ODER-Operator verbunden.</td>
   </tr>
   </tbody>
   </table>

   ![Einschließen, wenn das gesamte Dropdown-Menü oder ein beliebiges Dropdown-Menü oder true](assets/new-filters-all-or-any-are-true-drop-down-menu-nwe.png)

   Weitere Informationen zu Filteroperatoren finden Sie unter [Filterübersicht](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken Sie auf das Feld-Dropdown-Menü, um eine Liste der zuletzt verwendeten Felder und der vorgeschlagenen Felder anzuzeigen, nach denen gefiltert werden soll. Die vorgeschlagenen Felder werden derzeit in der Liste angezeigt, die Sie filtern.

   Sie können auch **Felder durchsuchen** auswählen, um eine Liste aller Felder anzuzeigen, nach denen Sie filtern können. Die Felder der erweiterten Suche werden nach Objektkategorie gruppiert.

   ![Suchen Sie ein Feld, nach dem Sie filtern möchten.](assets/new-filter-search-for-field.png)

1. Klicken Sie auf das Dropdown-Menü &quot;Modifikator&quot;, um einen Modifikator auszuwählen. Der Standard-Modifikator ist &quot;Gleich&quot;.

   Weitere Informationen finden Sie unter [Filter und Bedingungsmodifikatoren](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!TIP]
   >
   >Beim Erstellen des Filters werden die Ergebnisse sofort in der Liste angezeigt. Wenn der Filterbereich die Liste abdeckt, können Sie sie schließen, um die Anzeige zu sehen. Die eingegebenen Informationen bleiben beim erneuten Öffnen des Bedienfelds im Builder.

1. Geben Sie den Wert eines Felds ein, nach dem Sie filtern möchten. Geben Sie beispielsweise den Namen eines Problems ein, wenn Sie nach `Issue:Name` filtern möchten. Wählen Sie den Wert aus, wenn er in der Liste angezeigt wird.

   >[!TIP]
   >
   >Je nach ausgewähltem Modifikator können Sie mehrere Werte auswählen.

1. Klicken Sie auf **Filter hinzufügen** , um ein anderes Feld auszuwählen und der Filteranweisung ein Filterkriterium hinzuzufügen.
1. (Optional) Klicken Sie auf das Symbol **Löschen** ![Löschsymbol](assets/delete.png) , um vorhandene Filteranweisungen zu entfernen.

   Oder

   Klicken Sie auf **Alle löschen** , um alle Filterkriterien zu löschen.

1. (Optional) Klicken Sie auf **Filtergruppe hinzufügen** , um einen weiteren Satz von Filterkriterien hinzuzufügen. Der Standardoperator zwischen den Sets ist **AND**. Klicken Sie auf den Operator, um ihn in **ODER** zu ändern.

   >[!TIP]
   >
   >Möglicherweise möchten Sie eine andere Filtergruppe verwenden, wenn die Gruppen von einem anderen Operator als dem Operator in einer Filteranweisung verbunden werden sollen.

   >[!INFO]
   >
   >Wenn Sie nach Projekten filtern, die &quot;Marketing&quot;im Namen enthalten, die entweder nicht vollständig sind und sich nicht auf &quot;Auf Halten&quot;befinden, können Sie die folgenden Filtergruppen verwenden:
   >`(Project: Name Contains Marketing AND Project: Percent Complete Does not equal 100)`
   >`OR`
   >`(Project: Name Contains Marketing AND Project: Status Does not equal On Hold)`
   >In diesem Fall ist jede Filteranweisung durch ein UND verbunden und die Filtergruppen sind durch ein ODER verbunden.

1. (Optional) Klicken Sie auf **Textmodus** , um mit der Erstellung des Filters im Textmodus fortzufahren.

   ![Textmodus auswählen](assets/new-filter-select-text-mode.png)

   Die Textmodus-Benutzeroberfläche wird geöffnet.

   ![Textmodus-Benutzeroberfläche](assets/text-mode-interface-for-beta-filters-nwe.png)

   >[!TIP]
   >
   >Es wird empfohlen, möglichst viele Filter mit der Standard-Builder-Oberfläche zu erstellen und nur den Textmodus zu verwenden, wenn Sie die Filter ändern müssen, die nur im Textmodus unterstützt werden.

   Weitere Informationen zum Erstellen eines Filters mit der Textmodus-Oberfläche finden Sie unter [Bearbeiten eines Filters mit dem Textmodus](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. Klicken Sie auf **Textmodus beenden** , um zur standardmäßigen Builder-Oberfläche zurückzukehren.

   >[!WARNING]
   >
   >Einige Textmodusanweisungen werden im Standard-Builder oder in der alten Benutzeroberfläche nicht unterstützt. Wenn Sie den Textmodus beenden, wenn Sie diese Arten von Anweisungen erstellt haben, wird möglicherweise eine Warnmeldung angezeigt.

1. (Optional) Klicken Sie auf **Anwenden** , um den Filter auf die Liste anzuwenden und die Ergebnisse anzuzeigen.

   Wenn der Filter keine Ergebnisse liefert, ist die Liste leer.

1. Klicken Sie auf **Als neu speichern** , um den Filter für die zukünftige Verwendung zu speichern.

   ![Benennen und speichern Sie den Filter](assets/save-as-untitled-filter-ui-nwe.png)

1. Wählen Sie **Unbenannter Filter** aus und geben Sie stattdessen den Namen des neuen Filters ein.

   >[!TIP]
   >
   >Benennen Sie den Filter unbedingt, damit Sie ihn später finden können. Wenn Sie den Filter nicht benennen, wird er im System als &quot;Unbenannter Filter&quot;bezeichnet.

1. Wählen Sie aus dem Dropdownmenü **Symbol** ein Symbol für den neuen Filter aus.

   ![Wählen Sie ein Symbol für den Filter](assets/new-filter-select-icon.png)

1. (Optional) Fügen Sie eine Beschreibung für den Filter hinzu, um anzugeben, was eindeutig ist. Die Beschreibung wird unter dem Filternamen in der Filterliste angezeigt.

   >[!TIP]
   >
   >Wenn Sie jederzeit auf **Abbrechen** klicken, gelangen Sie zurück zum Filterbaubereich.

1. Klicken Sie auf **Speichern**. Der Filter wird in der Liste &quot;Gespeichert&quot;gespeichert und auf die Liste der Elemente angewendet.
1. (Optional) Um einen Filter in die Liste &quot;Favoriten&quot;zu verschieben, bewegen Sie den Mauszeiger über einen beliebigen Filter in der Filterleiste und klicken Sie auf das Symbol **Favorit** ![Favoritensymbol](assets/favorites-icon-small.png).

   Oder

   Bewegen Sie den Mauszeiger über einen Filter in der Filterleiste, klicken Sie auf das Menü &quot;Mehr&quot;![Mehr Menü](assets/more-icon-spectrum.png) und klicken Sie auf **Favorit**.

1. (Optional) Klicken Sie auf die Schaltfläche **Filter stapeln** , um gestapelte Filter zu aktivieren. Mit dieser Option können Sie mehr als einen gespeicherten Filter anwenden. Die Filterregeln werden in der Reihenfolge angewendet, in der Sie sie auswählen.

   >[!TIP]
   >
   >Die Anzahl der Filter, die Sie auswählen können, ist unbegrenzt.
   >
   >Wenn Sie mehrere Filter auswählen, müssen alle zugehörigen Bedingungen gleichzeitig erfüllt sein, um übereinstimmende Ergebnisse anzuzeigen.

   ![Filter stapeln](assets/new-filter-stack-filters.png)

   Die Anzahl der ausgewählten Filter wird neben dem Filtersymbol oben in der Elementliste angezeigt.

   ![Anzahl der ausgewählten Filter](assets/number-of-filters-selected.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus:

   * Geben Sie den Filter für andere frei oder stellen Sie ihn systemweit zur Verfügung. Weitere Informationen finden Sie unter [Filter, Ansichten oder Gruppierungen freigeben](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

   * Löschen Sie den Filter, wenn er nicht mehr gültig ist oder ein Duplikat ist. Sie können nur Filter löschen, deren Inhaber Sie sind. Sie können Filter entfernen, die für Sie freigegeben wurden. Weitere Informationen finden Sie unter [Filter, Ansichten und Gruppierungen entfernen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).

## Erstellen oder Bearbeiten von Filtern im Legacy-Builder {#create-filter-in-legacy-builder}

Sie können veraltete Filter in Listen und Berichten wie folgt erstellen:

* Neu
* Vorhandenen Filter bearbeiten und als neuen Filter speichern

Unabhängig von der Methode, die Sie zum Erstellen von Filtern verwenden, ist das Erstellen eines Filters von Grund auf oder aus einem vorhandenen Filter ähnlich.

1. Markieren Sie eine Liste oder einen Bericht mit dem anzupassenden Filter.
1. Klicken Sie auf das Symbol &quot;**Filter**&quot;![Filter &quot;](assets/filter-nwepng.png)&quot;, klicken Sie dann auf das Symbol &quot;**Mehr**&quot;![Mehr &quot;](assets/more-icon.png) und klicken Sie auf &quot;**Zurück zu Legacy-Filtern&quot;**.

   >[!TIP]
   >
   >Der Ersteller des Berichts muss die Bearbeitung von Filtern zulassen, damit die Dropdownliste Filter in einem Bericht angezeigt werden kann. Der Filter Berichtsstandard wird standardmäßig auf einen Bericht angewendet. Der Filter Berichtsstandard kann nur angepasst werden, wenn Sie den Bericht bearbeiten.

1. Klicken Sie oben in der Filterliste auf **+ Neuer Filter** .

   Oder

   Bewegen Sie den Mauszeiger über den zu ändernden Filter und klicken Sie auf das Symbol **Bearbeiten** ![Bearbeiten-Symbol](assets/edit-icon.png).

   Der Builder zum Anpassen der Filterstarts.

1. Führen Sie einen der folgenden Schritte aus:

   * Ändern Sie vorhandene Filterregeln, indem Sie auf die vorhandene Regel klicken und eine neue Option auswählen.
   * Fügen Sie eine Filterregel hinzu, indem Sie auf &quot;**Andere Filterregel hinzufügen**&quot;klicken, mit der Eingabe des Namens der Option beginnen, für die Sie eine Regel hinzufügen möchten, und klicken Sie dann im Feld &quot;**Feldname eingeben&quot;** auf die Filterregel und dann auf sie, wenn sie in der Dropdownliste angezeigt wird.

     Felder, die mit dem Objekt Ihres Filters verknüpft sind, werden im Feld **Feldname eingeben** aufgeführt.

   * Klicken Sie beim Hinzufügen einer Filterregel auf **AND** oder **OR** .\
     Verwenden Sie beim Hinzufügen von Filterregeln die Filter-Modifikatoren, um die Bedingung Ihres Filters festzulegen. Weitere Informationen zu Filtermodifikatoren finden Sie unter [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

     >[!NOTE]
     >
     >Wenn Sie eine Gruppe von UND-Anweisungen durch mehrere OR-Anweisungen verbinden, müssen Sie die Felder wiederholen, die sich zwischen den OR-Anweisungen für jede Gruppe von Anweisungen nicht ändern.
     >
     >![Anweisungen für Connected filter](assets/filters-and-statements-connected-by-or-statements-builder-ui-legacy-filters.png)
     >
     >Wenn Sie einen Filter für Aufgaben erstellen, die das Wort &quot;Marketing&quot;enthalten und sich in Projekten mit dem Status Aktuell oder Planung befinden, müssen Sie über die folgenden Filterregeln verfügen:
     >
     >`Task: Name Contains Marketing`
     >`AND`
     >`Project: Status Equals Current`
     >`OR`
     >`Task: Name Contains Marketing`
     >`AND`
     >`Project: Status Equals Planning`
     >
     >Aufgabe: Name Enthält &quot;Marketing&quot;ändert sich zwar nicht zwischen den beiden UND-Filtergruppen, muss jedoch in der zweiten Gruppe wiederholt werden.

   * Löschen Sie eine vorhandene Filterregel durch Klicken auf das X-Symbol.

1. (Optional) Klicken Sie auf **Wechseln in den Textmodus** , um einen Filter über die Benutzeroberfläche &quot;Textmodus&quot;hinzuzufügen.

   Weitere Informationen zum Erstellen eines Filters mit der Textmodus-Oberfläche finden Sie unter [Bearbeiten eines Filters mit dem Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

1. Klicken Sie auf **Filter speichern** , um einen Filter zu erstellen oder den ausgewählten Filter durch Ihre Änderungen zu ersetzen.

   Oder

   Klicken Sie auf **Als neuen Filter speichern** , um einen neuen Filter aus dem ausgewählten Filter zu erstellen.

   Der neue Filter wird in der Filterliste angezeigt und automatisch auf die ausgewählte Liste oder den ausgewählten Bericht angewendet.

1. (Optional) Führen Sie einen der folgenden Schritte aus:

   * Geben Sie von Ihnen erstellte Filter für andere Benutzer frei oder stellen Sie sie systemweit zur Verfügung. Weitere Informationen finden Sie unter [Freigeben eines Filters, einer Ansicht oder einer Gruppierung](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
   * Entfernen Sie Filter, die nicht mehr in der Liste angezeigt werden sollen. Weitere Informationen finden Sie unter [Filter, Ansichten und Gruppierungen entfernen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).


