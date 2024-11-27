---
title: Kalenderansicht verwalten
description: Sie können Datensätze und ihre Felder in einer Kalenderansicht anzeigen. In diesem Artikel wird beschrieben, wie Sie eine Kalenderansicht erstellen und eine vorhandene bearbeiten oder löschen können.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: d962d60294295dd1f3771d1f0b737c9d1f03dfef
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# Kalenderansicht verwalten

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

Sie können Datensätze und ihre Felder in einer Kalenderansicht auf der Seite vom Typ Datensatz anzeigen.

Weitere Informationen zu Adobe Workfront-Planungsansichten und deren Verwaltung finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

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

<!--OLD: 

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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

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

      * **Monat**: Die Datensätze werden in einem monatlichen Kalender angezeigt.

     <div class="preview">

      * **Woche**: Datensätze werden in den folgenden Bereichen angezeigt:

         * Datensätze, die sich über mehrere Tage erstrecken, werden oben im Kalender angezeigt.
         * Datensätze, die einen Tag oder weniger dauern, werden in der unteren Hälfte der Kalenderansicht angezeigt. Wenn Sie ausgewählt haben, um die Stunde der Start- und Enddaten anzuzeigen, wird der Datensatz zu der gewünschten Zeit innerhalb des Tages angezeigt, an dem er auftritt.
     </div>

1. Aktualisieren Sie die folgenden Ansichtselemente wie in den folgenden Unterabschnitten beschrieben:
   * [Filter](#add-filters)
   * [Einstellungen](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
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

### Einstellungen der Kalenderansicht bearbeiten

Die Kalenderansichtseinstellungen werden genauso bearbeitet wie die Einstellungen einer Timeline-Ansicht.

Weitere Informationen finden Sie im Abschnitt &quot;Einstellungen für die Timeline-Ansicht bearbeiten&quot;im Artikel [Verwalten der Timeline-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).
