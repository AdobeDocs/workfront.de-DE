---
title: Layout der Datensatzseite verwalten
description: Sie können das Layout der Datensatzvorschau und -seite in der Adobe Workfront-Planung bearbeiten.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 5db940b197364e30ef6e1ea3e3c94ae3bda5b20c
workflow-type: tm+mt
source-wordcount: '1683'
ht-degree: 0%

---


# Layout der Datensatzseite verwalten

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

Sie können das Layout der Datensatzvorschau und -seite in der Adobe Workfront-Planung bearbeiten.

Die Datensatzvorschau ist eine kleinere Ansicht der Datensatzseite, die in der Ansicht eines Datensatztyps angezeigt wird.

Wenn Sie das Layout einer Datensatzvorschau und -seite ändern, wirken sich die Änderungen auf die Vorschaufelder und Detailseiten aller Datensätze desselben Typs aus.

In diesem Artikel wird beschrieben, wie Sie das Layout und Erscheinungsbild eines Datensatzvorschaufelds oder einer Datensatzseite ändern können. Informationen zum Bearbeiten von Datensätzen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

Sie müssen Datensatztypen und Datensätze erstellen, bevor Sie mit der Bearbeitung von Datensatzseiten beginnen können.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md)

* [Datensätze erstellen](/help/quicksilver/planning/records/create-records.md)

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
<p>Alle</p>
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
   <td>
   <p>Standard</p>
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
   <td>
   <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü und den Planungsbereich für Projekte, Portfolios und Programme enthält. </p> Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Übersicht über den Zugriff auf die Adobe-Planung</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Bearbeiten von Datensatzseiten

* Standardmäßig werden in den Details und Vorschauseiten eines Datensatzes alle mit dem Datensatz verknüpften Felder angezeigt.

* Auf der Vorschau- oder Detailseite können keine neuen Felder für einen Datensatz hinzugefügt werden. Sie müssen neue Felder in der Tabellenansicht hinzufügen, um sie auf den Seiten Vorschau und Details anzuzeigen.

* Sie können einer Datensatzvorschau oder Detailseite Abschnitte hinzufügen, um die Informationen nach allgemeinen Kriterien zu organisieren und die Suche zu erleichtern.

* Die folgenden Änderungen betreffen alle Datensätze desselben Typs und sind für alle Benutzer sichtbar, die auf diese Datensätze zugreifen:

   * Felder neu anordnen
   * Abschnitte hinzufügen oder entfernen

* Änderungen an der Anzeige, die Sie in der Datensatzvorschau vornehmen, werden sofort auf der Seite mit den Datensatzdetails angezeigt. Änderungen, die auf der Datensatzseite vorgenommen wurden, sind auch im Vorschaufeld der Datensätze sichtbar.

