---
title: Verwalten des Datensatzseiten-Layouts
description: Sie können das Layout der Datensatzvorschau und -seite in Adobe Workfront Planning bearbeiten.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: f5d6918889b7fed1159274105ee706a027f621bf
workflow-type: tm+mt
source-wordcount: '1568'
ht-degree: 0%

---


# Seiten-Layout des Datensatzes verwalten

<span class="preview">Die auf dieser Seite hervorgehobenen Informationen beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können das Layout der Datensatzvorschau und -seite in Adobe Workfront Planning bearbeiten.

Die Datensatzvorschau ist eine kleinere Ansicht der Datensatzseite, die in der Ansicht eines Datensatztyps angezeigt wird.

Wenn Sie das Layout einer Datensatzvorschau und -seite ändern, wirken sich die Änderungen auf die Vorschaufelder und Detailseiten aller Datensätze desselben Typs aus.

In diesem Artikel wird beschrieben, wie Sie das Layout und Aussehen eines Datensatzvorschaufelds oder einer Datensatzseite ändern können. Weitere Informationen zum Bearbeiten von Datensätzen finden Sie unter [Bearbeiten von Datensätzen](/help/quicksilver/planning/records/edit-records.md).

Sie müssen Datensatztypen und Datensätze erstellen, bevor Sie die Datensatzseiten bearbeiten können.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md)

* [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md)

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


<!--Old:
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
<p>Any of the following Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td>
   <td>
<p>Any</p>
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
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
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

## Überlegungen zum Arbeiten mit Datensatzseiten

* Standardmäßig werden auf der Detailseite eines Datensatzes alle mit dem Datensatz verknüpften Felder angezeigt.

* Sie können auf der Vorschau- oder Detailseite keine neuen Felder für einen Datensatz hinzufügen. Sie müssen neue Felder in der Tabellenansicht hinzufügen, um sie auf den Seiten „Vorschau“ und „Details“ anzuzeigen.

* Sie können einer Datensatzvorschau oder einer Detailseite Abschnitte hinzufügen, um die Informationen nach gemeinsamen Kriterien zu organisieren und das Auffinden zu erleichtern.

* Die folgenden Änderungen wirken sich auf alle Datensätze desselben Typs aus und sind für alle Benutzer sichtbar, die auf diese Datensätze zugreifen:

   * Felder neu anordnen
   * Hinzufügen oder Entfernen von Abschnitten
   * Hinzufügen oder Entfernen von verbundenen Datensatzseiten

* Änderungen an der Datensatzvorschau werden sofort auf der Seite mit den Datensatzdetails angezeigt. Auf der Datensatzseite vorgenommene Änderungen sind auch im Feld für die Datensatzvorschau sichtbar.

