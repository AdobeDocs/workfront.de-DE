---
title: Hinzufügen einer Miniaturansicht zu einem Datensatz
description: Sie können Datensatzinformationen in der Adobe Workfront-Planung bearbeiten und jeden Datensatz mit individuellen Miniaturansichten verknüpfen, damit sie leicht erkennbar sind.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---


# Hinzufügen einer Miniaturansicht zu einem Datensatz

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.


{{planning-important-intro}}

In der Adobe Workfront-Planung können Sie Datensätze mit eindeutigen Miniaturansichten verknüpfen, damit sie leicht erkennbar sind.

Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.
Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

## Zugriffsanforderungen

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Berechtigungen für einen Arbeitsbereich verwalten </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zu Miniaturansichten von Datensätzen

Um in einer Tabellenansicht visuell zwischen Datensätzen zu unterscheiden, können Sie jedem Datensatz ein eindeutiges Miniaturbild zuordnen.

Beachten Sie Folgendes:

* Eine Miniaturansicht ist für einen Datensatz eindeutig und gilt nicht für alle Datensätze desselben Typs.
* Sie können nur Bilddateien als Miniaturansichten hinzufügen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Sie können einzelnen Datensätzen in der Tabellenansicht oder auf der Datensatzseite oder im Vorschaufeld eine Miniaturansicht hinzufügen.
* Workfront lädt jedes Mal, wenn Sie einen Datensatz erstellen, automatisch ein Miniaturbild hoch. Sie können dieses Bild später ändern.
* Miniaturansichten gehören zu den Datensatzinformationen und werden in Bereichen angezeigt, in denen Datensätze angezeigt werden. Beispielsweise werden Miniaturansichten neben Datensatzinformationen in den folgenden Bereichen angezeigt:

   * Das primäre Feld eines Datensatzes in der Tabellenansicht
   * Die Datensatzleiste in der Timeline-Ansicht.
   * Vorschau und Seite der Details des Datensatzes.

## Hinzufügen einer Miniaturansicht zu einem Datensatz

Sie können eine Miniaturansicht wie folgt hinzufügen:

* [Hinzufügen einer Miniaturansicht zu einem Datensatz aus der Tabellenansicht](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Hinzufügen einer Miniaturansicht zu einem Datensatz von der Detailseite](#add-a-thumbnail-to-a-record-from-the-details-page)

### Hinzufügen einer Miniaturansicht zu einem Datensatz aus der Tabellenansicht

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, für dessen Datensätze Sie Miniaturansichten hinzufügen möchten, und dann auf die Karte vom Typ Datensatz.

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.
1. Wählen Sie eine Tabellenansicht aus dem Dropdownmenü **Ansicht** aus. Alle Datensätze des ausgewählten Typs werden in einer Tabelle angezeigt.
1. Bewegen Sie den Mauszeiger über die primären Feldinformationen, klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) und dann auf **Miniatur**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Das primäre Feld ist das Feld, das in der ersten Spalte einer Tabellenansicht angezeigt wird. Das Primärfeld ist immer eingefroren und kann nicht ausgeblendet oder neu positioniert werden. Die Option Miniaturansicht ist im Menü Mehr nicht verfügbar, wenn das primäre Feld ein Formelfeld ist.

   Die Registerkarte **Hochladen** wird standardmäßig im Feld **Miniaturansicht aufzeichnen** geöffnet.

   Weitere Informationen zum Hochladen der Miniaturansicht finden Sie im Abschnitt [Hinzufügen einer Miniaturansicht zu einem Datensatz von der Detailseite](#add-a-thumbnail-to-a-record-from-the-details-page) in diesem Artikel, beginnend mit Schritt 6 <!--see if this is accurate-->.

<!--
   ![](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**. -->

### Hinzufügen einer Miniaturansicht zu einem Datensatz von der Detailseite

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, für dessen Datensätze Sie Miniaturansichten hinzufügen möchten, und dann auf die Karte vom Typ Datensatz.

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.
1. Klicken Sie in einer beliebigen Ansicht auf einen Datensatz, um ihn zu öffnen.

   Das Vorschaufeld für Details wird angezeigt.
1. (Optional) Klicken Sie oben rechts auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) .

   Die Detailseite des Datensatzes wird geöffnet.

1. (Bedingt) Bewegen Sie in der Datensatzvorschau oder -seite den Mauszeiger über das Miniaturbild oder Symbol ![](assets/record-thumbnail-icon-on-details-page.png) und klicken Sie dann in der Produktionsumgebung auf das Menü **Mehr** > ![](assets/more-menu.png) > **Miniatur bearbeiten** .

   Oder

   <span class="preview">Bewegen Sie den Mauszeiger über den Bereich über dem Datensatznamen und klicken Sie dann in der Vorschauumgebung auf **Miniatur hinzufügen** oder **Miniatur bearbeiten** .</span>

   Die Registerkarte **Hochladen** wird standardmäßig im Feld **Miniaturansicht aufzeichnen** geöffnet.

   ![](assets/record-thumbnail-box-for-upload.png)

1. Datei per Drag-and-Drop als Miniaturansicht hinzufügen

   Oder

   Klicken Sie auf **Bilder durchsuchen** und suchen Sie dann nach einer Bilddatei, die hinzugefügt werden soll. Die Datei muss auf Ihrem Computer gespeichert werden.

1. (Optional) Nachdem die Bild-Uploads im Feld **Miniaturansicht aufzeichnen** durchgeführt wurden, verwenden Sie das Größenanpassungs-Tool, um das Bild zu beschneiden und die Größe zu ändern.
1. (Optional) Klicken Sie auf das Symbol **Neues Bild hochladen** ![](assets/upload-new-image-icon.png) , um ein anderes Bild hochzuladen.
1. (Optional) Klicken Sie auf die Registerkarte **Galerie** und dann auf ein Bild. Die Bildergalerie kann nicht geändert werden.

   ![](assets/record-thumbnail-box-for-gallery.png)

1. (Optional) Um die Miniaturansicht vor dem Speichern zu entfernen, klicken Sie auf das Symbol **Entfernen** ![](assets/remove-image-icon.png) rechts neben dem Bild.

1. Klicken Sie auf **Bild verwenden** , um das Bild als Miniaturansicht hinzuzufügen.
Dadurch wird das Feld **Miniaturansicht aufzeichnen** geschlossen.
Die Miniaturansicht wird in Bereichen der Workfront-Planung angezeigt, in denen der Datensatz angezeigt wird.

   >[!TIP]
   >
   >   Sie müssen das Feld &quot;Miniaturansicht&quot;in der Tabellenansicht aktivieren, damit in dieser Ansicht Miniaturansichten angezeigt werden. Sie ist standardmäßig deaktiviert.

1. (Optional) Um die Miniaturansicht nach dem Speichern zu entfernen, klicken Sie in einer beliebigen Ansicht auf einen Datensatz, um die Detailseite zu öffnen. Bewegen Sie dann den Mauszeiger über das Miniaturbild und klicken Sie auf das Symbol **Mehr** Menü ![](assets/more-menu.png)> **Entfernen** ![](assets/remove-image-icon.png). Das Miniaturbild wird entfernt.




<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->