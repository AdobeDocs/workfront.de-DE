---
product-previous: workfront-goals
navigation-topic: goal-management
title: Verwalten von Zielkommentaren in Adobe Workfront-Zielen
description: Sie können allen Zielen, die Sie in Adobe Workfront-Zielen anzeigen können, Kommentare hinzufügen.
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '1110'
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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Sie müssen über Folgendes verfügen, bevor Sie beginnen können:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Verwalten von Zielkommentaren

Sie können Ziele im Abschnitt &quot;Aktualisierungen&quot;auf der Seite eines Ziels mit Kommentaren versehen.

Sie können auf einen Kommentar antworten oder einen Kommentar erhalten, den Sie oder andere in diesem Bereich hinzugefügt haben.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke oder **Hauptmenü** icon ![](assets/lines-main-menu.png) in der oberen linken Ecke, falls verfügbar, klicken Sie auf **Ziele**.
Dadurch wird die Zielliste geöffnet.
1. Suchen Sie das Ziel, dem Sie Kommentare hinzufügen möchten, und klicken Sie dann auf seinen Namen, um die Zielseite zu öffnen.
1. Klicks  **Updates** im linken Bereich.
1. (Optional) Um einen vorhandenen Kommentar zu finden, beginnen Sie mit der Eingabe eines Suchbegriffs <!--or a user's name--> im **Suche** in der oberen rechten Ecke des **Kommentare** Registerkarte.

   ![](assets/search-field-in-updates-tab-goals.png)

   Der Suchbegriff <!--or user--> Sie nach gesucht haben, wird hervorgehoben und die Kommentare, die sie enthalten, werden oben im Abschnitt Aktualisierungen angezeigt.

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >Sie müssen nach einem Wort suchen, das in einem Kommentar oder einer Antwort enthalten ist. Sie können nicht nach einem getaggten Benutzer oder Team suchen.

   Weitere Informationen finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. Klicken Sie auf **x** im Suchfeld ein, um die Suchergebnisse zu löschen und zur vollständigen Aktualisierung zurückzukehren.
