---
title: Verwalten von Datensatzkommentaren
description: Sie können an Adobe Maestro-Datensätzen zusammenarbeiten, indem Sie im Kommentarbereich eines Datensatzes Updates hinzufügen und Fragen oder Antworten stellen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Verwalten von Datensatzkommentaren

Sie können an Adobe Maestro-Datensätzen arbeiten, indem Sie Aktualisierungen hinzufügen und Fragen oder Antworten im Kommentarbereich eines Datensatzes stellen.

## Überlegungen zum Kommentieren eines Datensatzes

* Sie können Kommentare und Antworten zu betrieblichen Datensätzen und Taxonomien in Maestro im Abschnitt Kommentare eines Datensatzes hinzufügen.

* Kommentare zu verknüpften Datensätzen werden nicht in den Datensätzen angezeigt, von denen Sie eine Verknüpfung herstellen. Wenn Sie beispielsweise einen Kommentar zu einem Projekt abgeben, das mit einem Campaign-Datensatz verknüpft ist, wird der Kommentar nur auf dem Projektdatensatz in Maestro und nicht auf dem Kampagnensatz angezeigt, von dem aus Sie eine Verknüpfung herstellen.

* Kommentare zu verknüpften Objekten in anderen Anwendungen werden nicht in Maestro angezeigt.
Kommentare zu verknüpften Objekten in Maestro werden in anderen Anwendungen nicht angezeigt.\
  Beispielsweise werden zu Projekten in Workfront hinzugefügte Kommentare nicht im selben Projekt angezeigt, das mit einer Kampagne in Maestro verknüpft ist.

* Sie können Benutzer taggen, um sie auf eine Aktualisierung aufmerksam zu machen. Mit Tags versehene Benutzer erhalten keine In-App-Benachrichtigung oder E-Mail über Ihre Aktualisierung. In einem Maestro-Kommentar können Sie keine Teams taggen.

  >[!TIP]
  >
  >* Kommentar-Eigentümer werden bei einer Aktualisierung nicht automatisch mit Tags versehen.
  >
  >* Sie können getaggte Benutzer nicht aus einer Aktualisierung entfernen, wenn Sie darauf antworten.

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


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### Kommentare zu Datensätzen verwalten

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](assets/dots-main-menu.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](assets/lines-main-menu.png) in der oberen linken Ecke auf **[!UICONTROL Maestro]**.

   Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet.
1. Wählen Sie eine Tabellenansicht aus dem **Ansicht** Dropdown-Menü.
1. Klicken Sie in der Tabellenansicht auf den Namen eines Datensatzes.

   Der Rekord **Details** Seite geöffnet.

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

1. (Optional und bedingt) Um nach einem vorhandenen Kommentar zu suchen, geben Sie in das Suchfeld in der oberen rechten Ecke des **Kommentare** Bereich.

   ![](assets/search-box-for-comments-area.png)

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

