---
title: Verwalten von Datensatzansichten
description: Bei Verwendung der Planungsfunktionen von Adobe Workfront können Sie Datensätze in einer Tabellen-, Timeline- oder Kalenderansicht anzeigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '949'
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
| Datensätze filtern | ✓ | ✓ | ✓ |
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

1. Klicks **+ Ansicht** , um eine neue Ansicht hinzuzufügen.
1. Wählen Sie aus den folgenden Arten von Ansichten:

   * Tabelle
   * Timeline
   * Kalender

   Eine neue Registerkarte wird mit der ausgewählten Ansicht erstellt.

   Je nach Breite des Bildschirms können zusätzliche Ansichten im **Mehr** Menü ![](assets/more-menu.png).


>[!TIP]
>
>Beim Erstellen eines Datensatztyps wird auch die Tabellenansicht standardmäßig erstellt.
>
>Um eine Timeline- oder Kalenderansicht zu erstellen, muss der Datensatztyp, für den Sie die Ansicht erstellen, mindestens zwei Datumsfelder aufweisen. Andernfalls sind die Optionen Timeline und Kalender abgeblendet.
>

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

   Die Ansicht wird als neue Registerkarte angezeigt. Ansichten werden in chronologischer Reihenfolge angezeigt, nachdem sie erstellt oder für Sie freigegeben wurden.
1. (Optional) Klicken Sie auf die **Mehr** Menü ![](assets/more-caret-down-icon-views.png) neben der letzten Ansicht, um alle Ansichten für den ausgewählten Datensatztyp anzuzeigen.

   Weitere Ansichten werden unter der **Mehr** Menü hinter der Registerkarte &quot;Letzte Ansicht&quot;aus. Die Zahl neben dem **Mehr** zeigt die Anzahl weiterer Ansichten an.
1. (Optional) Um eine Ansicht nach ihrer Erstellung umzubenennen, klicken Sie auf das Dropdown-Menü &quot;Ansicht&quot;und dann auf **Mehr** Menü ![](assets/more-menu.png) > **Umbenennen** , um den Ansichtsnamen zu aktualisieren

   Oder

   Doppelklicken Sie auf den Namen der Ansicht und geben Sie den neuen Namen ein.  <!--ensure there is not another saving step here?!-->

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

1. Bewegen Sie den Mauszeiger über einen der Namen der Ansicht auf der Registerkarte &quot;Ansicht&quot;und klicken Sie dann auf **Mehr** ![](assets/more-menu.png) auf der linken Seite des Ansichtsnamens und klicken Sie dann auf **Löschen**.
Zunächst müssen Sie möglicherweise auf **Mehr** auf der linken Seite der letzten Registerkarte, um die Ansicht zu finden, die Sie löschen möchten.

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
