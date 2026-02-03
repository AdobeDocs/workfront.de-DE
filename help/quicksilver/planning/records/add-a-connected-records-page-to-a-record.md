---
title: Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz
description: Sie können Informationen aus verbundenen Datensätzen oder Objekten anzeigen, indem Sie einem Datensatz eine Registerkarte für eine Seite „Verbundene Datensätze“ hinzufügen. Dadurch werden die verbundenen Datensätze in einer Tabellenansicht zur Registerkarte hinzugefügt.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '2020'
ht-degree: 0%

---


# Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Sie können Informationen aus verbundenen Datensätzen oder Objekten anzeigen, indem Sie in Adobe Workfront Planning eine Registerkarte für eine Seite „Verbundene Datensätze“ zu einem Datensatz hinzufügen. Dadurch werden die verbundenen Datensätze in einer Tabellenansicht zur Registerkarte hinzugefügt.

Beachten Sie beim Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz Folgendes:

* Sie können eine Seite „Verbundene Datensätze“ zu einem Datensatz hinzufügen, nachdem Sie über die Tabellenansicht Datensätze oder Objekttypen mit dem Datensatztyp verbunden haben.

* Sie können eine Seite „Verbundene Datensätze“ aus dem Vorschaubereich eines Datensatzes oder aus der Seite des Datensatzes hinzufügen.

* Für einen bestimmten Datensatztyp kann nur eine verbundene Datensatzseite verwendet werden.

  Wenn Sie beispielsweise eine Seite mit verbundenen Datensätzen für eine Kampagne erstellen und die zugehörigen Personas anzeigen möchten, können Sie für Personas nur eine einzige Seite mit verbundenen Datensätzen haben.

* Verbundene Datensatzseiten zeigen nur die verbundenen Objekte oder Datensätze eines Objekts oder Datensatztyps an. Auf der Seite werden nicht alle Datensätze dieses Typs angezeigt.

* Je nachdem, welches Objekt oder welcher Datensatztyp auf der Seite Verbundene Datensätze angezeigt wird, können Sie diese mithilfe der folgenden Ansichten anzeigen:

   * Sie können verbundene Planungsdatensätze in den folgenden Ansichten anzeigen:
      * Tabelle
      * Timeline
      * Kalender
   * Sie können verbundene Workfront-Projekte in einer Listenansicht anzeigen.

* Sie können Seiten mit verbundenen Datensätzen für die folgenden verbundenen Datensatz- oder Objekttypen hinzufügen:

   * Workfront-Planungs-Datensatztypen
   * Workfront-Projekte

     Sie können die verbundenen Workfront-Projekte anzeigen, selbst wenn Sie nicht über die erforderlichen Zugriffsberechtigungen für sie in Workfront verfügen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront und beliebiges Planungspaket</p>
<p>Beliebiger Workflow und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
<tr>
<td> 
   <p> Zusätzliche Produkte</p> </td> 
   <td> 
   <p> Zusätzlich zu Adobe Workfront müssen Sie über Folgendes verfügen, wenn Sie eine verbundene Datensatzseite für Objekte aus den folgenden Programmen hinzufügen möchten:</p>
   <ul><li><p>Eine Adobe Experience Manager Assets-Lizenz und eine Integration zwischen AEM Assets und Workfront, um AEM-Assets mit Planungs-Datensatztypen zu verbinden.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront für Experience Manager Assets und Assets Essentials: Artikelindex</a>. </p></li>
   <li><p> Eine Adobe GenStudio for Performance Marketing-Lizenz zum Verbinden von Datensatztypen mit GenStudio Brands</p>
   <p>Weitere Informationen finden Sie <a href="https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/get-started">Erste Schritte mit Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <p>Beitragen von oder höhere Berechtigungen für einen Arbeitsbereich und einen Datensatztyp </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> 
  </td>
  </tr>   
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz

Sie müssen zunächst Datensatztypen mit anderen Datensatztypen oder Workfront-Projekten verbinden, bevor Sie einem Datensatz eine verbundene Datensatzseite hinzufügen.

