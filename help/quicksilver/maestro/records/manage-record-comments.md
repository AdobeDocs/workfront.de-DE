---
title: Verwalten von Datensatzkommentaren
description: Sie können an Adobe Maestro-Datensätzen zusammenarbeiten, indem Sie Kommentare oder Antworten im Kommentarbereich eines Datensatzes hinzufügen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: bccd29ce284ca247b51971369102b5992061afb0
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---


# Verwalten von Datensatzkommentaren

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. </span>

<span class="preview">Weitere Informationen zum aktuellen Veröffentlichungsplan finden Sie unter [Übersicht über die Version des ersten Quartals 2024](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

Sie können an Adobe Maestro-Datensätzen zusammenarbeiten, indem Sie Kommentare oder Antworten im Kommentarbereich eines Datensatzes hinzufügen.

## Überlegungen zum Kommentieren eines Datensatzes

* Sie können Kommentare und Antworten zu betrieblichen Datensätzen und Taxonomien in Maestro im Abschnitt Kommentare eines Datensatzes hinzufügen.

* Kommentare zu verknüpften Datensätzen werden nicht in den Datensätzen angezeigt, von denen Sie eine Verknüpfung herstellen. Wenn Sie beispielsweise einen Maestro-Produktdatensatz kommentieren, der mit einem Campaign-Datensatz verknüpft ist, wird der Kommentar nur auf dem Produktdatensatz in Maestro und nicht auf dem Campaign-Datensatz angezeigt, mit dem Sie eine Verknüpfung herstellen.

* Sie können Maestro-Datensätzen Kommentare hinzufügen, die durch eine Verbindung zwischen einem Maestro-Datensatz und einem Objekt aus einer anderen Anwendung erstellt wurden.

  Beispielsweise können Sie den Projekt-Maestro-Datensatz kommentieren, nachdem Sie Workfront-Projekte mit Maestro-Datensätzen verbunden haben. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/maestro/records/connect-records.md).

* Kommentare zu verknüpften Objekten in anderen Anwendungen werden nicht in Maestro angezeigt und Kommentare, die zu verknüpften Objekten in Maestro hinzugefügt wurden, werden nicht in anderen Anwendungen angezeigt.

  Beispielsweise werden zu Projekten in Workfront hinzugefügte Kommentare nicht im selben Projekt angezeigt, das mit einer Kampagne in Maestro verknüpft ist, und Kommentare, die zum Projekt-Maestro-Datensatz hinzugefügt wurden, werden nicht in Workfront angezeigt.

* Sie können Benutzer taggen, um sie auf eine Aktualisierung aufmerksam zu machen. Mit Tags versehene Benutzer erhalten keine In-App-Benachrichtigung oder E-Mail über Ihre Aktualisierung. <!--this might change??-->

* Sie können Datensätze aus den folgenden Bereichen von Maestro aktualisieren:

   * Auf der Detailseite.

  <!--* From the table view.-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/grant-access.md">Zugriff auf Adobe Maestro gewähren</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

### Kommentare zu Datensätzen verwalten

{{step1-to-maestro}}

Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet.
1. Wählen Sie eine Tabellenansicht aus dem **Ansicht** Dropdown-Menü.
1. Klicken Sie in der Tabellenansicht auf den Namen eines Datensatzes.

   Der Rekord **Details** Seite geöffnet. Der Bereich Kommentare wird standardmäßig im rechten Bereich geöffnet.

