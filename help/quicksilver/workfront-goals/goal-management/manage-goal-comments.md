---
product-previous: workfront-goals
navigation-topic: goal-management
title: Verwalten von Zielkommentaren in Adobe Workfront-Zielen
description: Sie können allen Zielen, die Sie in Adobe Workfront-Zielen anzeigen können, Kommentare hinzufügen.
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 52e8ce6dd5146d72f698583b531b3db6bc5dbf25
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 0%

---

# Verwalten von Zielkommentaren in Adobe Workfront-Zielen

<!--Audited: 01/2024-->

<!--consider retiring this article when goals and all objects are in parity and we remove the legacy commenting from the system. From then on, there is just ONE way to comment and that will be documented in the Update Work article-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

Sie können allen Zielen, die Sie in Adobe Workfront-Zielen anzeigen können, Kommentare hinzufügen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> 
   <p>Für den neuen Plan und die Lizenzstruktur:
  <ul><li>Ein ultimativer Plan </li>
  Oder
  <li>Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. </li></ul> </p>
<p>Für den aktuellen Plan und die Lizenzstruktur: 
<ul><li> A Pro oder höher </li>
  <li>Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz</td>
 <td>
 <p>Alle</td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderung: Wenn Sie über das Select- oder Prime Adobe Workfront-Abonnement verfügen, müssen Sie auch eine zusätzliche Adobe Workfront Goals-Lizenz erwerben. Workfront-Ziele sind im Ultimate Workfront-Plan enthalten.</p>
 Oder
 <p>Aktuelle Produktanforderung: Sie müssen eine zusätzliche Lizenz für die in diesem Artikel beschriebene Funktion "Adobe Workfront Goals for Access"erwerben. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Konfiguration der Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele anzeigen oder höher</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen oder Höhere Berechtigungen für das Ziel</p>
  <p>Standardmäßig erhalten Benutzer keinen Zugriff auf Ziele </p>
 <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Verwalten von Zielkommentaren

Sie können Ziele im Abschnitt &quot;Aktualisierungen&quot;auf der Seite eines Ziels mit Kommentaren versehen.

