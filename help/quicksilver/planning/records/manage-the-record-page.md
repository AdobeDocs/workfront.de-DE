---
title: Datensatzseite verwalten
description: Sie können das Layout der Datensatzvorschau und -seite in der Adobe Workfront-Planung bearbeiten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 3856e56036a9845387d7dc6498a6f20728c8234a
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Datensatzseite verwalten

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
   <p>Neu: Licht oder höher</p>
   Oder
   <p>Aktuell: Arbeit oder höher</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für die Adobe Workfront-Planung</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Verwalten oder höhere Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Bearbeiten von Datensatzseiten

* Standardmäßig werden in den Details und Vorschauseiten eines Datensatzes alle mit dem Datensatz verknüpften Felder angezeigt.

* Auf der Vorschau- oder Detailseite können keine neuen Felder für einen Datensatz hinzugefügt werden. Sie müssen neue Felder in der Tabellenansicht hinzufügen, um sie auf den Seiten Vorschau und Details anzuzeigen.

* Sie können einer Datensatzvorschau oder Detailseite Abschnitte hinzufügen, um die Informationen nach allgemeinen Kriterien zu organisieren und die Suche zu erleichtern.

* Die folgenden Änderungen betreffen alle Datensätze desselben Typs und sind für alle Benutzer sichtbar, die auf diese Datensätze zugreifen:

   * Felder neu anordnen
   * Abschnitte hinzufügen oder entfernen

* Änderungen an der Anzeige, die Sie in der Datensatzvorschau vornehmen, werden sofort auf der Seite mit den Datensatzdetails angezeigt. Änderungen, die auf der Datensatzseite vorgenommen wurden, sind auch im Vorschaufeld der Datensätze sichtbar.

* Das Hinzufügen eines Titelbilds zu einem Datensatz ist nicht Teil des Gesamtlayouts der Datensatzvorschau oder -seite. Sie können jedem Datensatz eindeutige Titelbilder hinzufügen. Weitere Informationen finden Sie unter [Hinzufügen eines Titelbilds zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

## Abschnitte zur Datensatzvorschau oder -seite hinzufügen

Beachten Sie beim Hinzufügen von Abschnitten zu einer Datensatzseite Folgendes:

* Es gibt keine Beschränkung dafür, wie viele Abschnitte Sie auf einer Seite haben können.
* Sie können keinen leeren Abschnitt haben. Sie müssen mindestens ein Feld in einem Abschnitt haben.
* Sie können Felder per Drag-and-Drop von einem Abschnitt in einen anderen ziehen. Weitere Informationen finden Sie im Abschnitt . [Neuanordnen von Feldern auf der Datensatzvorschau- oder Detailseite](#rearrange-fields-in-the-record-preview-or-details-page) in diesem Artikel.
* Wenn Sie alle Felder aus einem Abschnitt entfernen, wird der Abschnitt automatisch gelöscht und kann nicht wiederhergestellt werden.

So fügen Sie einer Datensatzvorschau oder -seite einen Abschnitt hinzu:

{{step1-to-planning}}

Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Oder

   Klicken Sie in der Tabellenansicht auf die **Details öffnen** icon ![](assets/open-details-icon-in-table-name-field.png) auf der linken Seite eines Datensatznamens.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Sie können die **Details öffnen** Symbol links neben dem Feld &quot;Name&quot;eines Datensatzes in einer Tabellenansicht nur dann angezeigt, wenn das Feld &quot;Name&quot;ein primäres Feld ist.

1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) in der rechten oberen Ecke der Datensatzvorschau, um die Datensatzseite in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet.

   ![](assets/details-page.png)

1. Bewegen Sie in der Datensatzvorschau oder -seite den Mauszeiger über den Leerraum links von den Feldern und klicken Sie auf die Schaltfläche **Abschnitt hinzufügen** icon ![](assets/add-section-icon.png) , um einen Abschnitt hinzuzufügen.
1. Klicken Sie in den Namen des Abschnitts und ersetzen Sie **Unbenannter Abschnitt** mit einem Namen und klicken Sie dann auf &quot;Enter&quot;. Die unter dem Abschnitt angezeigten Felder sind automatisch Teil des neuen Abschnitts.
1. Ziehen Sie Felder in den neuen Abschnitt, wie im Abschnitt beschrieben. [Neuanordnen von Feldern auf der Datensatzvorschau- oder Detailseite](#rearrange-fields-in-the-record-preview-or-details-page) in diesem Artikel.

1. (Optional) Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf **Mehr** Menü ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Abschnitt zu bearbeiten:

   * Klicks **Umbenennen** , um den Abschnitt umzubenennen

     >[!TIP]
     >
     > Sie können einen Abschnitt inline umbenennen, indem Sie auf den Namen klicken.

   * Klicks **Nach oben** , um den Abschnitt um eine Position nach oben zu verschieben

     Oder

     Klicks **Nach unten** um den Abschnitt um eine Position nach unten zu verschieben.
Alle Felder im Abschnitt werden mit dem Abschnitt verschoben.

   * Klicks **Löschen** , um den Abschnitt zu löschen. Der Abschnitt wird gelöscht und kann nicht wiederhergestellt werden. Alle Benutzer, die auf die Datensätze dieses Typs zugreifen, sehen den gelöschten Abschnitt nicht mehr.

1. Klicken Sie auf den nach unten zeigenden Pfeil links neben einem Abschnittsnamen, um ihn zu reduzieren, oder auf den nach rechts zeigenden Pfeil, um ihn zu erweitern.
Alle Abschnitte werden standardmäßig erweitert.

1. (Optional) Klicken Sie auf die **Grab** icon ![](assets/grab-icon.png) links neben einem Abschnittsnamen, und ziehen Sie ihn an die gewünschte Stelle.

   Die neue Position des Abschnitts wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen an den Abschnitten und der Feldreihenfolge werden automatisch gespeichert.

## Neuanordnen von Feldern auf der Datensatzvorschau- oder Detailseite

{{step1-to-planning}}

Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Oder

   Klicken Sie in der Tabellenansicht auf die **Details öffnen** icon ![](assets/open-details-icon-in-table-name-field.png) auf der linken Seite eines Datensatznamens.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Sie können die **Details öffnen** Symbol links neben dem Feld &quot;Name&quot;eines Datensatzes in einer Tabellenansicht nur dann angezeigt, wenn das Feld &quot;Name&quot;ein primäres Feld ist.

1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der rechten oberen Ecke der Datensatzvorschau, um die Datensatzseite in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet.

   ![](assets/details-page.png)

1. Klicken Sie in der Datensatzvorschau oder -seite auf die **Grab** icon ![](assets/grab-icon.png) links neben einem Feldnamen, und ziehen Sie ihn per Drag-and-Drop an die gewünschte Position. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   Die neue Position des Felds wird sowohl in der Vorschau als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen am Layout der Datensatzvorschau oder der Seite werden automatisch gespeichert.

