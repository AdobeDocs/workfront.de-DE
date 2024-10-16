---
title: Verwalten von Datensatzkommentaren
description: Sie können an Adobe Workfront-Planungsdatensätzen zusammenarbeiten, indem Sie im rechten Bereich eines Datensatzes Kommentare oder Antworten hinzufügen. Sie können auch andere Änderungen anzeigen, die am Datensatz vorgenommen und vom System in diesem Bereich aufgezeichnet wurden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# Verwalten von Datensatzkommentaren

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

Sie können an Adobe Workfront-Planungsdatensätzen zusammenarbeiten, indem Sie im rechten Bereich eines Datensatzes Kommentare oder Antworten hinzufügen. Sie können auch andere Änderungen anzeigen, die am Datensatz vorgenommen und vom System in diesem Bereich aufgezeichnet wurden.

Im rechten Bereich eines Datensatzes werden die folgenden Abschnitte angezeigt:

* **Kommentare**: Zeigt Kommentare und Antworten an, die Benutzer zu Datensätzen hinzufügen.
* **Verlauf**: Zeigt systemaufgezeichnete Änderungen an, die Benutzer an den Datensatzfeldern vornehmen. Weitere Informationen finden Sie in der [Verlaufsübersicht](/help/quicksilver/planning/records/history-section-overview.md).

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
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td> 
   <td> 
<p>Alle </p> 
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
   <td><p> Mitwirkende, Licht oder Standard</p>
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
   <td>   <p>Anzeigen oder höherer Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Kommentieren eines Datensatzes

* Sie können in der Workfront-Planung im Abschnitt Kommentare eines Datensatzes Kommentare und Antworten zu Datensätzen hinzufügen.

* Kommentare zu verknüpften Datensätzen werden nicht in den Datensätzen angezeigt, von denen Sie eine Verknüpfung herstellen. Wenn Sie beispielsweise einen Workfront Planning-Produktdatensatz kommentieren, der mit einem Campaign-Datensatz verknüpft ist, wird der Kommentar nur im Produktdatensatz in der Workfront-Planung und nicht im Campaign-Datensatz angezeigt, mit dem Sie eine Verknüpfung herstellen.

* Sie können Workfront-Planungsdatensätzen Kommentare hinzufügen, die durch eine Verbindung zwischen einem Datensatz und einem Objekt aus einer anderen Anwendung erstellt wurden.

  Beispielsweise können Sie den Datensatz &quot;Projekt-Workfront-Planung&quot;kommentieren, nachdem Sie Workfront-Projekte mit Workfront-Planungsdatensätzen verbunden haben. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

* Kommentare zu verknüpften Objekten in anderen Anwendungen werden nicht in der Workfront-Planung angezeigt und Kommentare, die zu verknüpften Objekten in der Workfront-Planung hinzugefügt wurden, werden in anderen Anwendungen nicht angezeigt.

  Beispielsweise werden zu Projekten in Workfront hinzugefügte Kommentare nicht im selben Projekt angezeigt, das mit einer Kampagne in der Workfront-Planung verknüpft ist, und Kommentare, die zum Projekt Workfront Planning Record hinzugefügt wurden, werden nicht in Workfront angezeigt.

* Sie können Benutzer taggen, um sie auf eine Aktualisierung aufmerksam zu machen. Mit Tags versehene Benutzer erhalten keine In-App-Benachrichtigung oder E-Mail über Ihre Aktualisierung. <!--this might change??-->

* Sie können Benutzer taggen, um sie auf eine Aktualisierung aufmerksam zu machen. Mit Tags versehene Benutzer erhalten eine In-App-Benachrichtigung oder eine E-Mail-Benachrichtigung über Ihre Aktualisierung.

  >[!NOTE]
  >
  >   Nur Benutzer von Kunden, die mit Adobe Unified Experience integriert sind, erhalten sowohl eine In-App-Benachrichtigung als auch eine E-Mail-Benachrichtigung. Informationen dazu, ob Ihr Unternehmen das Adobe Unified Experience verwendet, finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Sie können Datensätze aktualisieren und den Verlauf von Änderungen in den folgenden Bereichen der Workfront-Planung überprüfen:

   * Auf der Seite mit den Datensatzdetails .
   * In einer Ansicht im Feld &quot;Datensatzdetails&quot;.