Sie können auf einen Kommentar antworten oder einen Kommentar erhalten, den Sie oder andere in diesem Bereich hinzugefügt haben.

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts oder, falls verfügbar, auf das Symbol **Hauptmenü** oben links, das Symbol ![](assets/lines-main-menu.png) und klicken Sie dann auf **Ziele**.
![](assets/main-menu-icon.png)
Dadurch wird die Zielliste geöffnet.
1. Suchen Sie das Ziel, dem Sie Kommentare hinzufügen möchten, und klicken Sie dann auf seinen Namen, um die Zielseite zu öffnen.
1. Klicken Sie im linken Bereich auf **Aktualisierungen** .
1. (Optional) Um einen vorhandenen Kommentar zu finden, geben Sie in das Feld **Suche** oben rechts auf der Registerkarte **Kommentare** den Suchbegriff <!--or a user's name--> ein.

   ![](assets/search-field-in-updates-tab-goals.png)

   Das Keyword <!--or user-->, nach dem Sie gesucht haben, wird hervorgehoben und die Kommentare, die es enthalten, werden oben im Abschnitt Updates angezeigt.

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >Sie müssen nach einem Wort suchen, das in einem Kommentar oder einer Antwort enthalten ist. Sie können nicht nach einem getaggten Benutzer oder Team suchen.

   Weitere Informationen finden Sie unter [Funktionsweise aktualisieren](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. Klicken Sie im Suchfeld auf das Symbol **x** , um die Suchergebnisse zu löschen und zur vollständigen Aktualisierung zurückzukehren.
1. Klicken Sie in der oberen linken Ecke des Bereichs Updates auf die Registerkarte **Kommentare** .
1. Geben Sie einen Kommentar in das Feld **Neuer Kommentar** ein.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Wenn Sie den Abschnitt Updates verlassen, bevor Sie mit der Eingabe und dem Senden eines Kommentars fertig sind, bleibt der Kommentar auf der Seite im Entwurfsmodus, auch wenn Sie sich abmelden und wieder anmelden. Entwürfe werden sieben Tage lang gespeichert und können nicht wiederhergestellt werden. Entworfene Kommentare sind nur für den Benutzer sichtbar, der sie eingibt.

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um eine Änderung rückgängig zu machen oder wiederherzustellen:
   * STRG + Z ( ⌘ + z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Y ( ⌘ + y für Mac) zum Wiederholen einer Änderung
1. (Optional) Um Ihrem Update, einem Hyperlink oder einem Emoji Rich-Text-Format hinzuzufügen, verwenden Sie alle Optionen in der Rich-Text-Symbolleiste oder die zugehörigen Symbole. Weitere Informationen finden Sie unter [Funktionsweise aktualisieren](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Beginnen Sie im Bereich **Personen oder Teams taggen** mit der Eingabe des Namens oder der E-Mail eines Benutzers oder eines Teams, das Sie in diesen Kommentar aufnehmen möchten, und wählen Sie ihn dann aus, wenn er in der Liste angezeigt wird.
1. Wählen Sie den Umschalter **Für mein Unternehmen privat** aus, um den Kommentar nur für Personen in Ihrem Unternehmen sichtbar zu machen.

   >[!TIP]
   >
   >Sie müssen ein Unternehmen in Ihrem Profil angeben, damit diese Option im Bereich Updates verfügbar ist.

1. Klicken Sie auf **Senden**.

   >[!TIP]
   >
   >Wenn ein anderer Benutzer einen Kommentar für dasselbe Element sendet, das Sie aktualisieren, wird eine rote Zeile mit der Anzeige &quot;Neu&quot;angezeigt, um Sie über die neueren Kommentare zu informieren, sowie eine blaue Benachrichtigung am unteren Rand des Bildschirms, die die Anzahl der neuen Kommentare angibt.
   >
   >Der Indikator wird nur angezeigt, nachdem der Kommentar zum Element gesendet wurde, nicht aber, wenn der Kommentar noch erstellt wurde.
   >![](assets/real-time-new-red-indicator-unified-commenting-copy.png)

1. (Optional) Klicken Sie zum Bearbeiten eines Kommentars auf das Menü **Mehr** Menü ![](assets/more-icon.png) rechts neben dem Symbol &quot;Gefällt mir&quot;und klicken Sie dann auf **Bearbeiten**.
1. Bearbeiten Sie die Informationen im Kommentar oder entfernen Sie einen der getaggten Benutzer.
Sie können Ihren Kommentar innerhalb von 15 Minuten nach seiner Übermittlung bearbeiten. Links neben dem Datumsstempel, der beim Aktualisieren des Kommentars angezeigt wird, wird ein Indikator &quot;bearbeitet&quot;hinzugefügt.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * Es wird eine E-Mail erzeugt, um die Benutzer nur dann über Ihre Aktualisierung zu informieren, wenn Sie die ursprüngliche Aktualisierung übermitteln. Nach Bearbeitung des Updates wird keine E-Mail erzeugt.
   >
   > * Der Datumsstempel ist das Datum des ursprünglichen Kommentars und nicht das Datum der letzten Aktualisierung.

1. (Optional) Klicken Sie auf das Menü **Mehr** ![](assets/more-icon.png) und dann auf eine der folgenden Optionen, um Informationen aus einem Kommentar in die Zwischenablage oder in eine neue Antwort zu kopieren:

   * **Link kopieren** , um den Link eines Updates zu kopieren, ohne die Antworten zu erhalten.
   * **Kopieren Sie den Textkörper**, um den Text einer Aktualisierung zu kopieren.
   * **Antwort zitieren**: Öffnet ein neues Kommentarfeld, in dem der ursprüngliche Kommentar in einer neuen Antwort zitiert und als Blockzitat markiert ist.

     Weitere Informationen finden Sie unter [Funktionsweise aktualisieren](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Optional) Klicken Sie auf das Menü **Mehr** rechts neben einem Kommentar und dann auf **Löschen** , um einen hinzugefügten Kommentar zu löschen. ![](assets/more-icon.png) Weitere Informationen finden Sie unter [Funktionsweise aktualisieren](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Klicken Sie auf **Antworten** , um auf einen vorhandenen Kommentar zu antworten, und führen Sie dann die Schritte 5 bis 9 oben aus. Weitere Informationen zur Beantwortung von Aktualisierungen finden Sie unter [Antworten auf Aktualisierungen](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md) <!--insure this stays accurate-->.
1. (Bedingt und optional) Wenn andere Benutzer Kommentare hinzugefügt haben, die außerhalb des sichtbaren Bereichs im Abschnitt Updates angezeigt werden, klicken Sie unten im Bildschirm auf **Anzeigen** im blauen **neuen Kommentarbanner** , um diese Kommentare anzuzeigen.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Weitere Kommentare werden unten auf dem Bildschirm angezeigt.
1. (Optional) Klicken Sie auf das Symbol **Gefällt mir**![](assets/like-icon.png), um einen Kommentar zu erhalten, den jemand anderes hinzugefügt hat. Das Symbol wird mit der Anzahl der &quot;Gefällt mir&quot;-Klicks aktualisiert.

1. (Optional) Klicken Sie auf die Registerkarte **Systemaktivität** , um die vom System protokollierten Aktualisierungen anzuzeigen. Wenn ein Ziel aktualisiert wird, generiert Workfront einen Hinweis zu dieser Aktualisierung und zeigt sie auf der Registerkarte Systemaktivität an. Workfront zeichnet auch eine Systemaktualisierung auf, wenn ein Ergebnis, eine Aktivität oder ein Projekt zum Ziel hinzugefügt oder aktualisiert wird. <!--ensure the casing on the tab has not changed-->


