---
title: Datensatzansichten verwalten
description: Bei Verwendung von Adobe Workfront Planning können Sie Datensätze in einer Tabellen-, Timeline- oder Kalenderansicht anzeigen. In diesem Artikel wird beschrieben, wie Sie eine Ansicht erstellen und eine vorhandene bearbeiten können.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: eb3db3b056cea359f77e56f77d6e9520954e2abb
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 1%

---


# Datensatzansichten verwalten

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Nachdem Sie im Bereich Adobe Workfront-Planung einen Datensatztyp ausgewählt haben, können Sie alle Datensätze dieses Typs in den folgenden Ansichten anzeigen:

* Tabelle

  Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

* Timeline

  Weitere Informationen finden Sie unter [Verwalten der Zeitleisten-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Kalender

  Weitere Informationen finden Sie unter [Verwalten der Kalenderansicht](/help/quicksilver/planning/views/manage-the-calendar-view.md).

In diesem Artikel werden die folgenden Informationen zu Datensatzansichten beschrieben:

* [Erstellen und Bearbeiten einer Ansicht](#create-or-edit-record-views)
* [Aktivieren der Echtzeit-Anwesenheitsindikatoren in einer Ansicht](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Weitere Informationen zum Verwalten von Workfront Planning-Datensatzansichten finden Sie in den folgenden Artikeln:

* [Datensatzansichten löschen](/help/quicksilver/planning/views/delete-record-views.md)
* [Doppelte Datensatzansichten](/help/quicksilver/planning/views/duplicate-record-views.md)
* [Ansichten freigeben](/help/quicksilver/planning/access/share-views.md)


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten der Berechtigungen für eine Ansicht</p>  
   <p>Anzeigeberechtigungen für eine Ansicht, um die Anzeigeeinstellungen vorübergehend zu ändern oder zu duplizieren</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>In der Produktionsumgebung müssen alle Benutzer, einschließlich der Systemadministratoren, einer Layoutvorlage zugewiesen werden, die Planning enthält.</p>
<p><span class="preview">In der Vorschau-Umgebung ist für Standardbenutzer und Systemadministratoren „Planung“ standardmäßig aktiviert.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen beim Arbeiten mit Datensatzansichten

* Die Ansichten in Workfront Planning sind vom Datensatztyp abhängig. Es ist nicht möglich, dieselbe Ansicht auf zwei verschiedene Datensatztypen anzuwenden.
* Ansichten, die Sie erstellen, sind nur für Sie und die Benutzer sichtbar, für die Sie die Ansichten freigeben.
* Wenn Sie eine Ansicht ändern oder löschen, wird sie für alle Benutzenden geändert und gelöscht, die über Berechtigungen für die Ansicht verfügen.
* Jeder Benutzer kann maximal 100 Ansichten erstellen. Sie können für einen Datensatztyp mehr als 100 Ansichten anzeigen, aber ein Benutzer kann nur 100 Ansichten erstellen.
* Obwohl einige Ansichtselemente auf mehrere Ansichten für denselben Datensatz angewendet werden können, sind sie für jede Datensatzansicht eindeutig:

   * Filter
   * Gruppierung (für die Tabellen- und Zeitleisten-Ansichten)
   * Darstellung der Leiste (für die Zeitleisten- und Kalenderansichten)

  Wenn Sie beispielsweise einen Filter in einer Tabellenansicht erstellen, sind die Filterergebnisse nur in der ausgewählten Ansicht (der Tabellenansicht) sichtbar und nicht in allen Ansichten, die mit dem Datensatztyp verknüpft sind.

  >[!TIP]
  >
  >Einige Ansichtselemente sind nicht für alle Ansichten verfügbar.


## Ähnlichkeiten und Unterschiede zwischen Datensatzansichten

Die folgende Tabelle zeigt die Ähnlichkeiten und Unterschiede zwischen der Tabellen-, Timeline- und Kalenderansicht:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Funktion | Tabellenansicht | Timeline-Ansicht | Kalenderansicht |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Anzeigen von Datensätzen in einer Liste oder Tabelle | ✓ |              | |
| Standardmäßig werden alle Felder als Spalten in der Tabelle angezeigt | ✓ |              |    |
| Felder (oder Spalten) ein- oder ausblenden | ✓ |               |    |
| Feldwerte für jeden Datensatz bearbeiten | ✓ |               |             |
| Datensätze als neue Zeilen in der Ansicht hinzufügen | ✓ |               |        |
| Felder als neue Spalten in der Ansicht hinzufügen | ✓ |               |         |
| Zeilen aus einer externen Liste kopieren und in eine Tabelle einfügen | ✓ |               |          |
| Anzeigen von Datensätzen in einer Zeitleiste |            | ✓ |             |
| Datensätze filtern | ✓ | ✓ | ✓ |
| Anzeigen von Datensätzen in einem Kalender |           |              | ✓ |
| Datensätze gruppieren | ✓ | ✓ |
| Datensätze sortieren | ✓ |              |
| <span class="preview">Farbcode-Datensätze</span> | <span class="preview">✓</span> | ✓ | ✓ |
| Farbgruppierungen |           | ✓ |
| Nach bestimmten Datensätzen suchen | ✓ | ✓ |
| Ansicht für andere freigeben | ✓ | ✓ | ✓ |
| Öffnet die Datensatzseite aus der Ansicht | ✓ | ✓ |    |
| Anzeigen von Datensätzen nach Jahr und Quartal |           | ✓ |    |
| Datensätze nach Monat anzeigen |           | ✓ | ✓ |
| Datensätze nach Woche anzeigen |           |               | ✓ |
| <span class="preview">Exportieren von Informationen aus einer Ansicht</span> | <span class="preview">✓</span> |               |    |


## Ansichten erstellen oder bearbeiten {#create-or-edit-views}

{{step1-to-planning}}


1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

   Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

1. Klicken Sie auf **+ Ansicht**, um eine neue Ansicht hinzuzufügen.
1. Wählen Sie aus den folgenden Ansichtstypen:

   * Tabelle
   * Timeline
   * Kalender

   Eine neue Registerkarte mit der ausgewählten Ansicht wird erstellt.

   Je nach Bildschirmbreite werden möglicherweise zusätzliche Ansichten im Menü **Mehr** (![) ](assets/more-menu.png).


>[!TIP]
>
>Beim Erstellen eines Datensatztyps wird standardmäßig auch die Tabellenansicht erstellt.
>
>Um eine Timeline- oder eine Kalenderansicht zu erstellen, muss der Datensatztyp, für den Sie die Ansicht erstellen, mindestens zwei Datumsfelder enthalten.
>
>Andernfalls sind die Optionen Timeline und Kalender abgeblendet.
>

![Anzeigen der Dropdown-Liste „Typen“ des Datensatztyps](assets/view-types-drop-down-from-record-type-list.png)

1. (Bedingt) Klicken Sie **Weiter**, wenn Sie eine Timeline- oder Kalenderansicht erstellen.

   Standardmäßig weist Workfront der Ansicht einen der folgenden Namen zu:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   Die Zahl ist ein automatisch generierter Inkrement.

1. (Bedingt) Wählen Sie die **Start** und **Enddatum** für die Datensätze aus, die in der Zeitleisten- oder Kalenderansicht angezeigt werden.

   >[!TIP]
   >
   >    Sie können aus Datensatzdatumsfeldern auswählen oder Datumsfelder aus verbundenen Datensatz- oder Objekttypen nachschlagen. Sie müssen Aggregatoren für Datumsfelder (MAX oder MIN) verwenden, wenn Sie Suchfelder als Start- und Enddatum für die Zeitleisten- und Kalenderansichten auswählen. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Klicken Sie auf **Erstellen**.

   Die Ansicht wird als neue Registerkarte angezeigt. Ansichten werden in der chronologischen Reihenfolge ab dem Zeitpunkt angezeigt, zu dem sie erstellt oder für Sie freigegeben wurden.
1. (Optional) Klicken Sie auf das **Mehr**-Menü ![Mehr Caret-Down-Symbol ](assets/more-caret-down-icon-views.png) neben der letzten Ansicht, um alle Ansichten für den ausgewählten Datensatztyp anzuzeigen.

   Zusätzliche Ansichten werden unter dem Menü **Mehr** nach der letzten Registerkarte Ansicht angezeigt. Die Zahl neben dem Menü **Mehr** zeigt die Anzahl der zusätzlichen Ansichten an.
1. (Optional) Um eine Ansicht nach ihrer Erstellung umzubenennen, klicken Sie auf das Dropdown-Menü „Ansicht“ und dann auf das Menü **Mehr** ![Mehr Menü](assets/more-menu.png) > **Umbenennen**, um den Ansichtsnamen zu aktualisieren

   Oder

   Doppelklicken Sie auf den Namen der Ansicht und geben Sie den neuen Namen ein.  <!--ensure there is not another saving step here?!-->

1. (Optional) Informationen zum Verwalten eines bestimmten Ansichtstyps finden Sie in folgenden Artikeln:

   * [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Zeitleisten-Ansicht verwalten](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Kalenderansicht verwalten](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## Aktivieren der Echtzeit-Anwesenheitsindikator in einer Ansicht

Sie können sehen, ob andere Benutzer gleichzeitig Datensätze bearbeiten, indem Sie den Echtzeit-Präsenzindikatoren in der Ansicht folgen.

Die Avatare anderer Benutzer, die Datensatzinformationen gleichzeitig bearbeiten, wie Sie standardmäßig in der oberen rechten Ecke aller Datensatzansichten anzeigen.

Wenn Sie die Tabellenansicht anzeigen, können Sie auch anzeigen, welches Feld ein anderer Benutzer zum Zeitpunkt der Anzeige des Datensatzes bearbeitet.

Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).



<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->
