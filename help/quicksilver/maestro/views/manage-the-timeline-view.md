---
title: Verwalten der Timeline-Ansicht
description: Sie können Datensätze in einer Timeline-Ansicht anzeigen, wenn Sie auf die Seite vom Typ Datensatz in Adobe Maestro zugreifen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: ef313bf912c65b9b316bd7403235ccf6f05a0ac6
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 0%

---

# Verwalten der Timeline-Ansicht

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Sie können Datensätze in einer Timeline-Ansicht anzeigen, wenn Sie auf die Seite vom Typ Datensatz in Adobe Maestro zugreifen.

Weitere Informationen zu Maestro-Ansichten finden Sie unter [Verwalten von Datensatzansichten in Adobe Maestro](../views/manage-record-views.md).

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
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
  </td>
  </tr>

<tr>
   <td role="rowheader">Konfiguration der Zugriffsebene</td>
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Maestro </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für die Ansicht verwalten</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


## Verwalten einer Timeline-Ansicht {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Beim Erstellen einer Timeline-Ansicht werden alle Datensätze des ausgewählten Datensatztyps in einer chronologischen Timeline angezeigt.

Beachten Sie Folgendes:

* Sie können eine Timeline-Ansicht nur erstellen, wenn mindestens zwei Datumsfelder mit einem Datensatztyp verknüpft sind. Wenn einem Datensatztyp ein oder keine Datumsfelder zugeordnet sind, ist die Option Timeline-Ansicht abgeblendet.
* Je nach Datum, das mit den Datensätzen verknüpft ist, werden in den folgenden Szenarien einige Datensätze möglicherweise nicht in der Timeline-Ansicht angezeigt:

   * Wenn Start- und Enddaten keine Werte haben
   * Wenn das Start- oder das Enddatum keinen Wert haben
   * Wenn das Startdatum nach dem Enddatum liegt

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

So verwalten Sie eine Timeline-Ansicht:

