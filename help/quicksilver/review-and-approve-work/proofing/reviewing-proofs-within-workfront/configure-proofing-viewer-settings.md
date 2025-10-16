---
product-area: documents;setup
navigation-topic: review-a-proof
title: Einstellungen der Proofing-Anzeige konfigurieren
description: Sie können Einstellungen für den Web Proofing Viewer und den Desktop Proofing Viewer konfigurieren.
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 385f4a6663cacfdcf519bf5699fc1840c2cb2adc
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 1%

---

# Einstellungen der Proofing-Anzeige konfigurieren

Sie können die folgenden Einstellungen für den Web Proofing Viewer und den Desktop Proofing Viewer konfigurieren:

* Ob Kommentarmarkierungen und Pins auf Korrekturabzügen angezeigt werden.
* Ob die Markup-Tools oben im Proofing Viewer oder in einem Dropdown-Menü angezeigt werden.
* Welche E-Mail-Benachrichtigungen Sie als Prüferin bzw. Prüfer für den geöffneten Korrekturabzug erhalten.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

Sie können die folgenden Einstellungen für den Desktop Proofing Viewer konfigurieren:

* Wie Links innerhalb von Website-Inhalten im Viewer geöffnet werden sollen.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* Was passiert, wenn Sie auf einen Link klicken, der in einer neuen Browser-Registerkarte oder einem neuen Fenster geöffnet werden soll?
* Löschen Sie die Cache-Daten, die mit dem Korrekturabzug gespeichert werden könnten, den Sie anzeigen, um die Anzeige von Inhalten wie Popups (die durch Browser-Cache-Daten blockiert werden können) im Viewer zu ermöglichen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rolle des Korrekturabzugs </td> 
   <td>Prüfer, Prüfer und genehmigende Person, Autor, Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einstellungen der Proofing-Anzeige konfigurieren

So konfigurieren Sie Einstellungen für die Proofing-Anzeige:

1. Öffnen Sie Web Proofing Viewer oder Desktop Proofing Viewer auf eine der folgenden Arten:

   * Wenn Sie einen Korrekturabzug in Adobe Workfront erstellen, gehen Sie zu einer Dokumentliste, die einen Korrekturabzug enthält, den Sie anzeigen möchten, bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf **Korrekturabzug öffnen**.
   * Wenn Sie Workfront Proof verwenden, klicken Sie auf das Symbol **Zum Korrekturabzug gehen** für den Korrekturabzug im Dashboard oder in einer Ansichtsliste ![Zum Korrekturabzug gehen](assets/go-to-proof-blue-icon.png).

