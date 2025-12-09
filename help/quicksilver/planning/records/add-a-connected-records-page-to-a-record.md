---
title: Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz
description: Sie können Informationen aus verbundenen Datensätzen oder Objekten anzeigen, indem Sie einem Datensatz eine Registerkarte für eine Seite „Verbundene Datensätze“ hinzufügen. Dadurch werden die verbundenen Datensätze in einer Tabellenansicht zur Registerkarte hinzugefügt.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 1%

---


# Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Sie können Informationen aus verbundenen Datensätzen oder Objekten anzeigen, indem Sie einem Datensatz eine Registerkarte für eine Seite „Verbundene Datensätze“ hinzufügen. Dadurch werden die verbundenen Datensätze in einer Tabellenansicht zur Registerkarte hinzugefügt.

Beachten Sie beim Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz Folgendes:

* Sie können eine Seite „Verbundene Datensätze“ zu einem Datensatz hinzufügen, nachdem Sie in der Tabellenansicht eines Datensatztyps Datensätze oder Objekttypen mit dem Datensatztyp verbunden haben.

* Sie können eine Seite „Verbundene Datensätze“ aus dem Vorschaubereich eines Datensatzes oder aus der Seite des Datensatzes hinzufügen.

* Verbundene Datensatzseiten zeigen nur die verbundenen Objekte oder Datensätze eines Objekts oder Datensatztyps in einer Tabellenansicht an. Auf der Seite werden nicht alle Datensätze dieses Typs angezeigt.

* Sie können Seiten mit verbundenen Datensätzen für die folgenden verbundenen Datensatz- oder Objekttypen hinzufügen:

   * Workfront-Planungs-Datensatztypen
   * Workfront-Projekte, -Programme, -Portfolios, -Gruppen oder -Unternehmen. Sie können die verbundenen Workfront-Objekte auch dann anzeigen, wenn Sie nicht über die erforderlichen Zugriffsberechtigungen für sie in Workfront verfügen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront und beliebiges Planungspaket</p>
<p>Beliebiger Workflow und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
<tr>
<td> 
   <p> Zusätzliche Produkte</p> </td> 
   <td> 
   <p> Zusätzlich zu Adobe Workfront müssen Sie über Folgendes verfügen, wenn Sie eine verbundene Datensatzseite für Objekte aus den folgenden Programmen hinzufügen möchten:</p>
   <ul><li><p>Eine Adobe Experience Manager Assets-Lizenz und eine Integration zwischen AEM Assets und Workfront, um AEM-Assets mit Planungs-Datensatztypen zu verbinden.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront für Experience Manager Assets und Assets Essentials: Artikelindex</a>. </p></li>
   <li><p> Eine Adobe GenStudio for Performance Marketing-Lizenz zum Verbinden von Datensatztypen mit GenStudio Brands</p>
   <p>Weitere Informationen finden Sie <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Erste Schritte mit Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <p>Beitragen von oder höhere Berechtigungen für einen Arbeitsbereich und einen Datensatztyp </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> 
  </td>
  </tr>   
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Hinzufügen einer Seite „Verbundene Datensätze“ zu einem Datensatz

