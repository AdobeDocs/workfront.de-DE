---
title: Hinzufügen eines Cover-Bildes zu einem Datensatz
description: Sie können Datensätze personalisieren, indem Sie der Datensatzseite in Adobe Workfront Planning ein Titelbild hinzufügen, wenn Sie einen Datensatz bearbeiten.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---


# Hinzufügen eines Cover-Bildes zu einem Datensatz

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können Datensätze personalisieren, indem Sie der Datensatzseite in Adobe Workfront Planning ein Titelbild hinzufügen, wenn Sie einen Datensatz bearbeiten.

Weitere Informationen zum Bearbeiten von Datensätzen finden Sie unter [Bearbeiten von Datensätzen](/help/quicksilver/planning/records/edit-records.md).

Sie müssen Datensatztypen erstellen, bevor Sie Datensätze erstellen und bearbeiten können.

Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für Workfront Planning anzuzeigen.

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
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience für Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


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

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen**, das in der ersten Spalte ![](assets/open-details-icon-in-table-name-field.png).

   Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

1. (Optional) Klicken Sie auf **Symbol** In neuer Registerkarte öffnen![](assets/open-details-in-a-new-tab-icon.png) in der oberen rechten Ecke der Datensatzvorschau <!--check the icon; they are changing it-->, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen.

   Die Datensatzseite wird geöffnet.

   ![](assets/details-page.png)

1. Klicken Sie in der Datensatzvorschau oder auf der Seite auf **Abdeckung hinzufügen** in der Produktionsumgebung, <span class="preview">oder bewegen Sie den Mauszeiger über den Bereich über dem Datensatznamen und klicken Sie dann in der **auf** Abdeckung hinzufügen </span>.

   Oder

   Bewegen Sie den Mauszeiger über ein vorhandenes Cover-Bild und klicken Sie auf das **Mehr**-![](assets/more-menu.png) und dann auf **Hochladen**. <!--check the casing here; I logged a bug for this-->
Das **„Datensatzabdeckung** wird auf der Registerkarte **Hochladen** geöffnet.

   ![](assets/record-cover-box-for-upload.png)

1. Klicken Sie **Bilder durchsuchen** und suchen Sie ein Bild auf Ihrem Computer, um es auszuwählen und hinzuzufügen.

1. (Optional) Um das Bild vor dem Speichern zu entfernen, klicken Sie auf das Symbol **Neues Bild hochladen** ![](assets/upload-new-image-icon.png) und laden Sie ein neues Bild hoch.

1. (Optional) Klicken Sie auf **Galerie** und klicken Sie dann auf ein Bild in der Galerie. Die Bildergalerie kann nicht geändert werden.

   ![](assets/record-cover-box-for-gallery.png)

1. Klicken Sie **Bild verwenden**.

   Das Bild wird oben auf der Datensatzvorschau oder Seite hochgeladen und die Änderungen werden automatisch gespeichert.

   ![](assets/record-page-with-cover-image.png)

1. (Optional) Bewegen Sie den Mauszeiger über das Bild und klicken Sie dann auf das **Mehr**-![](assets/more-menu.png) in der rechten unteren Ecke des Titelbilds. Führen Sie dann einen der folgenden Schritte aus:

   * Klicken Sie **Hochladen**, wenn Sie das Titelbild ersetzen möchten, und wiederholen Sie Schritt 6, um ein neues Bild hochzuladen und zu speichern.
   * Klicken Sie **Neu positionieren** und verwenden Sie das ![](assets/reposition-tool-icon.png) **Neu positionieren**, um das Titelbild zu zentrieren. Klicken Sie anschließend **Speichern**.
   * Klicken Sie **Entfernen**, um das Titelbild zu entfernen.

   Workfront speichert Ihre Änderungen automatisch.
