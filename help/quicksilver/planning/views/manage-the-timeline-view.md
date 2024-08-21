---
title: Verwalten der Timeline-Ansicht
description: Rufen Sie Datensätze in einer Timeline-Ansicht auf der Seite Adobe Workfront Planning record type auf und bearbeiten Sie sie. Passen Sie die Timeline mit Filtern, Gruppierungen und Einstellungen an. Mit der Aufschlüsselungsfunktion können Sie verbundene Datensätze anzeigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '1941'
ht-degree: 0%

---

# Verwalten der Timeline-Ansicht

<!--
title: Manage the timeline view 
description: You can display records in a timeline view, when accessing the record type page in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Sie können Datensätze in einer Timeline-Ansicht anzeigen, wenn Sie auf die Seite vom Typ Datensatz in der Adobe Workfront-Planung zugreifen.

Weitere Informationen zu Datensatzansichten finden Sie unter [Ansichten von Datensätzen verwalten](/help/quicksilver/planning/views/manage-record-views.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> Es gibt keine Zugriffskontrollen für die Adobe Workfront-Planung</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für eine Ansicht verwalten</p>  
   <p>Berechtigungen für eine Ansicht anzeigen, um die Anzeigeeinstellungen vorübergehend zu ändern</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--EDIT PERMISSIONS AND ACCESS AND REPLACE THE table above with the following table at Planning GA release: 
## Access requirements

You must have the following to be able to access Workfront Planning: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following new Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning plan*</p></td>
   <td>
<p>Any of the following Workfront Planning plans:</p>
<ul><li>Planning</li>
<li>Planning Plus</li>
</ul>
<p>For more information about what is included in each Workfront Planning plan, see <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront pricing and packaging</a>. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <ul><li><p>Any, to view Workfront Planning information</p></li>
   <li><p>Standard, to create workspaces</p></li></ul>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a> and and <a href="../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md">Assign users to a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

*********ensure that the link ^^^^^^^^above^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************

-->


## Verwalten einer Timeline-Ansicht {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

Beim Erstellen einer Timeline-Ansicht werden alle Datensätze des ausgewählten Datensatztyps in einer chronologischen Timeline angezeigt.

Beachten Sie Folgendes:

* Sie können eine Timeline-Ansicht nur erstellen, wenn mindestens zwei Datumsfelder mit einem Datensatztyp verknüpft sind. Wenn einem Datensatztyp ein oder keine Datumsfelder zugeordnet sind, ist die Option Timeline-Ansicht abgeblendet.

  Sie können beim Erstellen einer Timeline-Ansicht aus den folgenden Datumsfeldern auswählen:

   * Datensatzdaten
   * Systemgenerierte Felder aufzeichnen: Erstellungsdatum, Datum der letzten Änderung
   * Sucht Daten aus verbundenen Datensätzen oder Objekttypen.
* Je nach Datum, das mit den Datensätzen verknüpft ist, werden in den folgenden Szenarien einige Datensätze möglicherweise nicht in der Timeline-Ansicht angezeigt:

   * Wenn Start- und Enddaten keine Werte haben
   * Wenn das Start- oder das Enddatum keinen Wert haben
   * Wenn das Startdatum nach dem Enddatum liegt

So verwalten Sie eine Timeline-Ansicht:

1. Rufen Sie die Seite mit dem Datensatztyp auf, für die Sie die Timeline anzeigen möchten.
1. Erstellen Sie eine Timeline-Ansicht, wie im Artikel [Ansichten von Datensätzen verwalten](/help/quicksilver/planning/views/manage-record-views.md) beschrieben.

   ![](assets/timeline-view-example.png)

   Die Datensätze, die dem von Ihnen ausgewählten Datensatztyp zugeordnet sind, werden in einer Timeline als Balken angezeigt und sind standardmäßig in chronologischer Reihenfolge ihres Startdatums sortiert.

   >[!TIP]
   >
   >    Die Sortierung der Datensätze in der Timeline ist in der Ansicht &quot;Kompakt&quot;nicht sichtbar.

1. (Optional und bedingt) Wenn der Datensatzname abgeschnitten ist, halten Sie den Mauszeiger über eine Datensatzleiste, um den vollständigen Namen des Datensatzes und zusätzliche Informationen anzuzeigen.

1. Führen Sie einen der folgenden Schritte aus, um durch die Timeline zu navigieren:

   * Klicken Sie auf die Symbole links und rechts oder verwenden Sie den horizontalen Bildlauf, um in der Timeline rückwärts und vorwärts zu wechseln. Beim Aktualisieren der Seite wird der ausgewählte Zeitraum beibehalten.
   * Klicken Sie auf **Heute** , um die Timeline auf das aktuelle Datum zu zentrieren.
   * Wählen Sie eine der folgenden Optionen aus dem Dropdown-Menü für Zeitrahmen aus, um die Zeitabstände zu aktualisieren:

      * Jahr
      * Quartal
      * Monat
1. Klicken Sie auf die Ansicht **Zur Standardansicht wechseln** , um Datensätze in separaten Zeilen anzuzeigen <!--check to see if they updated the name of the setting here-->

   Oder

   Klicken Sie auf **Zur Kompaktansicht wechseln** , um die Datensätze anzuzeigen, deren Daten sich nicht in derselben Zeile überschneiden. <!--check to see if they updated the name of the setting here-->

   Datensätze werden standardmäßig in der Compact-Ansicht angezeigt.

1. Führen Sie die folgenden Schritte aus, um schnell nach Datensätzen zu suchen, die einem Keyword entsprechen:

   1. Klicken Sie auf das Symbol **Suchen** ![](assets/search-icon.png) und beginnen Sie mit der Eingabe eines Suchbegriffs, das mit einem Feld eines Datensatzes verknüpft ist, das auf dem Bildschirm angezeigt wird. Die Anzahl der richtigen Übereinstimmungen wird neben dem Suchelement angezeigt und der Datensatz mit der richtigen Übereinstimmung wird hervorgehoben.

      ![](assets/search-box-and-results-timeline-view.png)

      Sie können beliebige Wörter oder Sonderzeichen verwenden, die auf dem Bildschirm sichtbar sind.

      Sie können keine Suchbegriffe verwenden, die Feldern zugeordnet sind, die nicht in der Timeline-Ansicht angezeigt werden.

   1. Drücken Sie die Eingabetaste auf Ihrer Tastatur, um zum nächsten gefundenen Feld zu wechseln.
   1. (Optional) Wenn mehrere Übereinstimmungen vorliegen, klicken Sie auf die Pfeile nach oben und unten rechts neben dem Suchbegriff, um alle Übereinstimmungen in der Tabelle zu finden.
   1. Klicken Sie im Suchfeld auf das Symbol **x** , um den Suchbegriff zu löschen.

1. Aktualisieren Sie die folgenden Ansichtselemente wie in den folgenden Unterabschnitten beschrieben:
   * [Filter](#add-filters)
   * [Gruppierung](#add-grouping)
   * [Einstellungen](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### Filter hinzufügen

Mithilfe von Filtern können Sie die Anzahl der auf dem Bildschirm angezeigten Informationen verringern.

Beachten Sie beim Arbeiten mit Filtern in der Timeline-Ansicht Folgendes:

<!-- this list is almost identical to the one for the table view - update both-->

* Die Filter, die Sie für eine Timeline-Ansicht erstellen, funktionieren unabhängig von den Filtern in jeder anderen Ansicht, die auf denselben Datensatztyp angewendet wird.

* Die Filter sind für die ausgewählte Ansicht eindeutig. Bei zwei Timeline-Ansichten desselben Datensatztyps können unterschiedliche Filter angewendet werden.

* Zwei Benutzer, die sich dieselbe Timeline-Ansicht ansehen, sehen denselben Filter, der derzeit angewendet wird.

* Sie können die von Ihnen erstellten Filter nicht für eine Timeline-Ansicht benennen.

* Wenn Sie Filter entfernen, werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp zugreifen wie Sie und die dieselbe Ansicht wie Sie anzeigen.

* Das Hinzufügen von Filtern in der Timeline-Ansicht ist mit dem Hinzufügen von Filtern in der Tabellenansicht identisch.

  Weitere Informationen finden Sie im Abschnitt &quot;Filter hinzufügen&quot;im Artikel [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

* Sie können nach verbundenen Datensatzfeldern oder Suchfeldern filtern.
* Sie können nach Suchfeldern filtern, die mehrere Werte anzeigen.


### Gruppierung hinzufügen

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

Sie können Datensätze nach ähnlichen Informationen gruppieren, wenn Sie eine Gruppierung auf eine Ansicht anwenden.

Das Hinzufügen von Gruppierungen in der Timeline-Ansicht ähnelt dem Hinzufügen von Gruppierungen zur Tabellenansicht.

Beachten Sie beim Arbeiten mit Gruppierungen in der Timeline-Ansicht Folgendes:

* Sie können Gruppierungen sowohl in der Tabellen- als auch in der Timeline-Ansicht anwenden. Die Gruppierungen der Tabellenansicht sind unabhängig von denen in der Timeline-Ansicht desselben Datensatztyps.
* Sie können in einer Ansicht drei Gruppierungsebenen anwenden. Die Datensätze werden in der von Ihnen ausgewählten Reihenfolge gruppiert.
&lt;!—* Bei Verwendung der API können Sie bis zu 4 Gruppierungsebenen verwenden. —jetzt mit diesem hier abgleichen—>
* Die Gruppierungen unterscheiden sich je nach ausgewählter Ansicht. Bei zwei Tabellenansichten desselben Datensatztyps können unterschiedliche Gruppierungen angewendet werden. Zwei Benutzer, die sich dieselbe Tabellenansicht ansehen, sehen dieselbe Gruppierung, die derzeit angewendet wird.
* Sie können die für eine Tabellenansicht erstellten Gruppierungen nicht benennen.
* Durch das Entfernen von Gruppierungen werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp zugreifen wie Sie und die dieselbe Ansicht wie Sie anzeigen.
* Sie können die unter einer Gruppierung aufgelisteten Datensätze bearbeiten.
* Sie können nach verbundenen Datensatzfeldern oder Suchfeldern gruppieren.
* Wenn Sie nach Suchfeldern mit mehreren Werten gruppieren (die nicht von einem Aggregator zusammengefasst wurden), werden Datensätze nach jeder eindeutigen Kombination von Feldwerten gruppiert.
* Sie können auf ein Feld verweisen, das bis zu vier Ebenen vom aktuellen Datensatztyp entfernt ist. Wenn Sie beispielsweise eine Gruppierung für einen Aktivitäts-Record-Typ erstellen und die Aktivität mit dem Produktdatensatz-Typ verbunden ist, der mit dem Campaign-Datensatz-Typ verbunden ist, der mit einem Workfront-Projekt verbunden ist, können Sie den Projektstatus in der für den Aktivitäts-Record-Typ erstellten Gruppierung referenzieren.
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

So fügen Sie eine Gruppierung in der Timeline-Ansicht hinzu:

1. Erstellen Sie eine Timeline-Ansicht für einen Datensatztyp, wie im Artikel [Ansichten von Datensätzen verwalten](/help/quicksilver/planning/views/manage-record-views.md) beschrieben.
1. Klicken Sie oben rechts in der Timeline-Ansicht auf **Gruppierung** .

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. Klicken Sie auf eines der vorgeschlagenen Felder oder auf **Ein anderes Feld auswählen**, suchen Sie nach einem anderen Feld und klicken Sie dann auf dieses Feld, wenn es in der Liste angezeigt wird.

   Die Gruppierung wird automatisch auf die Timeline angewendet und Datensätze werden innerhalb des Gruppierungsfelds angezeigt.

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. (Optional) Wiederholen Sie die obigen Schritte, um bis zu 3 Gruppierungen hinzuzufügen.

   Die Anzahl der für die Gruppierung ausgewählten Felder wird neben dem Gruppierungssymbol angezeigt.

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. (Optional) Klicken Sie im Feld **Datensatz gruppieren nach** auf das Symbol **x** rechts neben einem Feld, das für die Gruppierung ausgewählt wurde, um die Gruppierung zu entfernen.

   Oder

   Klicken Sie auf **Alle löschen** , um alle Felder zu entfernen.

1. Klicken Sie auf außerhalb des Felds **Gruppeneinträge nach** , um sie zu schließen.
1. (Optional) Klicken Sie auf **Einstellungen** und dann auf **Farbe** , um Farbcode-Gruppierungen vorzunehmen. Weitere Informationen finden Sie im Abschnitt [Einstellungen für die Timeline-Ansicht bearbeiten](#edit-the-timeline-view-settings) in diesem Artikel.
   <!--1. (Optional) Click **Breakdown** to display connected records on the timeline. For information, see the section [Use the Breakdown feature to display connected records in the timeline view](#break-down-connected-records-in-the-timeline-view)-->

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### Einstellungen der Timeline-Ansicht bearbeiten {#edit-the-timeline-view-settings}

Aktualisieren Sie die Einstellungen der Timeline-Ansicht, um anzugeben, welche Informationen im Timeline-Abschnitt der Ansicht angezeigt werden.

1. Erstellen Sie eine Timeline-Ansicht für einen Datensatztyp, wie im Artikel [Ansichten von Datensätzen verwalten](/help/quicksilver/planning/views/manage-record-views.md) beschrieben.
1. Klicken Sie auf **Einstellungen**.
1. Klicken Sie im linken Bereich auf **Datum und Uhrzeit** und wählen Sie dann ein **Startdatum** und ein **Enddatum** aus, die in der Timeline angezeigt werden sollen. Sie können das standardmäßige Start- und Enddatum oder ein beliebiges Datumsfeld auswählen. Die den Datensätzen entsprechenden Balken beginnen am Datum, das Sie für das Startdatum angeben, und enden an dem Datum, das dem Enddatum entspricht.

   >[!NOTE]
   >
   >Datensätze, die keine Werte für das Start- oder Enddatum oder ein Startdatum nach dem Enddatum haben, werden nicht in der Timeline-Ansicht angezeigt.

1. Klicken Sie im linken Bereich auf **Balkenstil** , um anzugeben, welche Felder in den Datensatzbalken angezeigt werden sollen.

   Das in der Tabellenansicht des Datensatzes definierte primäre Feld (oder Titel) wird standardmäßig ausgewählt. <!--adjust this when the primary field is released??-->

1. (Optional und bedingt) Wenn Sie den Datensätzen Miniaturansichten hinzugefügt haben, wählen Sie die Option Miniatur aus, um das den Datensätzen zugeordnete Bild in der Symbolleiste anzuzeigen.

   >[!NOTE]
   >
   >    Sie müssen zuerst Miniaturansichten in der Tabellenansicht hinzufügen, bevor Sie sie in der Timeline-Ansicht anzeigen können. Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Klicken Sie auf **Feld hinzufügen** , um den Datensatzleisten bis zu 4 Felder hinzuzufügen.
1. Klicken Sie in das Feld **Suchfelder** und klicken Sie auf das Feld, das Sie hinzufügen möchten.

   >[!TIP]
   >
   >   * Sie müssen die Felder erstellen, bevor Sie sie zu den Datensatzbalken hinzufügen können.
   > 
   >   * Sie müssen mindestens ein Feld ausgewählt haben. **Name** ist standardmäßig ausgewählt.

   Eine Vorschau der Balken wird auf der rechten Seite angezeigt.

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. Klicken Sie im linken Bereich auf **Farbe** , um die Farben der Datensätze und Gruppierungen in der Timeline anzupassen.

   ![](assets/color-tab-timeline-view.png)

1. (Bedingt und optional) Wenn Sie der Timeline-Ansicht eine Gruppierung hinzugefügt haben, wählen Sie aus den folgenden Optionen aus, um eine Farbe für die Gruppierung im Abschnitt **Gruppierungsfarbe festlegen** festzulegen:

   * **Standard (grau)**: Die Farbe der Gruppierungen ist auf grau eingestellt. Dies ist die Standardeinstellung.
   * **Feldwerte**: Die Farbe der Gruppierungen stimmt mit der Farbe des Felds überein, nach dem Sie die Gruppe bilden.

     >[!NOTE]
     >
     >    * Sie können die Farbe nur mit Feldern mit farbcodierten Optionen abgleichen. Beispielsweise können Sie die Farbe mit Statusfeldern oder Feldern mit Optionen, die Farben zugeordnet sind, abgleichen.
     >    
     >    * Sie können die Farbe nicht mit Suchfeldern aus verknüpften Datensätzen oder Objekttypen abgleichen.


   Beispielsweise können Felder mit Mehrfachauswahl oder Einzelauswahl farbkodierte Optionen aufweisen.

   Wenn Sie eine Gruppierung nach Feldern ohne farbkodierte Optionen durchführen, bleibt die Gruppierungsfarbe grau.

   >[!TIP]
   >
   >Wenn Sie der Timeline-Ansicht keine Gruppierungen hinzugefügt haben, wird dieser Abschnitt nicht angezeigt.

1. Wählen Sie im Abschnitt **Datensatzfarbe festlegen** aus den folgenden Optionen aus, um eine Farbe für die Datensätze festzulegen:

   * **Record type**: Die Farbe der Datensätze entspricht der Farbe des von Ihnen ausgewählten Datensatztyps. Dies ist die Standardoption.
   * **Feldwerte**: Die Farbe der Datensätze entspricht der Farbe eines von Ihnen angegebenen Felds. Fahren Sie mit Schritt 10 fort. <!--ensure this stays accurate-->
   * **Gruppierung**: Die Farbe der Datensätze entspricht der Farbe, die Sie für die Gruppierungen angegeben haben. Diese Option ist abgeblendet, wenn Sie keine Gruppierungen auf die Timeline-Ansicht angewendet haben.
   * **None**: Datensätze werden in einer weißen Leiste angezeigt.

1. (Bedingt) Wenn Sie **Feldwerte** für die Datensatzfarben ausgewählt haben, wählen Sie ein Feld aus dem Dropdownmenü **Datensatzfarbe mit** abgleichen aus.

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   Im Dropdown-Menü werden nur Felder mit farbcodierten Optionen angezeigt.

   Beispielsweise können Felder mit Mehrfachauswahl oder Einzelauswahl farbkodierte Optionen aufweisen.

   Wenn Sie kein Feld mit farbcodierten Optionen für den ausgewählten Datensatztyp haben, ist diese Option abgeblendet.

1. Klicken Sie auf **Speichern**.

   Die Datensätze werden in der Timeline-Ansicht mit den von Ihnen ausgewählten Spezifikationen angezeigt.

<!--
### Use the Breakdown feature to display connected records in the timeline view

You can display connected records in a record's timeline view by using the Breakdown feature. Breaking down records by their connections allows you to view the timelines of other connected records and understand how they might affect the performance and deadlines of your records. 

#### Considerations when using the Breakdown feature

* You can display connected records or objects under the records of the selected record type in the timeline view. 
* You can display the following in the timeline view, using the Breakdown feature:
    * Workfront Planning records connected to the selected record type. 
    * Workfront (*************or AEM Assets*************)  object types connected to the selected record type.
    * Workfront Planning records or objects from other application that are connected to records connected to the selected record type. 
    
        For example, you might connect campaigns to portfolios. In addition, you might connect  another record type, products, with projects, as well as with campaigns. When you build the campaign timeline view, you can break down the campaigns by portfolios, products, and projects. 

* You cannot display object types that are connected only to Workfront objects in Workfront, but are not connected to a Workfront Planning record type. You can only display object or record types that are connected in Workfront Planning. 

    For example, tasks, are connected to projects in Workfront. Using the Breakdown feature, you can display projects that are connected to campaigns in Planning, but not tasks connected to projects in Workfront. 

    If you want to display both portfolios and projects in the timeline view of a Workfront Planning record type, both the portfolios and the projects must be connected to the Planning record or to a record connected to the Planning record whose timeline view you are managing.
* You can only display record types that are associated with at least two date fields. 
* The date fields for the record types you want to display in the timeline view must be visible in the table view of the selected record type, as lookup fields. 
* The Start and End dates of the record types you want to display in the timeline view must by in chronological order. For example, if a record has a Start date of January 31 and an End date of January 1, it does not display in the timeline view. For more information, see the section [Manage a timeline view](#manage-a-timeline-view) in this article. 
* There is a limit of 5 record types that you can include in a record's breakdown. 


#### Break down connected records in the timeline view

1. Create a timeline view for a record type, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 
1. Click **Breakdown**.
1. Expand the **Select a linked record type** box and select a connected record type. (**************add new screen shot***************)

    ![](assets/breakdown-picker-and-button-on-timeline.png)

    >[!TIP]
    >
    >    If you do not have any connected records, or if the connected records do not have at least two date fields, the **Select a linked record type** box is not available.

1. Choose a **Start date** and an **End date field**.

    >[!TIP]
    >
    >    The Start and End dates must be sequential. If the End date is before the Start date, no records will display in the timeline. 

    A right-pointing arrow displays on the selected record's bar in the timeline, if they they are connected with other records. 

    ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)    


1. (Optional) Repeat the steps above to add more connected records. 

    >[!TIP]
    >
    >    You can add up to 5 connected records in a timeline using the Breakdown feature. 


-->