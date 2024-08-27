---
title: Datensätze bearbeiten
description: Sie können Datensatzinformationen in der Adobe Workfront-Planung bearbeiten. Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '1868'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Datensätze bearbeiten

{{planning-important-intro}}

Sie können Datensatzinformationen in der Adobe Workfront-Planung bearbeiten, indem Sie die Werte der mit den Datensätzen verknüpften Felder bearbeiten.

Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

Informationen zum Erstellen von Datensätzen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

&lt;!— Erwähnen Sie hier, dass die Felder in der Detailansicht mit denen in der Tabellenansicht identisch sind. Dieser Artikel ist über die Option Datensatzansichten verwalten verknüpft, um auf diese Informationen zu verweisen.—>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

Für den Zugriff auf die Workfront-Planung benötigen Sie Folgendes:

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
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen finden Sie unter <a href="https://business.adobe.com/products/workfront/pricing.html">Preise und Verpackung für Adobe Workfront</a>. </p> 
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
   <td> <p>Standard</p> 
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
   <td>  <p>Contribute oder höhere Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Überlegungen zum Bearbeiten von Datensätzen

* Sie können von Ihnen erstellte Datensätze oder von anderen Benutzern erstellte Datensätze bearbeiten, wenn Sie über Berechtigungen für den Arbeitsbereich verfügen.
* Sie können Datensatzfelder aus den folgenden Bereichen bearbeiten:

   * Vorschau des Datensatzes in einer Datensatzansicht
   * Die Datensatzseite
   * Inline in einer Tabellenansicht.

* Wenn ein Benutzer einen Datensatz in einer Ansicht bearbeitet, sind die Änderungen sofort in allen Ansichten und den Datensatzseiten für alle anderen Benutzer sichtbar.

* Die folgenden Feldtypen werden automatisch aktualisiert und ihre Werte können nicht manuell bearbeitet werden:
   * Verknüpfte Felder anderer Datensätze
   * Felder vom Typ Formel
   * Systemfelder (erstellt von, Erstellungsdatum, Letzte Änderung durch, Datum der letzten Änderung)
* Wenn die angezeigten Datensätze mit anderen Datensätzen verknüpft sind, werden die neuen Informationen der von Ihnen bearbeiteten Datensätze in den verknüpften Datensätzen angezeigt.
* Datensätze können nicht stapelweise bearbeitet werden. <!--this will probably change-->
* URLs werden nur dann als Links in einzeiligen Textfeldtypen erkannt, wenn sie mit den folgenden Begriffen beginnen: http://, https://, ftp:// oder www. .
* Sie können jedem Datensatz ein Titelbild hinzufügen. Das Bild ist für jeden Datensatz eindeutig und gilt nicht für alle Datensätze derselben Zeit.
* Sie können die Reihenfolge der Felder auf einer Datensatzseite bearbeiten und ein Titelbild für einen Datensatz hinzufügen. Weitere Informationen finden Sie unter [Layout der Datensatzseite verwalten](/help/quicksilver/planning/records/manage-the-record-page.md).

## Datensätze bearbeiten

Sie können einen Datensatz aus den folgenden Bereichen bearbeiten:

