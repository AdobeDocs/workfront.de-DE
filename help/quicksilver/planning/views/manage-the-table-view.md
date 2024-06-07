---
title: Tabellenansicht verwalten
description: Beim Zugriff auf die Datensatztypseite in der Adobe Workfront-Planung können Sie Datensätze und deren Felder in einer Tabellenansicht anzeigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '2403'
ht-degree: 3%

---

# Tabellenansicht verwalten

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Workfront Planning. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Beim Zugriff auf die Datensatztypseite in der Adobe Workfront-Planung können Sie Datensätze und deren Felder in einer Tabellenansicht anzeigen.

Informationen zu Datensatzansichten und deren Verwaltung finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss in der Phase des frühen Zugriffs für die Workfront-Planung eingeschrieben sein </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
   <p>Systemadministratoren haben nur Zugriff auf die von ihnen erstellten oder für sie freigegebenen Ansichten. </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">Konfiguration der Zugriffsebene</td>
   <td> <p>Es gibt keine Zugriffsebenen-Steuerelemente für die Adobe Workspace-Planung</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für die Ansicht verwalten</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Tabellenansicht verwalten {#manage-a-table-view}

<!--insert screen shot of table view-->

Bei der Erstellung einer Tabellenansicht werden alle Datensätze des ausgewählten Typs in einer Tabelle angezeigt. Jede Zeile ist ein eindeutiger Datensatz und jede Spalte ist ein Datensatzfeld. Alle Felder und Datensätze werden standardmäßig angezeigt.

So verwalten Sie eine Tabellenansicht:

1. Erstellen Sie eine Tabellenansicht, wie im Artikel beschrieben [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. (Optional) Klicken Sie auf **Zeilenhöhe** und wählen Sie dann aus den folgenden Optionen aus, um die Höhe der Tabellenzeilen zu ändern:
   * Klein
   * Mittel
   * Groß

1. Aktualisieren Sie die folgenden Ansichtselemente wie in den folgenden Unterabschnitten beschrieben:
   * [Spalten (oder Felder)](#add-columns-or-fields)
   * [Zeilen (oder Datensätze)](#add-rows-or-records)
   * [Filter](#add-filters)
   * [Gruppierung](#add-groupings)
   * [Sortieren](#add-a-sort)


### Spalten (oder Felder) hinzufügen {#add-columns}

Die Spaltenüberschriften einer Tabellenansicht zeigen Felder an, die mit den Datensätzen in der Ansicht verknüpft sind. Dieselben in der Tabellenansicht angezeigten Felder werden auch im Abschnitt Details eines Datensatzes angezeigt. Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

Das Hinzufügen von Spalten zu einer Ansicht entspricht dem Hinzufügen von Feldern zu einem Datensatztyp.

Sie können bis zu 500 Felder (oder Spalten) in einer Tabellenansicht hinzufügen.

1. Gehen Sie zu einer Seite vom Typ Datensatz und wählen Sie eine **Verzeichnis** Ansicht aus dem Dropdown-Menü &quot;Ansicht&quot;aus.

   <!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. Fügen Sie Felder (oder Spalten) hinzu, wie im Artikel beschrieben [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

   Die hinzugefügten Spalten sind für alle Benutzer sichtbar, die auf den Datensatztyp zugreifen und als neue Felder auf der Datensatzseite hinzugefügt werden.

1. Führen Sie einen der folgenden Schritte aus, um die Spalten in der Tabelle neu anzuordnen:

   * Ziehen Sie die Spaltenüberschrift in den Arbeitsbereich und legen Sie sie an der gewünschten Position ab. Die Spalte, die Sie kurz verschoben haben, wird mit blauem Hintergrund angezeigt, bis Sie weitere Anpassungen an der Tabelle vornehmen.

   * Klicks **Felder** Ziehen Sie die Felder in die Symbolleiste der Tabelle und legen Sie sie in der gewünschten Reihenfolge ab. Klicken Sie dann außerhalb der **Sichtbarkeit und Reihenfolge der Felder** zum Schließen.

     ![](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* Das Feld Name ist standardmäßig immer das erste Feld in der Tabellenansicht. Dies gilt als primäres Feld.
     >
     >* Sie können das Feld Name nicht an eine andere Position verschieben, es sei denn, Sie bestimmen ein anderes Feld als primäres Feld. Weitere Informationen erhalten Sie, wenn Sie mit Schritt 4 fortfahren. <!--accurate?-->
     >
     >* Ein primäres Feld kann nicht ausgeblendet oder gelöscht werden.
     >
     >* Das Primärfeld ist eingefroren und nicht Teil des horizontalen Bildlaufs.

   * Ersetzen Sie das Feld in der ersten Spalte durch ein anderes Feld, indem Sie das primäre Feld ändern. Weitere Informationen erhalten Sie, wenn Sie mit Schritt 4 fortfahren. <!--accurate?-->

1. (Optional) Bewegen Sie den Mauszeiger über einen Feldnamen in der Spaltenüberschrift eines Felds, das nicht in der ersten Spalte der Tabelle angezeigt wird, klicken Sie auf den Pfeil nach unten rechts neben dem Feldnamen und klicken Sie dann auf **Als primäres Feld festlegen**.

   ![](assets/set-as-primary-field-option-table-view.png)

1. Klicks **Feld festlegen** zur Bestätigung.

   Das Feld wird zu einem primären Feld, was bedeutet, dass es als erste Spalte der Tabellenansicht angezeigt wird. Das vorherige primäre Feld wechselt zur zweiten Spalte.

   >[!NOTE]
   >
   >   * Nur Felder der folgenden Typen können Primärfelder sein:
   >
   >       * Einzeiliger Text
   >       * Zahl
   >       * Formel
   >
   >   * Das Primärfeld ist immer eingefroren und kann nicht verschoben werden. Sie können ein primäres Feld durch ein anderes ersetzen, wenn Sie es an eine andere Position verschieben möchten.
   >
   >   * Das Ändern des Primärfelds in der Tabellenansicht wirkt sich auf die Ansicht aller anderen Benutzer aus, die das Feld auswählen.
   >
   >   * Eine Änderung des Primärfelds in einer Tabellenansicht wirkt sich auf alle Tabellenansichten aus.
   >
   >   * Ein primäres Feld kann nicht gelöscht oder ausgeblendet werden.
   >
   >   * Der im primären Feld angegebene Wert ist immer per Hyperlink zur Datensatzseite gekennzeichnet.

1. Klicken Sie auf die Spaltentrennlinien und ziehen Sie sie an die gewünschte Stelle, um die Spaltenbreite zu vergrößern.

   >[!TIP]
   >
   >Die Änderungen an der Spaltenbreite und -reihenfolge sind dauerhaft und für alle Benutzer sichtbar, die auf den Datensatztyp zugreifen.

1. Bewegen Sie den Mauszeiger über die Spaltenüberschrift, klicken Sie dann auf den nach unten zeigenden Pfeil und klicken Sie dann auf **Feld ausblenden**

   Oder

   Klicks **Felder** in der Tabellen-Symbolleiste und deaktivieren Sie den Umschalter, der den auszublendenden Feldern (oder Spalten) zugeordnet ist. Die **Sichtbarkeit und Reihenfolge der Felder** angezeigt.

   >[!TIP]
   >
   >Die Anzahl der ausgeblendeten Felder wird links neben dem Symbol Felder in der Symbolleiste angezeigt.


1. Klicken Sie auf **Felder** und aktivieren Sie den Umschalter, der den Feldern zugeordnet ist, die in den Spalten der Tabelle angezeigt werden sollen. Alle Felder werden standardmäßig angezeigt.

1. Führen Sie die folgenden Schritte aus, um schnell nach Datensätzen zu suchen, die einem Keyword entsprechen:

   1. Klicken Sie auf **Suche** icon ![](assets/search-icon.png) und beginnen Sie mit der Eingabe eines Suchbegriffs, das mit einem Feld eines Datensatzes verknüpft ist, das auf dem Bildschirm angezeigt wird. Die Anzahl der richtigen Übereinstimmungen wird neben dem Suchelement angezeigt und das Feld mit der richtigen Übereinstimmung wird hervorgehoben.

      ![](assets/search-box-with-results-blue-outline-table-view.png)

      Sie können beliebige Wörter oder Sonderzeichen verwenden, die auf dem Bildschirm sichtbar sind.

      Sie können keine Suchbegriffe verwenden, die Feldern zugeordnet sind, die in der Tabellenansicht ausgeblendet sind.

   1. Presse **Eingabe** auf der Tastatur, um zum nächsten gefundenen Feld zu wechseln.

   1. (Optional) Wenn mehrere Übereinstimmungen vorliegen, klicken Sie auf die Pfeile nach oben und unten rechts neben dem Suchbegriff, um alle Übereinstimmungen in der Tabelle zu finden.

   1. Klicken Sie auf **x** in das Suchfeld ein, um den Suchbegriff zu löschen.


### Zeilen (oder Datensätze) hinzufügen {#add-rows}

Die Zeilen einer Tabellenansicht zeigen einzelne Datensätze des ausgewählten Datensatztyps an.

Sie können bis zu 50.000 Datensätze (oder Zeilen) für einen Datensatztyp haben.

1. Gehen Sie zu einer Seite vom Typ Datensatz und wählen Sie eine **Verzeichnis** Ansicht aus dem Dropdown-Menü &quot;Ansicht&quot;aus.

<!-- replace above with this when view redesign: Go to a record type page and click a table view tab, or click **+ View **to add a new view, then choose **Table**. -->
1. Fügen Sie Einträge (oder Zeilen) hinzu, wie im Artikel beschrieben. [Datensätze erstellen](/help/quicksilver/planning/records/create-records.md).

   Die Datensätze, die Sie in der Tabellenansicht hinzufügen, werden sofort gespeichert und sind für alle Benutzer sichtbar, die über Ansicht oder höhere Berechtigungen für den Arbeitsbereich verfügen.

1. (Optional) Fügen Sie jedem Datensatz eine Miniaturansicht hinzu und klicken Sie auf **Felder** in der oberen rechten Ecke der Tabelle und wählen Sie dann den Umschalter für **Miniatur** -Feld, um es links neben dem primären Feld anzuzeigen. Die Auswahl ist standardmäßig aufgehoben.

   Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. (Optional) Wählen Sie einen oder mehrere Datensätze in einer Zeile aus, ziehen Sie die **handle** icon ![](assets/handle-icon.png) links neben dem Datensatznamen, um die Zeilen neu anzuordnen.

   >[!NOTE]
   >
   >Wenn Sie mindestens eine Sortierung auf die Tabellenansicht anwenden, können Sie die Reihenfolge der Zeilen nicht ändern.

   <!-- this is not possible right now:

    1. To reorder the rows, click the row header, drag and drop it in the desired location. 

        The changes you make to the row order are permanent and visible to all users who access the record type
    -->

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### Filter hinzufügen {#add-filters}

Mithilfe von Filtern können Sie die Anzahl der auf dem Bildschirm angezeigten Informationen verringern.

Beachten Sie Folgendes beim Arbeiten mit Filtern in der Tabellenansicht:
<!-- this list is almost identical to the one for the table view - update both-->

* Die Filter, die Sie für die Tabellenansicht erstellen, funktionieren unabhängig von den Filtern in der Timeline-Ansicht, wenn sie auf denselben Datensatztyp angewendet werden.

* Die Filter sind für die ausgewählte Ansicht eindeutig. Für zwei Tabellenansichten desselben Datensatztyps können unterschiedliche Filter angewendet werden. Zwei Benutzer, die sich dieselbe Tabellenansicht ansehen, sehen denselben Filter, der derzeit angewendet wird.

* Sie können die erstellten Filter nicht benennen und auf eine Tabellenansicht anwenden.

* Durch das Entfernen von Filtern werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp wie Sie zugreifen, und es wird die gleiche Ansicht wie die von Ihnen verwendete verwendet.

* Das Hinzufügen von Filtern zur Tabellenansicht entspricht dem Hinzufügen von Filtern zur Timeline-Ansicht.

* Sie können nach verbundenen Datensatzfeldern oder Suchfeldern filtern, jedoch nicht nach Feldern, die eine Verknüpfung mit mehreren Datensätzen ermöglichen.

So fügen Sie einer Tabellenansicht einen Filter hinzu:

1. Erstellen Sie eine Tabellenansicht für eine Seite vom Typ Datensatz, wie im Artikel beschrieben [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).
1. Wählen Sie eine Tabellenansicht aus und klicken Sie auf **Filter** in der oberen rechten Ecke der Tabelle.
1. Klicks **Bedingung hinzufügen** und fügen Sie die folgenden Informationen hinzu:

   * **Feld auswählen** nach dem Sie filtern möchten <!-- the tip below might change-->

   * **Option auswählen** (oder ein Filter-Modifikator) zum Definieren der Bedingungen, die das Feld erfüllen muss

     Die nachstehende Tabelle zeigt die verfügbaren Modifikatoren für jeden Feldtyp.

     <table>
        <thead>
        <tr>
            <th><b>Feldtyp</b></th>
            <th><b>Modifikatoren</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Einzeiliger Absatz, Formel </td>
            <td><p>Enthält</p>
            <p>Enthält nicht</p>
            <p>Ist</p>
            <p>Ist nicht</p>
            <p>Ist leer</p>
            <p>Ist nicht leer</p></td>
        </tr>
        <tr><td>Einzelauswahl</td>
            <td><p>Ist</p>
            <p>Ist nicht</p>
            <p>Ist ein beliebiges von</p>
            <p>Ist keines von</p>
            <p>Ist leer</p>
            <p>Ist nicht leer</p></td>
        </tr>
        <tr>
            <td>Mehrfachauswahl, Personen</td>
            <td><p>Hat eines von</p>
            <p>Hat alle von</p>
            <p>Ist genau</p>
            <p>Hat keines von</p>
            <p>Ist leer</p>
            <p>Ist nicht leer</p></td>
        </tr>
        <tr>
            <td>Zahl, Prozentsatz, Währung</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>Ist leer</p>
            <p>Ist nicht leer</p></td>
        </tr>
        <tr>
            <td>Datum</td>
            <td><p>Ist</p>
            <p>Ist nicht</p>
            <p>Ist nach</p>
            <p>Ist vor</p>
            <p>Ist zwischen</p><p>Ist nicht zwischen</p>
            <p>Ist leer</p><p>Ist nicht leer</p></td>
        </tr>

     <tr>
            <td>Kontrollkästchen</td>
            <td><p>Ist</p>
        </tr>
        </tbody>
        </table>

   * Wählen Sie einen Wert für das ausgewählte Feld aus.

   ![](assets/filter-ui-table-view.png)

   Es gibt keine Beschränkung für die Anzahl der Filterbedingungen, die Sie hinzufügen können.

1. (Optional) Klicken Sie auf **Bedingung hinzufügen** um eine weitere Filteroption hinzuzufügen und die oben beschriebenen Schritte zu wiederholen. Die Anzahl der angewendeten Filter wird links neben dem Symbol Filter angezeigt.
1. Klicken Sie auf die folgenden Operatoren, um anzugeben, wie die Filterbedingungen verbunden werden und angewendet werden sollen:

   * **und**: Alle angegebenen Bedingungen müssen erfüllt sein.
   * **Oder**: Jede der angegebenen Bedingungen muss erfüllt sein. Dies ist die Standardoption.

   Die Liste der Datensätze wird automatisch gefiltert.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Optional) Klicken Sie auf **Filter** und klicken Sie dann auf **x** -Symbol, um einen Filter zu entfernen. <!--right now you cannot "clear all" for filters, but this might come later-->

### Gruppierungen hinzufügen {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

Sie können Datensätze nach ähnlichen Informationen gruppieren, wenn Sie eine Gruppierung auf eine Ansicht anwenden.

Das Hinzufügen von Gruppierungen in der Tabellenansicht ähnelt dem Hinzufügen von Gruppierungen zur Timeline-Ansicht.

Beachten Sie Folgendes:

* Sie können Gruppierungen sowohl in der Tabellen- als auch in der Timeline-Ansicht anwenden. Die Gruppierungen der Tabellenansicht sind unabhängig von denen in der Timeline-Ansicht desselben Datensatztyps.
* Sie können in einer Ansicht drei Gruppierungsebenen anwenden. Die Datensätze werden in der von Ihnen ausgewählten Reihenfolge gruppiert.
&lt;!—* Bei Verwendung der API können Sie bis zu 4 Gruppierungsebenen verwenden. —jetzt mit diesem hier abgleichen—>
* Die Gruppierungen unterscheiden sich je nach ausgewählter Ansicht. Bei zwei Tabellenansichten desselben Datensatztyps können unterschiedliche Gruppierungen angewendet werden. Zwei Benutzer, die sich dieselbe Tabellenansicht ansehen, sehen dieselbe Gruppierung, die derzeit angewendet wird.
* Sie können die für eine Tabellenansicht erstellten Gruppierungen nicht benennen.
* Durch das Entfernen von Gruppierungen werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp zugreifen wie Sie und die dieselbe Ansicht wie Sie anzeigen.
* Sie können die unter einer Gruppierung aufgelisteten Datensätze bearbeiten.
* Sie können nach verbundenen Datensatzfeldern oder Suchfeldern gruppieren, jedoch nicht nach Feldern, die eine Verknüpfung mit mehreren Datensätzen ermöglichen.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

So fügen Sie eine Gruppierung hinzu:

1. Erstellen Sie eine Timeline-Ansicht für einen Datensatztyp, wie im Artikel beschrieben [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).
1. Klicks **Gruppierung** in der oberen rechten Ecke der Tabellenansicht.

   ![](assets/grouping-ui-table-view-with-linked-fields.png)

1. Klicken Sie auf eines der vorgeschlagenen Felder oder auf **Andere Felder auswählen**, suchen Sie nach einem anderen Feld und klicken Sie darauf, wenn es in der Liste angezeigt wird.

   Die Gruppierung wird automatisch auf die Tabelle angewendet und Datensätze werden unter der Trennlinie der Gruppierung angezeigt.

1. (Optional) Klicken Sie auf **Bedingung hinzufügen** und wiederholen Sie die obigen Schritte, um bis zu 3 Gruppierungen hinzuzufügen.

   Die Anzahl der für die Gruppierung ausgewählten Felder wird neben dem Gruppierungssymbol angezeigt.

   ![](assets/grouping-applied-in-table-view.png)

1. (Optional) Innerhalb des **Gruppiert Datensätze nach** und klicken Sie auf das **x** rechts neben einem Feld, das zum Entfernen der Gruppierung ausgewählt wurde

   Oder

   Klicks **Alle löschen** um alle Felder zu entfernen.

1. Klicken Sie außerhalb der **Gruppiert Datensätze nach** zum Schließen.
1. (Optional) Klicken Sie auf **+ Neu &lt; Name des Datensatztyps >** am Ende jeder Gruppierung, um neue Datensätze hinzuzufügen, und aktualisieren Sie dann Ihre Seite, um den neuen Datensatz zur entsprechenden Gruppierung hinzuzufügen. <!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

### Sortierung hinzufügen {#sort-information}

Durch Anwendung einer Sortierung können Sie Informationen in einer bestimmten Reihenfolge organisieren.

Sie können die folgenden Informationen sortieren:

* Alle Datensätze in einer Tabellenansicht. <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

Beachten Sie beim Sortieren von Datensätzen in der Tabellenansicht Folgendes:

<!-- if this is available for the timeline view, update both when you update one-->

* Die Sortierung ist für die ausgewählte Ansicht eindeutig. Für zwei Tabellenansichten desselben Datensatztyps können unterschiedliche Sortierkriterien angewendet werden. Zwei Benutzer, die sich dieselbe Tabellenansicht ansehen, sehen dieselbe Sortierung, die derzeit angewendet wird.

* Sie können die erstellten Sortierungen nicht benennen und auf eine Tabellenansicht anwenden.

* Die von Ihnen erstellte Sortierung wird beim Navigieren beibehalten.

* Sie können so viele Felder sortieren, wie in der Tabellenansicht eines Datensatztyps angezeigt werden.

* Verknüpfte Felder können nur sortiert werden, wenn sie einzelne Werte zulassen oder wenn sie Mehrfachauswahlwerte mit ausgewählter Zusammenfassungsoption zulassen (Summe, Durchschnitt, max, min).

* Wenn Sie Sortierungskriterien entfernen, werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp wie Sie zugreifen, und es wird die gleiche Ansicht wie Sie verwendet.

* Sie können nach verbundenen Datensatzfeldern oder Suchfeldern sortieren, jedoch nicht nach Feldern, die eine Verknüpfung mit mehreren Datensätzen ermöglichen.

Zum Sortieren <!--ungrouped (add this when sorting for groupings will be available--> -Einträge, führen Sie folgende Schritte aus:

1. Erstellen Sie eine Tabellenansicht, wie im Artikel beschrieben [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).
1. Klicken Sie auf **Sortieren** icon ![](assets/sort-icon.png) in der oberen rechten Ecke der Tabelle

   Oder

   Bewegen Sie den Mauszeiger über den Namen einer Spalte in der Tabellenansicht, klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Spaltenüberschriftsnamen und klicken Sie dann auf **Nach diesem Feld sortieren**. Das Feld wird als Sortierungsauswahl im Sortiersymbol in der oberen rechten Ecke der Tabellenansicht hinzugefügt.

1. (Bedingt) Im **Sortieren von Datensätzen nach** auf eines der vorgeschlagenen Felder klicken oder auf **Andere Felder auswählen** und suchen Sie nach einem anderen Feld und klicken Sie dann darauf, wenn es in der Liste angezeigt wird.

   Die Sortierung wird automatisch auf die Tabellenansicht angewendet und die Datensätze werden nach den von Ihnen ausgewählten Kriterien sortiert angezeigt.

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. (Optional) Klicken Sie auf **Bedingung hinzufügen** und wiederholen Sie die oben genannten Schritte, um nach zusätzlichen Feldern zu sortieren.

   Die Anzahl der Felder, nach denen Sie sortieren möchten, wird links neben dem Symbol Sortieren in der oberen rechten Ecke der Symbolleiste angezeigt. Sie können nur Felder auswählen, die in den Spalten der Tabellenansicht angezeigt werden.

1. (Optional) Im **Sortieren von Datensätzen nach** und klicken Sie auf das **x** Symbol rechts neben einem Sortierfeld zum Entfernen der Sortierung

   Oder

   Klicks **Alle löschen** , um alle Felder aus der Sortierung zu entfernen.

1. Klicken Sie außerhalb der **Sortieren von Datensätzen nach** zum Schließen.

   ![](assets/sorting-in-table-view.png)

   Die in der Tabelle angezeigten Informationen werden nach den von Ihnen ausgewählten Kriterien sortiert.

   In den für die Sortierung ausgewählten Feldern wird ein Sortiersymbol angezeigt, gefolgt von einer Zahl, die die Reihenfolge angibt, in der die Sortierung angewendet wird.

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->
