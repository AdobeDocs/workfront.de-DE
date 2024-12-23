---
title: Ansichten von Datensätzen verwalten
description: Bei Verwendung der Adobe Workfront-Planung können Sie Datensätze in einer Tabellen-, Timeline- oder Kalenderansicht anzeigen. In diesem Artikel wird beschrieben, wie Sie eine Ansicht erstellen und eine vorhandene bearbeiten oder löschen können.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: d962d60294295dd1f3771d1f0b737c9d1f03dfef
workflow-type: tm+mt
source-wordcount: '1485'
ht-degree: 1%

---


# Verwalten von Datensatzansichten

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.


{{planning-important-intro}}

Nach Auswahl eines Datensatztyps im Adobe Workfront-Planungsbereich können Sie alle Datensätze dieses Typs in den folgenden Ansichten anzeigen:

* Tabelle

  Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

* Timeline

  Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Kalender

  Weitere Informationen finden Sie unter [Kalenderansicht verwalten](/help/quicksilver/planning/views/manage-the-calendar-view.md).

In diesem Artikel werden die folgenden Informationen zu Datensatzansichten beschrieben:

* [Erstellen und Bearbeiten einer Ansicht](#create-or-edit-record-views)
* [Ansicht löschen](#delete-views)
* [Ansicht duplizieren](#duplicate-views)
* [Aktivieren Sie die Echtzeit-Präsenz-Indikatoren in einer Ansicht](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## Zugriffsanforderungen

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
   <td>   <p>Berechtigungen für eine Ansicht verwalten</p>  
   <p>Berechtigungen für eine Ansicht anzeigen, um die Anzeigeeinstellungen vorübergehend zu ändern</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old: 

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
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->


## Überlegungen zum Arbeiten mit Datensatzansichten

* Ansichten in der Workfront-Planung sind typspezifisch für Datensätze. Sie können dieselbe Ansicht nicht auf zwei verschiedene Datensatztypen anwenden.
* Von Ihnen erstellte Ansichten sind nur für Sie und Benutzer sichtbar, für die Sie die Ansichten freigeben.
* Wenn Sie eine Ansicht ändern oder löschen, wird sie für alle Benutzer mit Berechtigungen für die Ansicht geändert und gelöscht.
* Jeder Benutzer kann maximal 100 Ansichten erstellen. Sie können mehr als 100 Ansichten für einen Datensatztyp anzeigen, aber ein Benutzer kann nur 100 Ansichten erstellen.
* Sie können von Ihnen erstellte Ansichten für andere freigeben. Weitere Informationen finden Sie unter [Ansichten freigeben](/help/quicksilver/planning/access/share-views.md).
* Die folgenden Elemente sind für jede Datensatzansicht eindeutig:

   * Filter
   * Gruppierung
   * Sortieren
   * Balken-Erscheinungsbild (für die Timeline-Ansicht)

  <!-- some of these are not available in all of the views - edit above-->

  Wenn Sie beispielsweise einen Filter in einer Tabellenansicht erstellen, sind die Filterergebnisse nur in der ausgewählten Ansicht und nicht in allen mit dem Datensatztyp verknüpften Ansichten sichtbar.

  >[!NOTE]
  >
  > Einige Ansichtselemente stehen möglicherweise nicht für alle Ansichten zur Verfügung.


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
| Ansicht für andere freigeben | ✓ | ✓ | ✓ |
| Öffnen Sie die Seite des Datensatzes in der Ansicht | ✓ | ✓ |    |
| Datensätze nach Jahr und Quartal anzeigen |           | ✓ |    |
| Anzeigen von Datensätzen nach Monat |           | ✓ | ✓ |
| <span class="preview">Anzeigen von Datensätzen nach Woche</span> |           |               | ✓ |


## Ansichten erstellen oder bearbeiten {#create-or-edit-views}

{{step1-to-planning}}


1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

   Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

1. Klicken Sie auf **+ Ansicht** , um eine neue Ansicht hinzuzufügen.
1. Wählen Sie aus den folgenden Arten von Ansichten:

   * Tabelle
   * Timeline
   * Kalender

   Eine neue Registerkarte wird mit der ausgewählten Ansicht erstellt.

   Abhängig von der Breite Ihres Bildschirms können im Menü **Mehr** ![](assets/more-menu.png) zusätzliche Ansichten angezeigt werden.


>[!TIP]
>
>Beim Erstellen eines Datensatztyps wird auch die Tabellenansicht standardmäßig erstellt.
>
>Um eine Timeline- oder Kalenderansicht zu erstellen, muss der Datensatztyp, für den Sie die Ansicht erstellen, mindestens zwei Datumsfelder aufweisen.
>
>Andernfalls sind die Optionen Timeline und Kalender abgeblendet.
>

![](assets/view-types-drop-down-from-record-type-list.png)

1. (Bedingt) Klicken Sie beim Erstellen einer Timeline- oder Kalenderansicht auf **Weiter**.

   Standardmäßig gibt Workfront der Ansicht einen der folgenden Namen:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Die Zahl ist ein automatisch generiertes Inkrement.

1. (Bedingt) Wählen Sie für die Datensätze, die in der Timeline- oder Kalenderansicht angezeigt werden sollen, die **Start** und das **Enddatum** aus.

   >[!TIP]
   >
   >    Sie können aus Datensatzdatumsfeldern auswählen oder Datumsfelder aus verbundenen Datensätzen oder Objekttypen suchen. Sie müssen Aggregatoren für Datumsfelder (MAX oder MIN) verwenden, wenn Sie Suchfelder als Start- und Enddatum für die Timeline- und Kalenderansichten auswählen. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Klicken Sie auf **Erstellen**.

   Die Ansicht wird als neue Registerkarte angezeigt. Ansichten werden in chronologischer Reihenfolge angezeigt, nachdem sie erstellt oder für Sie freigegeben wurden.
1. (Optional) Klicken Sie auf das Menü **Mehr** neben der letzten Ansicht, um alle Ansichten für den ausgewählten Datensatztyp anzuzeigen.![](assets/more-caret-down-icon-views.png)

   Zusätzliche Ansichten werden nach der Registerkarte &quot;Letzte Ansicht&quot;im Menü **Mehr** angezeigt. Die Zahl neben dem Menü **Mehr** gibt die Anzahl der zusätzlichen Ansichten an.
1. (Optional) Um eine Ansicht nach ihrer Erstellung umzubenennen, klicken Sie auf das Dropdown-Menü &quot;Ansicht&quot;und dann auf das Menü **Mehr** Menü ![](assets/more-menu.png) > **Umbenennen** , um den Ansichtsnamen zu aktualisieren

   Oder

   Doppelklicken Sie auf den Namen der Ansicht und geben Sie den neuen Namen ein.  <!--ensure there is not another saving step here?!-->

1. (Optional) Informationen zum Verwalten einer bestimmten Ansicht finden Sie in den folgenden Artikeln:

   * [Tabellenansicht verwalten](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Verwalten der Timeline-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Kalenderansicht verwalten](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## Ansichten löschen

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

   Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

1. Bewegen Sie den Mauszeiger über einen der Namen der Ansicht auf der Registerkarte &quot;Ansicht&quot;, klicken Sie dann links neben dem Ansichtsnamen auf **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Löschen**.
Zunächst müssen Sie möglicherweise links neben der letzten Registerkarte auf **Mehr** klicken, um die Ansicht zu finden, die Sie löschen möchten.

1. Klicken Sie zur Bestätigung auf **Löschen** . <!--ensure there is not another saving step here?!-->

   Die Ansicht wird für alle Benutzer gelöscht, die auf den Datensatzbereich zugreifen können, und kann nicht wiederhergestellt werden.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Ansicht duplizieren

Wenn Sie mehrere Versionen einer Ansicht beibehalten und geringfügige Änderungen zwischen den Versionen vornehmen möchten, können Sie eine Ansicht duplizieren.

Durch das Duplizieren einer Ansicht werden identische Kopien einer vorhandenen Ansicht erstellt.

Die Freigabeberechtigungen der ursprünglichen Ansicht werden nicht an die duplizierte Ansicht übertragen.

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

1. Bewegen Sie den Mauszeiger über die Registerkarte der Ansicht, die Sie duplizieren möchten, klicken Sie auf das Menü **Mehr** rechts neben dem Ansichtsnamen und klicken Sie dann auf **Duplizieren** .![](assets/more-menu.png)

   ![](assets/view-more-menu-with-duplicate-option.png)


   Die Ansicht wird dupliziert und der Name der neuen Ansicht folgt dem folgenden Muster: `Original view's name (Copy)`. Die neue Registerkarte &quot;Ansicht&quot;wird am Ende aller Ansichtsregisterkarten angezeigt.

## Echtzeitpräsenzanzeige in einer Ansicht aktivieren

Die Avatare anderer Benutzer, die Datensatzinformationen gleichzeitig mit der Anzeige in der oberen rechten Ecke aller Datensatzansichten bearbeiten, werden standardmäßig angezeigt.

Wenn Sie die Tabellenansicht anzeigen, können Sie auch anzeigen, welches Feld ein anderer Benutzer zum Zeitpunkt der Anzeige des Datensatzes bearbeitet.

1. Gehen Sie zu einer Seite vom Typ Datensatz und öffnen Sie eine beliebige Ansicht.
1. (Bedingt) Wenn andere Benutzer die Datensätze des ausgewählten Typs gleichzeitig bearbeiten, werden ihre Avatare in der oberen rechten Ecke der Ansicht angezeigt.
1. Klicken Sie auf das Dropdown-Menü neben den Avataren und wählen Sie den Umschalter **Mitwirkende anzeigen** aus. Der Umschalter ist standardmäßig ausgewählt.

   ![](assets/show-collaborators-toggle-selected.png)

1. (Bedingt) Öffnen Sie eine Tabellenansicht. Das Feld, das eine andere Person aktiv bearbeitet, wird in der Tabellenansicht in der Farbe hervorgehoben, die dem Umriss ihres Avatars entspricht.

   Wenn die Hervorhebungsfarbe des Avatars grau ist, hat der Benutzer den Datensatz vor mehr als 30 Sekunden nicht mehr aktiv bearbeitet.

   ![](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >Sie können in jeder Ansicht den Umschalter **Mitwirkende anzeigen** auswählen. Das derzeit von anderen Benutzern bearbeitete Feld wird nur in der Tabellenansicht dargestellt.