1. Klicken Sie auf den Namen des Datensatzes, um ihn in jeder Ansicht einer Datensatztypseite zu öffnen.
1. Klicken Sie **einem der** Bereiche auf „Seite hinzufügen“:

   * Das Vorschaufenster des Datensatzes
   * Die Detailseite des Datensatzes, nachdem Sie auf das Symbol **In neuer Registerkarte öffnen** (![Details in einer neuen Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) in der oberen rechten Ecke der Vorschauseite geklickt haben.

   Das **Seite erstellen** wird geöffnet.

   ![Modal „Verbundene Datensätze hinzufügen“](assets/add-connection-view-page-modal.png)

1. Fügen Sie den **Seitennamen** hinzu, klicken Sie auf **Seite „Verbundene Datensätze** für den **Seitentyp** und klicken Sie dann auf **Erstellen**.
1. (Optional) Klicken Sie auf den Namen eines verbundenen Datensatzes oder Objekttyps in der Liste, oder suchen Sie nach dem Datensatz oder Objekttyp. Klicken Sie dann auf den Datensatz oder Objekttyp, wenn er in der Liste angezeigt wird, um die Seite für diesen Datensatz oder Objekttyp zu erstellen.

   >[!TIP]
   >
   >Sie können für jeden Datensatztyp eine verbundene Datensatzseite erstellen. Wenn ein verbundener Datensatztyp bereits über eine Seite verfügt, wird sie nicht mehr als Option angezeigt.
   >

1. (Optional und bedingt) Wenn mehr als ein verbundenes Feld des Datensatz- oder Objekttyps angezeigt wird, für den Sie die Seite erstellen, klicken Sie in der Liste „Referenzfeld **&quot; auf das Feld, dessen Datensätze oder Objekte Sie auf der Seite „Verbundene Datensätze“ anzeigen**.

   ![Referenzfeldliste auswählen](assets/select-reference-field-list-on-connected-records-page.png)

   Eine der folgenden Seiten wird der Seite „Verbundene Datensätze“ hinzugefügt:

   * Die Tabellenansicht eines Datensatztyps
   * Die Listenansicht eines Projektobjekttyps

   Die Datensätze oder Projekte, die mit dem aktuellen Datensatz verbunden sind, werden in der Tabellen- oder Listenansicht angezeigt.

   >[!TIP]
   >
   >Sie müssen verbundene Datensätze im Tabellen- oder Detailbereich eines Datensatzes hinzufügen, bevor Sie sie auf einer Seite mit verbundenen Datensätzen anzeigen können. Andernfalls ist die Tabelle oder Liste leer.

   Die ersten fünf Felder der verbundenen Datensätze werden standardmäßig angezeigt. Standardmäßig werden keine Suchfelder angezeigt.

   ![Tabellenansicht mit Audience-Verbindung unter Kampagnendetails](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Bedingt) Führen Sie je nachdem, welche Art von Datensätzen Sie auf der Seite „Verbundener Datensatz“ anzeigen, einen der folgenden Schritte aus:

   * Verwalten von Planungsdatensätzen
Weitere Informationen finden Sie im Abschnitt [Verwalten der Seite „Verbundene Datensätze“ für Planungsdatensätze](#manage-the-connected-records-page-for-planning-records) in diesem Artikel.
   * Verwalten von Workfront-Projekten
Weitere Informationen finden Sie im Abschnitt [Verwalten der Seite „Verbundene Datensätze“ für Workfront-Projekte](#manage-the-connected-records-page-for-workfront-projects) in diesem Artikel.

1. (Optional) Doppelklicken Sie auf den Namen der Registerkarte **Seite „Verbundene Datensätze**

   ODER

   Bewegen Sie den Mauszeiger über den Namen der Registerkarte und klicken Sie dann auf **Mehr** ![Mehr &#x200B;](assets/more-menu.png) und klicken Sie dann auf **Umbenennen**, um die Registerkarte in neue verbundene Datensatzerseite umzubenennen.

1. (Optional) Bewegen Sie den Mauszeiger über den Namen der Registerkarte „Verbundene Datensatzerseite“ und klicken Sie auf **Mehr** ![Mehr](assets/more-menu.png) und dann auf **Löschen**, um die Registerkarte zu entfernen.

### Verwalten der Seite „Verbundene Datensätze“ für Planungsdatensätze

<!--

#### Manage the connected records page for Planning records in the Production environment

When you create a connected records page for  connected Planning records in the Production environment, do the following: (****or AEM Assets - AEM is not available yet?? see note below********)

1. Go to a record type page and click the name of a record. This opens the record's preview page.
1. Click the tab for a connected records page that display Planning records.
   The records connected to the record you selected display in the table view. 
1. Click **Connect** at the bottom of the table view to connect existing records, select them from the connection box, then click outside the box to close it. The records are automatically added to the table and connected to the record you selected. The records must exist before you can add them.

   For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).

1. Edit any information from the connected records inline in the table view. 
1. Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png)

   Or 
   
   Select one of the records, then click one of the following options in the blue bar at the bottom of the list: 

   * **View** to open the record page in a new tab
   * **Copy link** to copy a link to the record page
   * **Edit thumbnail** to open the **Record thumbnail** box and edit the record's thumbnail image
   * **Duplicate** to duplicate the connected record. The duplicated record is also connected to the current record.
   * **Insert record above or below** to add new records to the connected record type. New records added here are also connected to the current record. This option is not available in the blue bar when selecting a record in the table.
   * **Delete** to delete the record. Deleting a connected record deletes it from its record type and from everywhere where the record is connected. The deleted records move to the **Recently deleted** bin of their record type.

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

      >[!TIP]
      >
      >You can select more than one record or object to delete them.
      >

1. Inline edit any of the records in the table on the connected records page.
1. Use any of the following view elements in the toolbar of a connected record page to manage the table view:

   * **Filters**
   * **Sort**
   * **Grouping**
   * **Fields**, to display, hide, or rearrange fields
   * **Row height**
   * **Search**

   For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

   >[!NOTE]
   >
   >You cannot create, edit, or delete fields in the table view of a connected record's tab.
   >

#### Manage the connected records page for Planning records in the Preview environment

When you create a connected records page for connected Planning records in the Preview environment, do the following: (***********or AEM Assets -- AEM is not available yet?? see note below**********)

-->

1. Wechseln Sie zu einer Seite vom Typ Datensatz und klicken Sie auf den Namen eines Datensatzes. Dadurch wird die Vorschauseite des Datensatzes geöffnet.
1. Klicken Sie auf die Registerkarte für eine Seite mit verbundenen Datensätzen, auf der Planungsdatensätze angezeigt werden.
Die mit dem ausgewählten Datensatz verbundenen Datensätze werden in der Tabellenansicht angezeigt.
1. Klicken Sie **Datensätze verbinden** oben rechts auf der Seite „Verbundene Datensätze“, um vorhandene Datensätze zu verbinden, wählen Sie sie aus dem Feld „Verbindung“ aus und klicken Sie dann außerhalb des Felds, um sie zu schließen. Die Datensätze werden automatisch der Tabelle hinzugefügt und mit dem ausgewählten Datensatz verbunden. Die Datensätze müssen vorhanden sein, bevor Sie sie hinzufügen können.

   Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

1. Klicken Sie **Neue Zeile** unten in der Tabelle, um neue Datensätze hinzuzufügen. Die neuen Datensätze werden automatisch mit den ausgewählten Datensätzen verbunden.
1. Bearbeiten Sie alle Informationen aus den verbundenen Datensätzen inline in der Tabellenansicht.
1. Bewegen Sie den Mauszeiger über den Namen eines verbundenen Datensatzes und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png)

   ODER

   Wählen Sie einen der Datensätze aus und klicken Sie dann auf eine der folgenden Optionen in der blauen Leiste unten in der Liste:

   * **Anzeigen**, um die Datensatzseite in einer neuen Registerkarte zu öffnen
   * **Link kopieren**, um einen Link auf die Datensatzseite zu kopieren
   * **Miniaturansicht bearbeiten** um das Feld **Miniaturansicht aufzeichnen** zu öffnen und das Miniaturbild des Datensatzes zu bearbeiten
   * **Duplizieren** um den verbundenen Datensatz zu duplizieren. Der duplizierte Datensatz ist auch mit dem aktuellen Datensatz verbunden.
   * **Datensatz oberhalb oder unterhalb einfügen**, um dem verbundenen Datensatztyp neue Datensätze hinzuzufügen. Neue hier hinzugefügte Datensätze sind auch mit dem aktuellen Datensatz verbunden. Diese Option ist bei der Auswahl eines Datensatzes in der Tabelle in der blauen Leiste nicht verfügbar.
   * **Löschen**, um den Datensatz zu löschen. Wenn Sie einen verbundenen Datensatz löschen, wird er aus seinem Datensatztyp und überall dort, wo der Datensatz verbunden ist, gelöscht. Die gelöschten Datensätze werden in den **kürzlich gelöschte** Bin ihres Datensatztyps verschoben.

     Weitere Informationen zum Bearbeiten von Datensätzen in der Tabellenansicht finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >Sie können mehrere Datensätze oder Objekte auswählen, um sie zu löschen.

1. Inline-Bearbeitung eines beliebigen Datensatzes in der Tabelle auf der Seite „Verbundene Datensätze“.
1. Verwenden Sie eines der folgenden Ansichtselemente in der Symbolleiste einer verbundenen Datensatzseite, um die Tabellenansicht zu verwalten:

   * **Filter**
   * **sort**
   * **Gruppierung**
   * **Felder**, zum Anzeigen, Ausblenden oder Neuanordnen von Feldern
   * **Zeilenhöhe**
   * **Suche**

   Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Sie können keine Felder in der Tabellenansicht der Registerkarte eines verbundenen Datensatzes erstellen, bearbeiten oder löschen.
   >

1. Klicken Sie auf das Dropdown-Menü „Ansichten“ in der oberen rechten Ecke der Seite „Verbundene Datensätze“ und klicken Sie auf **Neue Ansicht**, um eine neue Ansicht für die Seite hinzuzufügen. Gehen Sie dann wie folgt vor:

   1. Fügen Sie einen **Ansichtsnamen“**.
   1. Wählen Sie im Bereich **Ansichtstyp** einen der folgenden Ansichtstypen aus:

      * Tabelle
Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md)
      * Zeitleiste