1. Wenn die linke Symbolleiste nicht angezeigt wird, klicken Sie auf **Menü**-Symbol in der linken oberen Ecke der Web-Korrekturabzugsanzeige.

   ![Menüsymbol](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Klicken Sie in der linken Symbolleiste auf das Symbol **Einstellungen** (![) &#x200B;](assets/settings-icon-in-pv.png).

1. Konfigurieren Sie eine der folgenden **Einstellungen** die angezeigt werden.

   Die verfügbaren Einstellungen variieren je nach dem Typ des geöffneten Korrekturabzugs.

   * **Markierungen anzeigen** (immer im Web Proofing Viewer und im Desktop Proofing Viewer verfügbar): Dies sind die Kommentarzeichen, die Prüfer zu Korrekturabzügen hinzufügen, wenn sie die Markup-Tools verwenden. Wenn Sie sie deaktivieren, können Sie sie weiterhin sehen, wenn Sie auf einen Kommentar in der Kommentarliste klicken.

     Diese Einstellung wirkt sich auf alle geöffneten Korrekturabzüge aus.

   * **Pins anzeigen** (immer im Web Proofing Viewer und im Desktop Proofing Viewer verfügbar): Dies sind die nummerierten Pins, die Prüfer zu Korrekturabzügen hinzufügen, wenn sie die Markup-Tools verwenden. Sie geben an, wo und in welcher Reihenfolge der Prüfer Kommentare hinzugefügt hat. Wenn Sie sie deaktivieren, können Sie sie weiterhin sehen, wenn Sie auf einen Kommentar in der Kommentarliste klicken.

     Diese Einstellung wirkt sich auf alle geöffneten Korrekturabzüge aus.

   * **Erweiterte Markup-Tools verwenden** (immer im Web Proofing Viewer und im Desktop Proofing Viewer verfügbar): Standardmäßig werden die Optionen des Markup-Tools oben im Proofing Viewer angezeigt. Sie können sie so konfigurieren, dass sie in einem vertikalen Menü angezeigt werden, das nur geöffnet wird, wenn Sie darauf klicken.

     Diese Einstellung gilt für alle Korrekturabzüge, die Sie öffnen.

   * **E-Mail-Benachrichtigungen senden über** (immer verfügbar in der Web Proofing Viewer und der Desktop Proofing Viewer): Klicken Sie auf eine der folgenden Optionen. Diese Einstellung wirkt sich nur auf den geöffneten Korrekturabzug aus. Weitere Informationen finden Sie unter [Benachrichtigungen für Korrekturabzugskommentare und Entscheidungen - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Alle Aktivitäten</td> 
        <td>Workfront sendet jedes Mal eine E-Mail an den Prüfer, wenn eine Aktivität im Korrekturabzug stattfindet, z. B. ein neuer Kommentar, eine neue Antwort oder eine neue Entscheidung. <p>Dies ist eine hervorragende Option für die Person, die den Proofing-Prozess verwaltet, da sie die Aktivität direkt sehen kann. </p><p>Benutzende erhalten keine E-Mail-Benachrichtigung über ihre eigene Aktivität.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Antworten auf meine Kommentare</td> 
        <td>Eine E-Mail wird nur dann an den Prüfer gesendet, wenn jemand explizit auf seinen Kommentar antwortet (dies schließt die eigenen Antworten auf seine eigenen Kommentare aus). Das bedeutet, dass, wenn jemand auf dem Korrekturabzug einen neuen Kommentar abgibt, der Prüfer nicht benachrichtigt wird.<p>Diese Einstellung wird für Ihre Kunden auf dem Korrekturabzug empfohlen, damit sie nicht über andere Kommentare zu dem Korrekturabzug benachrichtigt werden und nur über Antworten auf ihre eigenen Kommentare.</p><p>Reviewer mit dieser E-Mail-Warnhinweiseinstellung werden zwar nicht über andere neue Kommentare benachrichtigt, sie können jedoch alle Kommentare zum Korrekturabzug in der Proofing-Anzeige anzeigen.</p><p>Weitere Informationen zu Kommentaren finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Kommentare zu Korrekturabzügen anzeigen und </a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Entscheidungen</td> 
        <td>Workfront sendet eine E-Mail nur dann an den Validierungsverantwortlichen, wenn jemand eine Entscheidung trifft.<p>Dies kann für die Person nützlich sein, die den Genehmigungsprozess verwaltet (z. B. einen Projektmanager) und den Fortschritt beim Korrekturabzug überwachen muss, um zu sehen, welche Benutzer ihre Entscheidung getroffen haben.</p><p>Sie werden über Ihre eigene Entscheidung nur benachrichtigt, wenn Sie beim Senden Ihrer Entscheidung eine E-Mail-Bestätigungsoption auswählen.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Finale Entscheidung</td> 
        <td>Workfront sendet eine E-Mail, wenn die letzte genehmigende Person für den Korrekturabzug ihre Entscheidung getroffen hat.<p>Dieser Warnhinweis wird häufig vom Designer verwendet, der normalerweise nicht an der eigentlichen Überprüfungsdiskussion teilnehmen muss. Wenn die endgültige Entscheidung getroffen wird, wird der Designer benachrichtigt und kann dann die erforderlichen Änderungen vornehmen.</p><p>Dieser Warnhinweis kann auch für einen Abteilungsleiter nützlich sein, der erst benachrichtigt werden muss, wenn der Überprüfungsprozess abgeschlossen ist.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Stündliche Zusammenfassung</td> 
        <td>Workfront sendet stündlich eine E-Mail mit einer Zusammenfassung aller Kommentare, Antworten und Entscheidungen, die in dieser Stunde aufgetreten sind, an die validierungsverantwortlichen Personen.<p>Die E-Mail wird nur gesendet, wenn innerhalb der letzten Stunde eine andere Aktivität als die eigene stattgefunden hat. </p><p>Dieser Warnhinweis bietet eine gute Möglichkeit, einen Überblick über das Projekt zu erhalten.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein leitender Prüfer, der einen Überblick über das Projekt benötigt, aber nicht sofort über alle Aktivitäten im Korrekturabzug benachrichtigt werden muss.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Tägliche Zusammenfassung</td> 
        <td>Workfront sendet eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen nur an Tagen, an denen außer Ihrer eigenen Aktivität eine andere Aktivität stattfindet.<p>Dieser Warnhinweis bietet eine gute Möglichkeit, eine Zusammenfassung des Projekts anzuzeigen, ohne im Laufe des Tages durch mehrere Updates überfordert zu werden.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Abteilungsleiter, der den Gesamtfortschritt des Projekts überwachen möchte.</p><p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Verwalten von Benachrichtigungen für Kommentare und Entscheidungen zu Korrekturabzügen</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Keine E-Mail</td> 
        <td>Workfront sendet keine E-Mail-Warnungen.<br>Dies ist für Personen nützlich, die einem Korrekturabzug nur zu Referenzzwecken hinzugefügt werden und nicht über Änderungen benachrichtigt werden müssen.<p>Der Systemstandard lautet „Tägliche Zusammenfassung“ (wird auch als „Nicht festgelegt“ angezeigt). Wenn Sie oder Ihre Prüfer keine anderen Änderungen vornehmen, haben alle Ihre Korrekturabzüge diese Einstellung.</p></td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **Beim Klicken auf Hyperlinks in einem Korrekturabzug** (nur im Desktop Proofing Viewer verfügbar): Wählen Sie eine Option aus, um festzulegen, was im Desktop Proofing Viewer geschieht, wenn Sie auf einen Link klicken, der in einer neuen Browser-Registerkarte oder einem neuen Fenster geöffnet werden soll.

     Diese Einstellung gilt für alle interaktiven Korrekturabzüge, die Sie öffnen.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">In der Proofing-Anzeige öffnen</td> 
        <td>Links werden immer im Desktop Proofing Viewer geöffnet und Sie können den verknüpften Inhalt prüfen. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Im Browser öffnen</td> 
        <td>Links werden immer im Browser geöffnet, nicht in einer Proofing-Anzeige. Sie können den verlinkten Inhalt nicht prüfen.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Jedes Mal fragen</td> 
        <td> <p>Sie werden jedes Mal gefragt, ob Sie den Link im Desktop Proofing Viewer oder im Browser öffnen möchten. Wenn Sie den Link im Desktop Proofing Viewer öffnen, können Sie den verknüpften Inhalt prüfen. Wenn Sie den Link im Browser öffnen, können Sie den verlinkten Inhalt nicht prüfen.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysAsk.png" style="width: 350;height: 243;"> </p> <p>Diese Einstellung wirkt sich nur auf den geöffneten Korrekturabzug aus.</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **Cache löschen**: Löscht die Browser-Cache-Daten, die möglicherweise mit einem interaktiven Korrekturabzug gespeichert werden, den Sie anzeigen. Dadurch können Inhalte wie Popups (die durch Browser-Cache-Daten blockiert werden können) im Desktop Proofing Viewer angezeigt werden.

     Die Daten, die gelöscht werden, umfassen den HTTP-Cache (z. B. Bilder, die nach der nächsten Seitenaktualisierung wiederverwendet werden sollen) und den Web-Datenspeicher (z. B. Cookies und Daten, die Benutzer identifizieren).

     Diese Einstellung wirkt sich nur auf den geöffneten Korrekturabzug aus.