1. Rufen Sie die Seite mit dem Datensatztyp auf, für die Sie die Timeline anzeigen möchten.
1. Erstellen Sie eine Timeline-Ansicht, wie im Artikel beschrieben [Verwalten von Datensatzansichten](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Die Datensätze, die dem von Ihnen ausgewählten Datensatztyp zugeordnet sind, werden in einer Timeline als Balken angezeigt und sind standardmäßig in chronologischer Reihenfolge ihres Startdatums sortiert.

   >[!TIP]
   >
   >    Die Sortierung der Datensätze in der Timeline ist in der Ansicht &quot;Kompakt&quot;nicht sichtbar.


1. Führen Sie einen der folgenden Schritte aus, um durch die Timeline zu navigieren:

   * Klicken Sie auf die Symbole links und rechts oder verwenden Sie den horizontalen Bildlauf, um in der Timeline rückwärts und vorwärts zu wechseln.
   * Klicks **Heute** , um die Timeline auf das aktuelle Datum zu zentrieren.
   * Wählen Sie eine der folgenden Optionen aus dem Dropdown-Menü für den Zeitrahmen aus, um die Zeitabstände zu aktualisieren:

      * Jahr
      * Quartal
      * Monat
1. Klicks **In Standard wechseln** Anzeigen von Datensätzen in separaten Zeilen <!--check to see if they updated the name of the setting here-->

   Oder

   Klicks **Zur Kompaktansicht wechseln** um die Datensätze anzuzeigen, deren Daten sich nicht in derselben Zeile überschneiden. <!--check to see if they updated the name of the setting here-->

   Datensätze werden standardmäßig in der Compact-Ansicht angezeigt.

1. Führen Sie die folgenden Schritte aus, um schnell nach Datensätzen zu suchen, die einem Keyword entsprechen:

   1. Klicken Sie auf **Suche** icon ![](assets/search-icon.png) und beginnen Sie mit der Eingabe eines Suchbegriffs, das mit einem Feld eines Datensatzes verknüpft ist, das auf dem Bildschirm angezeigt wird. Die Anzahl der richtigen Übereinstimmungen wird neben dem Suchelement angezeigt und der Datensatz mit der richtigen Übereinstimmung wird hervorgehoben.

      ![](assets/search-box-and-results-timeline-view.png)

      Sie können beliebige Wörter oder Sonderzeichen verwenden, die auf dem Bildschirm sichtbar sind.

      Sie können keine Suchbegriffe verwenden, die Feldern zugeordnet sind, die nicht in der Timeline-Ansicht angezeigt werden.

   1. Drücken Sie die Eingabetaste auf Ihrer Tastatur, um zum nächsten gefundenen Feld zu wechseln.
   1. (Optional) Wenn mehrere Übereinstimmungen vorliegen, klicken Sie auf die Pfeile nach oben und unten rechts neben dem Suchbegriff, um alle Übereinstimmungen in der Tabelle zu finden.
   1. Klicken Sie auf **x** in das Suchfeld ein, um den Suchbegriff zu löschen.

1. Aktualisieren Sie die folgenden Ansichtselemente wie in den folgenden Unterabschnitten beschrieben:
   * [Filter](#add-filters)
   * [Gruppierung](#add-grouping)
   * [Einstellungen](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### Filter hinzufügen

Mithilfe von Filtern können Sie die Anzahl der auf dem Bildschirm angezeigten Informationen verringern.

Beachten Sie beim Arbeiten mit Filtern in der Timeline-Ansicht Folgendes:

<!-- this list is almost identical to the one for the table view - update both-->

* Die Filter, die Sie für die Timeline-Ansicht erstellen, funktionieren unabhängig von den Filtern in der Tabellenansicht, wenn sie auf denselben Datensatztyp angewendet werden.

* Die Filter sind für die ausgewählte Ansicht eindeutig. Bei zwei Timeline-Ansichten desselben Datensatztyps können unterschiedliche Filter angewendet werden. Zwei Benutzer, die sich dieselbe Timeline-Ansicht ansehen, sehen denselben Filter, der derzeit angewendet wird.

* Sie können die von Ihnen erstellten Filter nicht für eine Timeline-Ansicht benennen.

* Wenn Sie Filter entfernen, werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp zugreifen wie Sie und die dieselbe Ansicht wie Sie anzeigen.

* Das Hinzufügen von Filtern in der Timeline-Ansicht ist mit dem Hinzufügen von Filtern in der Tabellenansicht identisch.

  Weitere Informationen finden Sie im Abschnitt &quot;Filter hinzufügen&quot;im Artikel [Tabellenansicht verwalten](../views/manage-the-table-view.md).

### Gruppierung hinzufügen

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Sie können Datensätze nach ähnlichen Informationen gruppieren, wenn Sie eine Gruppierung auf eine Ansicht anwenden.

Das Hinzufügen von Gruppierungen in der Timeline-Ansicht ähnelt dem Hinzufügen von Gruppierungen zur Tabellenansicht.

Beachten Sie beim Arbeiten mit Gruppierungen in der Timeline-Ansicht Folgendes:

* Sie können Gruppierungen sowohl in der Tabellen- als auch in der Timeline-Ansicht anwenden. Die Gruppierungen der Tabellenansicht sind unabhängig von denen in der Timeline-Ansicht desselben Datensatztyps.
* Sie können in einer Maestro-Ansicht drei Gruppierungsebenen anwenden. Die Datensätze werden in der von Ihnen ausgewählten Reihenfolge gruppiert.
* Bei Verwendung der API können Sie bis zu 4 Gruppierungsebenen verwenden.
* Die Gruppierungen unterscheiden sich je nach ausgewählter Ansicht. Bei zwei Timeline-Ansichten desselben Datensatztyps können unterschiedliche Gruppierungen angewendet werden. Zwei Benutzer, die sich dieselbe Timeline-Ansicht ansehen, sehen dieselbe Gruppierung, die derzeit angewendet wird.
* Sie können die für eine Timeline-Ansicht erstellten Gruppierungen nicht benennen.
* Durch das Entfernen von Gruppierungen werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp zugreifen wie Sie und die dieselbe Ansicht wie Sie anzeigen.

So fügen Sie eine Gruppierung in der Timeline-Ansicht hinzu:

1. Erstellen Sie eine Timeline-Ansicht für einen Datensatztyp, wie im Artikel beschrieben [Verwalten von Datensatzansichten](../views/manage-record-views.md).
1. Klicks **Gruppierung** in der rechten oberen Ecke der Timeline-Ansicht.

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Klicken Sie auf eines der vorgeschlagenen Felder oder auf **Andere Felder auswählen**, suchen Sie nach einem anderen Feld und klicken Sie darauf, wenn es in der Liste angezeigt wird.

   Die Gruppierung wird automatisch auf die Timeline angewendet und Datensätze werden innerhalb des Gruppierungsfelds angezeigt.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Optional) Wiederholen Sie die obigen Schritte, um bis zu 3 Gruppierungen hinzuzufügen.

   Die Anzahl der für die Gruppierung ausgewählten Felder wird neben dem Gruppierungssymbol angezeigt.

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Optional) Innerhalb des **Gruppiert Datensätze nach** und klicken Sie auf das **x** rechts neben einem Feld, das zum Entfernen der Gruppierung ausgewählt wurde

   Oder

   Klicks **Alle löschen** um alle Felder zu entfernen.

1. Klicken Sie außerhalb der **Gruppiert Datensätze nach** zum Schließen.
1. (Optional) Klicken Sie auf **Einstellungen**, dann **Farbe** Farbcode-Gruppierungen. Weitere Informationen finden Sie unter [Einstellungen der Timeline-Ansicht bearbeiten](#edit-the-timeline-view-settings) in diesem Artikel beschrieben.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Einstellungen der Timeline-Ansicht bearbeiten {#edit-the-timeline-view-settings}

Aktualisieren Sie die Einstellungen der Timeline-Ansicht, um anzugeben, welche Informationen im Timeline-Abschnitt der Ansicht angezeigt werden.

1. Erstellen Sie eine Timeline-Ansicht für einen Datensatztyp, wie im Artikel beschrieben [Verwalten von Datensatzansichten](../views/manage-record-views.md).
1. Klicks **Einstellungen**.
1. Klicks **Datum und Uhrzeit** im linken Bereich und wählen Sie dann eine **Startdatum** und **Enddatum** in der Timeline angezeigt. Sie können das standardmäßige Start- und Enddatum oder ein beliebiges Datumsfeld auswählen. Die den Datensätzen entsprechenden Balken beginnen am Datum, das Sie für das Startdatum angeben, und enden an dem Datum, das dem Enddatum entspricht.

   >[!NOTE]
   >
   >Datensätze, die keine Werte für das Start- oder Enddatum oder ein Startdatum nach dem Enddatum haben, werden nicht in der Timeline-Ansicht angezeigt.

1. Klicks **Balkenstil** im linken Bereich, um anzugeben, welche Felder in den Datensatzleisten angezeigt werden sollen.

   Das Feld Name ist standardmäßig ausgewählt. <!--adjust this when the primary field is released??-->

1. (Optional und bedingt) Wenn Sie den Datensätzen Miniaturansichten hinzugefügt haben, wählen Sie die Option Miniatur aus, um das den Datensätzen zugeordnete Bild in der Symbolleiste anzuzeigen.

   >[!NOTE]
   >
   >    Sie müssen zuerst Miniaturansichten in der Tabellenansicht hinzufügen, bevor Sie sie in der Timeline-Ansicht anzeigen können. Weitere Informationen finden Sie unter [Miniaturansichten zu Datensätzen hinzufügen](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

1. Klicks **Feld hinzufügen** , um bis zu 4 Felder zu den Datensatzbalken hinzuzufügen.
1. Klicken Sie in die **Suchfelder** und klicken Sie auf das Feld, das Sie hinzufügen möchten.

   >[!TIP]
   >
   >   * Sie müssen die Felder erstellen, bevor Sie sie zu den Datensatzbalken hinzufügen können.
   > 
   >   * Sie müssen mindestens ein Feld ausgewählt haben. **Name** ist standardmäßig ausgewählt.

   Eine Vorschau der Balken wird auf der rechten Seite angezeigt.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Klicks **Farbe** im linken Bereich, um die Farben der Datensätze und Gruppierungen in der Timeline anzupassen.

   ![](assets/color-tab-timeline-view.png)

1. (Bedingt und optional) Wenn Sie der Timeline-Ansicht eine Gruppierung hinzugefügt haben, wählen Sie aus den folgenden Optionen aus, um eine Farbe für die Gruppierung im **Festlegen der Gruppierungsfarbe** Abschnitt:

   * **Standard (grau)**: Die Farbe der Gruppierungen ist auf grau eingestellt. Dies ist die Standardeinstellung.
   * **Feldwerte**: Die Farbe der Gruppierungen entspricht der Farbe des Felds, nach dem Sie die Gruppe bilden.
Sie können die Farbe der Gruppierungen nur mit Feldern mit farbcodierten Optionen abgleichen.

   Beispielsweise können Felder mit Mehrfachauswahl oder Einzelauswahl farbkodierte Optionen aufweisen.

   Wenn Sie eine Gruppierung nach Feldern ohne farbkodierte Optionen durchführen, bleibt die Gruppierungsfarbe grau.

   >[!TIP]
   >
   >Wenn Sie der Timeline-Ansicht keine Gruppierungen hinzugefügt haben, wird dieser Abschnitt nicht angezeigt.

1. Im **Datensatzfarbe festlegen** Wählen Sie aus den folgenden Optionen aus, um eine Farbe für die Datensätze festzulegen:

   * **Record Type**: Die Farbe der Datensätze entspricht der Farbe des von Ihnen ausgewählten Datensatztyps. Dies ist die Standardoption.
   * **Feldwerte**: Die Farbe der Datensätze entspricht der Farbe eines von Ihnen angegebenen Felds. Fahren Sie mit Schritt 10 fort. <!--ensure this stays accurate-->
   * **Gruppierung**: Die Farbe der Datensätze entspricht der Farbe, die Sie für die Gruppierungen angegeben haben. Diese Option ist abgeblendet, wenn Sie keine Gruppierungen auf die Timeline-Ansicht angewendet haben.
   * **Keines**: Datensätze werden in einer weißen Leiste angezeigt.

1. (Bedingt) Bei Auswahl von **Feldwerte** Wählen Sie für die Datensatzfarben ein Feld aus der **Übereinstimmung der Datensatzfarbe mit** Dropdown-Menü.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Im Dropdown-Menü werden nur Felder mit farbcodierten Optionen angezeigt.

   Beispielsweise können Felder mit Mehrfachauswahl oder Einzelauswahl farbkodierte Optionen aufweisen.

   Wenn Sie kein Feld mit farbcodierten Optionen für den ausgewählten Datensatztyp haben, ist diese Option abgeblendet.

1. Klicken Sie auf **Speichern**.

   Die Datensätze werden in der Timeline-Ansicht mit den von Ihnen ausgewählten Spezifikationen angezeigt.
