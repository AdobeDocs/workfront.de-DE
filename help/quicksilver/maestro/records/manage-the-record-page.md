---
title: Datensatzseite verwalten
description: Sie können das Layout der Datensatzvorschau und -seite in der Adobe Workfront-Planung bearbeiten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: ace194b584601f9edd7862dbd74f639538891370
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Datensatzseite verwalten

{{maestro-important-intro}}

Sie können das Layout der Datensatzvorschau und -seite in der Adobe Workfront-Planung bearbeiten.

Die Datensatzvorschau ist eine kleinere Ansicht der Datensatzseite, die in der Ansicht eines Datensatztyps angezeigt wird.

Wenn Sie das Layout einer Datensatzvorschau und -seite ändern, wirken sich die Änderungen auf die Vorschaufelder und Detailseiten aller Datensätze desselben Typs aus.

In diesem Artikel wird beschrieben, wie Sie das Layout und Erscheinungsbild eines Datensatzvorschaufelds oder einer Datensatzseite ändern können. Informationen zum Bearbeiten von Datensätzen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/maestro/records/edit-records.md).

Sie müssen Datensatztypen und Datensätze erstellen, bevor Sie mit der Bearbeitung von Datensatzseiten beginnen können.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Erstellen von Datensatztypen](../architecture/create-record-types.md)

* [Datensätze erstellen](/help/quicksilver/maestro/records/create-records.md)

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
<p>Ihr Unternehmen muss am Betaprogramm für die Adobe Workfront-Planung teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   <p>Neu: Licht oder höher</p>
   Oder
   <p>Aktuell: Arbeit oder höher</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für die Adobe Workfront-Planung</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Verwalten oder höhere Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Bearbeiten von Datensatzseiten

* Durch das Neuanordnen von Feldern in der Datensatzvorschau oder Seite werden die Felder für alle Datensätze dieses Typs und für alle Benutzer, die auf diese Datensätze zugreifen, neu angeordnet.

* Änderungen an der Anzeige, die Sie in der Datensatzvorschau vornehmen, werden sofort auf der Seite mit den Datensatzdetails angezeigt. Änderungen, die auf der Datensatzseite vorgenommen wurden, sind auch im Vorschaufeld der Datensätze sichtbar.

<!--Replace the first bullet with this when we add sections:

* The following changes affect all the records of the same type and are visible to all users accessing those records: 

   * Rearranging fields
   * Adding or removing sections
-->

* Das Hinzufügen eines Titelbilds zu einem Datensatz ist nicht Teil des Gesamtlayouts der Datensatzvorschau oder -seite. Sie können jedem Datensatz eindeutige Titelbilder hinzufügen. Weitere Informationen finden Sie unter [Hinzufügen eines Titelbilds zu einem Datensatz](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

<!--

## Add sections to a record preview or page

You can add sections to a record preview or page, to organize the information by common criteria and make it easier to find. 

Consider the following when adding sections to a record page:

* There is no limit to how many sections you can have on a page (***************IS THIS TRUE???***********)
* You cannot have an empty section. You must have at least one field in a section. 
* You can drag and drop fields from one section to another. 
* When you remove all the fields from a section, the section is automatically deleted and cannot be recovered. 

To add a section to a record preview or page: 

{{step1-to-maestro}}

The workspace that you access last opens. 

1. (Optional) Click the downward-pointing arrow to the right of the workspace name to select the workspace whose records you want to update. 
1. Click a record type card. 

    The record type page opens. 

1. From a view of any type, click the name of a record 

    Or 
    
    From the table table view, click the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of a record name. 
    
    The record's preview opens in the view.

    ![](assets/details-box.png) 

    >[!TIP]
    >
    >You can view the **Open details** icon to the left of the Name field of a record in a table view only when the Name field is a primary field. 

1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) (****************check the icon; they are changing it**********)  in the upper-right corner of the record preview  to open the record's page in a new tab. 

    The record page opens. 

    ![](assets/details-page.png)

1. In the record preview or page, hover over the white space to the left of the fields, then click the **Add section** icon ![](assets/add-section-icon.png) to add a section. 
1. Click inside the section's name and replace **Untitled** with a name, then click Enter. (************has this changed to Untitled section???**********)
1. Start dragging and dropping fields to the new section, as described in the section [Rearrange fields in the record preview or page](#rearrange-fields-in-the-record-preview-or-page) in this article. 

1. (Optional) Hover over the name of a section and click the **More** menu ![](assets/more-menu.png). 

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Optional) Do one of the following to edit the section: 

   * Click **Rename** to rename the section

      >[!TIP]
      >
      > You can rename a section inline, by clicking the name.
   
   * Click **Move up** to move the section up one position 

      Or 
      
      Click **Move down** to move the section down one position.
      All fields in the section move with the section. 

   * Click **Delete** to delete the section. The section is deleted and it cannot be recovered. All users accessing the records of this type will no longer view the deleted section. 

1. Click the downward-pointing arrow to the left of a section name to collapse it, or the right-pointing arrow  to expand it. 
   All sections are expanded by default. 

1. (Optional) Click the **grab** icon ![](assets/grab-icon.png) to the left of a section name, then drag and drop it in a desired spot. 

    The new position of the section updates in both the preview and the page of all records of the same type for all users viewing the records. 

    All changes to sections and field order are saved automatically. 

-->

## Neuanordnen von Feldern in der Datensatzvorschau oder auf der Seite

{{step1-to-maestro}}

Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Oder

   Klicken Sie in der Tabellenansicht auf die **Details öffnen** icon ![](assets/open-details-icon-in-table-name-field.png) auf der linken Seite eines Datensatznamens.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Sie können die **Details öffnen** Symbol links neben dem Feld &quot;Name&quot;eines Datensatzes in einer Tabellenansicht nur dann angezeigt, wenn das Feld &quot;Name&quot;ein primäres Feld ist.

1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der rechten oberen Ecke der Datensatzvorschau, um die Datensatzseite in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet.

   ![](assets/details-page.png)

1. Klicken Sie in der Datensatzvorschau oder -seite auf die **Grab** icon ![](assets/grab-icon.png) links neben einem Feldnamen, und ziehen Sie ihn per Drag-and-Drop an die gewünschte Position. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   Die neue Position des Felds wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen am Layout der Datensatzvorschau oder der Seite werden automatisch gespeichert.

