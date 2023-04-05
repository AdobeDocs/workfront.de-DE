---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Update der Arbeit
description: Sie können ein Update für ein Adobe Workfront-Objekt (Projekt, Aufgabe oder Problem) hinzufügen, um über den Fortschritt des Objekts zu kommunizieren. Benutzer, die dem Objekt zugewiesen sind oder es abonniert haben, können Ihre Aktualisierung anzeigen. Sie können Benutzer auch mit Tags versehen, um sie auf die Aktualisierung aufmerksam zu machen.
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 92fb1ee0b641d2f4b527e17df272e4c37c0feaef
workflow-type: tm+mt
source-wordcount: '2732'
ht-degree: 1%

---

# Update der Arbeit

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

>[!NOTE]
>
>Die Kommentarerfahrung in Adobe Workfront wird derzeit umgestaltet.
>Weitere Informationen zum neuen Aktualisierungserlebnis finden Sie unter [Neues Kommentierungserlebnis](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).
>
>Sie können auf das neue Design für die folgenden Objekte zugreifen:
> * Probleme beim Aktivieren der Beta-Kommentarfunktion.
   >
   >     Diese Funktion ist nur für den Abschnitt Aktualisierungen von Problemen verfügbar und nicht für die folgenden Bereiche:
   >
   >     * Startseite
   >     * Zusammenfassungsbereich in Listen
   >     * Zusammenfassungsbereich in Timesheets