* Das Hinzufügen eines Cover- oder Miniaturbilds zu einem Datensatz gehört nicht zum Gesamtlayout der Datensatzvorschau oder -seite. Sie können jedem Datensatz eindeutige Titelbilder oder Miniaturansichten hinzufügen. Weitere Informationen finden Sie unter [Hinzufügen eines Titelbilds zu einem &#x200B;](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) und [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

* Sie können der Seite eines Datensatzes zusätzliche Seiten der folgenden Typen hinzufügen:

   * Seite „Verbundene Einträge“

     Weitere Informationen finden Sie im Abschnitt [Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz](#add-a-connected-records-page-to-a-record).

## Hinzufügen von Abschnitten zu einer Datensatzvorschau oder Seite

Beachten Sie beim Hinzufügen von Abschnitten zu einer Datensatzseite Folgendes:

* Es gibt keine Begrenzung dafür, wie viele Abschnitte Sie auf einer Seite haben können.
* Es ist nicht möglich, einen leeren Abschnitt zu verwenden. Mindestens ein Feld in einem Abschnitt ist erforderlich.
* Sie können Felder per Drag-and-Drop von einem Abschnitt in einen anderen ziehen. Weitere Informationen finden Sie im Abschnitt [Verwalten von Feldern auf der Datensatzvorschau oder Detailseite](#manage-fields-in-the-records-details-tab) in diesem Artikel.
* Wenn Sie alle Felder aus einem Abschnitt entfernen, wird der Abschnitt automatisch gelöscht und kann nicht wiederhergestellt werden.

So fügen Sie einen Abschnitt zu einer Datensatzvorschau oder Seite hinzu:

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes

   ODER

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen** ![Detailsymbol öffnen im Feld „Tabellenname](assets/open-details-icon-in-table-name-field.png) in der ersten Spalte.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![Detailfeld](assets/details-box.png)

1. (Optional) Klicken Sie auf **Symbol** In neuer Registerkarte öffnen![&#x200B; (Details in einer neuen Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) in der oberen rechten Ecke der Datensatzvorschau, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet. Die Registerkarte Details wird standardmäßig geöffnet.

   ![Detailseite](assets/details-page.png)

1. Bewegen **auf der Registerkarte** Details“ der Datensatzvorschau oder -seite den Mauszeiger über den Leerraum links neben den Feldern und klicken Sie dann auf das Symbol **Abschnitt hinzufügen** ![Abschnittssymbol hinzufügen](assets/add-section-icon.png), um einen Abschnitt hinzuzufügen.
1. Klicken Sie in den Namen des Abschnitts und ersetzen Sie **Nicht benannter Abschnitt** durch einen Namen. Klicken Sie dann auf die Eingabetaste. Die unter dem Abschnitt angezeigten Felder sind automatisch Teil des neuen Abschnitts.
1. Ziehen Sie die Felder per Drag-and-Drop in den neuen Abschnitt, wie im Abschnitt [Verwalten von Feldern in der Datensatzvorschau oder auf der Detailseite](#manage-fields-in-the-records-details-tab) in diesem Artikel beschrieben.

1. (Optional) Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png).

   ![Weitere Menüoptionen für Abschnitt auf Datensatzseite](assets/more-menu-options-for-section-on-record-page.png)
1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Abschnitt zu bearbeiten:

   * Klicken Sie auf **Umbenennen**, um den Abschnitt umzubenennen

     >[!TIP]
     >
     > Sie können einen Abschnitt inline umbenennen, indem Sie auf den Namen klicken.

   * Klicken Sie **Nach oben**, um den Abschnitt um eine Position nach oben zu verschieben

     ODER

     Klicken Sie **Nach unten**, um den Abschnitt um eine Position nach unten zu verschieben.
Alle Felder im Abschnitt werden mit dem Abschnitt verschoben.

   * Klicken Sie **Löschen**, um den Abschnitt zu löschen. Der Abschnitt wurde gelöscht und kann nicht wiederhergestellt werden. Alle Benutzer, die auf die Datensätze dieses Typs zugreifen, sehen den gelöschten Abschnitt nicht mehr.

1. Klicken Sie auf den nach unten zeigenden Pfeil links neben einem Abschnittsnamen, um ihn zu reduzieren, oder auf den nach rechts zeigenden Pfeil, um ihn zu erweitern.
Alle Abschnitte sind standardmäßig erweitert.

1. (Optional) Klicken Sie auf das **grab**-Symbol ![grab-Symbol](assets/grab-icon.png) links neben dem Namen eines Abschnitts und ziehen Sie ihn dann an die gewünschte Stelle.

   Die neue Position des Abschnitts wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen an Abschnitten und der Feldreihenfolge werden automatisch gespeichert.

1. (Optional) Klicken Sie auf das **Export**-Menü ![Export-Symbol auf der Seite mit &#x200B;](assets/export-icon-in-record-details-page.png) Datensatzdetails), um die Registerkarte Details in eine Word- oder PDF-Datei zu exportieren. Weitere Informationen finden Sie [Exportieren der Details eines Datensatzes](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Optional) Klicken Sie auf die Registerkarte **Verbindungen** neben der Registerkarte **Details**. Möglicherweise müssen Sie auf **Mehr** klicken, bevor Sie auf die Registerkarte **Verbindungen** klicken.

   Alle Datensätze oder Objekte, die mit dem ausgewählten Datensatz verbunden sind, werden unter den Namen des Datensatztyps oder der Anwendung, zu der sie gehören, angezeigt.

   ![Registerkarte „Verbindungen“ im Datensatz in Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Optional) Wählen Sie die Einstellung **Alle Datensätze anzeigen** in der oberen rechten Ecke der Registerkarte Verbindungen aus. Alle verbundenen Datensatztypen werden angezeigt, einschließlich der Datensätze, die noch keine verbundenen Datensätze haben. Standardmäßig ist der Umschalter deaktiviert und Datensatztypen ohne verbundene Datensätze sind ausgeblendet.

1. (Optional) Klicken Sie auf **Verbinden**, um den verbundenen Datensatztypen weitere Datensätze hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine Datensatzkarte und klicken Sie dann auf das Symbol zum Trennen des Datensatzes **-** und anschließend auf **Trennen**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
Folgendes geschieht:
   * Der Datensatz ist nicht mehr mit dem Workfront-Objekt verbunden.
   * Das Workfront-Objekt wird auch aus dem verknüpften Feld des Datensatzes aus Workfront Planning entfernt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden ebenfalls gelöscht.

## Felder in der Registerkarte „Details“ des Datensatzes verwalten

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes

   ODER

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen** ![Detailsymbol öffnen im Feld „Tabellenname](assets/open-details-icon-in-table-name-field.png) in der ersten Spalte.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![Detailfeld](assets/details-box.png)

1. <span class="preview">(Optional und bedingt) Führen Sie je nachdem, welche Felder auf der Detailseite angezeigt werden sollen, einen der folgenden Schritte aus:</span>

   <div class="preview">

   * Wählen Sie die Einstellung **Tabellenfelder anzeigen**, um nur Felder anzuzeigen, die nicht in der Tabellenansicht des Datensatzes ausgeblendet sind. Dies ist die Standardeinstellung
   * Deaktivieren Sie die Einstellung **Tabellenfelder anzeigen**, um alle Felder in der Tabellenansicht des Datensatzes anzuzeigen, einschließlich der ausgeblendeten.

   >[!TIP]
   >
   >Die Einstellung **Tabellenfelder anzeigen** ist nur im Vorschaufeld Details des Datensatzes verfügbar. Sie ist nicht auf der Detailseite des Datensatzes verfügbar.


   <!--replace with this when they fix the UI text:
   * Select the **Show all fields** setting to include all the record's fields in the **Details** page. This is the default setting. 
   * Deselect the **Show all fields** setting to exclude the record's fields that are hidden in the table view of the record from the **Details** page.
   -->

   </div>

1. (Optional) Klicken Sie auf **Symbol** In neuer Registerkarte öffnen![&#x200B; (Detailfeld in einem neuen Registerkartensymbol öffnen](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke der Datensatzvorschau, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen.

   Die **Details** des Datensatzes wird standardmäßig geöffnet.

   ![Detailseite](assets/details-page.png)

1. Klicken Sie auf der **„Details** auf das **grab**-Symbol ![grab icon](assets/grab-icon.png) links neben einem Feldnamen und ziehen Sie es dann an die gewünschte Stelle.

   >[!TIP]
   >
   >Sie können Felder per Drag-and-Drop in einen anderen Abschnitt ziehen.
   >Mindestens ein Feld in einem Abschnitt ist erforderlich.
   >

   Die neue Position des Felds wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen am Layout der Datensatzvorschau oder -seite werden automatisch gespeichert.

## Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz

Sie können Informationen aus verbundenen Datensätzen oder Objekten anzeigen, indem Sie eine Registerkarte für eine Seite „Verbundene Datensätze“ zum Detailbereich eines Datensatzes hinzufügen. Dadurch werden die verbundenen Datensätze in einer Tabellen- oder Listenansicht zur Registerkarte hinzugefügt.

Weitere Informationen finden Sie unter [Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

<!--this content has been moved to the page linked above
Consider the following when adding a Connected records page to a record: 

* You can add a Connected records page to a record after you connected record or object types to the record type from the table view of a record type.

* You can add a Connected records page from a record's preview area or the record's page.

* Connected records pages display only the connected objects or records from one object or record type in a table view. The page does not display all records of that type. 

* You can add Connected records pages for the following connected record or object types:

   * Workfront Planning record types
   * Workfront projects, programs, portfolios, groups, or companies. You can view the connected Workfront objects even when you do not have permissions to access them in Workfront. 

To add a Connected records page:

1. Click the name of the record to open it from any view of a record type page. 
1. Click **Add page** from one of the following areas: 

   * The record's preview window
   * The record's details page, after clicking the **Open in new tab** icon ![Open details in a new tab icon](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the preview page.  

   The **Create page** box opens.

   ![Add Connected records page modal](assets/add-connection-view-page-modal.png) 

1. Add the **Page name**, click **Connected records page**, then click **Create**.

   A new connected records page is added as a new tab to the record's page.
   
   The records that are connected to the current record display in the table view.  

      >[!TIP]
      >
      >You must add connected records in the table or Details area of a record before you can display them in a connected records page.

   (^^^^^^All fields of the connected record display in the table view of the connected record's tab.^^^^^^^^)
   
   The first five fields of the connected records display by default. (^^^^No lookup fields display by default.^^^^^^^)

   ![Audience connected table view under campaign details](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optional) Search for or click the name of a connected record or object type in the list.

1. (Optional and conditional) In the table view of the connected records page, do any of the following when viewing connected Planning records or any Workfront objects except for projects: 

   * Click the name of a record. This opens the record's page in a new tab. 

   * Click **Connect** at the bottom of the table view to connect more records, then click outside the connection box to close it. The new records are automatically added to the table. 

      For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
   * Edit any information from the connected records inline in the table view. 

   * Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png)
   
      Or 
      
      Select one of the records, then click one of the following options in the blue bar at the bottom of the list: 

      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Edit thumbnail** to open the **Record thumbnail** box and edit the record's thumbnail image
      * **Duplicate** to duplicate the connected record. The duplicated record is also connected to the current record.
      * **Insert record above or below** to add new records to the connected record type. New records added here are also connected to the current record. This option is not available in the blue bar when selecting a record in the table.
      * **Delete** to delete the record. Deleting a connected record deletes it from its record type and from everywhere where the record is connected.

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

      >[!TIP]
      >
      >You can select more than one record or object to delete them.

   * Inline edit any of the Planning records in the table on the Connected records page. 
   
      All other Workfront objects display in a read-only table view and you cannot edit them. 
   
1. (Optional and conditional) In the table view of the connected records page, do any of the following when viewing connected Workfront projects:

     * Click **Connect records** in the upper-right corner of the connected record page to connect existing projects.

      For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
     * Inline edit project information in the table.
     * Click **New row** to create a project without a template. The new project is connected to the current record immediately.

         For more information, see [Create Workfront objects from Workfront Planning as you connect them to records](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
     * Hover over a project and click the **More** menu [More menu](assets/more-menu.png)
     
         Or

         Select one or more projects, and notice the blue bar at the bottom of the list, then click one of the following:
         
         * **Delete** to delete the project. Deleting a project disconnects it from the record and moves it to the Workfront's Recycle Bin. 
         * **Disconnect** to disconnect the project from the record. Disconnecting a project removes it and all the values of its lookup fields from the current record.
      
1. (Optional) Double-click the name of the **Connected records page** tab

   Or

   Hover over the name of the tab, then click **More** ![More menu](assets/more-menu.png), then click **Rename** to rename to new Connected view tab.
1. (Optional) Use any of the following view elements in the toolbar of a connected record page to manage the table view:

   * Filters
   * Sort
   * Grouping
   * Fields, to display, hide, or rearrange fields
   * Row height
   * Search

   For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

   >[!NOTE]
   >
   >You cannot create, edit, or delete fields in the table view of a connected record's tab.
   
1. (Optional)  Hover over the name of the Connected records page tab, click **More** ![More menu](assets/more-menu.png), then click **Delete** to remove to tab.-->


<!--
## Add a Brief page to a record

(^^^^^^^^^^move this content to its own article, like you did above - leave the header here with a link^^^^^^^^^^^^)

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