1. Klicken Sie auf **Kommentare** in der linken oberen Ecke des Bereichs Updates.
1. Beginnen Sie mit der Eingabe eines Kommentars im **Neuer Kommentar** ankreuzen.

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Wenn Sie den Abschnitt Updates verlassen, bevor Sie mit der Eingabe und dem Senden eines Kommentars fertig sind, bleibt der Kommentar auf der Seite im Entwurfsmodus, auch wenn Sie sich abmelden und wieder anmelden. Bilder, die dem Kommentar hinzugefügt werden, werden ebenfalls im Entwurf gespeichert. Entwürfe werden sieben Tage lang gespeichert und können nicht wiederhergestellt werden. Entworfene Kommentare sind nur für den Benutzer sichtbar, der sie eingibt.

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um eine Änderung rückgängig zu machen oder wiederherzustellen:
   * STRG + Z ( ⌘ + z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Y ( ⌘ + y für Mac) zum Wiederholen einer Änderung
1. (Optional) Um Ihrer Aktualisierung, einem Hyperlink oder einem Bild Rich-Text-Formatierung hinzuzufügen, verwenden Sie alle Optionen in der Rich-Text-Symbolleiste oder die zugehörigen Symbole. Weitere Informationen finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Im **Personen oder Teams taggen** eingeben, den Namen oder die E-Mail-Adresse eines Benutzers oder eines Teams eingeben, das Sie in diesen Kommentar aufnehmen möchten, und ihn dann auswählen, wenn er in der Liste angezeigt wird.
1. Wählen Sie die **Privatperson in meinem Unternehmen** umschalten, um den Kommentar nur für Personen in Ihrem Unternehmen sichtbar zu machen.

   >[!TIP]
   >
   >Sie müssen ein Unternehmen in Ihrem Profil angeben, damit diese Option im Bereich Updates verfügbar ist.

1. Klicks **Einsenden**.

   >[!TIP]
   >
   >Wenn ein anderer Benutzer einen Kommentar für dasselbe Element sendet, das Sie aktualisieren, wird eine rote Zeile mit der Anzeige &quot;Neu&quot;angezeigt, um Sie über die neueren Kommentare zu informieren, sowie eine blaue Benachrichtigung am unteren Rand des Bildschirms, die die Anzahl der neuen Kommentare angibt.
   >
   >Der Indikator wird nur angezeigt, nachdem der Kommentar zum Element gesendet wurde, nicht aber, wenn der Kommentar noch erstellt wurde.
   >![](assets/real-time-new-red-indicator-unified-commenting-copy.png)

1. (Optional) Um einen Kommentar zu bearbeiten, klicken Sie auf die **Mehr** Menü ![](assets/more-icon.png) rechts neben dem Symbol &quot;Gefällt mir&quot;und klicken Sie dann auf **Bearbeiten**.
1. Bearbeiten Sie die Informationen im Kommentar, fügen Sie Bilder hinzu, entfernen Sie sie oder entfernen Sie einen der getaggten Benutzer.
Sie können Ihren Kommentar innerhalb von 15 Minuten nach seiner Übermittlung bearbeiten. Links neben dem Datumsstempel, der beim Aktualisieren des Kommentars angezeigt wird, wird ein Indikator &quot;bearbeitet&quot;hinzugefügt.

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * Es wird eine E-Mail erzeugt, um die Benutzer nur dann über Ihre Aktualisierung zu informieren, wenn Sie die ursprüngliche Aktualisierung übermitteln. Nach Bearbeitung des Updates wird keine E-Mail erzeugt.
   >
   > * Der Datumsstempel ist das Datum des ursprünglichen Kommentars und nicht das Datum der letzten Aktualisierung.

1. (Optional) Klicken Sie auf die **Mehr** Menü ![](assets/more-icon.png)und klicken Sie dann auf eine der folgenden Optionen, um Informationen aus einem Kommentar in die Zwischenablage oder in eine neue Antwort zu kopieren:

   * **Link kopieren** , um den Link einer Aktualisierung ohne die Antworten zu kopieren.
   * **Textkörper kopieren** , um den Text einer Aktualisierung zu kopieren.
   * **Anführungsantwort** , um ein neues Kommentarfeld zu öffnen, in dem der ursprüngliche Kommentar in einer neuen Antwort zitiert und als Blockanführungszeichen markiert ist.

     Weitere Informationen finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Optional) Klicken Sie auf die **Mehr** Menü ![](assets/more-icon.png) rechts neben einem Kommentar klicken Sie auf **Löschen** , um einen hinzugefügten Kommentar zu löschen. Weitere Informationen finden Sie unter [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Optional) Klicken Sie auf **Antwort** um auf einen vorhandenen Kommentar zu antworten, folgen Sie dann den Schritten 5 bis 9 oben. Weitere Informationen zur Beantwortung von Aktualisierungen finden Sie unter [Antworten auf Aktualisierungen](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md). <!--insure this stays accurate-->
1. (Bedingt und optional) Wenn andere Benutzer Kommentare hinzugefügt haben, die außerhalb des sichtbaren Bereichs im Abschnitt Updates angezeigt werden, klicken Sie auf **Ansicht** in Blau **neues Kommentarbanner** unten auf dem Bildschirm, um diese Kommentare anzuzeigen.

   ![](assets/blue-new-comments-banner-with-view-button.png)

   Weitere Kommentare werden unten auf dem Bildschirm angezeigt.
1. (Optional) Klicken Sie auf die **liken** icon![](assets/like-icon.png) , um einen Kommentar zu erhalten, den jemand anderes hinzugefügt hat. Das Symbol wird mit der Anzahl der &quot;Gefällt mir&quot;-Klicks aktualisiert.

1. (Optional) Klicken Sie auf die **Systemaktivität** -Tab, um vom System protokollierte Aktualisierungen anzuzeigen. Wenn ein Ziel aktualisiert wird, generiert Workfront einen Hinweis zu dieser Aktualisierung und zeigt sie auf der Registerkarte Systemaktivität an. Workfront zeichnet auch eine Systemaktualisierung auf, wenn ein Ergebnis, eine Aktivität oder ein Projekt zum Ziel hinzugefügt oder aktualisiert wird. <!--ensure the casing on the tab has not changed-->