* Das Hinzufügen eines Titelbilds oder einer Miniaturansicht zu einem Datensatz ist nicht Teil des Gesamtlayouts der Datensatzvorschau oder -seite. Sie können jedem Datensatz eindeutige Titelbilder oder Miniaturansichten hinzufügen. Weitere Informationen finden Sie unter [Hinzufügen eines Titelbilds zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) und [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Abschnitte zur Datensatzvorschau oder -seite hinzufügen

Beachten Sie beim Hinzufügen von Abschnitten zu einer Datensatzseite Folgendes:

* Es gibt keine Beschränkung dafür, wie viele Abschnitte Sie auf einer Seite haben können.
* Sie können keinen leeren Abschnitt haben. Sie müssen mindestens ein Feld in einem Abschnitt haben.
* Sie können Felder per Drag-and-Drop von einem Abschnitt in einen anderen ziehen. Weitere Informationen finden Sie im Abschnitt [Felder in der Datensatzvorschau oder Detailseite neu anordnen](#rearrange-fields-in-the-record-preview-or-details-page) in diesem Artikel.
* Wenn Sie alle Felder aus einem Abschnitt entfernen, wird der Abschnitt automatisch gelöscht und kann nicht wiederhergestellt werden.

So fügen Sie einer Datensatzvorschau oder -seite einen Abschnitt hinzu:

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Oder

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen** ![](assets/open-details-icon-in-table-name-field.png) in der ersten Spalte.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

1. (Optional) Klicken Sie oben rechts in der Datensatzvorschau auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) , um die Datensatzseite in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet. Die Registerkarte Details wird standardmäßig geöffnet.

   ![](assets/details-page.png)

1. Bewegen Sie auf der Registerkarte **Details** der Datensatzvorschau oder -seite den Mauszeiger über den Leerraum links von den Feldern und klicken Sie dann auf das Symbol **Abschnitt hinzufügen** ![](assets/add-section-icon.png) , um einen Abschnitt hinzuzufügen.
1. Klicken Sie in den Namen des Abschnitts und ersetzen Sie den Abschnitt **Unbenannt** durch einen Namen. Klicken Sie dann auf &quot;Enter&quot;. Die unter dem Abschnitt angezeigten Felder sind automatisch Teil des neuen Abschnitts.
1. Ziehen Sie Felder in den neuen Abschnitt, wie im Abschnitt [Felder in der Datensatzvorschau oder Detailseite neu anordnen](#rearrange-fields-in-the-record-preview-or-details-page) in diesem Artikel beschrieben.

1. (Optional) Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das Menü **Mehr** ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Abschnitt zu bearbeiten:

   * Klicken Sie auf **Umbenennen** , um den Abschnitt umzubenennen.

     >[!TIP]
     >
     > Sie können einen Abschnitt inline umbenennen, indem Sie auf den Namen klicken.

   * Klicken Sie auf **Nach oben verschieben** , um den Abschnitt um eine Position nach oben zu verschieben

     Oder

     Klicken Sie auf **Nach unten verschieben** , um den Abschnitt um eine Position nach unten zu verschieben.
Alle Felder im Abschnitt werden mit dem Abschnitt verschoben.

   * Klicken Sie auf **Löschen** , um den Abschnitt zu löschen. Der Abschnitt wird gelöscht und kann nicht wiederhergestellt werden. Alle Benutzer, die auf die Datensätze dieses Typs zugreifen, sehen den gelöschten Abschnitt nicht mehr.

1. Klicken Sie auf den nach unten zeigenden Pfeil links neben einem Abschnittsnamen, um ihn zu reduzieren, oder auf den nach rechts zeigenden Pfeil, um ihn zu erweitern.
Alle Abschnitte werden standardmäßig erweitert.

1. (Optional) Klicken Sie auf das Symbol **grab** links neben einem Abschnittsnamen, ziehen Sie es dann per Drag-and-Drop an die gewünschte Position.![](assets/grab-icon.png)

   Die neue Position des Abschnitts wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen an den Abschnitten und der Feldreihenfolge werden automatisch gespeichert.

1. (Optional) Klicken Sie auf das Menü **Exportieren** , um die Registerkarte &quot;Details&quot;in eine Word- oder PDF-Datei zu exportieren. ![](assets/export-icon-in-record-details-page.png) Weitere Informationen finden Sie unter [Details eines Datensatzes exportieren](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Optional) Klicken Sie auf die Registerkarte **Verbindungen** neben der Registerkarte **Details**. Möglicherweise müssen Sie auf **Mehr** klicken, bevor Sie auf die Registerkarte **Verbindungen** klicken.

   Alle Datensätze oder Objekte, die mit dem ausgewählten Datensatz verbunden sind, werden unter den Namen des Datensatztyps oder der Anwendung angezeigt, zu der sie gehören.

   ![](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Optional) Wählen Sie die Einstellung **Alle Datensätze anzeigen** in der oberen rechten Ecke der Registerkarte &quot;Verbindungen&quot;aus. Es werden alle verbundenen Datensatztypen angezeigt, einschließlich derjenigen, die noch keine Datensätze mit dem System verbunden haben. Standardmäßig ist der Umschalter deaktiviert und die Datensatztypen ohne verbundene Datensätze werden ausgeblendet.

1. (Optional) Klicken Sie auf **Verbinden** , um den verbundenen Datensatztypen weitere Datensätze hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine Datensatzkarte, klicken Sie auf das Symbol zum Trennen des Datensatzes **-** und klicken Sie dann auf **Trennen**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
Folgendes geschieht:
   * Der Datensatz ist nicht mehr mit dem Workfront-Objekt verbunden.
   * Das Workfront-Objekt wird auch aus dem verbundenen Feld des Datensatzes aus der Workfront-Planung entfernt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden ebenfalls gelöscht.

## Ordnen Sie die Felder im Tab Details des Datensatzes neu an.

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Oder

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen** ![](assets/open-details-icon-in-table-name-field.png) in der ersten Spalte.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

1. (Optional) Klicken Sie oben rechts in der Datensatzvorschau auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> , um die Datensatzseite in einer neuen Registerkarte zu öffnen.

   Die Registerkarte **Details** des Datensatzes wird standardmäßig geöffnet.

   ![](assets/details-page.png)

1. Klicken Sie auf der Registerkarte **Details** des Datensatzes auf das Symbol **Grab** ![](assets/grab-icon.png) links neben dem Feldnamen und ziehen Sie es dann an die gewünschte Stelle. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   Die neue Position des Felds wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen am Layout der Datensatzvorschau oder der Seite werden automatisch gespeichert.

<span class="preview">

## Hinzufügen einer Seite mit der Verbindungsansicht zur Seite eines Datensatzes

Beachten Sie beim Hinzufügen einer Verbindungsansicht zu einer Datensatzseite Folgendes:

* Sie können der Seite eines Datensatzes eine Seite zur Ansicht &quot;Verbindung&quot;hinzufügen.

* Es ist nicht möglich, dem Vorschaubereich eines Datensatzes eine Seite mit der Verbindungsansicht hinzuzufügen.

* Auf den Seiten der Verbindungsansicht wird eine verbundene Datensatzseite in der Tabellenansicht angezeigt. Die Tabellenansicht ist schreibgeschützt.

* Sie können für jeden verbundenen Datensatztyp eine Ansichtsseite &quot;Verbindung&quot;hinzufügen.  <!--edit this when we can remove fields from this page-->

* Nachdem Sie die Seite Verbindungsansicht zu einer Datensatzseite hinzugefügt haben, ist die Seite im Vorschaubereich des Datensatzes sichtbar.

So fügen Sie eine Seite zur Ansicht der Verbindung hinzu:

1. Klicken Sie in einer Datensatzseitenansicht auf den Namen eines Datensatzes, um ihn zu öffnen, und klicken Sie dann oben rechts auf der Vorschauseite auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) .
1. Klicken Sie auf **Seite hinzufügen** > **Verbindungsansicht**.

   ![](assets/add-connection-view-page-modal.png)
1. Fügen Sie den **Seitennamen** hinzu, klicken Sie auf **Verbindungsansicht** und dann auf **Erstellen**.

   Der Datensatzseite wird eine neue Registerkarte hinzugefügt.
1. Suchen oder klicken Sie in der Liste auf den Namen eines verbundenen Datensatzes oder Objekttyps.
Die Tabellenansicht des ausgewählten Datensatztyps wird angezeigt und die verbundenen Datensätze werden in der Tabellenansicht angezeigt.
Die Tabellenansicht ist schreibgeschützt.

   ![](assets/audience-connected-table-view-under-campaign-details-page.png)
1. (Optional) Doppelklicken Sie auf den Namen der Registerkarte

   Oder

   Bewegen Sie den Mauszeiger über den Namen der Registerkarte, klicken Sie dann auf **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Umbenennen** , um in die neue Registerkarte &quot;Connected view&quot;umzubenennen.
1. (Optional) Verwenden Sie beliebige Ansichtselemente in der Symbolleiste, um die Tabellenansicht zu verwalten. Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).
1. (Optional) Bewegen Sie den Mauszeiger über den Namen der Registerkarte, klicken Sie auf **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Löschen** , um die Registerkarte &quot;Connected view&quot;zu entfernen.

</span>

<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



