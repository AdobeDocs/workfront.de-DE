---
title: Hinzufügen eines Titelbilds zu einem Datensatz
description: Sie können Datensätze personalisieren, indem Sie bei der Datensatzbearbeitung der Datensatzseite in der Adobe Workfront-Planung ein Titelbild hinzufügen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---


<!--update the metadata with real information-->

# Hinzufügen eines Titelbilds zu einem Datensatz

{{planning-important-intro}}

Sie können Datensätze personalisieren, indem Sie bei der Datensatzbearbeitung der Datensatzseite in der Adobe Workfront-Planung ein Titelbild hinzufügen.

Informationen zum Bearbeiten von Datensätzen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/maestro/records/edit-records.md).

Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

## Zugriffsanforderungen

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für die Workfront-Planung </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Beitragen oder höhere Berechtigungen zu einem Arbeitsbereich </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td>  <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/maestro/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Überlegungen zu Hintergrundbildern von Datensatzseiten

Sie können die Seite eines Datensatzes personalisieren, indem Sie ihm ein Titelbild hinzufügen.

Beachten Sie Folgendes:

* Ein Titelbild ist für einen Datensatz eindeutig und gilt nicht für alle Datensätze desselben Typs.
* Sie können nur Bilddateien als Titelbilder hinzufügen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Sie können einzelnen Datensätzen über die Datensatzvorschau in jeder Ansicht oder über die Datensatzseite ein Titelbild hinzufügen.
* Es ist nicht möglich, Titelbilder inline aus Datensatzansichten hinzuzufügen.

## Hinzufügen eines Titelbilds zu einem Datensatz

Sie können einen Datensatz personalisieren, indem Sie oben auf der Datensatzvorschau oder -seite ein Titelbild hinzufügen.

{{step1-to-maestro}}

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

1. Klicken Sie in der Datensatzvorschau oder -seite auf **Deckblatt hinzufügen**. <!--check the casing here; I logged a bug for this-->
Die **Datensatzabdeckung** wird geöffnet.

1. Klicks **Hochladen auswählen** und suchen Sie nach einem Bild auf Ihrem Computer, das Sie auswählen, hinzufügen und klicken Sie dann auf **Bild verwenden**.

   Das Bild wird oben auf der Datensatzvorschau oder Seite hochgeladen und die Änderungen werden automatisch gespeichert.

   ![](assets/record-page-with-cover-image.png)

1. (Optional) Bewegen Sie den Mauszeiger über das Bild und klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) Führen Sie in der rechten unteren Ecke des Titelbilds einen der folgenden Schritte aus:

   * Klicks **Hochladen** , wenn Sie das Titelbild ersetzen und Schritt 6 wiederholen möchten, um ein neues Bild hochzuladen und zu speichern.
   * Klicks **Reposition** und verwenden Sie die **Reposition** Tool ![](assets/reposition-tool-icon.png) , um das Titelbild zu zentrieren, und klicken Sie dann auf **Speichern** wann geschehen.
   * Klicks **Entfernen** , um das Titelbild zu entfernen.

   Workfront speichert Ihre Änderungen automatisch.
