---
title: Kalenderansicht verwalten
description: Sie können Datensätze und ihre Felder in einer Kalenderansicht anzeigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 1%

---

# Kalenderansicht verwalten

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Sie können Datensätze und ihre Felder in einer Kalenderansicht auf der Seite vom Typ Datensatz anzeigen.

Weitere Informationen zu Adobe Workfront-Planungsansichten und deren Verwaltung finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
<p>Ihr Unternehmen muss in der Phase des frühen Zugriffs für die Workfront-Planung eingeschrieben sein </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> Es gibt keine Zugriffskontrollen für die Adobe Workfront-Planung</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für eine Ansicht verwalten</p>  
   <p>Berechtigungen für eine Ansicht anzeigen, um die Anzeigeeinstellungen vorübergehend zu ändern</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Kalenderansicht verwalten {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Beachten Sie Folgendes:

* Sie können eine Kalenderansicht nur erstellen, wenn einem Datensatztyp mindestens zwei Datumsfelder zugeordnet sind. Wenn einem Datensatztyp ein oder keine Datumsfelder zugeordnet sind, ist die Kalenderansichtsoption abgeblendet.

  Sie können aus Datensatzdatumsfeldern auswählen oder Datumsfelder aus verbundenen Datensätzen oder Objekttypen suchen.
* Die folgenden Szenarien existieren:

   * Wenn das Start- und das Enddatum keine Werte aufweisen, werden die Datensätze nicht im Kalender angezeigt
   * Wenn das Start- oder das Enddatum keinen Wert haben, wird der Datensatz als ein eintägiges Ereignis angezeigt
   * Wenn das Startdatum nach dem Enddatum liegt, wird der Datensatz nicht im Kalender angezeigt.

So verwalten Sie eine Kalenderansicht:

1. Rufen Sie die Seite mit dem Datensatztyp auf, für die Sie den Kalender anzeigen möchten.
1. Erstellen Sie eine Kalenderansicht, wie im Artikel [Ansichten von Datensätzen verwalten](/help/quicksilver/planning/views/manage-record-views.md) beschrieben.

   ![](assets/calendar-view-example.png)

   Die Datensätze, die dem von Ihnen ausgewählten Datensatztyp zugeordnet sind, werden in einem Kalender als Balken angezeigt. Die Farbe der Balken entspricht der Farbe des Datensatzsymbols.

1. Führen Sie einen der folgenden Schritte aus, um durch den Kalender zu navigieren:

   * Klicken Sie auf die Symbole links und rechts oder verwenden Sie den horizontalen Bildlauf, um im Kalender rückwärts und vorwärts zu gehen.
   * Klicken Sie auf **Heute** , um den Kalender auf das aktuelle Datum zu zentrieren.
   * Wählen Sie eine der folgenden Optionen aus dem Dropdown-Menü für den Zeitrahmen aus, um die Zeitabstände zu aktualisieren:

      * Monat
1. Aktualisieren Sie die folgenden Ansichtselemente wie in den folgenden Unterabschnitten beschrieben:
   * [Filter](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Filter hinzufügen

Mithilfe von Filtern können Sie die Anzahl der auf dem Bildschirm angezeigten Informationen verringern.

Beachten Sie beim Arbeiten mit Filtern in der Kalenderansicht Folgendes:

<!-- this list is almost identical to the one for the table view - update both-->

* Die Filter, die Sie für eine Kalenderansicht erstellen, funktionieren unabhängig von den Filtern in jeder anderen Ansicht, die auf denselben Datensatztyp angewendet wird.

* Die Filter sind für die ausgewählte Ansicht eindeutig. Für zwei Kalenderansichten desselben Datensatztyps können unterschiedliche Filter angewendet werden.

* Zwei Benutzer, die sich dieselbe Kalenderansicht ansehen, sehen denselben Filter, der derzeit angewendet wird.

* Sie können die von Ihnen erstellten Filter nicht für eine Kalenderansicht benennen.

* Wenn Sie Filter entfernen, werden diese von allen Benutzern entfernt, die auf denselben Datensatztyp zugreifen wie Sie und die dieselbe Ansicht wie Sie anzeigen.

* Das Hinzufügen von Filtern in der Kalenderansicht entspricht dem Hinzufügen von Filtern in der Tabellenansicht.

  Weitere Informationen finden Sie im Abschnitt &quot;Filter hinzufügen&quot;im Artikel [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

* Sie können nach verbundenen Datensatzfeldern oder Suchfeldern filtern.

* Sie können nach Suchfeldern filtern, die mehrere Werte anzeigen.