Weitere Informationen finden Sie unter [Verwalten der Zeitleisten-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).
      * Kalender
Weitere Informationen finden Sie unter [Verwalten der Kalenderansicht](/help/quicksilver/planning/views/manage-the-calendar-view.md).

        Weitere Informationen finden Sie im Abschnitt [Verwalten mehrerer Ansichten auf der Seite „Verbundene Datensätze](#manage-multiple-views-from-the-connected-records-page) in diesem Artikel.

   1. Klicken Sie **Erstellen**.
Dem Dropdown-Menü „Ansichten“ wird eine neue Ansicht hinzugefügt.

   1. (Optional) Bewegen Sie den Mauszeiger über den Namen einer von Ihnen erstellten Ansicht und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und dann auf eine der folgenden Optionen:

      * **Umbenennen**, um einen neuen Namen für die Ansicht hinzuzufügen.
      * **Freigeben**

        Weitere Informationen finden Sie unter [Freigeben von Ansichten](/help/quicksilver/planning/access/share-views.md).
      * **Exportieren**

      * **Löschen**
Weitere Informationen finden Sie [Löschen von Datensatzansichten](/help/quicksilver/planning/views/delete-record-views.md).

        ![Menü „Mehr anzeigen“ auf der Seite „Projekte mit verbundenen Datensätzen“](assets/view-more-menu-projects-connected-records-page.png)

        >[!NOTE]
        >
        >Sie können eine von Workfront erstellte Systemansicht nicht löschen.

### Verwalten der verbundenen Datensatzseite für Workfront-Projekte

Gehen Sie wie folgt vor, wenn Sie eine Seite „Verbundene Datensätze“ für verbundene Workfront-Projekte erstellen:

1. Wechseln Sie zu einer Seite vom Typ Datensatz und klicken Sie auf den Namen eines Datensatzes. Dadurch wird die Vorschauseite des Datensatzes geöffnet.
1. Klicken Sie auf die Registerkarte für eine Seite mit verbundenen Datensätzen, die Workfront-Projekte anzeigt.
Die mit dem ausgewählten Datensatz verbundenen Projekte werden in der Listenansicht angezeigt.
1. Klicken Sie **Datensätze verbinden** in der oberen rechten Ecke der Seite „Verbundene Datensätze“, um vorhandene Projekte zu verbinden.

   Weitere Informationen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).
