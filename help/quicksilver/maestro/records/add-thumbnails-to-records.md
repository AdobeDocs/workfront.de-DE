---
title: Miniaturansichten zu Datensätzen hinzufügen
description: Sie können Datensatzinformationen in Adobe Maestro bearbeiten und jeden Datensatz mit individuellen Miniaturansichten verknüpfen, damit sie leicht erkennbar sind.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Miniaturansichten zu Datensätzen hinzufügen

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Datensätze mit eindeutigen Miniaturansichten in Adobe Maestro verknüpfen, um sie leicht zu erkennen.

Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.
Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

## Zugriffsanforderungen

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für Maestro </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Beitragen oder höhere Berechtigungen zu einem Arbeitsbereich </p>  
   <p>Beitragen oder höhere Berechtigungen zur Tabellenansicht </p> 
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>


## Überlegungen zu Miniaturansichten von Datensätzen

Um in einer Tabellenansicht visuell zwischen Datensätzen zu unterscheiden, können Sie jedem Datensatz ein eindeutiges Miniaturbild zuordnen.

Beachten Sie Folgendes:

* Sie können nur Bilddateien als Miniaturansichten hinzufügen.
* Sie können einzelnen Datensätzen in der Tabellenansicht ein Miniaturbild hinzufügen.
* Auf der Detailseite des Datensatzes oder in der Timeline-Ansicht können Sie keine Datensatzminiaturansichten hinzufügen.
* Das Miniaturbild wird unabhängig vom Feldtyp immer links neben dem primären Feld jedes Datensatzes angezeigt.

  Felder mit einzeiligem Text, Zahlen oder Formeln können als primäre Felder bezeichnet werden.
Weitere Informationen finden Sie unter [Tabellenansicht verwalten](/help/quicksilver/maestro/views/manage-the-table-view.md).

<!--above: when you know exactly what type of files are allowed, add the exact extensions above-->

## Hinzufügen einer Miniaturansicht zu einem Datensatz

{{step1-to-maestro}}

1. Wählen Sie den Arbeitsbereich aus, für dessen Datensätze Sie Miniaturansichten hinzufügen möchten, und klicken Sie dann auf die Karte vom Typ Datensatz .

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.
1. Wählen Sie eine Tabellenansicht aus dem **Ansicht** Dropdown-Menü. Alle Datensätze des ausgewählten Typs werden in einer Tabelle angezeigt.
1. Bewegen Sie den Mauszeiger über die primären Feldinformationen und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Miniatur**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   Das primäre Feld ist das Feld, das in der ersten Spalte einer Tabellenansicht angezeigt wird. Das Primärfeld ist immer eingefroren und kann nicht ausgeblendet oder neu positioniert werden.

   Die **Miniaturansicht aufzeichnen** wird geöffnet.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. Im **Hochladen** Registerkarte eine Datei per Drag-and-Drop als Miniaturansicht hinzufügen, oder klicken Sie auf **Hochladen auswählen**, suchen Sie dann nach einer Bilddatei, die hinzugefügt werden soll. Die Datei muss auf Ihrem Computer gespeichert werden.
1. (Optional) Verwenden Sie das Größenanpassungs-Tool, um das Bild zu beschneiden und seine Größe zu ändern.
1. Klicks **Bild verwenden** , um das Bild als Miniaturansicht hinzuzufügen.
Dadurch wird die **Miniaturansicht aufzeichnen** ankreuzen.
1. Klicken Sie in der oberen rechten Ecke der Tabellenansicht auf Felder .
1. Wählen Sie die **Miniatur** umschalten, um die Miniaturansicht anzuzeigen. Diese Option ist standardmäßig deaktiviert.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   Die Miniaturansicht wird links neben dem primären Feldwert angezeigt.
1. (Optional) Um die Miniaturansicht zu entfernen, bewegen Sie den Mauszeiger über das primäre Feld und klicken Sie auf **Mehr** Menü ![](assets/more-menu.png)> **Miniatur** > die **Entfernen** icon ![](assets/remove-image-icon.png)Klicken Sie auf **Änderungen speichern**.