1. Klicken Sie auf den Namen des Datensatzes, um ihn in jeder Ansicht einer Datensatztypseite zu öffnen.
1. Klicken Sie **einem der** Bereiche auf „Seite hinzufügen“:

   * Das Vorschaufenster des Datensatzes
   * Die Detailseite des Datensatzes, nachdem Sie auf das Symbol **In neuer Registerkarte öffnen** (![Details in einer neuen Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) in der oberen rechten Ecke der Vorschauseite geklickt haben.

   Das **Seite erstellen** wird geöffnet.

   ![Modal „Verbundene Datensätze hinzufügen“](assets/add-connection-view-page-modal.png)

1. Fügen Sie den **Seitennamen** hinzu, klicken Sie auf **Seite „Verbundene Datensätze** und klicken Sie dann auf **Erstellen**.

   Eine neue Seite „Verbundene Datensätze“ wird als neue Registerkarte zur Seite des Datensatzes hinzugefügt.

   Die Datensätze, die mit dem aktuellen Datensatz verbunden sind, werden in der Tabellenansicht angezeigt.

   >[!TIP]
   >
   >Sie müssen verbundene Datensätze im Tabellen- oder Detailbereich eines Datensatzes hinzufügen, bevor Sie sie auf einer Seite mit verbundenen Datensätzen anzeigen können.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   Die ersten fünf Felder der verbundenen Datensätze werden standardmäßig angezeigt. <!--No lookup fields display by default.-->

   ![Tabellenansicht mit Audience-Verbindung unter Kampagnendetails](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Optional) Suchen Sie nach dem Namen eines verbundenen Datensatzes oder Objekttyps in der Liste oder klicken Sie darauf.

1. (Optional und bedingt) Führen Sie in der Tabellenansicht der Seite Verbundene Datensätze einen der folgenden Schritte aus, wenn Sie verbundene Planungsdatensätze oder Workfront-Objekte mit Ausnahme von Projekten anzeigen: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Klicken Sie auf den Namen eines Datensatzes. Dadurch wird die Seite des Datensatzes in einer neuen Registerkarte geöffnet.

   * Klicken **unten in** Tabellenansicht auf „Verbinden“, um weitere Datensätze zu verbinden. Klicken Sie dann außerhalb des Verbindungsfelds, um es zu schließen. Die neuen Datensätze werden der Tabelle automatisch hinzugefügt.

     Weitere Informationen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).
   * Bearbeiten Sie alle Informationen aus den verbundenen Datensätzen inline in der Tabellenansicht.

   * Bewegen Sie den Mauszeiger über den Namen eines verbundenen Datensatzes und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png)

     ODER

     Wählen Sie einen der Datensätze aus und klicken Sie dann auf eine der folgenden Optionen in der blauen Leiste unten in der Liste:

      * **Anzeigen**, um die Datensatzseite in einer neuen Registerkarte zu öffnen
      * **Link kopieren**, um einen Link auf die Datensatzseite zu kopieren
      * **Miniaturansicht bearbeiten** um das Feld **Miniaturansicht aufzeichnen** zu öffnen und das Miniaturbild des Datensatzes zu bearbeiten
      * **Duplizieren** um den verbundenen Datensatz zu duplizieren. Der duplizierte Datensatz ist auch mit dem aktuellen Datensatz verbunden.
      * **Datensatz oberhalb oder unterhalb einfügen**, um dem verbundenen Datensatztyp neue Datensätze hinzuzufügen. Neue hier hinzugefügte Datensätze sind auch mit dem aktuellen Datensatz verbunden. Diese Option ist bei der Auswahl eines Datensatzes in der Tabelle in der blauen Leiste nicht verfügbar.
      * **Löschen**, um den Datensatz zu löschen. Wenn Sie einen verbundenen Datensatz löschen, wird er aus seinem Datensatztyp und überall dort, wo der Datensatz verbunden ist, gelöscht.

     Weitere Informationen zum Bearbeiten von Datensätzen in der Tabellenansicht finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >Sie können mehrere Datensätze oder Objekte auswählen, um sie zu löschen.

   * Inline-Bearbeitung eines beliebigen Planungsdatensatzes in der Tabelle auf der Seite „Verbundene Datensätze“.

     Alle anderen Workfront-Objekte werden in einer schreibgeschützten Tabellenansicht angezeigt und können nicht bearbeitet werden.

1. (Optional und bedingt) Führen Sie in der Tabellenansicht der Seite „Verbundene Datensätze“ beim Anzeigen von verbundenen Workfront-Projekten einen der folgenden Schritte aus:

   * Klicken Sie **Datensätze verbinden** in der oberen rechten Ecke der Seite „Verbundene Datensätze“, um vorhandene Projekte zu verbinden.

   Weitere Informationen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).
   * Inline-Bearbeitung der Projektinformationen in der Tabelle.
   * Klicken Sie auf **Neue Zeile**, um ein Projekt ohne Vorlage zu erstellen. Das neue Projekt wird sofort mit dem aktuellen Datensatz verbunden.

     Weitere Informationen finden Sie unter [Erstellen von Workfront-Objekten aus Workfront Planning beim Verbinden mit Datensätzen](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * Bewegen Sie den Mauszeiger über ein Projekt und klicken Sie auf das **Mehr** Menü [Mehr](assets/more-menu.png)

     ODER

     Wählen Sie ein oder mehrere Projekte aus, beachten Sie den blauen Balken unten in der Liste und klicken Sie dann auf eines der folgenden Elemente:

      * **Löschen**, um das Projekt zu löschen. Durch das Löschen eines Projekts wird es vom Datensatz getrennt und in den Papierkorb von Workfront verschoben.
      * **Trennen**, um das Projekt vom Datensatz zu trennen. Wenn Sie ein Projekt trennen, werden es und alle Werte seiner Suchfelder aus dem aktuellen Datensatz entfernt.

1. (Optional) Doppelklicken Sie auf den Namen der Registerkarte **Seite „Verbundene Datensätze**

   ODER

   Bewegen Sie den Mauszeiger über den Namen der Registerkarte und klicken Sie dann auf **Mehr** ![Mehr ](assets/more-menu.png) und klicken Sie dann auf **Umbenennen**, um die Registerkarte in eine neue Ansicht umzubenennen.
1. (Optional) Verwenden Sie eines der folgenden Ansichtselemente in der Symbolleiste einer verbundenen Datensatzseite, um die Tabellenansicht zu verwalten:

   * Filter
   * Sortieren
   * Gruppierung
   * Felder, zum Anzeigen, Ausblenden oder Neuanordnen von Feldern
   * Zeilenhöhe
   * Suchen

   Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Sie können keine Felder in der Tabellenansicht der Registerkarte eines verbundenen Datensatzes erstellen, bearbeiten oder löschen.

   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Optional) Bewegen Sie den Mauszeiger über den Namen der Registerkarte „Verbundene Datensätze“ und klicken Sie auf **Mehr** ![Mehr](assets/more-menu.png) und dann auf **Löschen**, um die Registerkarte zu entfernen.

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage views from the connected records page of a record. 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->