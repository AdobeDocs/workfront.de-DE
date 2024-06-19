---
title: Hinzufügen eines Titelbilds zu einem Datensatz
description: Sie können Datensätze personalisieren, indem Sie bei der Datensatzbearbeitung der Datensatzseite in der Adobe Workfront-Planung ein Titelbild hinzufügen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 8bfada77ac7b1b2a8d8fb2feec8a8167a1397cdc
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---


<!--update the metadata with real information-->

# Hinzufügen eines Titelbilds zu einem Datensatz

{{planning-important-intro}}

Sie können Datensätze personalisieren, indem Sie bei der Datensatzbearbeitung der Datensatzseite in der Adobe Workfront-Planung ein Titelbild hinzufügen.

Informationen zum Bearbeiten von Datensätzen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

## Zugriffsanforderungen

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding cover images-->

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
   <p>Aktuell: Arbeit oder höher</p>
   <p>Neu: Standard</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für die Workfront-Planung </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td>  <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Arbeitsdokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zu Hintergrundbildern von Datensatzseiten

Sie können die Seite eines Datensatzes personalisieren, indem Sie ihm ein Titelbild hinzufügen.

Beachten Sie Folgendes:

* Ein Titelbild ist für einen Datensatz eindeutig und gilt nicht für alle Datensätze desselben Typs.
* Sie können nur Bilddateien als Titelbilder hinzufügen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Sie können einzelnen Datensätzen über die Datensatzvorschau in jeder Ansicht oder über die Datensatzseite ein Titelbild hinzufügen.
* Es ist nicht möglich, Titelbilder aus einer Datensatzansicht hinzuzufügen.
* Workfront lädt jedes Mal, wenn Sie einen Datensatz erstellen, automatisch ein Titelbild hoch. Sie können dieses Bild später ändern.

## Hinzufügen eines Titelbilds zu einem Datensatz

Sie können einen Datensatz personalisieren, indem Sie oben auf der Datensatzvorschau oder -seite ein Titelbild hinzufügen.

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie personalisieren möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichnamen und wählen Sie den Arbeitsbereich aus, dessen Datensätze Sie personalisieren möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer Ansicht eines beliebigen Typs auf einen Datensatz

   Oder

   Klicken Sie in der Tabellenansicht auf die **Details öffnen** icon ![](assets/open-details-icon-in-table-name-field.png) in der ersten Spalte.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der rechten oberen Ecke der Datensatzvorschau, um die Datensatzseite in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet.

   ![](assets/details-page.png)

1. Klicken Sie in der Datensatzvorschau oder -seite auf **Deckblatt hinzufügen**


   Oder

   Bewegen Sie den Mauszeiger über ein vorhandenes Titelbild und klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) Klicken Sie auf **Hochladen**. <!--check the casing here; I logged a bug for this-->
Die **Datensatzabdeckung** wird in der **Hochladen** Registerkarte.

   ![](assets/record-cover-box-for-upload.png)

1. Klicks **Bilder durchsuchen** und suchen Sie nach einem Bild auf Ihrem Computer, um es auszuwählen und hinzuzufügen.

1. (Optional) Um das Bild vor dem Speichern zu entfernen, klicken Sie auf das **Neues Bild hochladen** icon ![](assets/upload-new-image-icon.png) und laden Sie ein neues Bild hoch.

1. (Optional) Klicken Sie auf die **Galerie** und klicken Sie auf ein Bild in der Bildergalerie. Die Bildergalerie kann nicht geändert werden.

   ![](assets/record-cover-box-for-gallery.png)

1. Klicks **Bild verwenden**.

   Das Bild wird oben auf der Datensatzvorschau oder Seite hochgeladen und die Änderungen werden automatisch gespeichert.

   ![](assets/record-page-with-cover-image.png)

1. (Optional) Bewegen Sie den Mauszeiger über das Bild und klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) Führen Sie in der rechten unteren Ecke des Titelbilds einen der folgenden Schritte aus:

   * Klicks **Hochladen** , wenn Sie das Titelbild ersetzen und Schritt 6 wiederholen möchten, um ein neues Bild hochzuladen und zu speichern.
   * Klicks **Reposition** und verwenden Sie die **Reposition** Tool ![](assets/reposition-tool-icon.png) , um das Titelbild zu zentrieren, und klicken Sie dann auf **Speichern** wann geschehen.
   * Klicks **Entfernen** , um das Titelbild zu entfernen.

   Workfront speichert Ihre Änderungen automatisch.
