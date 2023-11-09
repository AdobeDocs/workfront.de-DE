---
title: Verwalten von Datensatzansichten
description: Bei Verwendung von Adobe Maestro können Datensätze in einer Tabellen- oder Timeline-Ansicht angezeigt werden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 4cdebe4890b775a097469e7d7035a38397b71094
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# Verwalten von Datensatzansichten

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

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
   <p> Adobe</p> </td>
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
<p>Beliebig</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Beliebig</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Beliebig</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/grant-access.md">Zugriff auf Adobe Maestro gewähren</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Überlegungen beim Arbeiten mit Maestro-Ansichten

* Ansichten in Maestro sind typspezifisch für Datensätze. Sie können dieselbe Ansicht nicht auf zwei verschiedene Datensatztypen anwenden.
* Von Ihnen erstellte Ansichten sind für alle sichtbar, die auf den Maestro-Bereich zugreifen. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* Das Erstellen von Ansichten für betriebliche Datensatztypen ist mit dem Erstellen von Ansichten für Taxonomiedatensatztypen identisch.
* Wenn Sie eine Ansicht ändern oder löschen, wird sie für alle Benutzer geändert und gelöscht, die auf den Maestro-Bereich zugreifen können.
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
  <!--* [Share a view](#share-views) - not possible yet-->

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
| Gruppeneinträge |           | ✓ |
| Datensätze sortieren | ✓ |              |
| Farbcode-Datensätze |           | ✓ |
| Farbcode-Gruppierungen |           | ✓ |

<!--| Sort groupings                                                        | ✓          | ✓             |-->
<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

## Ansichten erstellen oder bearbeiten {#create-or-edit-views}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke oder **Hauptmenü** icon ![](assets/main-menu-shell.png) in der oberen linken Ecke, falls verfügbar, klicken Sie auf **Maestro** ![](assets/maestro-icon.png).
Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet. Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md).
1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

   Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

1. Klicken Sie auf **Ansicht** und wählen Sie entweder ein vorhandenes **Tabellenansicht** ![](assets/table-view-icon.png) oder klicken Sie **Ansicht erstellen > Tabelle** zum Erstellen einer Tabellenansicht

   Oder

   Existierende Auswahl **Timeline-Ansicht** ![](assets/timeline-view-icon.png) Ansicht oder Klicken **Ansicht erstellen > Timeline** , um eine Timeline-Ansicht zu erstellen.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Um eine Timeline-Ansicht zu erstellen, muss der Datensatztyp, für den Sie die Ansicht erstellen, mindestens zwei Datumsfelder aufweisen. Andernfalls ist die Option Timeline abgeblendet.

1. (Optional) Aktualisieren Sie den Namen der Ansicht und klicken Sie auf **Erstellen** , um es zu speichern.

   Standardmäßig benennt Maestro die Ansicht &quot;Tabelle &lt; Zahl >&quot;oder &quot;Timeline &lt; Zahl >&quot;. Die Zahl ist ein automatisch generiertes Inkrement.

1. (Optional) Um eine Ansicht nach ihrer Erstellung umzubenennen, klicken Sie auf das Dropdown-Menü &quot;Ansicht&quot;und dann auf **Mehr** Menü ![](assets/more-menu.png) > **Umbenennen** , um den Ansichtsnamen zu aktualisieren. <!--ensure there is not another saving step here?!-->
1. (Optional) Weitere Informationen zum Verwalten einer Ansicht finden Sie in den folgenden Artikeln:

   * [Tabellenansicht verwalten](../views/manage-the-table-view.md)
   * [Verwalten der Timeline-Ansicht](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## Ansichten löschen

1. Aus dem **Hauptmenü** ![](assets/main-menu-workfront.png) in der oberen rechten Ecke des Bildschirms, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> click **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet. Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md).
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

   Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

1. Klicken Sie auf das Dropdown-Menü &quot;Ansicht&quot;, bewegen Sie den Mauszeiger über eine der Ansichten in der Liste und klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) > **Löschen**.
1. Klicks **Löschen** zur Bestätigung. <!--ensure there is not another saving step here?!-->

   Die Ansicht wird für alle Benutzer gelöscht, die auf den Maestro-Bereich zugreifen können, und kann nicht wiederhergestellt werden.

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
