---
title: Hinzufügen eines Cover-Bildes zu einem Datensatz
description: Sie können Datensätze personalisieren, indem Sie der Datensatzseite in Adobe Workfront Planning ein Titelbild hinzufügen, wenn Sie einen Datensatz bearbeiten.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 0%

---


# Hinzufügen eines Cover-Bildes zu einem Datensatz

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie können Datensätze personalisieren, indem Sie der Datensatzseite in Adobe Workfront Planning ein Titelbild hinzufügen, wenn Sie einen Datensatz bearbeiten.

Weitere Informationen zum Bearbeiten von Datensätzen finden Sie unter [Bearbeiten von Datensätzen](/help/quicksilver/planning/records/edit-records.md).

Sie müssen Datensatztypen erstellen, bevor Sie Datensätze erstellen und bearbeiten können.

Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

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
<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
Oder
<li><p>Beliebiger Workflow und beliebiges Planungspaket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Beitragen von oder höhere Berechtigungen für einen Arbeitsbereich und einen Datensatztyp  </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr>   
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Überlegungen zu Aufzeichnungs-Seitenabdeckungsbildern

Sie können die Seite eines Datensatzes personalisieren, indem Sie ihr ein Titelbild hinzufügen.

Beachten Sie Folgendes:

* Ein Cover-Bild ist für einen Datensatz eindeutig und gilt nicht für alle Datensätze desselben Typs.
* Sie können nur Bilddateien als Titelbilder hinzufügen.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Sie können einzelnen Datensätzen aus der Datensatzvorschau in jeder Ansicht oder aus der Datensatzseite ein Cover-Bild hinzufügen.
* Sie können keine Cover-Bilder aus einer Datensatzansicht hinzufügen.
* Workfront lädt bei jeder Erstellung eines Datensatzes automatisch ein Titelbild hoch. Sie können dieses Bild später ändern.

## Hinzufügen eines Cover-Bildes zu einem Datensatz

Sie können einen Datensatz personalisieren, indem Sie oben auf der Datensatzvorschau oder der Seite ein Titelbild hinzufügen.

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie personalisieren möchten,

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf einen Datensatz

   Oder

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen** (![) &#x200B;](assets/open-details-icon-in-table-name-field.png) der ersten Spalte.

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![Vorschaufeld Details](assets/details-box.png)


1. (Optional) Klicken Sie auf **Symbol „In neuer Registerkarte** öffnen![&#x200B; Symbol „In neuer Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke der Datensatzvorschau, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet.

   ![Detailseite](assets/details-page.png)

1. Bewegen Sie auf der Seite „Datensatzvorschau“ oder „Details“ den Mauszeiger über den Bereich über dem Datensatznamen und klicken Sie dann auf **Abdeckung hinzufügen**.

   Oder

   Bewegen Sie den Mauszeiger über ein vorhandenes Titelbild und klicken Sie auf das Menü **Mehr** ![Mehr &#x200B;](assets/more-menu.png) und dann auf **Hochladen**. <!--check the casing here; I logged a bug for this-->
Das **„Datensatzabdeckung** wird auf der Registerkarte **Hochladen** geöffnet.

   ![Plattenhülle zum Hochladen](assets/record-cover-box-for-upload.png)

1. Klicken Sie **Bilder durchsuchen** und suchen Sie ein Bild auf Ihrem Computer, um es auszuwählen und hinzuzufügen.

1. (Optional) Um das Bild vor dem Speichern zu entfernen, klicken Sie auf das Symbol **Neues Bild hochladen** ![&#x200B; (Symbol Neues Bild hochladen](assets/upload-new-image-icon.png) und laden Sie ein neues Bild hoch.

1. (Optional) Klicken Sie auf **Galerie** und klicken Sie dann auf ein Bild in der Galerie. Die Bildergalerie kann nicht geändert werden.

   ![Plattendeckelkasten für Galerie](assets/record-cover-box-for-gallery.png)

1. Klicken Sie **Bild verwenden**.

   Das Bild wird oben auf der Datensatzvorschau- oder Detailseite hochgeladen und die Änderungen werden automatisch gespeichert.

   ![Seite mit Titelbild aufzeichnen](assets/record-page-with-cover-image.png)

1. (Optional) Bewegen Sie den Mauszeiger über das Bild und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) in der rechten unteren Ecke des Titelbilds. Führen Sie dann einen der folgenden Schritte aus:

   * Klicken Sie **Hochladen**, wenn Sie das Titelbild ersetzen möchten, und wiederholen Sie Schritt 6, um ein neues Bild hochzuladen und zu speichern.
   * Klicken Sie **Neu positionieren** und verwenden Sie das **Neu positionieren** Tool ![Symbol „Neu positionieren“](assets/reposition-tool-icon.png), um das Titelbild zu zentrieren, und klicken Sie dann auf **Speichern** wenn Sie fertig sind.
   * Klicken Sie **Entfernen**, um das Titelbild zu entfernen.

   Workfront speichert Ihre Änderungen automatisch.
