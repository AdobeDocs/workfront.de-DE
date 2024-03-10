---
title: Verwalten von Datensatzansichten
description: Bei Verwendung der Planungsfunktionen von Adobe Workfront können Sie Datensätze in einer Tabellen-, Timeline- oder Kalenderansicht anzeigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 2c630ad348955380620eef073b0c7dde81d11835
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 1%

---

# Verwalten von Datensatzansichten

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Nach Auswahl eines Datensatztyps im Adobe Workfront-Planungsbereich können Sie alle Datensätze dieses Typs in den folgenden Ansichten anzeigen:

* Tabelle

  Weitere Informationen finden Sie unter [Tabellenansicht verwalten](../views/manage-the-table-view.md).

* Timeline

  Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](../views/manage-the-timeline-view.md).

* Kalender

  Weitere Informationen finden Sie unter [Kalenderansicht verwalten](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

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
<p>Ihr Unternehmen muss am geschlossenen Betaprogramm für Planungsfunktionen der Adobe Workfront teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   <td> <p>Es gibt keine Zugriffssteuerungsmöglichkeiten für Workfront-Planungsfunktionen</p>  
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

## Überlegungen zum Arbeiten mit Datensatzansichten

* Ansichten im Workfront-Planungsbereich sind typspezifisch für Datensätze. Sie können dieselbe Ansicht nicht auf zwei verschiedene Datensatztypen anwenden.
* Von Ihnen erstellte Ansichten sind nur für Sie und Benutzer sichtbar, für die Sie die Ansichten freigeben.
* Das Erstellen von Ansichten für betriebliche Datensatztypen ist mit dem Erstellen von Ansichten für Taxonomiedatensatztypen identisch.
* Wenn Sie eine Ansicht ändern oder löschen, wird sie für alle Benutzer mit Berechtigungen für die Ansicht geändert und gelöscht.
* Die folgenden Elemente sind für jede Datensatzansicht eindeutig:

   * Filter
   * Gruppierung
   * Sortieren

  <!-- some of these are not available in all of the views - edit above-->

  Wenn Sie beispielsweise einen Filter in einer Tabellenansicht erstellen, sind die Filterergebnisse nur in der ausgewählten Ansicht sichtbar und nicht in allen im Dropdown-Menü Ansicht aufgeführten Ansichten.

  >[!NOTE]
  >
  > Da sich die Planungsfunktionen von Adobe Workfront derzeit in der Beta-Phase befinden, stehen einige Ansichtselemente möglicherweise nicht allen Ansichten zur Verfügung.

In diesem Artikel werden die folgenden Informationen zu Datensatzansichten beschrieben:

* [Erstellen und Bearbeiten einer Ansicht](#create-or-edit-record-views)
* [Ansicht löschen](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Anzeigen freigeben](#share-a-view)

## Ähnlichkeiten und Unterschiede zwischen Datensatzansichten

Die folgende Tabelle zeigt die Ähnlichkeiten und Unterschiede zwischen der Tabellen-, Timeline- und Kalenderansicht:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funktion | Tabellenansicht | Timeline-Ansicht | Kalenderansicht |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Anzeigen von Datensätzen in einer Liste oder Tabelle | ✓ |              | |
| Alle Felder standardmäßig als Spalten in der Tabelle anzeigen | ✓ |              |    |
| Felder (oder Spalten) aus- oder einblenden | ✓ |               |    |
| Feldwerte für jeden Datensatz bearbeiten | ✓ |               |             |
| Hinzufügen von Datensätzen als neue Zeilen in der Ansicht | ✓ |               |        |
| Felder als neue Spalten in der Ansicht hinzufügen | ✓ |               |         |
| Zeilen aus einer externen Liste kopieren und in eine Tabelle einfügen | ✓ |               |          |
| Anzeigen von Datensätzen in einer Timeline |            | ✓ |             |
| Datensätze filtern | ✓ | ✓ |           |
| Datensätze in einem Kalender anzeigen |           |              | ✓ |
| Gruppeneinträge | ✓ | ✓ |
| Datensätze sortieren | ✓ |              |
| Farbcode-Datensätze |           | ✓ | ✓ |
| Farbcode-Gruppierungen |           | ✓ |
| Suche nach bestimmten Datensätzen | ✓ | ✓ |
| Freigabeansicht | ✓ | ✓ | ✓ |
| Öffnen Sie die Detailseite des Datensatzes in der Ansicht. | ✓ | ✓ |    |


## Ansichten erstellen oder bearbeiten {#create-or-edit-views}

{{step1-to-maestro}}


Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet. Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).

1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

   Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

<!--
1. Click **+ View** to add a new view. 
1. Select from the following types of views: 

    * Table
    * Timeline
    * Calendar

>[!TIP]
>
>When you create a record type, the table view is also created by default. 
>
>To create a timeline or a calendar view, the record type you build the view for must have at least two date fields. Otherwise, the Timeline and the Calendar options are dimmed.
>
>(*********remove the step below and replace the screen shot when calendar view releases*********)
-->

1. Klicken Sie auf **Ansicht** und wählen Sie entweder ein vorhandenes **Tabellenansicht** ![](assets/table-view-icon.png) oder klicken Sie **Ansicht erstellen > Tabelle** zum Erstellen einer Tabellenansicht

   Oder

   Existierende Auswahl **Timeline-Ansicht** ![](assets/timeline-view-icon.png) oder klicken Sie **Ansicht erstellen > Timeline** , um eine Timeline-Ansicht zu erstellen.

   Oder

   Existierende Auswahl **Kalenderansicht** ![](assets/calendar-view-icon.png) oder klicken Sie **Ansicht erstellen > Kalender** um eine Kalenderansicht zu erstellen.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Um eine Timeline- oder Kalenderansicht zu erstellen, muss der Datensatztyp, für den Sie die Ansicht erstellen, mindestens zwei Datumsfelder aufweisen. Andernfalls sind die Optionen Timeline oder Kalender abgeblendet.

1. (Bedingt) Klicken Sie auf **Nächste** beim Erstellen einer Timeline- oder Kalenderansicht.

   Standardmäßig gibt Workfront der Ansicht einen der folgenden Namen:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Die Zahl ist ein automatisch generiertes Inkrement.

1. (Bedingt) Wählen Sie die **Starten** und **Enddaten** für die Datensätze, die in der Timeline- oder Kalenderansicht angezeigt werden.
1. Klicken Sie auf **Erstellen**.

   <!--add for view redesign: The view displays as a new tab. Views display in the chronological order from when they were created or shared with you. -->
<!--1. (Optional) Click the **More** menu ![](assets/more-caret-down-icon-views.png) next to the last view to view all views for the selected record type. 

    Additional views display under the **More** menu after the last view tab. The number next to the **More** menu shows the number of additional views. -->
1. (Optional) Um eine Ansicht nach ihrer Erstellung umzubenennen, klicken Sie auf das Dropdown-Menü &quot;Ansicht&quot;und dann auf **Mehr** Menü ![](assets/more-menu.png) > **Umbenennen** , um den Ansichtsnamen zu aktualisieren. <!--ensure there is not another saving step here?!-->
   <!--1. (Optional) To rename a view after it is created, double-click the view name and start typing the new name, or click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Rename**.-->
1. (Optional) Informationen zum Verwalten einer bestimmten Ansicht finden Sie in den folgenden Artikeln:

   * [Tabellenansicht verwalten](../views/manage-the-table-view.md)
   * [Verwalten der Timeline-Ansicht](../views/manage-the-timeline-view.md)
   * [Kalenderansicht verwalten](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## Ansichten löschen

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet. Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

   Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

<!--1. Hover over on the of the view's names in the view tab, then click **More** ![](assets/more-menu.png) > **Delete**. (********delete the instructions in the point below but keep the last step***********)-->
1. Klicken Sie auf das Dropdown-Menü &quot;Ansicht&quot;, bewegen Sie den Mauszeiger über eine der Ansichten in der Liste und klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) > **Löschen**.
1. Klicks **Löschen** zur Bestätigung. <!--ensure there is not another saving step here?!-->

   Die Ansicht wird für alle Benutzer gelöscht, die auf den Datensatzbereich zugreifen können, und kann nicht wiederhergestellt werden.

## Anzeigen freigeben

Informationen zum Freigeben von Ansichten finden Sie unter [Ansichten freigeben](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
