---
title: Datensatzseite verwalten
description: Sie können das Layout des Datensatzfelds und der Seite in der Adobe Workfront-Planung bearbeiten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 02d20209b8bf53c84308707a89a5abf399494b64
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Datensatzseite verwalten

{{maestro-important-intro}}

Sie können das Layout des Datensatzfelds und der Seite in der Adobe Workfront-Planung bearbeiten. Sie können das Datensatzfeld in einer Datensatzansicht anzeigen.

Das Datensatzfeld ist eine kleinere Ansicht der Datensatzseite, die in der Ansicht eines Datensatztyps angezeigt wird.

Wenn Sie das Layout eines Datensatzfelds und einer Seite ändern, werden das Feld und die Seite für alle Datensätze desselben Typs geändert.

Sie müssen Datensatztypen und Datensätze erstellen, bevor Sie mit der Bearbeitung von Datensatzseiten beginnen können.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Erstellen von Datensatztypen](../architecture/create-record-types.md)

* [Datensätze erstellen](/help/quicksilver/maestro/records/create-records.md)

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
<p>Ihr Unternehmen muss am Betaprogramm für die Adobe Workfront-Planung teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Bearbeiten von Datensatzseiten

* Durch das Neuanordnen von Feldern in der Datensatzbox oder Seite werden die Felder für alle Datensätze dieses Typs und für alle Benutzer, die auf diese Datensätze zugreifen, neu angeordnet.
* Das Hinzufügen eines Titelbilds zu einem Datensatz ist nicht Teil des Gesamtlayouts des Datensatzfelds oder der Seite. Sie können jedem Datensatz eindeutige Titelbilder hinzufügen.

## Felder im Datensatzfeld oder auf der Seite neu anordnen

{{step1-to-maestro}}

Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Oder

   Klicken Sie in der Tabellenansicht auf die **Details öffnen** icon ![](assets/open-details-icon-in-table-name-field.png) auf der linken Seite eines Datensatznamens.

   Das Feld des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Sie können die **Details öffnen** Symbol links neben dem Feld &quot;Name&quot;eines Datensatzes in einer Tabellenansicht nur dann angezeigt, wenn das Feld &quot;Name&quot;ein primäres Feld ist.

1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke des Datensatzfelds, um die Datensatzseite in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet.

   ![](assets/details-page.png)

1. Klicken Sie im Datensatzfeld oder auf der Seite auf das Symbol &quot;Grab&quot; ![](assets/grab-icon.png) links neben einem Feldnamen, und ziehen Sie ihn per Drag-and-Drop an die gewünschte Position.

   Die neue Position des Felds wird sowohl im Feld als auch auf der Seite aller Datensätze desselben Typs für alle Benutzer aktualisiert, die die Datensätze anzeigen.

   Alle Änderungen am Layout des Datensatzfelds oder der Seite werden automatisch gespeichert.


## Hinzufügen eines Titelbilds zum Datensatzfeld oder zur Seite

Sie können einen Datensatz personalisieren, indem Sie am oberen Rand des Datensatzfelds oder der Seite ein Titelbild hinzufügen.

{{step1-to-maestro}}

Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Oder

   Klicken Sie in der Tabellenansicht auf die **Details öffnen** icon ![](assets/open-details-icon-in-table-name-field.png) auf der linken Seite eines Datensatznamens.

   Das Feld des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Sie können die **Details öffnen** Symbol links neben dem Feld &quot;Name&quot;eines Datensatzes in einer Tabellenansicht nur dann angezeigt, wenn das Feld &quot;Name&quot;ein primäres Feld ist.

1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke des Datensatzfelds, um die Datensatzseite in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet.

   ![](assets/details-page.png)

1. Klicken Sie im Datensatzfeld oder auf der Seite auf **Deckblatt hinzufügen**. <!--check the casing here; I logged a bug for this-->
Die **Datensatzabdeckung** wird geöffnet.

1. Klicks **Hochladen auswählen** und suchen Sie nach einem Bild auf Ihrem Computer, das Sie auswählen, hinzufügen und klicken Sie dann auf **Bild verwenden**.

   Das Bild wird am oberen Rand des Datensatzfelds oder der Seite hochgeladen und die Änderungen werden automatisch gespeichert.

   ![](assets/record-page-with-cover-image.png)

1. (Optional) Bewegen Sie den Mauszeiger über das Bild und klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) Führen Sie in der rechten unteren Ecke des Titelbilds einen der folgenden Schritte aus:

   * Klicks **Hochladen** , wenn Sie das Titelbild ersetzen und Schritt 6 wiederholen möchten, um ein neues Bild hochzuladen und zu speichern.
   * Klicks **Reposition** und verwenden Sie die **Reposition** Tool ![](assets/reposition-tool-icon.png) , um das Titelbild zu zentrieren, und klicken Sie dann auf **Speichern** wann geschehen.
   * Klicks **Entfernen** , um das Titelbild zu entfernen.

   Alle Änderungen werden sofort wirksam.

