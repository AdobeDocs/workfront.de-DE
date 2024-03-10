---
title: Kalenderansicht verwalten
description: Sie können Datensätze und ihre Felder in einer Kalenderansicht anzeigen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 26d6fecf02541fff649deabe61e65dbe5ae5f688
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

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

{{maestro-important-intro}}

Sie können Datensätze und ihre Felder in einer Kalenderansicht auf der Seite vom Typ Datensatz anzeigen.

Informationen zu den Ansichten der Adobe Workfront-Planungsfunktionen und deren Verwaltung finden Sie unter [Verwalten von Datensatzansichten](../views/manage-record-views.md).

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
   <td> <p>Es gibt keine Zugriffssteuerungsmöglichkeiten für Adobe Workfront-Planungsfunktionen  </p>  
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


## Kalenderansicht verwalten {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Beachten Sie Folgendes:

* Sie können eine Kalenderansicht nur erstellen, wenn einem Datensatztyp mindestens zwei Datumsfelder zugeordnet sind. Wenn einem Datensatztyp ein oder keine Datumsfelder zugeordnet sind, ist die Kalenderansichtsoption abgeblendet.
* Die folgenden Szenarien existieren:

   * Wenn das Start- und das Enddatum keine Werte aufweisen, werden die Datensätze nicht im Kalender angezeigt
   * Wenn das Start- oder das Enddatum keinen Wert haben, wird der Datensatz als ein eintägiges Ereignis angezeigt
   * Wenn das Startdatum nach dem Enddatum liegt, wird der Datensatz nicht im Kalender angezeigt.

So verwalten Sie eine Kalenderansicht:

1. Rufen Sie die Seite mit dem Datensatztyp auf, für die Sie den Kalender anzeigen möchten.
1. Erstellen Sie eine Kalenderansicht, wie im Artikel beschrieben. [Verwalten von Datensatzansichten](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   Die Datensätze, die dem von Ihnen ausgewählten Datensatztyp zugeordnet sind, werden in einem Kalender als Balken angezeigt. Die Farbe der Balken entspricht der Farbe des Datensatzsymbols.

1. Führen Sie einen der folgenden Schritte aus, um durch den Kalender zu navigieren:

   * Klicken Sie auf die Symbole links und rechts oder verwenden Sie den horizontalen Bildlauf, um im Kalender rückwärts und vorwärts zu gehen.
   * Klicks **Heute** um den Kalender auf das heutige Datum zu zentrieren.
   * Wählen Sie eine der folgenden Optionen aus dem Dropdown-Menü für den Zeitrahmen aus, um die Zeitabstände zu aktualisieren:

      * Monat