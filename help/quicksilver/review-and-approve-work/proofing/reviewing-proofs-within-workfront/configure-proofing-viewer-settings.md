---
product-area: documents;setup
navigation-topic: review-a-proof
title: Konfigurieren der Einstellungen des Testversand-Viewers
description: Sie können Einstellungen für den Web Proofing Viewer und den Desktop Proofing Viewer konfigurieren.
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 0%

---

# Konfigurieren der Einstellungen des Testversand-Viewers

Sie können die folgenden Einstellungen sowohl für den Web Proofing Viewer als auch für den Desktop Proofing Viewer konfigurieren:

* Ob Kommentar-Markups und Pins bei Testsendungen angezeigt werden.
* Ob die Markup-Tools oben im Testversand-Viewer oder in einem Dropdown-Menü angezeigt werden.
* Welche E-Mail-Benachrichtigungen erhalten Sie als Validierer für den geöffneten Testversand?

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

Sie können die folgenden Einstellungen für den Desktop Proofing Viewer konfigurieren:

* Wie Sie möchten, dass Links innerhalb des Website-Inhalts im Viewer geöffnet werden.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* Was passiert, wenn Sie auf einen Link klicken, der in einer neuen Browserregisterkarte oder einem neuen Browserfenster geöffnet werden soll?
* Löschen Sie die Cachedaten, die möglicherweise mit dem Testversand gespeichert werden, den Sie anzeigen, um Inhalte wie Popups (die durch Browsercache-Daten blockiert werden können) für die Anzeige im Viewer zu aktivieren.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Wählen Sie oder Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Konfigurieren der Einstellungen des Testversand-Viewers

So konfigurieren Sie die Testversand-Viewer-Einstellungen:

1. Öffnen Sie den Web Proofing Viewer oder den Desktop Proofing Viewer auf eine der folgenden Arten:

   * Wenn Sie einen Testversand in Adobe Workfront durchführen, wechseln Sie zu einer Dokumentliste mit einem Testversand, den Sie anzeigen möchten, bewegen Sie den Mauszeiger über das Dokument und klicken Sie auf **Testversand öffnen**.
   * Wenn Sie Workfront Proof verwenden, klicken Sie auf das Symbol &quot;**Gehe zu Testversand**&quot;für den Testversand im Dashboard oder in der Liste &quot;Ansichten&quot;![](assets/go-to-proof-blue-icon.png).

1. Wenn die linke Symbolleiste nicht angezeigt wird, klicken Sie auf das Symbol &quot;**Menü**&quot;, das sich in der linken oberen Ecke des Web Proofing Viewers befindet.

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Klicken Sie in der linken Symbolleiste auf das Symbol **Einstellungen** ![](assets/settings-icon-in-pv.png).

