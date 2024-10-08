---
title: Verwalten von Datensatzkommentaren
description: Sie können an Adobe Workfront-Planungsdatensätzen zusammenarbeiten, indem Sie im rechten Bereich eines Datensatzes Kommentare oder Antworten hinzufügen. Sie können auch andere Änderungen anzeigen, die am Datensatz vorgenommen und vom System in diesem Bereich aufgezeichnet wurden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '1267'
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

Für den Zugriff auf die Workfront-Planung benötigen Sie Folgendes:

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

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
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
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->

## Überlegungen zum Kommentieren eines Datensatzes

* Sie können in der Workfront-Planung im Abschnitt Kommentare eines Datensatzes Kommentare und Antworten zu Datensätzen hinzufügen.

* Kommentare zu verknüpften Datensätzen werden nicht in den Datensätzen angezeigt, von denen Sie eine Verknüpfung herstellen. Wenn Sie beispielsweise einen Workfront Planning-Produktdatensatz kommentieren, der mit einem Campaign-Datensatz verknüpft ist, wird der Kommentar nur im Produktdatensatz in der Workfront-Planung und nicht im Campaign-Datensatz angezeigt, mit dem Sie eine Verknüpfung herstellen.

* Sie können Workfront-Planungsdatensätzen Kommentare hinzufügen, die durch eine Verbindung zwischen einem Datensatz und einem Objekt aus einer anderen Anwendung erstellt wurden.

  Beispielsweise können Sie den Datensatz &quot;Projekt-Workfront-Planung&quot;kommentieren, nachdem Sie Workfront-Projekte mit Workfront-Planungsdatensätzen verbunden haben. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

* Kommentare zu verknüpften Objekten in anderen Anwendungen werden nicht in der Workfront-Planung angezeigt und Kommentare, die zu verknüpften Objekten in der Workfront-Planung hinzugefügt wurden, werden in anderen Anwendungen nicht angezeigt.

  Beispielsweise werden zu Projekten in Workfront hinzugefügte Kommentare nicht im selben Projekt angezeigt, das mit einer Kampagne in der Workfront-Planung verknüpft ist, und Kommentare, die zum Projekt Workfront Planning Record hinzugefügt wurden, werden nicht in Workfront angezeigt.

* Sie können Benutzer taggen, um sie auf eine Aktualisierung aufmerksam zu machen. Mit Tags versehene Benutzer erhalten keine In-App-Benachrichtigung oder E-Mail über Ihre Aktualisierung. <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

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
1. (Optional) Fügen Sie **@** hinzu, gefolgt vom Namen eines Benutzers, der eine Person in der Aktualisierung taggt.

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. (Optional) Verwenden Sie die Optionen in der Rich-Text-Symbolleiste, um Ihren Text zu formatieren, Emojis, Links oder Bilder zu Ihrer Aktualisierung hinzuzufügen und Ihren Inhalt zu verbessern. Weitere Informationen finden Sie im Abschnitt &quot;Verwenden von Rich Text in einem Workfront-Update&quot;im Artikel [Arbeit aktualisieren](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >Wenn ein anderer Benutzer einen Kommentar für dasselbe Element sendet, das Sie aktualisieren, wird eine rote Zeile mit der Anzeige &quot;Neu&quot;angezeigt, die Sie über die neueren Kommentare informiert.
   >
   >Der Indikator wird erst angezeigt, nachdem der Kommentar zum Element gesendet wurde, und nicht, wenn der Kommentar noch erstellt wurde.
   >
   >![](assets/new-line-indicator-comments.png)

1. Klicken Sie auf **Senden** , um die Aktualisierung zum Datensatz hinzuzufügen.
1. (Optional) Um einen Kommentar zu bearbeiten, klicken Sie in der oberen rechten Ecke des Kommentars auf das Menü **Mehr** und dann auf **Bearbeiten**.![](assets/more-menu.png)

   >[!IMPORTANT]
   >
   >Sie können Ihren Kommentar nur innerhalb von 15 Minuten nach seiner Übermittlung bearbeiten.

1. Bearbeiten Sie die Informationen im Kommentar, fügen Sie Bilder hinzu oder entfernen Sie sie oder einen der getaggten Benutzer. Links neben dem Kommentar wird ein Indikator &quot;bearbeitet&quot;hinzugefügt.

   >[!TIP]
   >
   >Kommentare aus dem aktuellen Jahr zeigen das Jahr nicht im Datumsstempel an. Wenn Sie den Mauszeiger über einen Zeitstempel bewegen, wird das vollständige Datum einschließlich des Jahres angezeigt.

1. (Optional und bedingt) Um nach einem vorhandenen Kommentar zu suchen, beginnen Sie mit der Eingabe eines Suchbegriffs in das Suchfeld in der oberen rechten Ecke des Bereichs **Kommentare** .

   ![](assets/search-box-for-comments-area.png)

1. (Optional) Klicken Sie auf **Antworten** oder geben Sie einen Kommentar in den Bereich **Antwort hinzufügen ...** ein, um auf einen vorhandenen Kommentar zu antworten, und führen Sie dann die Schritte 4 bis 8 oben aus. <!--(**************accurate??***********)-->

1. (Bedingt und optional) Wenn andere Benutzer Kommentare hinzugefügt haben, die außerhalb des sichtbaren Bereichs im Abschnitt Kommentare angezeigt werden, während Sie Ihre Kommentare hinzugefügt haben, klicken Sie unten auf dem Bildschirm auf **Anzeigen** im Banner **neue Kommentare** , um diese Kommentare anzuzeigen.

   ![](assets/new-comments-banner-on-record.png)

   Weitere Kommentare werden unten auf dem Bildschirm angezeigt.

1. (Optional) Klicken Sie auf das Symbol **Gefällt mir** , um ein Update zu mögen oder zu bestätigen, dass Sie es gelesen haben. Das Symbol wird mit der Anzahl der &quot;Gefällt mir&quot;-Klicks aktualisiert.
1. (Bedingt und optional) Wenn Sie weitere Personen in Ihren Kommentar aufgenommen haben, klicken Sie auf die Avatare der in der Aktualisierung enthaltenen Benutzer, um eine Liste der Benutzer anzuzeigen, für die der Kommentar freigegeben ist.
1. (Optional) Klicken Sie oben rechts im Kommentar auf das Symbol **Mehr** ![](assets/more-menu.png) und klicken Sie auf eine der folgenden Optionen, um Informationen aus einem Kommentar zu kopieren:

   * **Link kopieren**: Kopiert einen Link zum Kommentar in die Zwischenablage.
   * **Textkörper kopieren**: Kopiert den Text des Kommentars in die Zwischenablage.
   * **Antwort zitieren**: Kopiert den Inhalt Ihres Kommentars in eine neue Antwort. Bilder sind nicht in der kopierten Antwort enthalten.

   Weitere Informationen finden Sie unter [Funktionsweise aktualisieren](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Klicken Sie oben rechts im Kommentar auf das Symbol **Mehr** ![](assets/more-menu.png) und dann auf **Löschen** , um den Kommentar zu löschen.
1. (Optional) Klicken Sie auf das Symbol **Kommentare ausblenden** ![](assets/hide-comments-icon.png) , um den rechten Bereich zu schließen.

## Übersicht über den Verlaufsabschnitt

Sie können die am Datensatz vorgenommenen Änderungen im Abschnitt Verlauf des rechten Bereichs eines Datensatzes überprüfen.

Weitere Informationen finden Sie in der [Verlaufsübersicht](/help/quicksilver/planning/records/history-section-overview.md).