1. Beginnen Sie mit der Eingabe eines Kommentars im **Neuer Kommentar** ankreuzen.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Wenn Sie den Abschnitt Kommentare verlassen, bevor Sie mit der Eingabe und dem Senden eines Kommentars fertig sind, bleibt der Kommentar auf der Seite im Entwurfsmodus, auch wenn Sie sich abmelden und wieder anmelden. Bilder, die dem Kommentar hinzugefügt werden, werden ebenfalls im Entwurf gespeichert. Entwürfe werden sieben Tage lang gespeichert und können nicht wiederhergestellt werden. Entworfene Kommentare sind nur für den Benutzer sichtbar, der sie eingibt.

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um eine Änderung rückgängig zu machen oder wiederherzustellen:
   * STRG + Z ( ⌘ + z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Y ( ⌘ + y für Mac) zum Wiederholen einer Änderung
1. (Optional) Hinzufügen **@** gefolgt vom Namen eines Benutzers, der in der Aktualisierung jemanden taggt.
1. (Optional) Verwenden Sie die Optionen in der Rich-Text-Symbolleiste, um Ihren Text zu formatieren, Emojis, Links oder Bilder zu Ihrer Aktualisierung hinzuzufügen und Ihren Inhalt zu verbessern. Weitere Informationen finden Sie im Artikel im Abschnitt &quot;Verwenden von Rich Text in einem Workfront-Update&quot; [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Wenn ein anderer Benutzer einen Kommentar für dasselbe Element sendet, das Sie aktualisieren, wird eine rote Zeile mit der Anzeige &quot;Neu&quot;angezeigt, die Sie über die neueren Kommentare informiert.
   >
   >Der Indikator wird erst angezeigt, nachdem der Kommentar zum Element gesendet wurde, und nicht, wenn der Kommentar noch erstellt wurde.
   >
   >![](assets/new-line-indicator-comments.png)

1. Klicks **Einsenden** , um die Aktualisierung zum Datensatz hinzuzufügen.
1. (Optional) Um einen Kommentar zu bearbeiten, klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) in der oberen rechten Ecke des Kommentars klicken Sie auf **Bearbeiten**.

   >[!IMPORTANT]
   >
   >Sie können Ihren Kommentar nur innerhalb von 15 Minuten nach seiner Übermittlung bearbeiten.

1. Bearbeiten Sie die Informationen im Kommentar, fügen Sie Bilder hinzu oder entfernen Sie sie oder einen der getaggten Benutzer. Links neben dem Kommentar wird ein Indikator &quot;bearbeitet&quot;hinzugefügt.

   >[!TIP]
   >
   >Kommentare aus dem aktuellen Jahr zeigen das Jahr nicht im Datumsstempel an. Wenn Sie den Mauszeiger über einen Zeitstempel bewegen, wird das vollständige Datum einschließlich des Jahres angezeigt.

1. <span class="preview">(Optional und bedingt) Um nach einem vorhandenen Kommentar zu suchen, geben Sie in das Suchfeld in der oberen rechten Ecke des **Kommentare** Bereich.</span>

   <span class="preview">![](assets/search-box-for-comments-area.png)</span>

1. (Optional) Klicken Sie auf **Antwort** oder beginnen Sie mit der Eingabe eines Kommentars im **Antwort hinzufügen ...** -Bereich, um auf einen vorhandenen Kommentar zu antworten, und führen Sie dann die Schritte 4 bis 8 oben aus. <!--(**************accurate??***********)-->

1. (Bedingt und optional) Wenn andere Benutzer Kommentare hinzugefügt haben, die beim Hinzufügen Ihrer Kommentare außerhalb des sichtbaren Bereichs im Abschnitt Kommentare angezeigt werden, klicken Sie auf **Ansicht** innerhalb der **neues Kommentarbanner** unten auf dem Bildschirm, um diese Kommentare anzuzeigen.

   ![](assets/new-comments-banner-on-record.png)

   Weitere Kommentare werden unten auf dem Bildschirm angezeigt.

1. (Optional) Klicken Sie auf die **liken** -Symbol, um ein Update zu mögen oder zu bestätigen, dass Sie es gelesen haben. Das Symbol wird mit der Anzahl der &quot;Gefällt mir&quot;-Klicks aktualisiert.
1. (Bedingt und optional) Wenn Sie weitere Personen in Ihren Kommentar aufgenommen haben, klicken Sie auf die Avatare der in der Aktualisierung enthaltenen Benutzer, um eine Liste der Benutzer anzuzeigen, für die der Kommentar freigegeben ist.
1. (Optional) Klicken Sie auf die **Mehr** icon ![](assets/more-menu.png) in der oberen rechten Ecke des Kommentars klicken und auf eine der folgenden Optionen klicken, um Informationen aus einem Kommentar zu kopieren:

   * **Link kopieren**: Dadurch wird ein Link zum Kommentar in die Zwischenablage kopiert.
   * **Textkörper kopieren** t: Kopiert den Text des Kommentars in die Zwischenablage.
   * **Anführungsantwort**: Kopiert den Inhalt Ihres Kommentars in eine neue Antwort. Bilder sind nicht in der kopierten Antwort enthalten.

   Weitere Informationen finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Klicken Sie auf die **Mehr** icon ![](assets/more-menu.png) in der oberen rechten Ecke des Kommentars klicken Sie auf **Löschen** , um den Kommentar zu löschen.

