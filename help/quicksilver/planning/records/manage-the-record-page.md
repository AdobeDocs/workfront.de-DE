---
title: Verwalten des Datensatzseiten-Layouts
description: Sie können das Layout der Datensatzvorschau und -seite in Adobe Workfront Planning bearbeiten.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 8fcc6c75811080f3ee152849a149542be8ae820c
workflow-type: tm+mt
source-wordcount: '1974'
ht-degree: 0%

---


# Seiten-Layout des Datensatzes verwalten

<span class="preview">Die auf dieser Seite hervorgehobenen Informationen beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können das Layout der Datensatzvorschau und -seite in Adobe Workfront Planning bearbeiten.

Die Datensatzvorschau ist eine kleinere Ansicht der Datensatzseite, die in der Ansicht eines Datensatztyps angezeigt wird.

Wenn Sie das Layout einer Datensatzvorschau und -seite ändern, wirken sich die Änderungen auf die Vorschaufelder und Detailseiten aller Datensätze desselben Typs aus.

In diesem Artikel wird beschrieben, wie Sie das Layout und Aussehen eines Datensatzvorschaufelds oder einer Datensatzseite ändern können. Weitere Informationen zum Bearbeiten von Datensätzen finden Sie unter [Bearbeiten von Datensätzen](/help/quicksilver/planning/records/edit-records.md).

Sie müssen Datensatztypen und Datensätze erstellen, bevor Sie die Datensatzseiten bearbeiten können.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md)

* [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md)

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
<p>Beliebig</p>
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
   <td>
   <p>Standard</p>
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
   <td>
   <p>Mitwirken an oder höhere Berechtigungen für einen Arbeitsbereich <span class="preview">und einen Datensatztyp</span> </a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü und den Bereich Planung für Projekte, Portfolios und Programme enthält. </p> Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht für Adobe Planning</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 

<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Überlegungen zum Bearbeiten von Datensatzseiten

* Standardmäßig zeigen die Details und die Vorschauseiten eines Datensatzes alle mit dem Datensatz verknüpften Felder an.

* Sie können auf der Vorschau- oder Detailseite keine neuen Felder für einen Datensatz hinzufügen. Sie müssen neue Felder in der Tabellenansicht hinzufügen, um sie auf den Seiten „Vorschau“ und „Details“ anzuzeigen.

* Sie können einer Datensatzvorschau oder einer Detailseite Abschnitte hinzufügen, um die Informationen nach gemeinsamen Kriterien zu organisieren und das Auffinden zu erleichtern.

* Die folgenden Änderungen wirken sich auf alle Datensätze desselben Typs aus und sind für alle Benutzer sichtbar, die auf diese Datensätze zugreifen:

   * Felder neu anordnen
   * Hinzufügen oder Entfernen von Abschnitten

* Änderungen an der Datensatzvorschau werden sofort auf der Seite mit den Datensatzdetails angezeigt. Auf der Datensatzseite vorgenommene Änderungen sind auch im Feld für die Datensatzvorschau sichtbar.

