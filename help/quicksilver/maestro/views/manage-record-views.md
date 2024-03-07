---
title: Verwalten von Datensatzansichten
description: Bei Verwendung von Adobe Maestro können Datensätze in einer Tabellen- oder Timeline-Ansicht angezeigt werden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: ff52e43fc5ed5a7939b9e28b2bda195e94e81724
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Verwalten von Datensatzansichten

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Nach Auswahl eines Datensatztyps in Adobe Maestro können Sie alle Datensätze dieses Typs in den folgenden Ansichten anzeigen:

* Tabelle

  Weitere Informationen finden Sie unter [Tabellenansicht verwalten](../views/manage-the-table-view.md).
* Timeline

  Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](../views/manage-the-timeline-view.md).

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
   <td role="rowheader">Konfiguration der Zugriffsebene</td>
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Maestro</p>  
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

## Überlegungen beim Arbeiten mit Maestro-Ansichten

* Ansichten in Maestro sind typspezifisch für Datensätze. Sie können dieselbe Ansicht nicht auf zwei verschiedene Datensatztypen anwenden.
* Von Ihnen erstellte Ansichten sind nur für Sie und Benutzer sichtbar, für die Sie die Ansichten freigeben.
* Das Erstellen von Ansichten für betriebliche Datensatztypen ist mit dem Erstellen von Ansichten für Taxonomiedatensatztypen identisch.
* Wenn Sie eine Ansicht ändern oder löschen, wird sie für alle Benutzer mit Berechtigungen für die Ansicht geändert und gelöscht.
* Die folgenden Elemente sind für jede Ansicht in Maestro eindeutig:

   * Filter
   * Gruppierung
   * Sortieren

  <!-- some of these are not available in all of the views - edit above-->

  Wenn Sie beispielsweise einen Filter in einer Tabellenansicht erstellen, sind die Filterergebnisse nur in der ausgewählten Ansicht sichtbar und nicht in allen im Dropdown-Menü Ansicht aufgeführten Ansichten.

  >[!NOTE]
  >
  > Da Maestro derzeit einen Beta-Status aufweist, sind einige Ansichtselemente möglicherweise nicht für beide Ansichten verfügbar.

In diesem Artikel werden die folgenden Informationen zu Maestro-Ansichten beschrieben:

* [Erstellen und Bearbeiten einer Ansicht](#create-or-edit-record-views)
* [Ansicht löschen](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Anzeigen freigeben](#share-a-view)

## Ähnlichkeiten und Unterschiede zwischen Tabellen- und Timeline-Ansichten

Die folgende Tabelle zeigt die Ähnlichkeiten und Unterschiede zwischen den Tabellen- und Timeline-Ansichten in Maestro:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funktion | Tabellenansicht | Timeline-Ansicht |
|-----------------------------------------------------------------------|------------|---------------|
| Anzeigen von Datensätzen in einer Liste oder Tabelle | ✓ |              |
| Alle Felder standardmäßig als Spalten in der Tabelle anzeigen | ✓ |              |
| Felder (oder Spalten) aus- oder einblenden | ✓ |               |
| Feldwerte für jeden Datensatz bearbeiten | ✓ |               |
| Hinzufügen von Datensätzen als neue Zeilen in der Ansicht | ✓ |               |
| Felder als neue Spalten in der Ansicht hinzufügen | ✓ |               |
| Zeilen aus einer externen Liste kopieren und in eine Tabelle einfügen | ✓ |               |
| Anzeigen von Datensätzen in einer Timeline |            | ✓ |
| Datensätze filtern | ✓ | ✓ |
| Gruppeneinträge | ✓ | ✓ |
| Datensätze sortieren | ✓ |              |
| Farbcode-Datensätze |           | ✓ |
| Farbcode-Gruppierungen |           | ✓ |
| Suche nach bestimmten Datensätzen | ✓ | ✓ |
| Freigabeansicht | ✓ | ✓ |
| Öffnen Sie die Detailseite des Datensatzes in der Ansicht. | ✓ | ✓ |

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
        >(*********remove all of the below steps and replace the screen shot when calendar view releases*********)
    -->

1. Klicken Sie auf **Ansicht** und wählen Sie entweder ein vorhandenes **Tabellenansicht** ![](assets/table-view-icon.png) oder klicken Sie **Ansicht erstellen > Tabelle** zum Erstellen einer Tabellenansicht

   Oder

   Existierende Auswahl **Timeline-Ansicht** ![](assets/timeline-view-icon.png) Ansicht oder Klicken **Ansicht erstellen > Timeline** , um eine Timeline-Ansicht zu erstellen.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Um eine Timeline-Ansicht zu erstellen, muss der Datensatztyp, für den Sie die Ansicht erstellen, mindestens zwei Datumsfelder aufweisen. Andernfalls ist die Option Timeline abgeblendet.

1. (Optional) Aktualisieren Sie den Namen der Ansicht und klicken Sie auf **Erstellen** Speichern einer Tabellenansicht

   Oder klicken Sie auf **Nächste** beim Erstellen einer Timeline <!--or calendar--> anzeigen.

   Standardmäßig benennt Maestro die Ansicht &quot;Tabelle &lt; Zahl >&quot;oder &quot;Timeline &lt; Zahl >&quot;. Die Zahl ist ein automatisch generiertes Inkrement.

1. (Bedingt) Wählen Sie das Start- und Enddatum für die Datensätze aus, die in der Timeline angezeigt werden sollen <!--or calendar--> Ansicht und klicken Sie dann auf **Erstellen**.
1. (Optional) Um eine Ansicht nach ihrer Erstellung umzubenennen, klicken Sie auf das Dropdown-Menü &quot;Ansicht&quot;und dann auf **Mehr** Menü ![](assets/more-menu.png) > **Umbenennen** , um den Ansichtsnamen zu aktualisieren. <!--ensure there is not another saving step here?!-->
   <!--1. (Optional) To rename a view after it is created, double-click the view name and start typing the new name, or click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Rename**.-->
1. (Optional) Informationen zum Verwalten einer bestimmten Ansicht finden Sie in den folgenden Artikeln:

   * [Tabellenansicht verwalten](../views/manage-the-table-view.md)
   * [Verwalten der Timeline-Ansicht](../views/manage-the-timeline-view.md)
     <!--* [Manage the calendar view](/help/quicksilver/maestro/views/manage-the-calendar-view.md)-->


## Ansichten löschen

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet. Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

   Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

<!--1. Hover over on the of the view's names in the view tab, then click **More** ![](assets/more-menu.png) > **Delete**. (********delete the instructions below but keep the last step***********)-->
1. Klicken Sie auf das Dropdown-Menü &quot;Ansicht&quot;, bewegen Sie den Mauszeiger über eine der Ansichten in der Liste und klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) > **Löschen**.
1. Klicks **Löschen** zur Bestätigung. <!--ensure there is not another saving step here?!-->

   Die Ansicht wird für alle Benutzer gelöscht, die auf den Maestro-Bereich zugreifen können, und kann nicht wiederhergestellt werden.

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