1. Konfigurieren Sie eine der folgenden **Einstellungen**, die angezeigt werden.

   Die verfügbaren Einstellungen variieren je nach Art des geöffneten Testversands.

   * **Markups anzeigen** (immer im Web Proofing Viewer und im Desktop Proofing Viewer verfügbar): Dies sind die Kommentarzeichen, die Prüfer bei der Verwendung der Markup-Tools zu Testsendungen hinzufügen. Wenn Sie sie deaktivieren, können Sie sie immer noch sehen, wenn Sie auf einen Kommentar in der Kommentarliste klicken.

     Diese Einstellung wirkt sich auf alle geöffneten Testsendungen aus.

   * **Pins anzeigen** (immer im Web Proofing Viewer und im Desktop Proofing Viewer verfügbar): Dies sind die nummerierten Pins, die Prüfer bei Verwendung der Markup Tools zu Testsendungen hinzufügen. Sie geben an, wo und in welcher Reihenfolge der Validierer Kommentare hinzugefügt hat. Wenn Sie sie deaktivieren, können Sie sie immer noch sehen, wenn Sie auf einen Kommentar in der Kommentarliste klicken.

     Diese Einstellung wirkt sich auf alle geöffneten Testsendungen aus.

   * **Verwenden Sie erweiterte Markup-Tools** (immer verfügbar im Web Proofing Viewer und im Desktop Proofing Viewer): Standardmäßig werden die Markup-Tool-Optionen oben im Testversand-Viewer angezeigt. Sie können sie so konfigurieren, dass sie nur in einem vertikalen Menü angezeigt werden, das nur durch Klicken geöffnet wird.

     Diese Einstellung gilt für alle Testsendungen, die Sie öffnen.

   * **Senden Sie mir E-Mail-Benachrichtigungen über** (immer verfügbar im Web Proofing Viewer und im Desktop Proofing Viewer): Klicken Sie auf eine der folgenden Optionen. Diese Einstellung wirkt sich nur auf den geöffneten Testversand aus. Weitere Informationen finden Sie unter [Übersicht über Testversand-Kommentare und -Entscheidungen über Benachrichtigungen](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Alle Aktivitäten</td> 
        <td>Workfront sendet eine E-Mail an den Validierer, sobald eine Aktivität im Testversand vorhanden ist, z. B. einen neuen Kommentar, eine neue Antwort oder eine neue Entscheidung. <p>Dies ist eine großartige Option für die Person, die den Testversand verwaltet, da sie die Aktivität so sehen kann, wie sie ausgeführt wird. </p><p>Benutzer erhalten keine E-Mail-Warnung zu ihrer eigenen Aktivität.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Antworten auf meine Kommentare</td> 
        <td>Eine E-Mail wird nur dann an den Validierer gesendet, wenn jemand explizit auf seinen Kommentar antwortet (dabei werden eigene Antworten auf eigene Kommentare ausgeschlossen). Das bedeutet, dass der Validierer nicht benachrichtigt wird, wenn jemand, der den Testversand durchführt, einen neuen Kommentar abgibt.<p>Diese Einstellung wird Ihren Kunden empfohlen, den Testversand durchzuführen, damit sie über keine weiteren Kommentare zum Testversand informiert und nur über Antworten auf ihre eigenen Kommentare informiert werden.</p><p>validierungsverantwortliche Benutzer mit dieser E-Mail-Warnungseinstellung werden zwar nicht über andere neue Kommentare benachrichtigt, können aber dennoch alle Kommentare zum Testversand im Testversand-Viewer anzeigen.</p><p>Informationen zu Kommentaren finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Anzeigen und Antworten auf Testkommentare</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Entscheidungen</td> 
        <td>Workfront sendet eine E-Mail nur dann an den Validierer, wenn ein Benutzer eine Entscheidung trifft.<p>Dies kann für die Person nützlich sein, die den Validierungsprozess verwaltet (z. B. einen Projektmanager), und muss den Fortschritt des Testversands überwachen und sehen, welche Benutzer ihre Entscheidung getroffen haben.</p><p>Sie werden nicht über Ihre eigene Entscheidung informiert, es sei denn, Sie wählen beim Senden Ihrer Entscheidung eine E-Mail-Bestätigungsoption aus.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Finale Entscheidung</td> 
        <td>Workfront sendet eine E-Mail, wenn der letzte Genehmiger des Testversands seine Entscheidung getroffen hat.<p>Dieser Warnhinweis wird häufig vom Designer verwendet, der normalerweise nicht an der eigentlichen Reviewdiskussion teilnehmen muss. Wenn die endgültige Entscheidung getroffen wird, wird der Designer benachrichtigt und kann dann alle notwendigen Änderungen vornehmen.</p><p>Dieser Warnhinweis kann auch für einen Abteilungsleiter nützlich sein, der nur benachrichtigt werden muss, wenn der Überprüfungsprozess abgeschlossen ist.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Stündliche Zusammenfassung</td> 
        <td>Workfront sendet stündlich eine E-Mail mit einer Zusammenfassung aller Kommentare, Antworten und Entscheidungen, die in dieser Stunde getroffen wurden.<p>Die E-Mail wird nur gesendet, wenn neben Ihrer eigenen Aktivität innerhalb der letzten Stunde stattgefunden hat. </p><p>Mit diesem Warnhinweis können Sie einen Überblick über das Projekt erhalten.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Senior Reviewer, der einen Überblick über das Projekt benötigt, aber nicht sofort über alle Aktivitäten auf dem Testversand benachrichtigt werden muss.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Tägliche Zusammenfassung</td> 
        <td>Workfront sendet eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen, die nur an Tagen aufgelistet sind, an denen neben Ihrer eigenen Aktivität Aktivitäten stattfinden.<p>Mit diesem Warnhinweis können Sie eine Zusammenfassung des Projekts anzeigen, ohne über den gesamten Tag hinweg durch mehrere Aktualisierungen überlastet zu sein.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Abteilungsleiter, der den Gesamtfortschritt des Projekts überwachen möchte.</p><p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Benachrichtigungen für Testversand-Kommentare und -Entscheidungen verwalten</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Keine E-Mail</td> 
        <td>Workfront sendet keine E-Mail-Warnungen.<br>Dies ist für eine Person nützlich, die einem Testversand nur zu Referenzzwecken hinzugefügt wird und nicht über Änderungen benachrichtigt werden muss.<p>Der Systemstandard lautet Tägliche Zusammenfassung (wird auch als Nicht festgelegt angesehen). Wenn Sie oder Ihre Validierer keine anderen Änderungen vornehmen, haben alle Testsendungen diese Einstellung.</p></td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **Beim Klicken auf Hyperlinks in einem Testversand** (nur im Desktop Proofing Viewer verfügbar): Wählen Sie eine Option aus, um festzulegen, was im Desktop Proofing Viewer passiert, wenn Sie auf einen Link klicken, der auf einer neuen Browserregisterkarte oder in einem neuen Browserfenster geöffnet werden soll.

     Diese Einstellung gilt für alle interaktiven Testsendungen, die Sie öffnen.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Im Testversand-Viewer öffnen</td> 
        <td>Die Links werden immer im Desktop Proofing Viewer geöffnet und Sie können den verknüpften Inhalt testen. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Im Browser öffnen</td> 
        <td>Die Links werden immer im Browser geöffnet, nicht in einem Proofing-Viewer. Der verknüpfte Inhalt kann nicht getestet werden.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Jedes Mal fragen</td> 
        <td> <p>Sie werden jedes Mal gefragt, ob Sie den Link im Desktop Proofing Viewer oder im Browser öffnen möchten. Wenn Sie den Link im Desktop Proofing Viewer öffnen, können Sie den verknüpften Inhalt testen. Wenn Sie den Link im Browser öffnen, können Sie den verlinkten Inhalt nicht testen.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>Diese Einstellung wirkt sich nur auf den geöffneten Testversand aus.</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **Cache löschen**: Löscht die Browser-Cache-Daten, die möglicherweise mit einem interaktiven Testversand gespeichert werden, den Sie anzeigen. Dadurch können Inhalte wie Popups (die durch Browsercache-Daten blockiert werden können) im Desktop Proofing Viewer angezeigt werden.

     Zu den gelöschten Daten gehören der HTTP-Cache (z. B. Bilder, die nach der nächsten Seitenaktualisierung wiederverwendet werden sollen) und der Cache für Webspeicherdaten (z. B. Cookies und Daten, die Benutzer identifizieren).

     Diese Einstellung wirkt sich nur auf den geöffneten Testversand aus.
