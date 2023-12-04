---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Update der Arbeit
description: Sie können ein Adobe Workfront-Objekt (Projekt, Aufgabe oder Problem) aktualisieren, um über den Fortschritt des Objekts zu kommunizieren. Benutzer, die dem Objekt zugewiesen sind oder es abonniert haben, können Ihre Aktualisierung anzeigen. Sie können Benutzer auch mit Tags versehen, um sie auf die Aktualisierung aufmerksam zu machen.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 97f6e3390a2bf2a4f01c2780561bad80d271f03a
workflow-type: tm+mt
source-wordcount: '4052'
ht-degree: 1%

---

# Update der Arbeit

<!--take "legacy" and "new commenting" references out when we remove the legacy - Jan 2024???-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. </span>

<span class="preview">Weitere Informationen zum aktuellen Veröffentlichungsplan finden Sie unter [Übersicht über die Version des ersten Quartals 2024](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

>[!IMPORTANT]
>
>Die Kommentarerfahrung in Adobe Workfront wird derzeit umgestaltet.
>
>Je nachdem, für welche Objekte Sie auf das Kommentierungserlebnis zugreifen, sehen Sie möglicherweise die folgende Funktion für den Abschnitt Aktualisierungen :
>* Das neue Erlebnis
>* Das alte Erlebnis
>* Das neue und das veraltete Erlebnis
>
>Weitere Informationen über das neue Kommentierungserlebnis und dessen Verfügbarkeit finden Sie unter [Neues Kommentierungserlebnis](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Das neue Kommentarerlebnis ist nur für den Abschnitt Updates von Workfront-Objekten verfügbar und nicht verfügbar, wenn Sie auf Aktualisierungen aus den folgenden Bereichen zugreifen:
>
> * Startseite
> * Zusammenfassungsbereich in Listen
> * Zusammenfassungsbereich in Timesheets

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

## Überlegungen zum Aktualisieren der Arbeit

* Sie können den meisten Objekten in Adobe Workfront im Abschnitt Updates Kommentare hinzufügen. Weitere Informationen dazu, welche Objekte den Abschnitt Aktualisierungen anzeigen, finden Sie unter [Übersicht über den Aktualisierungsabschnitt](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

* Sie können Workfront-Objekten Kommentare aus anderen in Workfront integrierten Anwendungen oder aus der mobilen App Workfront hinzufügen.

  Nicht alle in Workfront integrierten Anwendungen können Workfront-Objekten Kommentare hinzufügen.

  Nicht alle Funktionen, die im Abschnitt &quot;Updates&quot;eines Objekts in Workfront verfügbar sind, sind in anderen Anwendungen verfügbar, wenn über die Anwendung auf Workfront-Objekte zugegriffen wird. Beispielsweise sind Rich-Text-Funktionen oder das private Einfügen eines Kommentars für ein Unternehmen möglicherweise nicht verfügbar, wenn einem Workfront-Objekt von einer Drittanbieteranwendung Kommentare hinzugefügt werden.

* Sie können während des Kommentars zum Objekt über den Fortschritt an einem Workfront-Objekt (Projekt, Aufgabe oder Problem) kommunizieren. Benutzer, die dem Objekt zugewiesen sind oder es abonniert haben, können eine Benachrichtigung über Ihre Aktualisierung erhalten. Jeder, der Zugriff auf das Objekt hat, kann Ihre Aktualisierung anzeigen.

* Sie können Benutzer taggen, um sie auf die Aktualisierung aufmerksam zu machen. Mit Tags versehene Benutzer erhalten eine In-App-Benachrichtigung und eine E-Mail über Ihre Aktualisierung.

  >[!TIP]
  >
  >   In der neuen Kommentarerfahrung werden die Eigentümer von Kommentaren automatisch mit Tags versehen. Weitere Informationen finden Sie unter [Tagging anderer Benutzer auf Updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
  <!--take the "in the new commenting experience" out when this is the only experience-->

* Sie können einem Objekt einen Kommentar hinzufügen, den Sie anzeigen können, oder Sie können sich als Workfront- oder Gruppenadministrator anmelden und einen Kommentar für einen anderen Benutzer hinzufügen. Weitere Informationen finden Sie unter [Melden Sie sich als anderer Benutzer an](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

* Sie können Projekte, Aufgaben und Probleme in den folgenden Bereichen von Workfront aktualisieren:

   * Von einem Workfront-Objekt im Abschnitt Updates
   * Im Startbereich (für Aufgaben und Probleme)
   * Über das Bedienfeld &quot;Zusammenfassung&quot;in einer Liste von Objekten oder aus einem Timesheet (für Aufgaben und Probleme)

Die Informationen auf dieser Seite beschreiben, wie Sie Kommentare zu Workfront-Objekten erstellen können und wie Sie Projekte, Aufgaben und Probleme aktualisieren, wenn Sie ihnen Kommentare hinzufügen.

<!--take this out (below) when we remove legacy out of the application-->

Informationen zur Kommentarkommentierung zu Zielen finden Sie unter [Verwalten von Zielkommentaren in Adobe Workfront-Zielen](../../workfront-goals/goal-management/manage-goal-comments.md). Sie benötigen eine zusätzliche Lizenz für den Zugriff auf Workfront Goals.

Weitere Informationen zur Kommentierung von Karten im Bereich &quot;Pinnwände&quot;finden Sie unter [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](../../agile/get-started-with-boards/add-card-to-board.md).

## Zugriffsanforderungen

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Anfrage oder höher für Probleme und Dokumente</p>
   <p> Überprüfen oder höher für alle anderen Objekte</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Anzeigen oder Bearbeiten des Zugriffs für das Objekt, auf dem die Aktualisierung ausgeführt wird</p> <p><b>NOTIZ</b>

Wenn Sie keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf das Objekt anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Hinzufügen einer Aktualisierung zu einem Arbeitselement

Das Hinzufügen eines Updates zu einem Arbeitselement hängt von der verwendeten Version des Abschnitts Updates ab.

Sie können Aktualisierungen zu den folgenden Objekten hinzufügen:

* Projekte
* Aufgaben
* Probleme
* Programme
* Portfolios
* Vorlagen
* Vorlagenaufgaben
* Benutzende
* Arbeitszeit- tabellen
* Teams
* Ziele
* Karten im Bereich der Karten
* Wiederholungen

### Hinzufügen einer Aktualisierung zu einem Arbeitselement im Abschnitt &quot;Legacy-Updates&quot;

>[!IMPORTANT]
>
>Die Informationen auf dieser Seite beschreiben, wie Sie Projekte, Aufgaben und Probleme aktualisieren.

1. Gehen Sie zu dem Arbeitselement, für das Sie eine Aktualisierung bereitstellen möchten (z. B. ein Projekt, eine Aufgabe oder ein Problem).
1. Klicken Sie auf **Updates** Abschnitt.
1. (Bedingt) Wenn sie aktiviert ist, klicken Sie auf die **Neue Kommentare** in der oberen rechten Ecke des Abschnitts Updates , um sie zu deaktivieren und das alte Kommentierungserlebnis zu aktivieren.
1. Klicks **Neue Aktualisierung starten,** Geben Sie dann Ihr Update ein.
1. (Optional) Verwenden Sie Rich Text oder fügen Sie Emojis, Links oder Bilder zu Ihrer Aktualisierung hinzu, um Ihre Inhalte zu verbessern. Weitere Informationen finden Sie unter [Verwenden von Rich Text in einem Workfront-Update](#use-rich-text-in-a-workfront-update) in diesem Artikel beschrieben.
1. (Optional) Aktualisieren Sie eine der folgenden Informationen zum Arbeitselement:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Benachrichtigen</strong></td> 
      <td>Identifizieren Sie Benutzer, die über die Aktualisierung benachrichtigt werden müssen. Benutzer, die dem Objekt zugewiesen sind oder es abonniert haben, erhalten bei einer Aktualisierung automatisch eine Benachrichtigung.<br><p>Informationen dazu, wie Sie andere in eine Aktualisierung einbeziehen, finden Sie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagging anderer Benutzer auf Updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Verpflichtungsdatum</strong></td> 
      <td>Wählen Sie in der Datumsauswahl das Datum aus, an dem Sie das Arbeitselement abschließen möchten. Weitere Informationen zum Übermittlungsdatum finden Sie unter <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Datum bestätigen - Übersicht</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bedingung</strong></td> 
      <td>Wählen Sie eine neue Bedingung für die Aufgabe oder das Problem aus. Informationen zum Auswählen einer Bedingung finden Sie unter <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Aktualisierungsbedingung für Aufgaben und Probleme</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Klicken Sie auf den Pfeil neben dem aktuellen Status und wählen Sie dann im Dropdown-Menü den gewünschten Status aus. Weitere Informationen zum Festlegen eines Status finden Sie unter <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aktualisierung des Aufgabenstatus</a>.<p>Beim Aktualisieren des Status eines Arbeitselements wird der Status eines Projekts nicht automatisch geändert. Je nachdem, wie Ihr Projekt eingerichtet ist, können Sie den Projektstatus separat aktualisieren. Weitere Informationen zu den verschiedenen Aktualisierungstypen finden Sie unter <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Wählen Sie den Projektaktualisierungstyp aus </a>.</p><p><b>NOTIZ</b>

   Sie können den Status eines Arbeitselements nicht ändern, während es sich im Status Ausstehende Genehmigung befindet.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Abschlussleiste</strong></td> 
      <td>(Nur für Aufgaben verfügbar) Geben Sie den Prozentsatz der abgeschlossenen Arbeiten an, indem Sie den Fortschrittsbalken auf den gewünschten Prozentsatz verschieben. Sie können auch auf die Abschlussleiste doppelklicken und den Prozentsatz eingeben, der abgeschlossen ist.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Vertraulich für meine Firma</strong></td> 
      <td> <p>Deaktivieren Sie diese Option, um zu verhindern, dass Benutzer außerhalb Ihres Unternehmens Zugriff auf diese Aktualisierung haben.</p> 
      <p><b>NOTIZ</b></p>
      <p>Diese Option wird nur angezeigt, wenn der Benutzer mit einem Unternehmen verknüpft ist.</p>
      <p>Diese Option ist nicht in allen Bereichen verfügbar, aus denen Sie Aktualisierungen hinzufügen können. Dies ist beispielsweise nicht in Drittanbieteranwendungen verfügbar, aus denen Sie Aktualisierungen hinzufügen können. </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **Aktualisieren** , um die Aktualisierung zum Workfront-Objekt hinzuzufügen.

   >[!NOTE]
   >
   >Nach dem Klicken auf wird ein kleines Popup-Fenster für sieben Sekunden angezeigt **Aktualisieren**, sodass Sie die Aktualisierung rückgängig machen und zum Bearbeitungsbereich zurückkehren können, bevor die Aktualisierung veröffentlicht wird. Das Update wird veröffentlicht, wenn Sie das Popup &quot;Rückgängig&quot;schließen, warten, bis es ausgeblendet wird, oder von der Seite weg navigieren.
   >
   >Wenn Ihr Workfront-Administrator in Ihrer Zugriffsebene die Einstellung &quot;Benutzer dürfen Kommentare nie löschen&quot;auswählt, können Sie einen Kommentar nicht rückgängig machen. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen und ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. Informationen zum Antworten auf eine Aktualisierung finden Sie unter [Antworten auf Aktualisierungen](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

### Hinzufügen einer Aktualisierung zu einem Arbeitselement mithilfe des neuen Kommentierungserlebnisses

1. Suchen Sie das zu aktualisierende Objekt (Projekt, Aufgabe oder Problem) und klicken Sie dann auf seinen Namen, um die Seite des Objekts zu öffnen.
1. Klicks  **Updates** im linken Bereich.
1. (Bedingt) Wenn die Variable **Neue Kommentare** deaktiviert ist, klicken Sie auf , um sie zu aktivieren.

   Dies ermöglicht das neue Kommentarerlebnis. Die **Kommentare** ist standardmäßig ausgewählt.
1. Beginnen Sie mit der Eingabe eines Kommentars im **Neuer Kommentar** ankreuzen.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Wenn Sie den Abschnitt Updates verlassen, bevor Sie mit der Eingabe und dem Senden eines Kommentars fertig sind, bleibt der Kommentar auf der Seite im Entwurfsmodus, auch wenn Sie sich abmelden und wieder anmelden. Bilder, die dem Kommentar hinzugefügt werden, werden ebenfalls im Entwurf gespeichert. Entwürfe werden sieben Tage lang gespeichert und können nicht wiederhergestellt werden. Entworfene Kommentare sind nur für den Benutzer sichtbar, der sie eingibt.

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um eine Änderung rückgängig zu machen oder wiederherzustellen:
   * STRG + Z ( ⌘ + z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Y ( ⌘ + y für Mac) zum Wiederholen einer Änderung
1. (Optional) Im **Personen oder Teams taggen** eingeben, den Namen oder die E-Mail-Adresse eines Benutzers oder eines Teams eingeben, das Sie in diesen Kommentar aufnehmen möchten, und ihn dann auswählen, wenn er in der Liste angezeigt wird.
1. (Optional) Verwenden Sie Rich Text oder fügen Sie Emojis, Links oder Bilder zu Ihrer Aktualisierung hinzu, um Ihre Inhalte zu verbessern. Weitere Informationen finden Sie unter [Verwenden von Rich Text in einem Workfront-Update](#use-rich-text-in-a-workfront-update) in diesem Artikel beschrieben.

   >[!TIP]
   >
   >Wenn ein anderer Benutzer einen Kommentar für dasselbe Element sendet, das Sie aktualisieren, wird eine rote Zeile mit der Anzeige &quot;Neu&quot;angezeigt, die Sie über die neueren Kommentare informiert.
   >
   >Der Indikator wird erst angezeigt, nachdem der Kommentar zum Element gesendet wurde, und nicht, wenn der Kommentar noch erstellt wurde.
   >
   >Der Indikator &quot;Neu&quot;wird nur angezeigt, wenn sowohl der Benutzer, der ein neues Update eingegeben hat, als auch der Benutzer, der derzeit ein Update aufruft, das neue Kommentarerlebnis verwenden.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. Klicks **Einsenden** , um die Aktualisierung zum Workfront-Objekt hinzuzufügen.
1. (Optional) Um einen Kommentar zu bearbeiten, klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) in der oberen rechten Ecke des Kommentars klicken Sie auf **Bearbeiten**.

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


1. (Optional) Klicken Sie auf **Antwort** oder beginnen Sie mit der Eingabe eines Kommentars im **Antwort hinzufügen ...** -Bereich, um auf einen vorhandenen Kommentar zu antworten, dann folgen Sie den Schritten 4 bis 8 oben. <!--(**************insure this stays accurate***********)--> Informationen zur Beantwortung einer Aktualisierung finden Sie unter [Antworten auf Aktualisierungen](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

1. (Bedingt und optional) Wenn andere Benutzer Kommentare hinzugefügt haben, die beim Hinzufügen Ihrer Kommentare außerhalb des sichtbaren Bereichs im Abschnitt Updates angezeigt werden, klicken Sie auf **Ansicht** in Blau **neues Kommentarbanner** unten auf dem Bildschirm, um diese Kommentare anzuzeigen.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Weitere Kommentare werden unten auf dem Bildschirm angezeigt.


   >[!NOTE]
   >
   >   Die Anzeige &quot;neue Kommentare&quot;und die Schaltfläche &quot;Anzeigen&quot;werden nur dann angezeigt, wenn sowohl die Benutzer, die die neuen Updates eingegeben haben, als auch der Benutzer, der sich derzeit den Abschnitt Updates ansieht, das neue Kommentierungserlebnis verwenden.

1. (Optional) Klicken Sie auf die **liken** icon![](assets/like-icon.png). Das Symbol wird mit der Anzahl der &quot;Gefällt mir&quot;-Klicks aktualisiert.
1. (Bedingt und optional) Wenn Sie Ihrem Kommentar weitere Personen hinzugefügt haben, klicken Sie auf die Anzahl der Mitglieder, die in der Aktualisierung enthalten sind, um eine Liste der Entitäten anzuzeigen, für die der Kommentar, den Sie eingegeben haben, freigegeben ist.

   ![](assets/members-icons-expanded-unshimmed.png)

   >[!TIP]
   >
   >Neben den Avataren werden die Namen der ersten beiden getaggten Entitäten angezeigt. Wenn mehr als zwei Entitäten mit Tags versehen sind, werden nur der Name des ersten und die Anzahl der zusätzlichen Entitäten angezeigt.

1. (Optional) Klicken Sie auf die **Systemaktivität** -Tab, um vom System protokollierte Aktualisierungen anzuzeigen. Wenn das Objekt oder seine untergeordneten Elemente aktualisiert werden, generiert Workfront einen Hinweis zu dieser Aktualisierung und zeigt sie auf der Registerkarte Systemaktivität an.

   Weitere Informationen finden Sie unter [Übersicht über den Aktualisierungsabschnitt](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >Sie können einem Systemupdate keinen Kommentar hinzufügen.

## Verwenden von Rich Text in einem Workfront-Update{#use-rich-text-in-a-workfront-update}

<!--October 2023: remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>Die folgenden Informationen beschreiben die Verwendung von Rich Text im neuen Kommentierungserlebnis, sofern nichts anderes angegeben ist.

Sie können Ihre Aktualisierungen durch Verwendung von Rich Text oder durch Hinzufügen verschiedener Elemente wie Emojis, Links oder Bilder verbessern.

1. Navigieren Sie zu **Updates** Bereich eines Workfront-Objekts erstellen und mit der Eingabe eines Kommentars beginnen.
1. (Optional) Um Ihrer Aktualisierung Rich-Text-Formatierung hinzuzufügen, verwenden Sie beliebige Attribute für die **Rich-Text** Symbolleiste bei der Eingabe.

   ![](assets/rich-text-toolbar.png)

   <!--October 2023: the individual icons in the toolbar will need replacing-->

   | **Attribut** | **Symbolleiste** | **Tastaturbefehle für Mac** | **Windows-Tastaturbefehle** |
   |---|---|---|---|
   | Fett | ![](assets/mceclip10.png) | η+b | Strg+B |
   | kursiv | ![mceclip9.png](assets/mceclip9.png) | Befehl+i | Strg+I |
   | Unterstreichen | ![mceclip8.png](assets/mceclip8.png) | η+u | Strg+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png) | <br>So öffnen Sie das Feld &quot;Links hinzufügen&quot;: ^+K</br> <br>So fügen Sie einen Link über den ausgewählten Text ein: SUMME+V</br> | <br>So öffnen Sie das Feld &quot;Links hinzufügen&quot;: Strg+K</br> <br>So fügen Sie einen Link über den ausgewählten Text ein: Strg+V</br> |
   | Aufzählung | ![mceclip6.png](assets/mceclip6.png) | η+Shift+8 | Strg+Umschalt+8 |
   | Nummerierte Liste | ![mceclip5.png](assets/mceclip5.png) | η+Shift+7 | Strg+Umschalt+7 |
   | Blockzitat | ![](assets/block-quote-icon-large.png) | η+Shift+9 | <br>Strg+Umschalt+9</br> <br>Dies ist im neuen Kommentierungserlebnis nicht verfügbar. </br> |

   <!--remove the last row when we remove legacy from the system-->

   Um die Textformatierung zu beenden, deaktivieren Sie das -Attribut auf der **Rich-Text** Symbolleiste.


   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* Die Formatierung wird auch in allen E-Mail-Benachrichtigungen angezeigt, die Benutzer mit Ihrer Aktualisierung erhalten.
   >* Die Rich-Text-Formatierung, die auf eine Aktualisierung in einer E-Mail angewendet wird, wird in der Aktualisierung nicht angezeigt, wenn sie auf der Registerkarte Aktualisierungen angezeigt wird.
   >* Wenn Ihr Unternehmen Workfront mit Internet Explorer verwendet, verliert jeder formatierte Text, der in eine Aktualisierung eingefügt wird, seine Rich-Text-Formatierung und wird als Nur-Text angezeigt. Sie können den Text mithilfe der Attribute in der Rich-Text-Symbolleiste neu formatieren.
   >* Die Rich-Text-Formatierung ist nicht für Aktualisierungen verfügbar, die im Bereich &quot;Timesheets&quot;vorgenommen werden, oder für die Objekte &quot;Hinweis&quot;und &quot;Letzte Bedingung&quot;in einem Bericht.

1. (Optional und bedingt) Wenn Sie Text aus früheren Aktualisierungen oder aus anderen Quellen einbeziehen und von Ihrer eigenen Aktualisierung unterscheiden möchten, können Sie ihn als Blockzitat markieren. Klicken Sie auf **Blockierungsangebot** icon ![](assets/block-quote-small.png) und geben Sie den Text ein, den Sie zitieren möchten. Der zitierte Text wird mit einer vertikalen grauen Linie markiert. Klicken Sie auf **Blockierungsangebot** erneut ein, um zur normalen Formatierung zurückzukehren. Dies ist im neuen Kommentierungserlebnis nicht verfügbar.

   <!--remove this picture below and the bullet above when we remove legacy-->

   ![](assets/block-quote-marked-350x144.png)</span>

1. (Optional) Klicken Sie auf die **Emoji** icon ![](assets/emoji-icon.png) , um Emojis zu Ihrer Aktualisierung hinzuzufügen.

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
   1. Im **Rich-Text** Symbolleiste, klicken Sie auf **Hyperlink** icon ![](assets/link-icon.png).

   1. Im **Link erstellen** Feld, das unter **URL**, geben Sie die URL der Quelle ein oder fügen Sie sie ein.

   1. under **Anzuzeigender Text**, geben Sie den Link-Text ein oder fügen Sie ihn ein.
   1. Klicken Sie auf **Speichern**.

1. (Optional) <span class="preview">Um ein Bild an Ihre Aktualisierung anzuhängen, kopieren Sie einen Screenshot von Ihrem Computer und fügen Sie ihn dann in den Kommentar ein </span>

   Oder

   Klicken Sie auf **Bild hinzufügen** icon ![](assets/add-image-mountain-with-plus-icon.png) und navigieren Sie zum Bild auf Ihrem Computer.

   >[!NOTE]
   >
   >* Der Workfront-Administrator muss das Hinzufügen von Bildern im Abschnitt &quot;Voreinstellungen für Feeds aktualisieren&quot;der Workfront-Benutzeroberfläche aktivieren, bevor die Symbole Bild oder Anhang hinzufügen angezeigt werden. Weitere Informationen finden Sie unter [Voreinstellungen für Benutzeraktualisierungen konfigurieren](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* Die maximale Bilddateigröße beträgt 7 MB. Unterstützte Bilddateitypen sind .jpg, .gif und .png.
   >* Auf Bilder kann über den Abschnitt Updates eines Objekts zugegriffen werden. Sie sind auch im Bereich Dokumente unter dem Hauptmenü verfügbar.
   >* <span class="preview">Sie können das Bild einfügen, indem Sie mit der rechten Maustaste auf den neuen Kommentar klicken oder indem Sie Strg + V für Windows (oder CMD + V für Mac) auf Ihrer Tastatur drücken.</span>
   >* Sie können ein Update mit einem Bild und ohne Text senden.
   >* Wenn Sie einen Kommentar löschen, der ein Bild enthält, gibt es je nach ausgewähltem Erlebnis die folgenden Szenarien:
   >
   >     * Im bisherigen Kommentierungserlebnis bleibt das Bild im Bereich Dokumente, ist jedoch nicht mehr im Abschnitt Aktualisierungen sichtbar.
   >     * Im neuen Kommentarerlebnis wird das Bild sowohl aus dem Abschnitt Updates als auch aus dem Bereich Dokumente entfernt. Das Bild wird auch aus dem Bereich &quot;Dokumente&quot;gelöscht, wenn Sie einen Kommentar bearbeiten und das Bild löschen.
   >* Wenn jemand ein Bild löscht, das mit einem Kommentar verknüpft ist, wird es auch aus dem Kommentar entfernt.

   <!--remove the statement above about legacy, when we remove the legacy environment.-->

1. Klicks **Einsenden** , um Ihren Kommentar hinzuzufügen.

<div class="preview">

## Nach einer Aktualisierung suchen

>[!NOTE]
>
>Diese Funktion ist nur für die Registerkarte Kommentare im neuen Kommentar-Erlebnis verfügbar. Dies ist nicht für die Registerkarte Systemaktivität im Abschnitt Updates verfügbar.

Sie können nach einem Kommentar oder einer Antwort im Abschnitt Updates eines Objekts suchen.

1. Navigieren Sie zu **Updates** -Abschnitt eines Objekts.
1. Eingabe eines Suchbegriffs beginnen <!--or a user's name --> im **Suche** in der oberen rechten Ecke des **Kommentare** Registerkarte.

   <!--Add this tip when it'll be possible: You can search for users who have been tagged or for comment owners.-->

   ![](assets/search-field-in-updates-tab.png)

   Der Suchbegriff <!--or user--> Sie nach gesucht haben, wird hervorgehoben und die Kommentare, die sie enthalten, werden oben im Abschnitt Aktualisierungen angezeigt.

   Workfront durchsucht den gesamten Update-Stream des Objekts außerhalb der auf dem Bildschirm sichtbaren Kommentare.

1. Klicken Sie auf **x** im Suchfeld ein, um die Suchergebnisse zu löschen und zu allen Kommentaren zurückzukehren.

</div>

<!-- when we release search to production, check above and make sure you don't have to add that the users tagged/ owners are also searchable-->

## Aktualisierte Informationen kopieren

Es gibt mehrere Möglichkeiten, ein Update zu kopieren. Nachdem Sie einen Link kopiert haben, können Sie ihn für andere freigeben, um ihn zur Aktualisierung weiterzuleiten.

Das Kopieren eines Updates hängt davon ab, welches Kommentierungserlebnis Sie verwenden.

### Kopieren von Aktualisierungen im neuen Kommentierungserlebnis

Informationen darüber, welche Funktionen für das neue Kommentierungserlebnis verfügbar sind und welche Objekte verfügbar sind, finden Sie unter [Neues Kommentierungserlebnis](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--when we remove and deprecate the legacy stream, add screen shots in the sections below- October 2023-->

Sie können Informationen aus einem vorhandenen Kommentar kopieren, indem Sie einen der folgenden Schritte ausführen:

* [Link kopieren](#copy-link)
* [Fließtext kopieren](#copy-body-text)
* [Anführungsantwort](#quote-reply-1)

![](assets/copy-comment-ways-from-more-menu-on-comment.png)

#### Link kopieren

Die Option Link kopieren kopiert den Kommentar- oder Thread-Link in die Zwischenablage, damit Sie den Kommentar oder den gesamten Thread für andere Benutzer freigeben können.

1. Gehen Sie zu der Aktualisierung, deren Link Sie kopieren möchten.

1. Klicken Sie auf **Mehr** Menü und klicken Sie auf **Link kopieren**.

1. Fügen Sie den Link, den Sie im vorherigen Schritt kopiert haben, in eine E-Mail oder eine andere Anwendung ein, um ihn für andere freizugeben. Der freigegebene Link öffnet den Kommentar, von dem Sie den Link freigegeben haben.

   >[!TIP]
   >
   >Wenn Sie die Verknüpfung einer Konversation mit einem untergeordneten Objekt von einem übergeordneten Objekt freigeben, öffnet die Verknüpfung den Thread im Bereich Updates des übergeordneten Objekts.
   >
   >Wenn Sie beispielsweise den Link eines Aufgabenkommentars aus dem Bereich &quot;Aktualisierungen&quot;des Projekts kopieren, öffnet der Kommentar die Projektseite.

#### Fließtext kopieren

Mit der Option Textkörper kopieren wird der Text von einem bestimmten Update in die Zwischenablage kopiert.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf **Mehr** Menü und klicken Sie auf **Textkörper kopieren**.

#### Anführungsantwort

Mit der Option Antwort zitieren wird der ursprüngliche Kommentar als Blockanführungszeichen in eine neue Antwort kopiert.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf **Mehr** Menü und klicken Sie auf **Anführungsantwort**.

   Ein neues Kommentarfeld wird geöffnet und die zitierte Antwort wird in den neuen Kommentar aufgenommen und als Blockanführungszeichen markiert.

   ![](assets/block-quote-highlighted-mid-comment-before-submit.png)

   <!--ensure the screen shot above is correct - missing he block quote icon in rich text -->

1. Fügen Sie Ihre Aktualisierung weiter hinzu und klicken Sie auf **Einsenden** , um den Kommentar hinzuzufügen.

### Kopieren einer Aktualisierung im alten Kommentierungserlebnis

<!--remove legacy when removed from the UI-->

* [Aktualisieren kopieren](#copy-the-update)
* [Den Thread-Link kopieren](#copy-the-thread-link)
* [Aktualisierungslink kopieren](#copy-the-update-link)
* [Antwort zitieren](#quote-reply)

  >[!TIP]
  >
  >Wenn Sie den Link einer Konversation über ein untergeordnetes Objekt aus einem übergeordneten Objekt kopieren und freigeben, öffnet die Verknüpfung den Thread im Bereich &quot;Aktualisierungen&quot;des untergeordneten Objekts.
  >
  >Wenn Sie beispielsweise den Link eines Aufgabenkommentars aus dem Bereich &quot;Aktualisierungen&quot;des Projekts kopieren, öffnet der Kommentar die Aufgabenseite.

#### Aktualisieren kopieren {#copy-the-update}

Mit dieser Option wird der Text von einem bestimmten Update in die Zwischenablage kopiert.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf **Mehr** Menü und klicken Sie auf **Textkörper kopieren**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Den Thread-Link kopieren {#copy-the-thread-link}

Mit dieser Option wird der vollständige Thread-Link in die Zwischenablage kopiert, damit Sie den Thread für andere Benutzer freigeben können.

1. Gehen Sie zum Aktualisierungs-Thread, den Sie kopieren möchten.

1. Klicken Sie auf **Mehr** Menü und klicken Sie auf **Link zum Kopieren des Threads**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Fügen Sie den Link, den Sie im vorherigen Schritt kopiert haben, in eine E-Mail oder eine andere Anwendung ein, um ihn für andere freizugeben. Der freigegebene Link öffnet den Kommentar, von dem Sie den Link freigegeben haben.

#### Aktualisierungslink kopieren {#copy-the-update-link}

Mit dieser Option wird ein bestimmter Aktualisierungslink in die Zwischenablage kopiert. Wenn Sie den Aktualisierungslink freigeben, sieht der Benutzer, der darauf folgt, einen Rahmen um die Aktualisierung.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf **Mehr** Menü neben der einzelnen Aktualisierung und klicken Sie auf **Link zum Aktualisieren kopieren**.

   ![](assets/copy-update-link-old-ui.png)

1. Fügen Sie den Link, den Sie im vorherigen Schritt kopiert haben, in eine E-Mail oder eine andere Anwendung ein, um ihn für andere freizugeben. Der freigegebene Link öffnet den Kommentar, von dem Sie den Link freigegeben haben.

#### Antwort zitieren

Mit der Option Antwort zitieren wird der ursprüngliche Kommentar als Blockanführungszeichen in eine neue Antwort kopiert.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf **Mehr** Menü und klicken Sie auf **Antwort zitieren**.

   Ein neues Kommentarfeld wird geöffnet und die zitierte Antwort wird in den neuen Kommentar aufgenommen und als Blockanführungszeichen markiert.

1. Fügen Sie Ihre Aktualisierung weiter hinzu und klicken Sie auf **Antwort** , um den Kommentar hinzuzufügen.

## Aktualisieren oder Antworten löschen

Je nachdem, welchen Zugriff Ihr Workfront-Administrator Ihnen gewährt, können Sie möglicherweise Aktualisierungen löschen, die Sie auf der Registerkarte Updates eines Objekts hinzugefügt haben. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) im Artikel [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Kein Workfront-Benutzer (einschließlich Workfront-Administrator) kann Aktualisierungen löschen, die von einem anderen Benutzer vorgenommen wurden. Wenn die Zugriffsebene eines Benutzers es ihm jedoch ermöglicht, eigene Aktualisierungen zu löschen, kann sich der Workfront-Administrator als dieser Benutzer anmelden und die vorgenommenen Aktualisierungen löschen. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) und [Melden Sie sich als anderer Benutzer an](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Gehen Sie zu dem Update oder der Antwort, das/die Sie löschen möchten.
1. Klicken Sie auf **Mehr** neben der Aktualisierung oder Antwort, die Sie löschen möchten, klicken Sie auf **Löschen**. <!--October 2023 - replace screen shot here-->

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Klicken Sie in der angezeigten Nachricht auf **Löschen**.

   >[!NOTE]
   >
   >Wenn Sie eine Aktualisierung mit einem angehängten Bild löschen, werden sowohl der Kommentar als auch das Bild gelöscht. Weitere Informationen finden Sie unter [Verwenden von Rich Text in einem Workfront-Update](#use-rich-text-in-a-workfront-update) in diesem Artikel beschrieben.

   Wenn dem Kommentar, den Sie löschen, Antworten zugeordnet sind, gibt es einen Hinweis darauf, dass der Kommentar mit dem Namen des Benutzers entfernt wurde, der ihn entfernt hat.

   ![](assets/removed-comment-indicator-new-experience.png)

   Gelöschte Kommentare werden sofort aus Workfront entfernt. Ein Benutzer, der den Abschnitt Updates verwendet, sieht, dass ein Kommentar von einem anderen Benutzer in Echtzeit gelöscht wird.

   <!--when we remove the beta, take out the first part of the sentence above about only when commenting in beta experience. Leave the rest though-->

<!--this is no longer needed - adding timesheet comments is just like adding comments to any other object now

## Add an update on a Timesheet

1. Go to a Timesheet on which you want to make an update.
1. Click the Timesheet to open it.
1. At the bottom of the Timesheet, click **Include a comment**.
1. In the box that displays at the bottom of the Timesheet, type an update.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Conditional) To save your update without submitting the Timesheet for approval, click **Save for Later**.

   Or

   To save your update and submit the Timesheet for approval, click **Submit for Approval**.

   Or

   If your Timesheet is not set up with an approver, click **Save and Close Timesheet** to save your update.

-->



## Systemaktualisierungen aktivieren oder deaktivieren

<!--update this section when we remove legacy, to just point to the article in green below and rename this section as "Review system activity updates" or something-->

<!--October 2023: when the new stream goes to all objects production, consider updating this article also, to say there is no System Activity tab to be disabled for objects anymore: help\quicksilver\administration-and-setup\set-up-workfront\system-tracked-update-feeds\system-tracked-update-feeds.md-->

>[!NOTE]
>
>Es ist nicht möglich, Systemaktualisierungen zu deaktivieren, wenn die neue Kommentarfunktion verwendet wird.
>Die Informationen in diesem Abschnitt beziehen sich nur auf die Funktionalität, die im Abschnitt &quot;Legacy-Updates&quot;verfügbar ist. &lt;!—Entfernen Sie diesen Abschnitt, wenn wir Legacy aus dem System entfernen ->
>Weitere Informationen zu Systemaktualisierungen im neuen Kommentierungserlebnis finden Sie unter [Übersicht über den Aktualisierungsabschnitt](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

Im Abschnitt Updates für ein Workfront-Objekt werden zwei Arten von Informationen angezeigt:

* **Benutzeraktualisierungen:** Benutzeraktualisierungen sind Kommentare, die Sie und andere Benutzer in Ihrem System eingeben. <!--October 2023 - new screen shot -->

  ![](assets/user-update-cl-350x277.png)

* **Systemaktualisierungen:** Das System aktualisiert den Datensatz zum Entfernen von Assets, zum Hinzufügen oder Löschen von Versionen, zum Anhängen oder Entfernen einer Genehmigungsanfrage sowie alle Änderungen oder Änderungen, die an den Dokumenten am Objekt vorgenommen wurden. <!--October 2023 - new screen shot -->

  ![](assets/system-updates-cl-350x277.png)

  Abhängig von Ihrer Workfront-Lizenz sind Systemaktualisierungen möglicherweise standardmäßig aktiviert. Workfront-Administratoren können bestimmen, was in Systemaktualisierungen verfolgt wird, wie unter [Vom System getrackte Aktualisierungen](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). Sie können auch Systemaktualisierungen oder Aktivitäten herausfiltern, sodass nur Benutzeraktualisierungen für alle Objekte angezeigt werden.

  Die folgenden Objekte verfügen nicht über systemgenerierte Aktualisierungen:

   * Team
   * Vorlage
   * Vorlagenaufgabe

So aktivieren oder deaktivieren Sie Systemaktualisierungen:

1. Klicken Sie auf **Updates** -Registerkarte auf einem Objekt.
1. Klicks **Systemaktualisierungen anzeigen** zum Schieben des Switches nach links (deaktiviert) oder rechts (aktiviert).

   ![](assets/show-system-updates-qs-350x55.png)

   Diese Option ist für alle Objekte in Workfront persistent und bleibt an der von Ihnen ausgewählten Position, auch wenn Sie sich von Workfront abmelden.

   >[!TIP]
   >
   >   Objekte, die keine Systemaktualisierungen aufzeichnen, haben nicht die Option Systemaktualisierungen anzeigen in ihrem Aktualisierungsbereich.

   <!--when Anna adds the new updates stream to ALL objects, she will remove the System Activity tab from the objects that don't record system updates - add another line to the TIP above to say: The System Activity tab is not available for objects that don't record system-generated updates.*************** OR: maybe make this part of the statement where we list which objects these are, above???  -->


