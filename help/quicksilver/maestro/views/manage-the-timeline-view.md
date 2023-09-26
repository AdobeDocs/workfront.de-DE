---
title: Verwalten der Timeline-Ansicht
description: Sie können Datensätze in einer Timeline-Ansicht anzeigen, wenn Sie auf die Seite vom Typ Datensatz in Adobe Maestro zugreifen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 1%

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

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Datensätze in einer Timeline-Ansicht anzeigen, wenn Sie auf die Seite vom Typ Datensatz in Adobe Maestro zugreifen.

Weitere Informationen zu Maestro-Ansichten finden Sie unter [Verwalten von Datensatzansichten in Adobe Maestro](../views/manage-record-views.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
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
<p>Beliebig</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Beliebig</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Beliebig</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/grant-access.md">Zugriff auf Adobe Maestro gewähren</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

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

Beim Erstellen einer Timeline-Ansicht werden standardmäßig alle Datensätze des ausgewählten Datensatztyps in einer Timeline als Balken angezeigt.

So verwalten Sie eine Timeline-Ansicht:

1. Rufen Sie die Seite mit dem Datensatztyp auf, für die Sie die Timeline anzeigen möchten.
1. Erstellen Sie eine Timeline-Ansicht, wie im Artikel beschrieben [Verwalten von Datensatzansichten](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   Die Datensätze, die dem von Ihnen ausgewählten Datensatztyp zugeordnet sind, werden in einer chronologischen Zeitleiste als Balken angezeigt.

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

1. Aktualisieren Sie die folgenden Ansichtselemente wie in den folgenden Unterabschnitten beschrieben:
   * [Filter](#add-filters)
   * [Gruppierung](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [Einstellungen](#edit-the-timeline-view-settings)

### Filter hinzufügen

Mithilfe von Filtern können Sie die Anzahl der auf dem Bildschirm angezeigten Informationen verringern.

Beachten Sie beim Arbeiten mit Filtern in der Timeline-Ansicht Folgendes:

<!-- this list is almost identical to the one for the table view - update both-->

* Die Filter, die Sie für die Timeline-Ansicht erstellen, funktionieren unabhängig von den Filtern in der Tabellenansicht, wenn sie auf denselben Datensatztyp angewendet werden.

* Die Filter sind für die ausgewählte Ansicht eindeutig. Bei zwei Timeline-Ansichten desselben Datensatztyps können unterschiedliche Filter angewendet werden. Zwei Benutzer, die sich dieselbe Timeline-Ansicht ansehen, sehen denselben Filter, der derzeit angewendet wird.

* Sie können die erstellten Filter nicht benennen und auf eine Timeline-Ansicht anwenden.

* Durch das Entfernen von Filtern werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp wie Sie zugreifen, und es wird die gleiche Ansicht verwendet, die Sie verwenden.

Das Hinzufügen von Filtern in der Timeline-Ansicht ist mit dem Hinzufügen von Filtern in der Tabellenansicht identisch.

Weitere Informationen finden Sie im Abschnitt &quot;Filter hinzufügen&quot;im Artikel [Tabellenansicht verwalten](../views/manage-the-table-view.md).

### Gruppierung hinzufügen

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


Sie können Datensätze nach ähnlichen Informationen gruppieren, wenn Sie eine Gruppierung auf eine Ansicht anwenden.

Beachten Sie beim Arbeiten mit Gruppierungen in der Timeline-Ansicht Folgendes:

* Sie können Gruppierungen sowohl in der Tabellen- als auch in der Timeline-Ansicht anwenden. Die Gruppierungen der Tabellenansicht sind unabhängig von denen in der Timeline-Ansicht desselben Datensatztyps.
* Sie können in einer Maestro-Ansicht drei Gruppierungsebenen anwenden. Die Datensätze werden in der von Ihnen ausgewählten Reihenfolge gruppiert.
* Bei Verwendung der API können Sie bis zu 4 Gruppierungsebenen verwenden.

So fügen Sie eine Gruppierung hinzu:

1. Erstellen Sie eine Timeline-Ansicht, wie im Artikel beschrieben [Verwalten von Datensatzansichten](../views/manage-record-views.md).
1. Klicks **Gruppierung**.

   ![](assets/grouping-ui-timeline-view.png)

1. Klicken Sie auf eines der vorgeschlagenen Felder oder auf **Andere Felder auswählen** und suchen Sie nach einem anderen Feld und klicken Sie dann darauf, wenn es in der Liste angezeigt wird.

   >[!TIP]
   >
   >Verknüpfte Felder können nicht ausgewählt werden.

   Die Gruppierung wird automatisch auf die Timeline angewendet und Datensätze werden innerhalb des Gruppierungsfelds angezeigt. Die Anzahl der Elemente in einer Gruppierung wird in der Gruppierungszeile angezeigt.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Optional) Wiederholen Sie die obigen Schritte, um bis zu 3 Gruppierungen hinzuzufügen.

   Die Anzahl der angewendeten Gruppierungen wird links neben dem Gruppierungssymbol in der oberen rechten Ecke der Symbolleiste angezeigt.

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Optional) Klicken Sie auf die **x** rechts neben einer Gruppierung, um die Gruppierung zu entfernen

   Oder

   Klicks **Alle löschen** um alle Gruppierungen zu entfernen.

1. Klicken Sie außerhalb der **Gruppiert Datensätze nach** zum Schließen.

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Einstellungen der Timeline-Ansicht bearbeiten {#edit-the-timeline-view-settings}

Aktualisieren Sie die Einstellungen der Timeline-Ansicht, um anzugeben, welche Informationen im Timeline-Abschnitt der Ansicht angezeigt werden.

1. Erstellen Sie eine Timeline-Ansicht, wie im Artikel beschrieben [Verwalten von Datensatzansichten](../views/manage-record-views.md).
1. Klicks **Einstellungen**.
1. Klicks **Datum und Uhrzeit** im linken Bereich und wählen Sie dann eine **Startdatum** und **Enddatum** in der Timeline angezeigt. Sie können das standardmäßige Start- und Enddatum oder ein beliebiges Datumsfeld auswählen. Die den Datensätzen entsprechenden Balken beginnen am Datum, das Sie für das Startdatum angeben, und enden an dem Datum, das dem Enddatum entspricht.

   >[!NOTE]
   >
   >    Datensätze, die keine Werte für das Start- oder Enddatum oder ein Startdatum nach dem Enddatum haben, werden nicht in der Timeline-Ansicht angezeigt.


1. Klicks **Datensatzdetails** , um anzugeben, welche Felder in den Datensatz-Bards angezeigt werden sollen.

   Das Feld Name ist standardmäßig ausgewählt.

1. Klicks **Feld hinzufügen** , um bis zu 4 Felder zu den Datensatzbalken hinzuzufügen.
1. Klicken Sie in die **Suchfelder** und klicken Sie auf das Feld, das Sie hinzufügen möchten.

   >[!TIP]
   >
   >   * Sie müssen die Felder erstellen, bevor Sie sie zu den Datensatzbalken hinzufügen können.
   > 
   >   * Sie müssen mindestens ein Feld ausgewählt haben. **Name** ist standardmäßig ausgewählt.

   Eine Vorschau der Balken wird auf der rechten Seite angezeigt.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Klicken Sie auf **Speichern**.

   Die Datensätze werden in der Timeline-Ansicht mit den von Ihnen ausgewählten Spezifikationen angezeigt.