1. Inline-Bearbeitung der Projektinformationen in der Tabelle.
1. Klicken Sie auf **Neue Zeile**, um ein Projekt ohne Vorlage zu erstellen. Das neue Projekt wird automatisch mit dem aktuellen Datensatz verbunden.

   Weitere Informationen finden Sie unter [Erstellen von Workfront-Objekten aus Workfront Planning beim Verbinden mit Datensätzen](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).

1. Bewegen Sie den Mauszeiger über einen Projektnamen in der Liste und klicken Sie auf das Menü **Mehr** [Mehr](assets/more-menu.png)

   ODER

   Wählen Sie ein oder mehrere Projekte aus, beachten Sie den blauen Balken unten in der Liste und klicken Sie dann auf eines der folgenden Elemente:

   * **Löschen**, um das Projekt zu löschen. Durch das Löschen eines Projekts wird es vom Datensatz getrennt und in den Papierkorb von Workfront verschoben. Workfront-Administratoren können gelöschte Projekte bis zu 30 Tage nach dem Löschen wiederherstellen.
   * **Trennen**, um das Projekt vom Datensatz zu trennen. Wenn Sie ein Projekt trennen, werden es und alle Werte seiner Suchfelder aus dem aktuellen Datensatz entfernt.

     >[!TIP]
     >
     >Sie können mehrere Projekte auswählen, um sie zu trennen oder zu löschen.
     >

