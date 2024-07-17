---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Update der Arbeit
description: Sie können ein Adobe Workfront-Objekt (Projekt, Aufgabe oder Problem) aktualisieren, um über den Fortschritt des Objekts zu kommunizieren. Benutzer, die dem Objekt zugewiesen sind oder es abonniert haben, können Ihre Aktualisierung anzeigen. Sie können Benutzer auch mit Tags versehen, um sie auf die Aktualisierung aufmerksam zu machen.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '2984'
ht-degree: 0%

---

# Update der Arbeit

<!-- Audited: 1/2024 -->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>  (*****for all customers or in Production for customers who enabled fast releases-->

<!--<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

<!--info for April 11: hide the "Important" box below-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span>
-->

Sie können ein Adobe Workfront-Objekt aktualisieren, um andere über den Fortschritt des Objekts zu informieren. Weitere Informationen dazu, welche Objekte Sie in Workfront aktualisieren können, finden Sie unter [Übersicht über den Abschnitt &quot;Aktualisieren&quot;](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

Die Informationen in diesem Artikel beschreiben, wie Sie Informationen zu Projekten, Aufgaben und Problemen kommentieren und aktualisieren können. Benutzer, die dem Objekt zugewiesen sind oder es abonniert haben, können Ihre Aktualisierung anzeigen. Sie können Benutzer auch mit Tags versehen, um sie auf die Aktualisierung aufmerksam zu machen.

Das Hinzufügen von Kommentaren zu anderen Objekten ähnelt dem Aktualisieren von Projekten, Aufgaben und Problemen. Weitere Informationen zum Kommentieren auf Karten und Zielen finden Sie in den folgenden Artikeln:

* [Verwalten Sie Zielkommentare in Adobe Workfront-Zielen](../../workfront-goals/goal-management/manage-goal-comments.md).

  Sie benötigen eine zusätzliche Lizenz für den Zugriff auf Workfront Goals.

* [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)

* [Angeschlossene Karten auf Pinnwänden verwenden](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)

<!--Add a bullet for record comments when Planning is in GA: help/quicksilver/planning/records/manage-record-comments.md-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Abo</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz</strong></td> 
   <td> 
   <p>Aktuell: Anfrage oder höher für Probleme und Dokumente; Überprüfung oder höher für alle anderen Objekte</p>
   <p>Neu: Mitarbeiter oder höher für Probleme und Dokumente: Für alle anderen Objekte leicht oder höher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>Anzeigen oder Bearbeiten des Zugriffs für das Objekt, auf dem die Aktualisierung ausgeführt wird</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf das Objekt anzeigen</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Aktualisieren der Arbeit

* Sie können den meisten Objekten in Adobe Workfront im Abschnitt Updates Kommentare hinzufügen. Weitere Informationen dazu, welche Objekte den Abschnitt &quot;Aktualisierungen&quot;anzeigen, finden Sie unter [Übersicht über den Abschnitt &quot;Aktualisierungen&quot;](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

* Sie können Workfront-Objekten Kommentare aus anderen in Workfront integrierten Anwendungen oder aus der mobilen App Workfront hinzufügen.

  Nicht alle in Workfront integrierten Anwendungen können Workfront-Objekten Kommentare hinzufügen.

  Nicht alle Funktionen, die im Abschnitt &quot;Updates&quot;eines Objekts in Workfront verfügbar sind, sind in anderen Anwendungen verfügbar, wenn über die Anwendung auf Workfront-Objekte zugegriffen wird. Beispielsweise sind Rich-Text-Funktionen oder das private Einfügen eines Kommentars für ein Unternehmen möglicherweise nicht verfügbar, wenn einem Workfront-Objekt von einer Drittanbieteranwendung Kommentare hinzugefügt werden.

* Sie können während des Kommentars zum Objekt über den Fortschritt an einem Workfront-Objekt (Projekt, Aufgabe oder Problem) kommunizieren. Benutzer, die dem Objekt zugewiesen sind oder es abonniert haben, können eine Benachrichtigung über Ihre Aktualisierung erhalten. Jeder, der Zugriff auf das Objekt hat, kann Ihre Aktualisierung anzeigen.

* Sie können Benutzer taggen, um sie auf die Aktualisierung aufmerksam zu machen. Mit Tags versehene Benutzer erhalten eine In-App-Benachrichtigung und eine E-Mail über Ihre Aktualisierung.

  >[!TIP]
  >
  >Kommentar-Eigentümer werden automatisch mit Tags versehen. Weitere Informationen finden Sie unter [Taggen anderer Benutzer bei Updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).


* Sie können einem Objekt einen Kommentar hinzufügen, den Sie anzeigen können, oder Sie können sich als Workfront- oder Gruppenadministrator anmelden und einen Kommentar für einen anderen Benutzer hinzufügen. Weitere Informationen finden Sie unter [Als anderer Benutzer anmelden](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

* Sie können Projekte, Aufgaben und Probleme in den folgenden Bereichen von Workfront aktualisieren:

   * Von einem Workfront-Objekt aus im Abschnitt Updates (für Projekte, Aufgaben und Probleme)
   * Im Startbereich (für Aufgaben und Probleme)
   * Im Bereich &quot;Zusammenfassung&quot;in den folgenden Bereichen (für Aufgaben, Probleme und Dokumente):

      * Eine Liste von Objekten
      * Ein Timesheet
      * Startseite
      * Der Lastenausgleich

<!--info for April 11: hide the section below: add an update to a work item-->

<!--
## Add an update to a work item

Adding an update to a work item differs depending on what version of the Updates section you use.

You can add updates to the following objects: 

* Projects
* Tasks
* Issues
* Programs
* Portfolios
* Templates
* Template tasks
* Users
* Timesheets
* Teams
* Goals
* Cards in the Boards area
* Iterations
-->

<!--info for April 11: hide the section below completely:-->

<!--
### Add an update to a work item in the legacy Updates section

>[!IMPORTANT]
>
>The information on this page describes how you update projects, tasks, and issues.

1. Go to the work item for which you want to provide an update (such as a project, task, or issue).
1. Click the **Updates** section.
1. (Conditional) If it is enabled, click the **New commenting** option in the upper-right corner of the Updates section to disable it and enable the legacy commenting experience.
1. Click **Start a new update,** then type your update.  
1. (Optional) Use the options in the Rich Text toolbar to format your text, add emojis, links, or images to your update, to enhance your content. For more information, see the [Use Rich Text in a Workfront update](#use-rich-text-in-a-workfront-update) section in this article.
1. (Optional) Update any of the following information about the work item:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notify</strong></td> 
      <td>Identify users who must be notified of the update. Users assigned or subscribed to the object automatically receive notification when an update is made.<br><p>For information about how to include others on an update, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Commit Date</strong></td> 
      <td>In the date picker, select the date that you commit to complete the work item. For information about Commit Date, see <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong></td> 
      <td>Select a new condition for the task or issue. For information about selecting a condition, see <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Click the arrow beside the current status, then select the desired status from the drop-down menu. For information about setting a Status, see <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.<p>Updating the status of a work item does not automatically change the status of a project. Depending on how your project is set up, you might make updates to the project status separately. For more information on the various project update types, see <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p><p><b>NOTE</b>
      
      You cannot change the status of a work item while it is in a Pending Approval status.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Bar</strong></td> 
      <td>(Only available on tasks) Indicate the percentage of work completed by sliding the progress bar to the desired percentage. You can also double-click the completion bar and enter the percent complete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Private to my company</strong></td> 
      <td> <p>Disable this option to prevent users outside your company from having access to view this update.</p> 
      <p><b>NOTE</b></p>
      <p>This option displays only when the user is associated with a Company.</p>
      <p>This option is not available in all areas where you can add updates from. For example, this is not available in third-party applications where you can add updates from. </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Update** to add the update to the Workfront object.

   >[!NOTE]
   >
   >A small pop-up window will appear for seven seconds after clicking **Update**, allowing you to undo the update and return to the editing pane before the update is posted. The update is posted if you dismiss the undo pop-up, wait for it to disappear, or navigate away from the page. 
   >
   >If your Workfront administrator selects the "Never allow users to delete comments" setting in your access level, you cannot undo a comment. For more information, see [Create and modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. To reply to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
-->

<!--info for April 11: reword the title of this section to: "Add an update to a work item"; take out the step that says you need to enable the "New commenting" toggle (I think it is step 3??)-->

## Hinzufügen einer Aktualisierung zu einem Arbeitselement

In diesem Artikel wird beschrieben, wie Sie Projekte, Aufgaben oder Probleme aktualisieren können. Die meisten anderen Objekte werden ähnlich aktualisiert.

1. Suchen Sie das Objekt, das Sie aktualisieren möchten, und klicken Sie dann auf seinen Namen, um die Seite des Objekts zu öffnen.
1. Klicken Sie im linken Bereich auf **Aktualisierungen** .
Die Registerkarte **Kommentare** ist standardmäßig ausgewählt.

   <!--
   1. (Conditional) If the **New commenting** option is disabled, click to enable it. 

      This enables the new commenting experience. 

         >[!TIP]
         >
         ><span class="preview">The New commenting option has been removed in the Preview environment.</span>
   -->

1. Geben Sie einen Kommentar in das Feld **Neuer Kommentar** ein.

   ![Neues Kommentarfeld](assets/comment-box-all-tabs.png)

   >[!TIP]
   >
   >Wenn Sie den Abschnitt Updates verlassen, bevor Sie mit der Eingabe und dem Senden eines Kommentars fertig sind, bleibt der Kommentar auf der Seite im Entwurfsmodus, auch wenn Sie sich abmelden und wieder anmelden. Bilder, die dem Kommentar hinzugefügt werden, werden ebenfalls im Entwurf gespeichert. Entwürfe werden sieben Tage lang gespeichert und können nicht wiederhergestellt werden. Entworfene Kommentare sind nur für den Benutzer sichtbar, der sie eingibt.

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um eine Änderung rückgängig zu machen oder wiederherzustellen:
   * STRG + Z ( ⌘ + z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Y ( ⌘ + y für Mac) zum Wiederholen einer Änderung

1. (Optional) Beginnen Sie im Bereich **Personen oder Teams taggen** mit der Eingabe des Namens oder der E-Mail eines Benutzers oder eines Teams, das Sie in diesen Kommentar aufnehmen möchten, und wählen Sie ihn dann aus, wenn er in der Liste angezeigt wird.
1. (Optional) Verwenden Sie die Optionen in der Rich-Text-Symbolleiste, um Ihren Text zu formatieren, Emojis, Links oder Bilder zu Ihrer Aktualisierung hinzuzufügen und Ihren Inhalt zu verbessern. Weitere Informationen finden Sie im Abschnitt [Verwenden von Rich Text in einem Workfront-Update](#use-rich-text-in-a-workfront-update) in diesem Artikel.

   >[!TIP]
   >
   >Wenn ein anderer Benutzer einen Kommentar für dasselbe Element sendet, das Sie aktualisieren, wird eine rote Zeile mit der Anzeige &quot;Neu&quot;angezeigt, die Sie über die neueren Kommentare informiert.
   >
   >Der Indikator wird erst angezeigt, nachdem der Kommentar zum Element gesendet wurde, und nicht, wenn der Kommentar noch erstellt wurde.
   >
   >Der Indikator &quot;Neu&quot;wird nur angezeigt, wenn sowohl der Benutzer, der ein neues Update eingegeben hat, als auch der Benutzer, der derzeit ein Update aufruft, das neue Kommentarerlebnis verwenden.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. Klicken Sie auf **Senden** , um die Aktualisierung zum Workfront-Objekt hinzuzufügen.
1. (Optional) Um einen Kommentar zu bearbeiten, klicken Sie in der oberen rechten Ecke des Kommentars auf das Menü **Mehr** und dann auf **Bearbeiten**.![](assets/more-menu.png)

   >[!IMPORTANT]
   >
   >Sie können Ihren Kommentar nur innerhalb von 15 Minuten nach seiner Übermittlung bearbeiten.

1. Bearbeiten Sie die Informationen im Kommentar, fügen Sie Bilder hinzu oder entfernen Sie sie oder einen der getaggten Benutzer. Links neben dem Datumsstempel, der bei der Eingabe des Kommentars angezeigt wird, wird die Anzeige &quot;Bearbeitet&quot;hinzugefügt.

   >[!TIP]
   >
   >Kommentare aus dem aktuellen Jahr zeigen das Jahr nicht im Datumsstempel an. Wenn Sie den Mauszeiger über einen Zeitstempel bewegen, wird das vollständige Datum einschließlich des Jahres angezeigt.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* Es wird eine E-Mail erzeugt, um die Benutzer nur dann über Ihre Aktualisierung zu informieren, wenn Sie die ursprüngliche Aktualisierung übermitteln. Nach Bearbeitung des Updates wird keine E-Mail erzeugt.
   >* Der Datumsstempel neben dem Kommentar ist das Datum des ursprünglichen Kommentars und nicht das Datum der letzten Bearbeitung.
   >* Wenn Sie einen Kommentar für einen anderen Benutzer hinzufügen (wenn Sie sich als anderer Benutzer als Workfront- oder Gruppenadministrator anmelden), können Sie den Kommentar nicht bearbeiten, wenn Sie als der andere Benutzer angemeldet sind. Sie können den Kommentar erst bearbeiten, nachdem Sie sich als Benutzer abgemeldet und sich wieder wie Sie selbst angemeldet haben.

1. (Optional) Klicken Sie auf **Antworten** oder geben Sie einen Kommentar im Bereich **Antwort hinzufügen ...** ein, um auf einen vorhandenen Kommentar zu antworten, und führen Sie dann die Schritte 3 bis 7 oben aus. <!--(**************insure this stays accurate***********)--> Informationen zur Antwort auf eine Aktualisierung finden Sie unter [Antworten auf Aktualisierungen](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

1. (Bedingt und optional) Wenn andere Benutzer Kommentare hinzugefügt haben, die außerhalb des sichtbaren Bereichs im Abschnitt Updates angezeigt werden, während Sie Ihre Kommentare hinzugefügt haben, klicken Sie unten auf dem Bildschirm auf **Anzeigen** im blauen **neuen Kommentarbanner** , um diese Kommentare anzuzeigen.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Weitere Kommentare werden unten auf dem Bildschirm angezeigt.

1. (Optional) Klicken Sie auf das Symbol **Gefällt mir**![](assets/like-icon.png). Das Symbol wird mit der Anzahl der &quot;Gefällt mir&quot;-Klicks aktualisiert.
1. (Bedingt und optional) Wenn Sie Ihrem Kommentar weitere Personen hinzugefügt haben, klicken Sie auf die Anzahl der Mitglieder, die in der Aktualisierung enthalten sind, um eine Liste der Entitäten anzuzeigen, für die der Kommentar, den Sie eingegeben haben, freigegeben ist.

   ![](assets/members-icons-expanded-unshimmed.png)

   >[!TIP]
   >
   >Neben den Avataren werden die Namen der ersten beiden getaggten Entitäten angezeigt. Wenn mehr als zwei Entitäten mit Tags versehen sind, werden nur der Name des ersten und die Anzahl der zusätzlichen Entitäten angezeigt.

1. (Optional) Klicken Sie auf den Namen eines Kommentars, um dessen Namen, Rolle und E-Mail-Adresse in einem Informationsfeld anzuzeigen. Klicken Sie im Informationsfeld erneut auf den Namen des Kommentars, um sein Benutzerprofil zu öffnen.
1. (Optional) Klicken Sie auf die Registerkarte **Systemaktivität** , um die vom System protokollierten Aktualisierungen anzuzeigen. Wenn das Objekt oder seine untergeordneten Elemente aktualisiert werden, generiert Workfront einen Hinweis zu dieser Aktualisierung und zeigt sie auf der Registerkarte Systemaktivität an.

   Weitere Informationen finden Sie in der [Übersicht über den Abschnitt &quot;Aktualisierungen&quot;](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

   >[!TIP]
   >
   >Sie können einem Systemupdate keinen Kommentar hinzufügen. Alle Antworten, die im alten Kommentierungserlebnis auf Systemaktivitätsereignisse geantwortet wurden, wurden jedoch auf der Registerkarte Systemaktivität als schreibgeschützt hinzugefügt. Die veraltete Kommentarfunktion wurde am 11. April 2024 aus Workfront entfernt.

1. (Optional) Klicken Sie auf die Registerkarte **Alle** , um sowohl Benutzerkommentare als auch Systemaktivitätskommentare an einer Stelle anzuzeigen. Dies ist eine Registerkarte &quot;Nur Ansicht&quot;.

   >[!TIP]
   >
   >Sie können auf Kommentare nicht antworten oder andere Benutzer in vorhandenen Kommentaren auf der Registerkarte &quot;Alle&quot;taggen. Um auf einen Kommentar auf der Registerkarte &quot;Alle&quot;zu antworten, klicken Sie auf **In Kommentaren antworten** , um den Kommentar auf der Registerkarte &quot;Kommentare&quot;zu öffnen.

## Verwenden von Rich Text in einem Workfront-Update{#use-rich-text-in-a-workfront-update}

Sie können Ihre Aktualisierungen durch Verwendung von Rich Text oder durch Hinzufügen verschiedener Elemente wie Emojis, Links oder Bilder verbessern.

1. Gehen Sie zum Bereich **Aktualisierungen** eines Workfront-Objekts und beginnen Sie mit der Eingabe eines Kommentars.
1. (Optional) Um Ihrer Aktualisierung Rich-Text-Formatierung hinzuzufügen, verwenden Sie beim Eingeben Attribute in der Symbolleiste **Rich-Text** .

   ![](assets/rich-text-toolbar.png)

   | **Attribut** | **Symbolleistenschaltfläche** | **Mac-Tastaturbefehle** | **Windows-Tastaturbefehle** |
   |---|---|---|---|
   | Fett | ![](assets/mceclip10.png) | η+b | Strg+B |
   | kursiv | ![mceclip9.png](assets/mceclip9.png) | Befehl+i | Strg+I |
   | Unterstreichen | ![mceclip8.png](assets/mceclip8.png) | η+u | Strg+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png) | <br>So öffnen Sie das Feld &quot;Verknüpfungen hinzufügen&quot;: ^K</br> <br>So fügen Sie einen Link über den ausgewählten Text ein: SUMME+V</br> | <br>So öffnen Sie das Feld &quot;Links hinzufügen&quot;: Strg+K</br> <br>So fügen Sie einen Link über den ausgewählten Text ein: Strg+V</br> |
   | Aufzählung | ![mceclip6.png](assets/mceclip6.png) | η+Shift+8 | Strg+Umschalt+8 |
   | Nummerierte Liste | ![mceclip5.png](assets/mceclip5.png) | η+Shift+7 | Strg+Umschalt+7 |
   <!--| Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |<br>Ctrl+Shift+9</br> <br>This is not available in the new commenting experience. </br> |-->

   <!--remove the last row when we remove legacy from the system-->

   Um die Formatierung von Text zu beenden, deaktivieren Sie das Attribut in der Symbolleiste **Rich Text** .


   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* Die Formatierung wird auch in allen E-Mail-Benachrichtigungen angezeigt, die Benutzer mit Ihrer Aktualisierung erhalten.
   >* Die Rich-Text-Formatierung, die auf eine Aktualisierung in einer E-Mail angewendet wird, wird in der Aktualisierung nicht angezeigt, wenn sie auf der Registerkarte Aktualisierungen angezeigt wird.
   >* Wenn Ihr Unternehmen Workfront mit Internet Explorer verwendet, verliert jeder formatierte Text, der in eine Aktualisierung eingefügt wird, seine Rich-Text-Formatierung und wird als Nur-Text angezeigt. Sie können den Text mithilfe der Attribute in der Rich-Text-Symbolleiste neu formatieren.
   >* Die Rich-Text-Formatierung ist nicht für Aktualisierungen verfügbar, die im Bereich &quot;Timesheets&quot;vorgenommen werden, oder für die Objekte &quot;Hinweis&quot;und &quot;Letzte Bedingung&quot;in einem Bericht.

   <!--1. (Optional and conditional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting. This is not available in the new commenting experience.-->

   <!--remove this picture below and the bullet above when we remove legacy-->

   <!--![](assets/block-quote-marked-350x144.png)-->

1. (Optional) Klicken Sie auf das Symbol **Emoji** ![](assets/emoji-icon.png), um Emojis zu Ihrer Aktualisierung hinzuzufügen.

   >[!NOTE]
   >
   >* Workfront ersetzt keine Interpunktions-Emoticons wie :) durch Emojis.
   >* Für die in einem Bericht angezeigten Objekte &quot;Notiz&quot;und &quot;Letzte Bedingung&quot;sind keine Emojis verfügbar.
   >* Die Emoji-Funktion in Workfront verwendet Unicode-Zeichen und wird daher nur auf Browsern und Betriebssystemen angezeigt, die Unicode-Codepunkte unterstützen. Benutzer auf einer Plattform, einem Browser oder einer Betriebssystemversion, die nicht Ihre ist, haben möglicherweise keinen Zugriff auf dieselben Emojis.
   >* Ein nicht unterstütztes Emoji wird durch eine schwarze oder weiße Box dargestellt.
   >* Windows 7 unterstützt nur Schwarzweiß-Emojis.
   >* Emojis, die auf eine per E-Mail vorgenommene Aktualisierung angewendet werden, werden nicht in der Aktualisierung angezeigt, wenn sie im Bereich Updates angezeigt werden.

1. (Optional) So fügen Sie einen URL-Link zu zusätzlichen Informationsquellen hinzu:

   1. Klicken Sie in der Aktualisierung auf die Stelle, an der Sie einen Link einfügen möchten.
   1. Klicken Sie in der Symbolleiste **Rich Text** auf das Symbol **Hyperlink** ![](assets/link-icon.png).

   1. Geben Sie im angezeigten Feld **Link erstellen** unter **URL** die URL der Quelle ein oder fügen Sie sie ein.

   1. Geben Sie unter &quot;**Text für die Anzeige**&quot;den Link-Text ein oder fügen Sie ihn ein.
   1. Klicken Sie auf **Speichern**.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um ein Bild an Ihre Aktualisierung anzuhängen:

   * Speichern Sie das Bild auf unserem Computer und ziehen Sie es in den Bereich Neuer Kommentar .
   * Kopieren Sie einen Screenshot von Ihrem Computer und fügen Sie ihn dann in den Kommentar ein.<!-- This is not available in the legacy commenting experience.-->
   * Klicken Sie auf das Symbol **Bild hinzufügen** ![](assets/add-image-mountain-with-plus-icon.png) und navigieren Sie zum Bild auf Ihrem Computer.


   >[!NOTE]
   >
   >**WICHTIG**
   >
   ><!--<span class="preview">You cannot add images to goals or ad-hoc cards on boards.</span> -->
   >
   >* Der Workfront-Administrator muss das Hinzufügen von Bildern im Abschnitt &quot;Voreinstellungen für Feeds aktualisieren&quot;der Workfront-Benutzeroberfläche aktivieren, bevor die Symbole Bild oder Anhang hinzufügen angezeigt werden. Weitere Informationen finden Sie unter [Konfigurieren von Voreinstellungen für Benutzeraktualisierungen](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* Die maximale Bilddateigröße beträgt 7 MB. Unterstützte Bilddateitypen sind .jpg, .gif und .png.
   >* Auf Bilder kann über den Abschnitt Updates eines Objekts zugegriffen werden. Sie sind auch im Bereich Dokumente unter dem Hauptmenü verfügbar.
   >* Sie können das Bild einfügen, indem Sie mit der rechten Maustaste auf den neuen Kommentar klicken oder indem Sie Strg + V für Windows (oder für Mac) auf die Tastatur drücken.
   >* Sie können ein Update mit einem Bild und ohne Text senden.
   >* Wenn Sie einen Kommentar löschen, der ein Bild enthält, wird das Bild sowohl aus dem Abschnitt &quot;Aktualisierungen&quot;als auch aus dem Bereich &quot;Dokumente&quot;entfernt. Das Bild wird auch aus dem Bereich &quot;Dokumente&quot;gelöscht, wenn Sie einen Kommentar bearbeiten und das Bild löschen.
   >* Wenn jemand ein Bild löscht, das mit einem Kommentar verknüpft ist, wird es auch aus dem Kommentar entfernt.

   <!--remove the statement above about legacy, when we remove the legacy environment.-->

1. (Optional) Führen Sie einen der folgenden Schritte aus, um ein Bild in der vorhandenen Aktualisierung anzuzeigen:

   * Klicken Sie auf das Symbol **Vorschau** ![](assets/previewimageicon-31x31.png) in der Miniaturansicht des Bildes, um das Bild in voller Größe in einer neuen Browser-Registerkarte zu öffnen.
   * Klicken Sie auf das Symbol **Download** ![](assets/downloadimageicon.png) in der Miniaturansicht, um das Bild herunterzuladen.

1. Klicken Sie auf **Senden** , um Ihren Kommentar hinzuzufügen.

## Nach einer Aktualisierung suchen

Sie können nach einem Kommentar oder einer Antwort im Abschnitt Updates eines Objekts suchen.

1. Wechseln Sie zum Abschnitt **Aktualisierungen** eines Objekts.
1. Geben Sie in das Feld **Suche** oben rechts auf der Registerkarte **Kommentare** den Suchbegriff <!--or a user's name --> ein.

   <!--Add this tip or note instead of the note below - when it'll be possible: You can search for users who have been tagged or for comment owners.-->

   >[!NOTE]
   >
   >Sie können nur nach Wörtern suchen, die zum Text eines Kommentars oder einer Antwort gehören. Sie können nicht nach Namen von Benutzern oder Teams suchen, die in einer Aktualisierung mit Tags versehen wurden.

   ![Suche in Updates](assets/updates-all-tabs-with-search-field.png)

   Das Keyword <!--or user-->, nach dem Sie gesucht haben, wird hervorgehoben und die Kommentare, die es enthalten, werden oben im Abschnitt Updates angezeigt.

   Workfront durchsucht den gesamten Update-Stream des Objekts außerhalb der auf dem Bildschirm sichtbaren Kommentare.

1. Klicken Sie im Suchfeld auf das Symbol **x** , um die Suchergebnisse zu löschen und zu allen Kommentaren zurückzukehren.

<!-- when we release search to production, check above and make sure you don't have to add that the users tagged/ owners are also searchable-->

## Aktualisierungen kopieren

Es gibt mehrere Möglichkeiten, ein Update zu kopieren.

Sie können einen Link zur Aktualisierung kopieren oder den Inhalt einer Aktualisierung kopieren, um ihn in einer neuen Aktualisierung zu verwenden.

<!--Copying an update differs depending on which commenting experience you use.-->

<!--info for April 11: take the sentence above out and reword the section title below to: Copy an update-->

### Update kopieren <!--in the new commenting experience-->

<!--For information about what features are available for the new commenting experience and for what objects, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).-->

Sie können Informationen aus einem vorhandenen Kommentar kopieren, indem Sie einen der folgenden Schritte ausführen:

* [Link kopieren](#copy-link)
* [Fließtext kopieren](#copy-body-text)
* [Anführungsantwort](#quote-reply)

![](assets/copy-comment-ways-from-more-menu-on-comment.png)

#### Link kopieren

Die Option Link kopieren kopiert den Kommentar- oder Thread-Link in die Zwischenablage, damit Sie den Kommentar oder den gesamten Thread für andere Benutzer freigeben können.

1. Gehen Sie zu der Aktualisierung, deren Link Sie kopieren möchten.

1. Klicken Sie auf das Menü **Mehr** und dann auf **Link kopieren**.

1. Fügen Sie den Link, den Sie im vorherigen Schritt kopiert haben, in eine E-Mail oder eine andere Anwendung ein, um ihn für andere freizugeben. Der freigegebene Link öffnet den Kommentar, von dem Sie den Link freigegeben haben.

   >[!TIP]
   >
   >Wenn Sie die Verknüpfung einer Konversation mit einem untergeordneten Objekt von einem übergeordneten Objekt freigeben, öffnet die Verknüpfung den Thread im Bereich Updates des übergeordneten Objekts.
   >
   >Wenn Sie beispielsweise den Link eines Aufgabenkommentars aus dem Bereich &quot;Aktualisierungen&quot;des Projekts kopieren, öffnet der Kommentar die Projektseite.

#### Fließtext kopieren

Mit der Option Textkörper kopieren wird der Text von einem bestimmten Update in die Zwischenablage kopiert.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf das Menü **Mehr** und dann auf **Textkörper kopieren**.

#### Anführungsantwort

Mit der Option Antwort zitieren wird der ursprüngliche Kommentar als Blockanführungszeichen in eine neue Antwort kopiert.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf das Menü **Mehr** und dann auf **Antwort zitieren**.

   Ein neues Kommentarfeld wird geöffnet und die zitierte Antwort wird in den neuen Kommentar aufgenommen und als Blockanführungszeichen markiert.

   ![](assets/block-quote-highlighted-mid-comment-before-submit.png)


1. Fügen Sie Ihre Aktualisierung hinzu und klicken Sie auf **Senden** , um den Kommentar hinzuzufügen.

<!--info for April 11: hide the entire section below - notice that there are several sub-sub sections below this main section - hide them all, all the way up to "Delete an update"-->

<!--
### Copy an update in the legacy commenting experience

* [Copy the update](#copy-the-update) 
* [Copy the thread link](#copy-the-thread-link) 
* [Copy the update link](#copy-the-update-link)
* [Quote Reply](#quote-reply)

   >[!TIP]
   >
   >When you copy and share the link of a conversation on a child object from a higher-ranking object, the link opens the thread in the child object's Updates area. 
   >
   >For example, if you copy the link of a task comment from the project's Updates area, the comment opens the task page.

#### Copy the update {#copy-the-update}

This option copies the text from a specific update to the clipboard.

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Copy body text**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Copy the thread link {#copy-the-thread-link}

This option copies the full thread link to the clipboard so you can share the thread with other users.

1. Go to the update thread you want to copy.

1. Click the **More** menu, then click **Copy thread link**.

   ![](assets/update-stream-comment-menu-marked-350x152.png) 

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Copy the update link {#copy-the-update-link}

This option copies a specific update link to the clipboard. When you share the update link, the user who follows it sees a border around the update.

1. Go to the update or reply you want to copy.
1. Click the **More** menu next to the individual update, then click **Copy update link**.

   ![](assets/copy-update-link-old-ui.png)

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Quote Reply  

The Quote Reply option copies the original comment to a new reply as a block quote. 

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Quote Reply**.

   A new comment box opens and the quoted reply is included in the new comment and marked as a block quote.

1. Continue adding your update and click **Reply** to add the comment.
-->

## Aktualisieren oder Antworten löschen

Je nachdem, welchen Zugriff Ihr Workfront-Administrator Ihnen gewährt, können Sie möglicherweise Aktualisierungen löschen, die Sie auf der Registerkarte Updates eines Objekts hinzugefügt haben. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) im Artikel [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Kein Workfront-Benutzer (einschließlich Workfront-Administrator) kann Aktualisierungen löschen, die von einem anderen Benutzer vorgenommen wurden. Wenn die Zugriffsebene eines Benutzers es ihm jedoch ermöglicht, eigene Aktualisierungen zu löschen, kann sich der Workfront-Administrator als dieser Benutzer anmelden und die vorgenommenen Aktualisierungen löschen. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) und [Als anderer Benutzer anmelden](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Gehen Sie zu dem Update oder der Antwort, das/die Sie löschen möchten.
1. Klicken Sie auf das Menü **Mehr** neben der Aktualisierung oder Antwort, die Sie löschen möchten, und klicken Sie dann auf **Löschen**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Klicken Sie in der angezeigten Meldung auf **Löschen**.

   >[!NOTE]
   >
   >Wenn Sie eine Aktualisierung mit einem angehängten Bild löschen, werden sowohl der Kommentar als auch das Bild gelöscht. Weitere Informationen finden Sie im Abschnitt [Verwenden von Rich Text in einem Workfront-Update](#use-rich-text-in-a-workfront-update) in diesem Artikel.

   Wenn dem Kommentar, den Sie löschen, Antworten zugeordnet sind, gibt es einen Hinweis darauf, dass der Kommentar mit dem Namen des Benutzers entfernt wurde, der ihn entfernt hat.

   ![](assets/removed-comment-indicator-new-experience.png)

   Gelöschte Kommentare werden sofort aus Workfront entfernt. Ein Benutzer, der den Abschnitt Updates verwendet, sieht, dass ein Kommentar von einem anderen Benutzer in Echtzeit gelöscht wird.


## Systemaktualisierungen überprüfen

Im Abschnitt Updates für ein Workfront-Objekt werden zwei Arten von Informationen angezeigt:

* **Benutzeraktualisierungen:** Benutzeraktualisierungen sind Kommentare, die Sie und andere Benutzer in Ihrem System eingeben. Die Benutzeraktualisierungen werden auf den Registerkarten Kommentare und Alle im Abschnitt Aktualisierungen angezeigt.

  ![](assets/user-update-cl-350x277.png)

* **Systemaktualisierungen:** Das System aktualisiert Datensätze, die Aufgaben oder Probleme entfernen, Dokumentversionen hinzufügen oder löschen, eine Genehmigungsanforderung anhängen oder entfernen sowie alle Änderungen oder Änderungen am Objekt. Systemaktualisierungen werden in den Registerkarten Systemaktivität und Alle im Abschnitt Updates angezeigt.

  ![](assets/system-updates-cl-350x277.png)

  Workfront-Administratoren können bestimmen, was in Systemaktualisierungen verfolgt wird, wie unter [Vom System getrackte Updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md) beschrieben. Sie können auch Systemaktualisierungen oder Aktivitäten herausfiltern, sodass nur Benutzeraktualisierungen für alle Objekte angezeigt werden.

  Die folgenden Objekte verfügen nicht über systemgenerierte Aktualisierungen:

   * Team
   * Vorlage
   * Vorlagenaufgabe
   * Ad-hoc-Karte

Weitere Informationen zu Systemaktualisierungen im Abschnitt Updates finden Sie unter [Überblick über den Abschnitt Updates](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

<!-- with October 26 release: add somewhere this, and decide where we need to keep information about the legacy commenting. Should we create an article about iterations comments like we have for goals and cards?!:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old message, before Auhust 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).
-->