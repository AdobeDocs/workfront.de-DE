---
title: Verwalten von Datensatzkommentaren
description: Sie können an Adobe Workfront Planning-Datensätzen zusammenarbeiten, indem Sie Kommentare oder Antworten im rechten Bedienfeld eines Datensatzes hinzufügen. Sie können auch andere Änderungen am Datensatz anzeigen, die vom System in diesem Bereich aufgezeichnet wurden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# Verwalten von Datensatzkommentaren

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können an Adobe Workfront Planning-Datensätzen zusammenarbeiten, indem Sie Kommentare oder Antworten im rechten Bedienfeld eines Datensatzes hinzufügen. Sie können auch andere Änderungen am Datensatz anzeigen, die vom System in diesem Bereich aufgezeichnet wurden.

Im rechten Bereich eines Datensatzes werden die folgenden Abschnitte angezeigt:

* **Kommentare**: Zeigt Kommentare und Antworten an, die Benutzende zu Datensätzen hinzufügen.
* **History**: Zeigt systemaufgezeichnete Änderungen an, die Benutzer an den Datensatzfeldern vornehmen. Weitere Informationen finden Sie unter [Übersicht über den Verlauf](/help/quicksilver/planning/records/history-section-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Mitwirkender, Licht oder Standard</p>
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
   <td>   <p>Anzeigen oder Erweitern von Berechtigungen für einen Arbeitsbereich <span class="preview">und Datensatztyp</span> </a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Kommentieren eines Datensatzes

* In Workfront Planning können Sie im Abschnitt „Kommentare“ eines Datensatzes Kommentare und Antworten zu Datensätzen hinzufügen.

* Kommentare, die verknüpften Datensätzen hinzugefügt wurden, werden nicht in den Datensätzen angezeigt, mit denen Sie verknüpfen. Wenn Sie beispielsweise einen Workfront Planning-Produktdatensatz kommentieren, der mit einem Kampagnendatensatz verknüpft ist, wird der Kommentar nur für den Produktdatensatz in Workfront Planning angezeigt und nicht für den Kampagnendatensatz, von dem aus Sie ihn verknüpfen.

* Sie können Workfront Planning-Datensätzen, die als Ergebnis einer Verbindung zwischen einem Datensatz und einem Objekt aus einer anderen Anwendung erstellt wurden, Kommentare hinzufügen.

  Sie können beispielsweise den Projekt-Workfront-Planungsdatensatz kommentieren, nachdem Sie Workfront-Projekte mit Workfront-Planungsdatensätzen verbunden haben. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

* Kommentare, die in anderen Programmen zu verknüpften Objekten hinzugefügt wurden, werden in Workfront Planning nicht angezeigt und Kommentare, die in Workfront Planning zu verknüpften Objekten hinzugefügt wurden, werden in anderen Programmen nicht angezeigt.

  So werden beispielsweise Kommentare, die Projekten in Workfront hinzugefügt wurden, nicht im selben Projekt angezeigt, das mit einer Kampagne in Workfront Planning verknüpft ist, und Kommentare, die zum Projekt-Workfront Planning-Datensatz hinzugefügt wurden, werden in Workfront nicht angezeigt.

* Sie können Benutzer taggen, um ihre Aufmerksamkeit auf ein Update zu lenken. Getaggte Benutzende erhalten keine In-App-Benachrichtigung oder E-Mail zu Ihrem Update. <!--this might change??-->

* Sie können Benutzer taggen, um ihre Aufmerksamkeit auf ein Update zu lenken. Getaggte Benutzende erhalten eine In-App-Benachrichtigung oder eine E-Mail-Benachrichtigung über Ihr Update.

  >[!NOTE]
  >
  >   Nur Benutzer von Kunden, die sich für Adobe Unified Experience entschieden haben, erhalten sowohl eine In-App-Benachrichtigung als auch eine E-Mail-Benachrichtigung. Informationen dazu, ob Ihr Unternehmen Adobe Unified Experience verwendet, finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Sie können eine Aktualisierung zu Datensätzen hinzufügen und den Änderungsverlauf aus den folgenden Bereichen von Workfront Planning überprüfen:

   * Auf der Seite mit den Datensatzdetails .
   * Aus einer Ansicht im Feld Datensatzdetails .

### Verwalten von Kommentaren zu Datensätzen

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet, und die Datensatztypen werden auf Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.
Die Seite „Datensatztyp“ wird geöffnet und alle Datensätze dieses Typs werden angezeigt.

1. Wählen Sie eine Tabellenansicht aus dem Dropdown **Menü** Ansicht“ aus.
1. Klicken Sie auf den Namen eines Datensatzes in der Tabellenansicht.

   Die Seite „Details **des** wird geöffnet. Der Bereich Kommentare wird standardmäßig im rechten Bedienfeld geöffnet.

1. (Bedingt) Wenn der rechte Bereich nicht standardmäßig geöffnet wird, klicken Sie auf das Symbol **Kommentare anzeigen** ![Kommentare anzeigen](assets/show-comments-icon.png) in der oberen rechten Ecke, um den Abschnitt Kommentare zu öffnen.

1. Beginnen Sie mit der Eingabe eines Kommentars in das Feld **Neuer Kommentar**.

   ![Leeres Kommentarfeld im Datensatz](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >Wenn Sie den Abschnitt Kommentare verlassen, bevor Sie mit dem Eingeben und Senden eines Kommentars fertig sind, befindet sich der Kommentar auf der Seite im Entwurfsmodus, auch wenn Sie sich ab- und wieder anmelden. <!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. (Optional) Um eine Änderung rückgängig zu machen oder wiederherzustellen, verwenden Sie die folgenden Tastenkombinationen:
   * Strg+Z (⌘+Z für Mac), um eine Änderung rückgängig zu machen
   * Strg+Y (⌘+Y für Mac), um eine Änderung wiederherzustellen
1. (Optional und bedingt) Wenn Ihre Workfront-Instanz Teil von Adobe Unified Experience ist, fügen Sie **@** hinzu, gefolgt vom Namen eines Benutzers, um jemanden in der Aktualisierung zu taggen. Weitere Informationen finden Sie im Abschnitt [Überlegungen zum Kommentieren eines Datensatzes](#considerations-about-commenting-on-a-record) in diesem Artikel.

1. (Optional) Verwenden Sie die Optionen in der Rich-Text-Symbolleiste, um Ihren Text zu formatieren, Emojis oder Links zu Ihrer Aktualisierung hinzuzufügen, um Ihren Inhalt zu verbessern.

   >[!TIP]
   >
   >Sie können keine Bilder zu einem Datensatzkommentar hinzufügen.


1. Fügen Sie dem Datensatz weitere Kommentare hinzu.

   Weitere Informationen zum Aktualisieren von Objekten, einschließlich Workfront-Planungsdatensätzen, finden Sie unter [Arbeit aktualisieren](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Optional) Klicken Sie auf das **Mehr**-Symbol ![Mehr ](assets/more-menu.png) oben rechts im Kommentar und dann auf **Löschen**, um den Kommentar zu löschen.
1. (Optional) Klicken Sie auf das Symbol **Kommentare ausblenden** ![Symbol „Kommentare ausblenden](assets/hide-comments-icon.png), um das rechte Bedienfeld zu schließen.

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ...** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## Übersicht über den Verlaufsabschnitt

Sie können die am Datensatz vorgenommenen Änderungen im Abschnitt Verlauf des rechten Bedienfelds eines Datensatzes überprüfen.

Weitere Informationen finden Sie unter [Übersicht über den Verlauf](/help/quicksilver/planning/records/history-section-overview.md).
