---
title: Hinzufügen einer Miniaturansicht zu einem Datensatz
description: Sie können Datensatzinformationen in Adobe Workfront Planning bearbeiten und jeden Datensatz mit individuellen Miniaturansichten verknüpfen, um ihn leicht erkennbar zu machen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# Hinzufügen einer Miniaturansicht zu einem Datensatz

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Sie können in Adobe Workfront Planning Datensätze mit eindeutigen Miniaturansichten verknüpfen, um sie leicht erkennbar zu machen.

Sie müssen Datensatztypen erstellen, bevor Sie Datensätze erstellen und bearbeiten können.
Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

## Zugriffsanforderungen

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
<p>Beliebiges Workfront und beliebiges Planungspaket</p> <p>Beliebiger Workflow und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Beitragen von oder höhere Berechtigungen für einen Arbeitsbereich und einen Datensatztyp  </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
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
<p>Any </p> 
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
   <td><p> Standard </p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


## Überlegungen zu Datensatzminiaturansichten

Um Datensätze in einer Tabellenansicht visuell unterscheiden zu können, können Sie jedem Datensatz ein eindeutiges Miniaturbild zuordnen.

Beachten Sie Folgendes:

* Eine Miniaturansicht ist für einen Datensatz eindeutig und gilt nicht für alle Datensätze desselben Typs.
* Sie können nur Bilddateien als Miniaturen hinzufügen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Sie können einzelnen Datensätzen in der Tabellenansicht oder über die Seite oder das Vorschaufeld des Datensatzes ein Miniaturbild hinzufügen.
* Workfront lädt bei jeder Erstellung eines Datensatzes automatisch ein Miniaturbild hoch. Sie können dieses Bild später ändern.
* Miniaturansichten gehören zu den Datensatzinformationen und werden in Bereichen angezeigt, in denen Datensätze angezeigt werden. Beispielsweise werden Miniaturansichten neben Datensatzinformationen in den folgenden Bereichen angezeigt:

   * Das primäre Feld eines Datensatzes in der Tabellenansicht
   * Die Datensatzleiste in der Zeitleisten -Ansicht.
   * Details und Vorschau des Datensatzes.

## Hinzufügen einer Miniaturansicht zu einem Datensatz

Sie können eine Miniaturansicht wie folgt hinzufügen:

* [Hinzufügen einer Miniaturansicht zu einem Datensatz aus der Tabellenansicht](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Hinzufügen einer Miniaturansicht zu einem Datensatz über die Detailseite](#add-a-thumbnail-to-a-record-from-the-details-page)

### Hinzufügen einer Miniaturansicht zu einem Datensatz aus der Tabellenansicht

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, für dessen Datensätze Sie Miniaturansichten hinzufügen möchten, und klicken Sie dann auf die Karte „Datensatztyp“.

   Dadurch wird die Seite „Datensatztyp“ geöffnet.
1. Wählen Sie eine Tabellenansicht aus dem Dropdown **Menü** Ansicht“ aus. Alle Datensätze des ausgewählten Typs werden in einer Tabelle angezeigt.
1. Bewegen Sie den Mauszeiger über die Primärfeldinformationen und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und dann auf **Miniatur**.

   ![Menü „Mehr aufzeichnen“ erweitert](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Das primäre Feld ist das Feld, das in der ersten Spalte einer Tabellenansicht angezeigt wird. Das primäre Feld ist immer eingefroren und kann nicht ausgeblendet oder verschoben werden. Die Option „Miniaturansicht“ ist im Menü Mehr nicht verfügbar, wenn das primäre Feld ein Formelfeld ist.

   Die **Hochladen** wird standardmäßig im Feld **Miniaturansicht aufzeichnen** geöffnet.

   Weitere Informationen zum Hochladen der Miniaturansicht finden Sie im Abschnitt [Hinzufügen einer Miniaturansicht zu einem Datensatz auf der Detailseite](#add-a-thumbnail-to-a-record-from-the-details-page) in diesem Artikel, beginnend mit Schritt 6. <!--see if this is accurate-->

<!--
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![Upload new image icon](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![Remove image icon](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![Record thumbnail box for gallery](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![More menu](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![Remove image icon](assets/remove-image-icon.png), then click **Save changes**. -->

### Hinzufügen einer Miniaturansicht zu einem Datensatz über die Detailseite

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, für dessen Datensätze Sie Miniaturansichten hinzufügen möchten, und klicken Sie dann auf die Karte „Datensatztyp“.

   Dadurch wird die Seite „Datensatztyp“ geöffnet.
1. Klicken Sie in einer beliebigen Ansicht auf einen Datensatz, um ihn zu öffnen.

   Das Vorschaufeld Details wird angezeigt.
1. (Optional) Klicken Sie auf **In neuer Registerkarte öffnen** Symbol ![Details in einer neuen Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) in der oberen rechten Ecke.

   Die Detailseite des Datensatzes wird geöffnet.

1. (Bedingt) Bewegen Sie auf der Seite „Datensatzvorschau“ oder „Details“ den Mauszeiger über das Miniaturbild oder Symbol ![Miniaturansicht aufzeichnen auf der Detailseite](assets/record-thumbnail-icon-on-details-page.png) bewegen Sie dann den Mauszeiger über den Bereich über dem Datensatznamen und klicken Sie dann auf **Miniaturansicht hinzufügen** oder **Miniaturansicht bearbeiten**.

   Die **Hochladen** wird standardmäßig im Feld **Miniaturansicht aufzeichnen** geöffnet.

   ![Aufzeichnen des Miniaturfelds zum Hochladen](assets/record-thumbnail-box-for-upload.png)

1. Datei per Drag-and-Drop ziehen, um sie als Miniatur hinzuzufügen

   Oder

   Klicken Sie **Bilder durchsuchen** und suchen Sie dann nach einer Bilddatei, die Sie hinzufügen möchten. Die Datei muss auf Ihrem Computer gespeichert werden.

1. (Optional) Verwenden Sie nach dem Hochladen des Bildes im Feld **Miniaturansicht aufzeichnen** das Größenänderungswerkzeug, um das Bild zuzuschneiden und seine Größe zu ändern.
1. (Optional) Klicken Sie auf das Symbol **Neues Bild hochladen** (![&#x200B; Symbol Neues Bild hochladen](assets/upload-new-image-icon.png), um ein anderes Bild hochzuladen.
1. (Optional) Klicken Sie auf die **Galerie** und dann auf ein Bild. Die Bildergalerie kann nicht geändert werden.

   ![Aufzeichnen des Miniaturfelds für die Galerie](assets/record-thumbnail-box-for-gallery.png)

1. (Optional) Um die Miniaturansicht vor dem Speichern zu entfernen, klicken Sie auf das Symbol **Entfernen** ![Symbol „Bild entfernen](assets/remove-image-icon.png) rechts neben dem Bild.

1. Klicken Sie **Bild verwenden**, um das Bild als Miniatur hinzuzufügen.
Dadurch wird das Feld **Miniaturansicht aufzeichnen** geschlossen.
Die Miniaturansicht wird in den Bereichen von Workfront Planning angezeigt, in denen der Datensatz angezeigt wird.

   >[!TIP]
   >
   >   Sie müssen das Feld Miniaturansicht in der Tabellenansicht aktivieren, um Miniaturansichten in dieser Ansicht anzuzeigen. Sie ist standardmäßig deaktiviert.

1. (Optional) Um die Miniaturansicht nach dem Speichern zu entfernen, klicken Sie auf einen Datensatz in einer beliebigen Ansicht, um die Detailseite zu öffnen. Bewegen Sie dann den Mauszeiger über das Miniaturbild und klicken Sie auf das **Mehr**-Menü ![Mehr Menüsymbol](assets/more-menu.png)> **Entfernen**-Symbol ![Entfernen-Symbol](assets/remove-image-icon.png). Das Miniaturbild wird entfernt.


<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![More menu](assets/more-menu.png), then click **Thumbnail**. 

   ![Record more menu expanded](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->