1. Klicken Sie auf das Dropdown-Menü „Ansichten **und klicken Sie auf &quot;** Ansicht“, um eine neue Ansicht für die Seite hinzuzufügen. Gehen Sie dann wie folgt vor:

   1. Fügen Sie einen **Ansichtsnamen“**.
   1. Wählen Sie **Liste** im Bereich **Ansichtstyp** aus.
   1. Klicken Sie **Erstellen**.
Eine neue Listenansicht wird dem Dropdown-Menü „Ansichten“ im Bereich &quot;**Ansichten“**.

      Weitere Informationen finden Sie im Abschnitt [Verwalten mehrerer Ansichten auf der Seite „Verbundene Datensätze](#manage-multiple-views-from-the-connected-records-page) in diesem Artikel.

   1. (Optional) Bewegen Sie den Mauszeiger über den Namen einer von Ihnen erstellten Ansicht und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und dann auf eine der folgenden Optionen:
      * **Umbenennen**, um einen neuen Namen für die Ansicht hinzuzufügen.
      * **Freigeben**

        Weitere Informationen finden Sie unter [Freigeben von Ansichten](/help/quicksilver/planning/access/share-views.md).

      * **Löschen**
Weitere Informationen finden Sie [Löschen von Datensatzansichten](/help/quicksilver/planning/views/delete-record-views.md).

        ![Menü „Mehr anzeigen“ auf der Seite „Projekte mit verbundenen Datensätzen“](assets/view-more-menu-projects-connected-records-page.png)

        >[!NOTE]
        >
        >Sie können eine von Workfront erstellte Systemansicht nicht umbenennen, freigeben oder löschen.

   1. Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-icon.png) und verwenden Sie den Filter, um bestimmte Projekte anzuzeigen.

      >[!TIP]
      >
      >Bei Feldern vom Typ „Personen“, z **B. „Inhaber** oder **Sponsor**, können Sie einen Platzhalter verwenden, um Projekte anzuzeigen, bei denen der angemeldete Benutzer diesen Rollen zugewiesen ist.
      >
      >![Mit Benutzer-Platzhalter nach der Seite mit projektbezogenen Datensätzen filtern](assets/filter-with-user-wildcard-project-connected-records-page.png)
      >

   1. Klicken Sie auf das **Spalten**-Symbol ![Spalten-Symbol](assets/columns-icon.png), um Spalten in der Liste auszublenden oder anzuzeigen.
   1. Klicken Sie auf das Symbol **+** in der oberen rechten Ecke der Tabellenansicht, um der Tabelle vorhandene Felder hinzuzufügen. Felder müssen vorhanden sein, bevor Sie sie hinzufügen können.

      Das Feld **Spalten-Manager** wird geöffnet. Gehen Sie folgendermaßen vor:

      1. Suchen Sie in der Spalte **Verfügbar** nach einem vorhandenen Objektfeld und klicken Sie dann auf **+** rechts neben dem Feldnamen, um es der Spalte **Ausgewählt** hinzuzufügen.

         Die ausgewählten Felder werden der Tabellenansicht auf der Seite Verbundene Datensätze hinzugefügt.
      1. Klicken Sie auf **-** rechts neben einem Feld in der Spalte **Ausgewählt**, um es aus der Tabellenansicht zu entfernen.
      1. Klicken Sie **Speichern**, um die verbundene Datensatz-Seitentabellenansicht zu speichern.

<!-- this is repetitive from an earlier section above: 

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. (Conditional) When displaying Planning records in the connected records page, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: 

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Delete**

   <!--not possible right now: * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).
      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. -->


<!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      TIP      
      You can select more than one record or object to disconnect them.
      -->