>
> * Ziele

   >
   >   Das neue Kommentarerlebnis ist die Standardeinstellung für Ziele. Sie benötigen eine zusätzliche Lizenz für den Zugriff auf Workfront Goals. Weitere Informationen finden Sie unter [Anforderungen für die Verwendung von Workfront-Zielen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    Informationen zur Kommentarkommentierung zu Zielen finden Sie unter [Verwalten von Zielkommentaren in Adobe Workfront-Zielen](../../workfront-goals/goal-management/manage-goal-comments.md).


Sie können den meisten Objekten in Adobe Workfront im Abschnitt Updates Kommentare hinzufügen. Weitere Informationen dazu, welche Objekte den Abschnitt Aktualisierungen anzeigen, finden Sie unter [Übersicht über den Aktualisierungsabschnitt](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

Sie können ein Workfront-Objekt (Projekt, Aufgabe oder Problem) aktualisieren, um über den Fortschritt des Objekts zu kommunizieren, während Sie Kommentare zum Objekt abgeben. Benutzer, die dem Objekt zugewiesen sind oder es abonniert haben, können Ihre Aktualisierung anzeigen. Sie können Benutzer auch mit Tags versehen, um sie auf die Aktualisierung aufmerksam zu machen. Mit Tags versehene Benutzer erhalten eine In-App-Benachrichtigung und eine E-Mail über Ihre Aktualisierung.

Die Informationen auf dieser Seite beschreiben, wie Sie Kommentare zu Workfront-Objekten erstellen können und wie Sie Projekte, Aufgaben und Probleme aktualisieren. Informationen zur Kommentarkommentierung zu Zielen finden Sie unter [Verwalten von Zielkommentaren in Adobe Workfront-Zielen](../../workfront-goals/goal-management/manage-goal-comments.md). Sie benötigen eine zusätzliche Lizenz für den Zugriff auf Workfront Goals.


Sie können Projekte, Aufgaben und Probleme in den folgenden Bereichen von Workfront aktualisieren:

* Von einem Workfront-Objekt im Abschnitt Updates
* Im Startbereich (für Aufgaben und Probleme)
* Im Bereich &quot;Zusammenfassung&quot;in einer Liste von Objekten (für Aufgaben und Probleme)
* Aus dem Timesheet (für Aufgaben und Probleme)

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
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Anfrage oder höher für Probleme und Dokumente; Überprüfen oder höher für alle anderen Objekte</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Anzeigen oder Bearbeiten des Zugriffs für das Objekt, auf dem die Aktualisierung ausgeführt wird</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf das Objekt anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Hinzufügen einer Aktualisierung zu einem Arbeitselement

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects -->

Das Hinzufügen eines Updates zu einem Arbeitselement hängt von der Version des Abschnitts Updates und dem ausgewählten Objekt ab.

### Hinzufügen eines Updates zu einem Arbeitselement im Abschnitt &quot;Aktuelle Updates&quot;

>[!NOTE]
>
>Die folgende Funktion ist für alle Objekte mit Ausnahme von Zielen verfügbar. Sie benötigen eine zusätzliche Lizenz für den Zugriff auf Workfront Goals. Informationen zur Kommentarkommentierung zu Zielen finden Sie unter [Verwalten von Zielkommentaren in Adobe Workfront-Zielen](../../workfront-goals/goal-management/manage-goal-comments.md)

1. Gehen Sie zu dem Arbeitselement, für das Sie eine Aktualisierung bereitstellen möchten (z. B. ein Projekt, eine Aufgabe oder ein Problem).
1. Klicken Sie auf **Updates** Abschnitt.
1. Klicken **Neue Aktualisierung starten,** Geben Sie dann Ihr Update ein.
1. (Optional) Verwenden Sie Rich Text oder fügen Sie Emojis, Links oder Bilder zu Ihrer Aktualisierung hinzu, um Ihre Inhalte zu verbessern. Weitere Informationen finden Sie im Abschnitt &quot;Verwenden von Rich Text in einem Workfront-Update&quot;in diesem Artikel
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
      <td>Klicken Sie auf den Pfeil neben dem aktuellen Status und wählen Sie dann im Dropdown-Menü den gewünschten Status aus. Informationen zum Festlegen eines Status finden Sie unter <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Aktualisierung des Aufgabenstatus</a>.<p>Beim Aktualisieren des Status eines Arbeitselements wird der Status eines Projekts nicht automatisch geändert. Je nachdem, wie Ihr Projekt eingerichtet ist, müssen Sie möglicherweise den Projektstatus separat aktualisieren. Weitere Informationen zu den verschiedenen Aktualisierungstypen finden Sie unter <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Wählen Sie den Projektaktualisierungstyp aus </a>.</p><p><b>NOTIZ</b>

   Sie können den Status eines Arbeitselements nicht ändern, während es sich im Status Ausstehende Genehmigung befindet.</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Abschlussleiste</strong></td> 
      <td>(Nur für Aufgaben verfügbar) Geben Sie den Prozentsatz der abgeschlossenen Arbeiten an, indem Sie den Fortschrittsbalken auf den gewünschten Prozentsatz verschieben. Sie können auch auf die Abschlussleiste doppelklicken und die Prozentangabe eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Vertraulich für meine Firma</strong></td> 
      <td> <p>Deaktivieren Sie diese Option, um zu verhindern, dass Benutzer außerhalb Ihres Unternehmens Zugriff auf diese Aktualisierung haben.</p> 
      <p><b>NOTIZ</b></p>
      <p>Diese Option wird nur angezeigt, wenn der Benutzer mit einem Unternehmen verknüpft ist.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Aktualisieren** , um die Aktualisierung zum Workfront-Objekt hinzuzufügen.

   >[!NOTE]
   >
   >Nach dem Klicken auf wird ein kleines Popup-Fenster für sieben Sekunden angezeigt **Aktualisieren**, sodass Sie die Aktualisierung rückgängig machen und zum Bearbeitungsbereich zurückkehren können, bevor die Aktualisierung veröffentlicht wird. Das Update wird veröffentlicht, wenn Sie das Popup &quot;Rückgängig&quot;schließen, warten, bis es ausgeblendet wird, oder von der Seite weg navigieren.
   >
   >Wenn Ihr Workfront-Administrator in Ihrer Zugriffsebene die Einstellung &quot;Benutzer dürfen Kommentare nie löschen&quot;auswählt, können Sie einen Kommentar nicht rückgängig machen. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen und ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. Informationen zum Antworten auf eine Aktualisierung finden Sie unter [Antworten auf Aktualisierungen](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

### Hinzufügen einer Aktualisierung zu einem Arbeitselement mithilfe des Beta-Kommentarerlebnisses

1. Suchen Sie das Objekt, das Sie aktualisieren möchten, und klicken Sie dann auf seinen Namen, um die Seite des Objekts zu öffnen.
1. Klicken  **Updates** im linken Bereich.
1. Aktivieren Sie die **Kommentieren von Beta** in der oberen rechten Ecke des Bereichs Updates ein- und klicken Sie dann auf **Zustimmen** zur Beta-Vereinbarung. Dadurch wird der Bereich Updates auf das Beta-Kommentarerlebnis umgestellt.
Die **Kommentare** ist standardmäßig ausgewählt.
1. Beginnen Sie mit der Eingabe eines Kommentars im **Neuer Kommentar** ankreuzen.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Wenn Sie den Abschnitt Updates verlassen, bevor Sie mit der Eingabe und dem Senden eines Kommentars fertig sind, bleibt der Kommentar auf der Seite im Entwurfsmodus, auch wenn Sie sich abmelden und wieder anmelden. Entworfene Kommentare sind nur für den Benutzer sichtbar, der sie eingibt.

1. (Optional) Im **Personen oder Teams taggen** eingeben, den Namen oder die E-Mail-Adresse eines Benutzers oder eines Teams eingeben, das Sie in diesen Kommentar aufnehmen möchten, und ihn dann auswählen, wenn er in der Liste angezeigt wird.
1. (Optional) Um Ihrer Aktualisierung Rich-Text-Formatierung hinzuzufügen, verwenden Sie eine der folgenden Optionen aus dem **Rich-Text** Symbolleiste zum Erweitern des Textes:

   * Fett
   * kursiv
   * Unterstreichen
   * Verknüpfung
   * Aufzählung
   * Nummerierte Liste
   * Anlage hinzufügen <!--(mark this parenthesis as draft: ************ this might be renamed to "Add image")-->

   Weitere Informationen finden Sie im Abschnitt &quot;Verwenden von Rich Text in einem Workfront-Update&quot;in diesem Artikel. <!--remove this list, above, when we get to parity for Rich Text-->

   >[!TIP]
   >
   >Wenn ein anderer Benutzer einen Kommentar für dasselbe Element sendet, das Sie aktualisieren, wird eine rote Zeile mit der Anzeige &quot;Neu&quot;angezeigt, die Sie über die neueren Kommentare informiert.
   >
   >Der Indikator wird nur angezeigt, nachdem der Kommentar zum Element gesendet wurde, nicht aber, wenn der Kommentar noch erstellt wurde.
   >
   >Der Indikator &quot;Neu&quot;wird nur angezeigt, wenn sowohl der Benutzer, der ein neues Update eingegeben hat, als auch der Benutzer, der derzeit ein Update aufruft, das neue Kommentarerlebnis verwenden.
   >![](assets/real-time-new-red-indicator-unified-commenting.png)


1. Klicken **Einsenden** , um die Aktualisierung zum Workfront-Objekt hinzuzufügen.
1. (Optional) Um einen Kommentar zu bearbeiten, klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Symbol &quot;Gefällt mir&quot;und klicken Sie dann auf **Bearbeiten**.
1. Informationen im Kommentar bearbeiten <!--or remove any of the tagged users-->.
Sie können Ihren Kommentar innerhalb von 15 Jahren nach seiner Übermittlung bearbeiten. Links neben dem Datumsstempel, der beim Aktualisieren des Kommentars angezeigt wird, wird die Anzeige &quot;Bearbeitet&quot;hinzugefügt.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   Es wird eine E-Mail erzeugt, um die Benutzer nur dann über Ihre Aktualisierung zu informieren, wenn Sie die ursprüngliche Aktualisierung übermitteln. Nach Bearbeitung des Updates wird keine E-Mail erzeugt.

1. (Optional) Klicken Sie auf **Antwort** um auf einen vorhandenen Kommentar zu antworten, führen Sie dann die Schritte 4 bis 7 aus. <!--(**************insure this stays accurate***********)-->. Informationen zur Beantwortung einer Aktualisierung finden Sie unter [Antworten auf Aktualisierungen](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. (Optional) Klicken Sie auf die **liken** icon![](assets/like-icon.png). Das Symbol wird mit der Anzahl der &quot;Gefällt mir&quot;-Klicks aktualisiert.
1. (Bedingt und Optional) Wenn Sie Ihrem Kommentar weitere Personen hinzugefügt haben, klicken Sie auf die Anzahl der Mitglieder, die in der Aktualisierung enthalten sind, um eine Liste der Entitäten anzuzeigen, für die der Kommentar, den Sie eingegeben haben, freigegeben ist.

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Optional) Klicken Sie auf die **Systemaktivität** -Tab, um vom System protokollierte Aktualisierungen anzuzeigen. Wenn das Objekt oder seine untergeordneten Elemente aktualisiert werden, generiert Workfront einen Hinweis zu dieser Aktualisierung und zeigt sie auf der Registerkarte Systemaktivität an.

   Weitere Informationen finden Sie unter [Übersicht über den Aktualisierungsabschnitt](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >Sie können einem Systemupdate keinen Kommentar hinzufügen.


## Verwenden von Rich Text in einem Workfront-Update

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>Einige der Optionen in der Rich-Text-Symbolleiste sind möglicherweise nicht für das Beta-Kommentar-Erlebnis verfügbar.

Sie können Ihre Aktualisierungen durch Verwendung von Rich Text oder durch Hinzufügen verschiedener Elemente wie Emojis, Links oder Bilder verbessern.

1. Geben Sie im Bereich Updates einen Kommentar ein.
1. (Optional) Um Ihrer Aktualisierung Rich-Text-Formatierung hinzuzufügen, verwenden Sie beliebige Attribute im **Rich-Text** Symbolleiste bei der Eingabe.

   | **Attribut** | **Schaltfläche &quot;Symbolleiste&quot;** | **Mac-Tastaturbefehle** | **PC-Tastaturbefehle** |
   |---|---|---|---|
   | Fett | ![mceclip10.png](assets/mceclip10.png) | η+b | Strg+B |
   | kursiv | ![mceclip9.png](assets/mceclip9.png) | Befehl+i | Strg+I |
   | Unterstreichen | ![mceclip8.png](assets/mceclip8.png) | η+u | Strg+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png) | ⌘+K | Strg+K |
   | Aufzählung | ![mceclip6.png](assets/mceclip6.png) | η+Shift+8 | Strg+Umschalt+8 |
   | Nummerierte Liste | ![mceclip5.png](assets/mceclip5.png) | η+Shift+7 | Strg+Umschalt+7 |
   | Blockzitat | ![](assets/block-quote-icon-large.png) | η+Shift+9 | Strg+Umschalt+9 |

   Um die Textformatierung zu beenden, deaktivieren Sie das -Attribut auf der **Rich-Text** Symbolleiste.

   >[!NOTE]
   >
   >* Die Formatierung wird auch in allen E-Mail-Benachrichtigungen angezeigt, die Benutzer mit Ihrer Aktualisierung erhalten.
   >* Die Rich-Text-Formatierung, die auf eine Aktualisierung in einer E-Mail angewendet wird, wird in der Aktualisierung nicht angezeigt, wenn sie auf der Registerkarte Aktualisierungen angezeigt wird.
   >* Wenn Ihr Unternehmen Workfront mit Internet Explorer verwendet, verliert jeder formatierte Text, der in eine Aktualisierung eingefügt wird, seine Rich-Text-Formatierung und wird als Nur-Text angezeigt. Sie können den Text mithilfe der Attribute in der Rich-Text-Symbolleiste neu formatieren.
   >* Die Rich-Text-Formatierung ist nicht für Aktualisierungen verfügbar, die im Bereich &quot;Timesheets&quot;vorgenommen werden, oder für die Objekte &quot;Hinweis&quot;und &quot;Letzte Bedingung&quot;in einem Bericht.


1. (Optional) Wenn Sie Text aus früheren Aktualisierungen oder aus anderen Quellen einbeziehen und von Ihrer eigenen Aktualisierung unterscheiden möchten, können Sie ihn als Blockzitat markieren. Klicken Sie auf **Blockierungsangebot** icon ![](assets/block-quote-small.png) und geben Sie den Text ein, den Sie zitieren möchten. Der zitierte Text wird mit einer vertikalen grauen Linie markiert. Klicken Sie auf **Blockierungsangebot** erneut ein, um zur normalen Formatierung zurückzukehren.

   ![](assets/block-quote-marked-350x144.png)

1. (Optional) Fügen Sie Ihrem Update Emojis hinzu.

   >[!NOTE]
   >
   >* Workfront ersetzt keine Interpunktions-Emoticons wie :) durch Emojis.
   >* Emojis ist nicht für Aktualisierungen verfügbar, die im Bereich &quot;Timesheets&quot;vorgenommen werden, oder für die Objekte &quot;Hinweis&quot;und &quot;Letzte Bedingung&quot;in einem Bericht.
   >* Die Emoji-Funktion in Workfront verwendet Unicode-Zeichen und wird daher nur auf Browsern und Betriebssystemen angezeigt, die Unicode-Codepunkte unterstützen. Benutzer auf einer Plattform, einem Browser oder einer Betriebssystemversion, die nicht Ihre ist, haben möglicherweise keinen Zugriff auf dieselben Emojis.
   >* Ein nicht unterstütztes Emoji wird durch eine schwarze oder weiße Box dargestellt.
   >* Windows 7 unterstützt nur Schwarzweiß-Emojis.
   >* Emojis, die auf eine per E-Mail vorgenommene Aktualisierung angewendet werden, werden nicht in der Aktualisierung angezeigt, wenn sie im Bereich Updates angezeigt werden.


1. (Optional) So fügen Sie einen URL-Link zu zusätzlichen Informationsquellen hinzu:

   1. Klicken Sie in der Aktualisierung auf die Stelle, an der Sie einen Link einfügen möchten.
   1. Im **Rich-Text** Symbolleiste, klicken Sie auf **Hyperlink** Symbol. ![](assets/link-icon.png)

   1. Im **Link erstellen** Feld, das angezeigt wird, unter **URL**, geben Sie die URL der Quelle ein oder fügen Sie sie ein.

   1. under **Anzuzeigender Text**, geben Sie den Link-Text ein oder fügen Sie ihn ein.
   1. Klicken Sie auf **Speichern**.

1. (Optional) Klicken Sie auf die Schaltfläche **Bild** icon ![](assets/addimageicon-35x32.png) und navigieren Sie zum Bild auf Ihrem Computer.\
   Oder\
   Ziehen Sie das Bild in den Aktualisierungsbereich.

   >[!NOTE]
   >
   >* Ihr Workfront-Administrator muss das Hinzufügen von Bildern aktivieren, bevor das Bildsymbol angezeigt wird.
   >* Die maximale Bilddateigröße beträgt 7 MB. Unterstützte Bilddateitypen sind .jpg, .gif und .png.
   >* Auf Bilder kann nur über die Registerkarte Aktualisierungen eines Objekts zugegriffen werden. Sie sind nicht auf der Registerkarte Dokumente verfügbar.
   >* Sie können ein Update mit einem Bild und ohne Text senden.

1. Klicken **Aktualisieren**  oder **Einsenden**, wenn Sie das Beta-Kommentarerlebnis verwenden.


## Aktualisierte Informationen kopieren

<!--drafted for beta release toggle - remove when copying an update will be available:

>[!NOTE]
>
>Copying an update is not possible when using the Beta commenting experience.
-->

Es gibt mehrere Möglichkeiten, ein Update zu kopieren. Nachdem Sie einen Link kopiert haben, können Sie ihn für andere freigeben, um ihn zur Aktualisierung weiterzuleiten.

* [Aktualisieren kopieren](#copy-the-update)
* [Den Thread-Link kopieren](#copy-the-thread-link)
* [Aktualisierungslink kopieren](#copy-the-update-link)

### Aktualisieren kopieren {#copy-the-update}

Mit dieser Option wird der Text von einem bestimmten Update in die Zwischenablage kopiert.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf **Mehr** Menü und klicken Sie auf **Textkörper kopieren**.

   ![Textkörper kopieren](assets/update-stream-copy-body-text-350x152.png)

### Den Thread-Link kopieren {#copy-the-thread-link}

Mit dieser Option wird der vollständige Thread-Link in die Zwischenablage kopiert, damit Sie den Thread für andere Benutzer freigeben können.

1. Gehen Sie zum Aktualisierungs-Thread, den Sie kopieren möchten.

1. Klicken Sie auf **Mehr** Menü und klicken Sie auf **Link zum Kopieren des Threads** oder **Link kopieren**, wenn Sie das Beta-Erlebnis verwenden.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### Aktualisierungslink kopieren {#copy-the-update-link}

Mit dieser Option wird ein bestimmter Aktualisierungslink in die Zwischenablage kopiert. Wenn Sie den Aktualisierungslink freigeben, sieht der Benutzer, der darauf folgt, einen Rahmen um die Aktualisierung.

1. Gehen Sie zu der Aktualisierung oder Antwort, die Sie kopieren möchten.
1. Klicken Sie auf **Mehr** Menü neben der einzelnen Aktualisierung und klicken Sie auf **Link zum Aktualisieren kopieren** oder **Link kopieren**, wenn Sie das Beta-Erlebnis verwenden.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## Aktualisieren oder Antworten löschen

Je nachdem, welchen Zugriff Ihr Workfront-Administrator Ihnen gewährt, können Sie möglicherweise Aktualisierungen löschen, die Sie auf der Registerkarte Updates eines Objekts hinzugefügt haben. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) im Artikel [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Kein Workfront-Benutzer (einschließlich Workfront-Administrator) kann Aktualisierungen löschen, die von einem anderen Benutzer vorgenommen wurden. Wenn die Zugriffsebene eines Benutzers es ihm jedoch ermöglicht, eigene Aktualisierungen zu löschen, kann sich der Workfront-Administrator als dieser Benutzer anmelden und die vorgenommenen Aktualisierungen löschen. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) und [Anmelden als anderer Benutzer](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. Gehen Sie zu dem Update oder der Antwort, das/die Sie löschen möchten.
1. Klicken Sie auf **Mehr** neben der Aktualisierung oder Antwort, die Sie löschen möchten, klicken Sie auf **Löschen**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. Klicken Sie in der angezeigten Nachricht auf **Bestätigen** oder **Löschen**, wenn Sie das Beta-Kommentarerlebnis verwenden.

>[!NOTE]
>
>Wenn Sie eine Aktualisierung mit einem angehängten Bild löschen, werden sowohl der Kommentar als auch das Bild gelöscht.

## Hinzufügen eines Updates zu einem Timesheet

1. Gehen Sie zu einem Timesheet, auf dem Sie eine Aktualisierung vornehmen möchten.
1. Klicken Sie auf das Datenblatt, um es zu öffnen.
1. Klicken Sie unten im Timesheet auf **Kommentar einschließen**.
1. Geben Sie in das Feld am unteren Rand des Datenblatts ein Update ein.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Bedingt) Um Ihre Aktualisierung zu speichern, ohne das Datenblatt zur Genehmigung zu senden, klicken Sie auf **Später speichern**.

   Oder

   Klicken Sie auf , um die Aktualisierung zu speichern und das Datenblatt zur Validierung zu senden. **Zur Genehmigung einreichen**.

   Oder

   Wenn Ihr Timesheet nicht mit einem Genehmiger eingerichtet ist, klicken Sie auf **Datenblatt speichern und schließen** , um Ihre Aktualisierung zu speichern.

## Systemaktualisierungen aktivieren oder deaktivieren

<!--remove the preview tag with 23.2 production, but keep the note till we remove Beta and it becomed the only exprience: -->

>[!NOTE]
>
>Es ist nicht möglich, Systemaktualisierungen zu deaktivieren, wenn die Beta-Kommentarfunktion verwendet wird.
>Die Informationen in diesem Abschnitt beziehen sich nur auf die Funktionalität, die im aktuellen Abschnitt &quot;Aktualisierungen&quot;verfügbar ist.
>Weitere Informationen zu Systemaktualisierungen in der Beta-Version finden Sie unter [Übersicht über den Aktualisierungsabschnitt](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


Im Abschnitt Updates für ein Workfront-Objekt werden zwei Arten von Informationen angezeigt:

* **Benutzeraktualisierungen:** Benutzeraktualisierungen sind Kommentare, die Sie und andere Benutzer in Ihrem System eingeben.

   ![](assets/user-update-cl-350x277.png)

* **Systemaktualisierungen:** Das System aktualisiert den Datensatz zum Entfernen von Assets, zum Hinzufügen oder Löschen von Versionen, zum Anhängen oder Entfernen einer Genehmigungsanfrage sowie alle Änderungen oder Änderungen, die an den Dokumenten am Objekt vorgenommen wurden.

   ![](assets/system-updates-cl-350x277.png)

Abhängig von Ihrer Workfront-Lizenz sind Systemaktualisierungen möglicherweise standardmäßig aktiviert. Workfront-Administratoren können bestimmen, was in Systemaktualisierungen verfolgt wird, wie unter [Vom System verfolgte Aktualisierungen](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). Sie können auch Systemaktualisierungen oder Aktivitäten herausfiltern, sodass nur Benutzeraktualisierungen für alle Objekte angezeigt werden.

Weitere Informationen zum Unterschied zwischen Benutzer- und Systemaktualisierungen finden Sie unter [Vom System verfolgte Aktualisierungen](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

So aktivieren oder deaktivieren Sie Systemaktualisierungen:

1. Klicken Sie auf **Updates** auf einem Objekt.
1. Klicken **Systemaktualisierungen anzeigen** um den Switch nach links (deaktiviert) oder rechts (aktiviert) zu schieben.

   ![](assets/show-system-updates-qs-350x55.png)

   Diese Option ist für alle Objekte in Workfront persistent und bleibt an der von Ihnen ausgewählten Position, auch wenn Sie sich von Workfront abmelden.