* Das Hinzufügen eines Cover- oder Miniaturbilds zu einem Datensatz gehört nicht zum Gesamtlayout der Datensatzvorschau oder -seite. Sie können jedem Datensatz eindeutige Titelbilder oder Miniaturansichten hinzufügen. Weitere Informationen finden Sie unter [Hinzufügen eines Titelbilds zu einem ](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) und [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Hinzufügen von Abschnitten zu einer Datensatzvorschau oder Seite

Beachten Sie beim Hinzufügen von Abschnitten zu einer Datensatzseite Folgendes:

* Es gibt keine Begrenzung dafür, wie viele Abschnitte Sie auf einer Seite haben können.
* Es ist nicht möglich, einen leeren Abschnitt zu verwenden. Mindestens ein Feld in einem Abschnitt ist erforderlich.
* Sie können Felder per Drag-and-Drop von einem Abschnitt in einen anderen ziehen. Weitere Informationen finden Sie im Abschnitt [Neuanordnen von Feldern auf der Datensatzvorschau oder der Detailseite](#rearrange-fields-in-the-record-preview-or-details-page) in diesem Artikel.
* Wenn Sie alle Felder aus einem Abschnitt entfernen, wird der Abschnitt automatisch gelöscht und kann nicht wiederhergestellt werden.

So fügen Sie einen Abschnitt zu einer Datensatzvorschau oder Seite hinzu:

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes

   Oder

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen** ![Detailsymbol öffnen im Feld „Tabellenname](assets/open-details-icon-in-table-name-field.png) in der ersten Spalte.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![Detailfeld](assets/details-box.png)

1. (Optional) Klicken Sie auf **Symbol** In neuer Registerkarte öffnen![ (Details in einer neuen Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) in der oberen rechten Ecke der Datensatzvorschau, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet. Die Registerkarte Details wird standardmäßig geöffnet.

   ![Detailseite](assets/details-page.png)

1. Bewegen **auf der Registerkarte** Details“ der Datensatzvorschau oder -seite den Mauszeiger über den Leerraum links neben den Feldern und klicken Sie dann auf das Symbol **Abschnitt hinzufügen** ![Abschnittssymbol hinzufügen](assets/add-section-icon.png), um einen Abschnitt hinzuzufügen.
1. Klicken Sie in den Namen des Abschnitts und ersetzen Sie **Nicht benannter Abschnitt** durch einen Namen. Klicken Sie dann auf die Eingabetaste. Die unter dem Abschnitt angezeigten Felder sind automatisch Teil des neuen Abschnitts.
1. Ziehen Sie die Felder per Drag-and-Drop in den neuen Abschnitt, wie im Abschnitt [Felder in der Datensatzvorschau oder auf der Detailseite neu anordnen](#rearrange-fields-in-the-record-preview-or-details-page) in diesem Artikel beschrieben.

1. (Optional) Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png).

   ![Weitere Menüoptionen für Abschnitt auf Datensatzseite](assets/more-menu-options-for-section-on-record-page.png)
1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Abschnitt zu bearbeiten:

   * Klicken Sie auf **Umbenennen**, um den Abschnitt umzubenennen

     >[!TIP]
     >
     > Sie können einen Abschnitt inline umbenennen, indem Sie auf den Namen klicken.

   * Klicken Sie **Nach oben**, um den Abschnitt um eine Position nach oben zu verschieben

     Oder

     Klicken Sie **Nach unten**, um den Abschnitt um eine Position nach unten zu verschieben.
Alle Felder im Abschnitt werden mit dem Abschnitt verschoben.

   * Klicken Sie **Löschen**, um den Abschnitt zu löschen. Der Abschnitt wurde gelöscht und kann nicht wiederhergestellt werden. Alle Benutzer, die auf die Datensätze dieses Typs zugreifen, sehen den gelöschten Abschnitt nicht mehr.

1. Klicken Sie auf den nach unten zeigenden Pfeil links neben einem Abschnittsnamen, um ihn zu reduzieren, oder auf den nach rechts zeigenden Pfeil, um ihn zu erweitern.
Alle Abschnitte sind standardmäßig erweitert.

1. (Optional) Klicken Sie auf das **grab**-Symbol ![grab-Symbol](assets/grab-icon.png) links neben dem Namen eines Abschnitts und ziehen Sie ihn dann an die gewünschte Stelle.

   Die neue Position des Abschnitts wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen an Abschnitten und der Feldreihenfolge werden automatisch gespeichert.

1. (Optional) Klicken Sie auf das **Export**-Menü ![Export-Symbol auf der Seite mit ](assets/export-icon-in-record-details-page.png) Datensatzdetails), um die Registerkarte Details in eine Word- oder PDF-Datei zu exportieren. Weitere Informationen finden Sie [Exportieren der Details eines Datensatzes](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Optional) Klicken Sie auf die Registerkarte **Verbindungen** neben der Registerkarte **Details**. Möglicherweise müssen Sie auf **Mehr** klicken, bevor Sie auf die Registerkarte **Verbindungen** klicken.

   Alle Datensätze oder Objekte, die mit dem ausgewählten Datensatz verbunden sind, werden unter den Namen des Datensatztyps oder der Anwendung, zu der sie gehören, angezeigt.

   ![Registerkarte „Verbindungen“ im Datensatz in Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Optional) Wählen Sie die Einstellung **Alle Datensätze anzeigen** in der oberen rechten Ecke der Registerkarte Verbindungen aus. Alle verbundenen Datensatztypen werden angezeigt, einschließlich der Datensätze, die noch keine verbundenen Datensätze haben. Standardmäßig ist der Umschalter deaktiviert und Datensatztypen ohne verbundene Datensätze sind ausgeblendet.

1. (Optional) Klicken Sie auf **Verbinden**, um den verbundenen Datensatztypen weitere Datensätze hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine Datensatzkarte und klicken Sie dann auf das Symbol zum Trennen des Datensatzes **-** und anschließend auf **Trennen**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
Folgendes geschieht:
   * Der Datensatz ist nicht mehr mit dem Workfront-Objekt verbunden.
   * Das Workfront-Objekt wird auch aus dem verknüpften Feld des Datensatzes aus Workfront Planning entfernt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden ebenfalls gelöscht.

## Neuanordnen von Feldern auf der Registerkarte Details des Datensatzes

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes

   Oder

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen** ![Detailsymbol öffnen im Feld „Tabellenname](assets/open-details-icon-in-table-name-field.png) in der ersten Spalte.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![Detailfeld](assets/details-box.png)

1. (Optional) Klicken Sie auf **Symbol** In neuer Registerkarte öffnen![ (Detailfeld in einem neuen Registerkartensymbol öffnen](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke der Datensatzvorschau, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen.

   Die **Details** des Datensatzes wird standardmäßig geöffnet.

   ![Detailseite](assets/details-page.png)

1. Klicken Sie auf der **„Details** auf das **grab**-Symbol ![grab icon](assets/grab-icon.png) links neben einem Feldnamen und ziehen Sie es dann an die gewünschte Stelle.

   >[!TIP]
   >
   >Sie können Felder per Drag-and-Drop in einen anderen Abschnitt ziehen.
   >Mindestens ein Feld in einem Abschnitt ist erforderlich.
   >

   Die neue Position des Felds wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen am Layout der Datensatzvorschau oder -seite werden automatisch gespeichert.

## Hinzufügen einer Registerkarte „Verbindungsansicht“ zur Seite eines Datensatzes

<!--suggested a new name for this type of page: "Connected records page" - check to see if this changed, and update this everywhere in this section-->

Sie können Informationen aus verbundenen Datensätzen oder Objekten anzeigen, indem Sie einem Datensatz eine Registerkarte für den Seitentyp „Verbindungsansicht“ hinzufügen. Die Informationen aus den verbundenen Datensätzen werden in einer schreibgeschützten Tabellenansicht angezeigt.

<!--replace the last sentence above with this at release:

In the Production environment, the information from the connected records or objects displays in a read-only table view. 

<Span class="preview">In the Preview environment, the information from the connected records can be edited in the table view. The information from the objects connected from another application is not editable in the table view.</span> -->

Beachten Sie Folgendes, wenn Sie eine Verbindungsansicht zur Seite eines Datensatzes hinzufügen:

* Sie können der Seite eines Datensatzes eine Seite für die Verbindungsansicht hinzufügen, nachdem Sie Datensätze oder Objekttypen mit dem Datensatztyp verbunden haben.

* Sie können keine Seite mit einer Verbindungsansicht zum Vorschaubereich eines Datensatzes hinzufügen.

* Verbindungsansichtsseiten zeigen in einer Tabellenansicht eine verbundene Datensatztypseite oder einen verbundenen Objekttyp aus einer anderen Anwendung an.

* Nachdem Sie der Seite eines Datensatzes eine Seite mit einer Verbindungsansicht hinzugefügt haben, wird die Registerkarte Seite im Vorschaubereich des Datensatzes angezeigt. Sie müssen zur vollständigen Seite gehen, um die Tabellenansicht für den verbundenen Datensatz anzuzeigen. <!--this might have changed? check and take disclaimer out-->

So fügen Sie eine Seite mit einer Verbindungsansicht hinzu:

1. Klicken Sie in einer Datensatzseitenansicht auf den Namen eines Datensatzes, um ihn zu öffnen, und klicken Sie dann oben rechts auf der Vorschauseite auf das Symbol **In neuer Registerkarte öffnen** ![Details in einer neuen ](assets/open-details-in-a-new-tab-icon.png) öffnen.
1. Klicken Sie **Seite hinzufügen**.

   ![Modal „Verbindungsansicht-Seite hinzufügen“](assets/add-connection-view-page-modal.png)
1. Fügen Sie den **Seitennamen** hinzu, klicken Sie auf **Verbindungsansicht** und klicken Sie dann auf **Erstellen**.

   Der Datensatzseite wird eine neue Registerkarte hinzugefügt.
1. Suchen Sie nach dem Namen eines verbundenen Datensatzes oder Objekttyps in der Liste oder klicken Sie darauf.
Die Tabellenansicht des ausgewählten Datensatztyps wird auf der neuen Seite angezeigt, und die verbundenen Datensätze werden in der Tabellenansicht angezeigt.
Alle Felder des verbundenen Datensatzes werden in der Tabellenansicht der Registerkarte des verbundenen Datensatzes angezeigt.

   Die ersten fünf Felder der verbundenen Datensatztabelle werden standardmäßig angezeigt. Standardmäßig werden keine Suchfelder angezeigt.

   <!--replace screen shot below when additional capabilities come to the table view - Fields, etc-->

   ![Tabellenansicht mit Audience-Verbindung unter Kampagnendetails](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optional) Führen Sie in der Tabellenansicht der verbundenen Datensätze einen der folgenden Schritte aus:

   * Klicken Sie auf den Namen eines Datensatzes. Dadurch wird die Seite des Datensatzes in einer neuen Registerkarte geöffnet. <!--<span class="preview">In the Preview environment, this opens the record's preview page.</span>-->
   * Klicken Sie auf **Verbinden**, um weitere Datensätze zu verbinden, und klicken Sie dann zum Schließen auf eine Stelle außerhalb des Verbindungsfelds. Die neuen Datensätze werden der Tabelle automatisch hinzugefügt.
     <!--* <span class="preview">Edit any information from the connected records inside the table view. </span>-->

   <!--<div class="preview">

   * Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following options: 
      * View 
      * Copy link
      * Edit thumbnail
      * Duplicate
      * Insert record above or below
      * Delete 
   * Select one of the records, then click one of the following options in the blue bar at the bottom of the screen: 
      * View
      * Copy link
      * Edit thumbnail
      * Duplicate
      * Delete. Delete is the only option available when you select more than one record. 

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

   </div>-->


1. (Optional) Doppelklicken Sie auf den Namen der Registerkarte Verbindungsansicht .

   Oder

   Bewegen Sie den Mauszeiger über den Namen der Registerkarte und klicken Sie dann auf **Mehr** ![Mehr ](assets/more-menu.png) und klicken Sie dann auf **Umbenennen**, um die Registerkarte in eine neue Ansicht umzubenennen.
1. (Optional) Verwenden Sie eines der folgenden Ansichtselemente in der Symbolleiste, um die Tabellenansicht zu verwalten:

   * Filter
   * Sortieren
   * Gruppierung
   * Felder, zum Anzeigen, Ausblenden oder Neuanordnen von Feldern

   Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >   Sie können keine Felder in der Tabellenansicht der Registerkarte eines verbundenen Datensatzes erstellen, bearbeiten oder löschen.
   >

1. Klicken Sie auf **Verbinden**, um Datensätze hinzuzufügen oder zu entfernen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md)
1. (Optional) Bewegen Sie den Mauszeiger über den Namen der Registerkarte „Verbindungsansicht“ und klicken Sie auf **Mehr** ![Mehr](assets/more-menu.png) und dann auf **Löschen**, um die Registerkarte zu entfernen.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