* [Aus der Tabellenansicht eines Datensatztyps](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [Über die Vorschau des Datensatzes in einer Ansicht](#edit-a-record-from-the-records-preview-in-a-view)
* [Auf der Datensatzseite](#edit-a-record-from-the-records-page)
* [Von einem Workfront-Objekt im Abschnitt Planung](#edit-a-record-from-a-workfront-object-in-the-planning-section)

### Datensatz in der Tabellenansicht eines Datensatztyps inline bearbeiten

Wenn Sie Datensätze aus der Tabellenansicht bearbeiten, gibt es einen Hinweis, welches Feld von anderen Benutzern zum Zeitpunkt der Anzeige des Datensatzes bearbeitet wird.

Weitere Informationen finden Sie unter [Ansichten von Datensätzen verwalten](/help/quicksilver/planning/views/manage-record-views.md).

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie bearbeiten möchten

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Klicken Sie auf die Registerkarte einer Tabellenansicht oder klicken Sie auf **+ Ansicht** , um eine Tabellenansicht zu erstellen. Die Tabellenansicht sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp beim letzten Zugriff in einer anderen Ansicht angezeigt.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Klicken Sie in die Zeile eines Datensatzes, um Informationen über den Datensatz inline zu bearbeiten.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  Sie können Informationen für die folgenden Felder nicht bearbeiten, da sie schreibgeschützt sind und Workfront sie automatisch aktualisiert:
   >  
   >  * Verknüpfte Felder, die durch Verbinden von Datensatztypen erstellt werden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Felder der folgenden Typen: Erstellt von, Erstellungsdatum, Letzte Änderung durch, Letztes Änderungsdatum, Formelfelder.

1. (Optional und bedingt) Verwenden Sie beim Bearbeiten eines Absatztypfelds die folgenden **Rich Text** -Formatierungsoptionen:

   * Fett
   * Kursiv
   * Unterstreichen
   * Link hinzufügen
   * Liste mit Aufzählungszeichen hinzufügen
   * Nummerierte Liste hinzufügen

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Optional) Doppelklicken Sie auf ein Feld für einen verbundenen Datensatz, um verbundene Datensätze oder Objekte zu einem anderen Datensatz hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).
1. Drücken Sie die **Eingabetaste** auf Ihrer Tastatur oder klicken Sie außerhalb einer Zeile auf , um Ihre Änderungen zu speichern. Die Änderungen werden automatisch gespeichert. In der oberen rechten Ecke der Tabellenansicht wird ein Indikator **Gespeichert** angezeigt, der anzeigt, dass die Änderungen gespeichert wurden.


1. (Optional) Um Informationen von einem Feld in ein anderes zu kopieren und einzufügen, führen Sie einen der folgenden Schritte aus:

   * Kopieren Sie einen oder mehrere vorhandene Werte eines Felds und fügen Sie sie dann in ein Feld desselben Typs in einen anderen Datensatz ein.
   * Klicken Sie auf die Spaltenüberschrift einer Spalte, um sie auszuwählen und zu kopieren. Klicken Sie dann auf die Spaltenüberschrift einer anderen Spalte und fügen Sie den Inhalt der kopierten Spalte ein. Die Spalten müssen ähnliche Feldtypen enthalten.
   * Klicken Sie bei gedrückter Umschalt-Taste auf mehrere Zeilen in einer Tabelle, kopieren Sie die Informationen in die ausgewählten Zeilen, klicken Sie dann auf eine andere Zeile und fügen Sie die ausgewählten Informationen in die neue Zeile und die folgenden Zeilen ein.
   * Kopieren Sie die Informationen aus einer Zelle, wählen Sie dann mehrere Zellen aus und fügen Sie dieselben Informationen in mehrere Zellen ein. Sie können mehrere Zellen auswählen und dieselben Informationen in mehrere Zellen aus benachbarten Zeilen und Spalten einfügen.
   * Wählen Sie die untere rechte Ecke einer vorhandenen Zelle aus, die die zu kopierenden Informationen enthält, und ziehen Sie sie per Drag-and-Drop über die angrenzenden Zellen, in die Sie dieselben Informationen einfügen möchten. Alle Zellen müssen denselben Informationstyp aufweisen.

     ![](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)

   >[!NOTE]
   >
   >Beachten Sie Folgendes:
   >
   >* Verwenden Sie die folgenden Tastaturbefehle zum Kopieren und Einfügen von Informationen:
   >   * Kopieren: STRG + C ( ⌘ + C für Mac)
   >   * Einfügen: STRG + V ( ⌘ + V für Mac)
   >
   >* Feldwerte können nicht kopiert und in die Datensatzseite eingefügt werden. Diese Funktion wird nur in der Tabellenansicht eines Datensatztyps unterstützt.
   >* Für die folgenden Feldtypen können Sie keine Feldwerte kopieren und einfügen:
   >
   >
   >    * Verknüpfte Felder (oder Suchfelder), die durch Verbinden von Datensatztypen erstellt werden. Sie können verknüpfte Datensatzfelder kopieren und einfügen. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   >    * Felder der folgenden Typen: Erstellt von, Erstellungsdatum, Letzte Änderung durch, Datum der letzten Änderung

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um die Bearbeitung oder das Kopieren und Einfügen von Datensatzinformationen rückgängig zu machen oder wiederherzustellen:

   * STRG + Z ( ⌘ + Z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Umschalt + Z ( ⌘ + Umschalt + Z für Mac) zum Wiederholen einer Änderung

   >[!TIP]
   >
   >    Sie können die Tastaturbefehle mehrmals hintereinander verwenden, um mehrere Änderungen rückgängig zu machen.

1. (Optional) Fügen Sie einem Datensatz eine Miniaturansicht hinzu. Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

### Datensatz aus der Datensatzvorschau in einer Ansicht bearbeiten

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie bearbeiten möchten

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer Ansicht beliebigen Typs auf den Datensatz.

   Oder

   Klicken Sie in der Tabellenansicht in der ersten Spalte auf das Symbol **Details öffnen** ![](assets/open-details-icon-in-table-name-field.png) . Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

1. (Optional) Klicken Sie auf das Menü **Mehr** rechts neben dem Titel des Datensatzes und dann auf **Umbenennen**. Dadurch wird das Feld aktualisiert, das als Titel des Datensatzes angezeigt wird.

   Der Titel des Datensatzes ist das primäre Feld des Datensatzes bei der Anzeige in einer Tabellenansicht. Weitere Informationen finden Sie unter [Übersicht über Primäre Felder](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Beginnen Sie mit der Bearbeitung der Feldinformationen in der Datensatzvorschau.

   >[!TIP]
   >
   >  Sie können Informationen für die folgenden Felder nicht bearbeiten, da sie schreibgeschützt sind und Workfront sie automatisch aktualisiert:
   >  
   >  * Suchfelder aus anderen Datensätzen, die durch Verbinden von Datensatztypen erstellt werden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Felder der folgenden Typen: Erstellt von, Erstellungsdatum, Letzte Änderung durch, Letztes Änderungsdatum, Formelfelder.

1. (Optional) Klicken Sie auf **Abdeckung hinzufügen** , um dem Datensatz ein Titelbild hinzuzufügen. Weitere Informationen finden Sie unter [Hinzufügen eines Titelbilds zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Optional) Bewegen Sie den Mauszeiger über das Miniaturbild-Symbol und klicken Sie dann auf **Mehr** ![](assets/more-menu.png) > **Miniaturansicht bearbeiten** , um ein Miniaturbild hinzuzufügen. Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront speichert Ihre Änderungen automatisch.

1. (Optional) Klicken Sie auf das Symbol **Exportieren** ![](assets/export-icon-in-record-details-page.png), um die Details des Datensatzes zu exportieren. Weitere Informationen finden Sie unter [Details eines Datensatzes exportieren](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Optional) Klicken Sie oben rechts in der Datensatzvorschau auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> , um die Datensatzseite in einer neuen Registerkarte zu öffnen. Fahren Sie mit der Bearbeitung des Datensatzes fort, wie im Abschnitt [Datensatz auf der Seite des Datensatzes bearbeiten](#edit-a-record-from-the-records-page) in diesem Artikel beschrieben.

### Datensatz auf der Datensatzseite bearbeiten

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie bearbeiten möchten

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Führen Sie einen der folgenden Schritte aus:

   * Rufen Sie in jeder Ansicht die Vorschau des Datensatzes auf, wie im Abschnitt [Datensatz aus der Datensatzvorschau in einer Ansicht bearbeiten](#edit-a-record-from-the-records-preview-in-a-view) in diesem Artikel beschrieben, und klicken Sie dann oben rechts in der Datensatzvorschau auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> , um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen.

   * Bewegen Sie in der Ansicht **Tabelle** den Mauszeiger über den Namen eines Datensatzes, klicken Sie dann auf das Menü **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Anzeigen** .

     ![](assets/contextual-menu-for-record-row.png)

     Die Datensatzseite wird geöffnet.

     ![](assets/details-page.png)

1. (Optional) Klicken Sie auf das Menü **Mehr** rechts neben dem Titel des Datensatzes und dann auf **Umbenennen**. Dadurch wird das Feld aktualisiert, das als Titel des Datensatzes angezeigt wird.

   Der Titel des Datensatzes ist das primäre Feld des Datensatzes bei der Anzeige in einer Tabellenansicht. Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

1. Klicken Sie auf ein beliebiges bearbeitbares Feld auf der Datensatzseite, um es zu bearbeiten.

   >[!TIP]
   >
   >  Sie können Informationen für die folgenden Felder nicht bearbeiten, da sie schreibgeschützt sind und Workfront sie automatisch aktualisiert:
   >  
   >  * Verknüpfte Felder, die durch Verbinden von Datensatztypen erstellt werden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Felder der folgenden Typen: Erstellt von, Erstellungsdatum, Letzte Änderung durch, Letztes Änderungsdatum, Formelfelder.

1. (Optional) Klicken Sie auf **Abdeckung hinzufügen** , um dem Datensatz ein Titelbild hinzuzufügen.

   Oder

   Bewegen Sie den Mauszeiger über das vorhandene Titelbild und klicken Sie dann auf das Menü **Mehr** ![](assets/more-menu.png) > **Hochladen** , um ein neues Titelbild für den Datensatz hinzuzufügen.

   Weitere Informationen finden Sie unter [Hinzufügen eines Titelbilds zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine vorhandene Miniaturansicht oder das **Miniatursymbol** ![](assets/record-thumbnail-icon-on-details-page.png) und klicken Sie dann auf das Menü **Mehr** > ![](assets/more-menu.png) > **Miniaturansicht bearbeiten** , um eine Miniaturansicht für den Datensatz hinzuzufügen.

   Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront speichert Ihre Änderungen automatisch.

1. (Optional) Klicken Sie auf das Symbol **Exportieren** ![](assets/export-icon-in-record-details-page.png), um die Details des Datensatzes zu exportieren. Weitere Informationen finden Sie unter [Details eines Datensatzes exportieren](/help/quicksilver/planning/records/export-the-record-page.md).


## Datensatz aus einem Workfront-Objekt im Abschnitt Planung bearbeiten

Nachdem Sie Datensätze mit Workfront-Objekten verbunden haben, können Sie die Workfront-Planungsdatensätze in Workfront im Bereich Planung des Objekts bearbeiten.

Weitere Informationen finden Sie unter [Verwalten von Datensätzen im Abschnitt &quot;Planung&quot;von Adobe Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).