### Kommentare zu Datensätzen verwalten

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden auf Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.
Die Seite mit dem Datensatztyp wird geöffnet und alle Datensätze dieses Typs werden angezeigt.

1. Wählen Sie eine Tabellenansicht aus dem Dropdownmenü **Ansicht** aus.
1. Klicken Sie in der Tabellenansicht auf den Namen eines Datensatzes.

   Die Seite **Details** des Datensatzes wird geöffnet. Der Bereich Kommentare wird standardmäßig im rechten Bereich geöffnet.

1. (Bedingt) Wenn das rechte Bedienfeld nicht standardmäßig geöffnet ist, klicken Sie oben rechts auf das Symbol **Kommentare anzeigen** ![](assets/show-comments-icon.png) , um den Abschnitt &quot;Kommentare&quot;zu öffnen.

1. Geben Sie einen Kommentar in das Feld **Neuer Kommentar** ein.

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Wenn Sie den Abschnitt Kommentare verlassen, bevor Sie mit der Eingabe und dem Senden eines Kommentars fertig sind, bleibt der Kommentar auf der Seite im Entwurfsmodus, auch wenn Sie sich abmelden und wieder anmelden. Bilder, die dem Kommentar hinzugefügt werden, werden ebenfalls im Entwurf gespeichert. Entwürfe werden sieben Tage lang gespeichert und können nicht wiederhergestellt werden. Entworfene Kommentare sind nur für den Benutzer sichtbar, der sie eingibt.

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um eine Änderung rückgängig zu machen oder wiederherzustellen:
   * STRG + Z ( ⌘ + z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Y ( ⌘ + y für Mac) zum Wiederholen einer Änderung
1. (Optional und bedingt) Wenn Ihre Workfront-Instanz Teil des Adobe Unified Experience ist, fügen Sie **@** hinzu, gefolgt vom Namen eines Benutzers, der eine Person in der Aktualisierung mit Tags versehen soll. Weitere Informationen finden Sie im Abschnitt [Überlegungen zum Kommentieren eines Datensatzes](#considerations-about-commenting-on-a-record) in diesem Artikel.

1. (Optional) Verwenden Sie die Optionen in der Rich-Text-Symbolleiste, um Ihren Text zu formatieren, Emojis, Links oder Bilder zu Ihrer Aktualisierung hinzuzufügen und Ihren Inhalt zu verbessern.

1. Fügen Sie dem Datensatz weiterhin Kommentare hinzu.

   Weitere Informationen zum Aktualisieren von Objekten, einschließlich Workfront-Planungsprotokollen, finden Sie unter [Aktualisieren der Arbeit](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![](assets/new-line-indicator-comments.png)

1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.

   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  

1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
   
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.

1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     

   ![](assets/search-box-for-comments-area.png)
     
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ...** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)

1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.

    ![](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
  
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 

    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

1. (Optional) Klicken Sie oben rechts im Kommentar auf das Symbol **Mehr** ![](assets/more-menu.png) und dann auf **Löschen** , um den Kommentar zu löschen.
1. (Optional) Klicken Sie auf das Symbol **Kommentare ausblenden** ![](assets/hide-comments-icon.png) , um den rechten Bereich zu schließen.

## Übersicht über den Verlaufsabschnitt

Sie können die am Datensatz vorgenommenen Änderungen im Abschnitt Verlauf des rechten Bereichs eines Datensatzes überprüfen.

Weitere Informationen finden Sie in der [Verlaufsübersicht](/help/quicksilver/planning/records/history-section-overview.md).
