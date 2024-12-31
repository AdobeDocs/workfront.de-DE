---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Freigeben eines Korrekturabzugs über die Korrekturabzugsansicht
description: Sie können einen Korrekturabzug über die Korrekturabzugsansicht freigeben, wenn die Freigabe durch die Person, die den Korrekturabzug besitzt oder erstellt, aktiviert ist.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: aaf5beb8692b2fdbb797ba908796d78b4ee8866c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# Freigeben eines Korrekturabzugs über die Korrekturabzugsansicht

Sie können einen Korrekturabzug über die Korrekturabzugsansicht freigeben, wenn die Freigabe durch die Person, die den Korrekturabzug besitzt oder erstellt, aktiviert ist.

>[!IMPORTANT]
>
>Die Einstellung Freigabe von Korrekturabzug über öffentliche URL oder Einbettungs-Code zulassen muss aktiviert sein.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Auswählen oder Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## URL freigeben

Sie können einen Korrekturabzug über eine URL freigeben, wenn der/die Verantwortliche den Korrekturabzug für die Freigabe konfiguriert hat. Die Verantwortlichen für Korrekturabzüge können die Freigabeeinstellungen jederzeit aktualisieren. Weitere Informationen finden Sie unter [Bearbeiten der Korrekturabzugseinstellungen](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Wenn das Menü mit dem Symbol auf der linken Seite nicht angezeigt wird **klicken Sie auf** Menü“ in der linken oberen Ecke der Korrekturabzugsansicht.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. Klicken Sie im Menü mit dem Symbol links im Proofing Viewer auf das Symbol **Freigeben**.

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. Stellen Sie in den **Korrekturabzug freigeben** angezeigten Optionen sicher, **Sie „Freigebbaren Link**&quot; ausgewählt haben.

1.  Führen Sie einen der folgenden Schritte aus:

   * Um den Link in die Zwischenablage zu kopieren, klicken Sie auf **Link kopieren**.

     Sie können den Link jetzt über ein Tool eines Drittanbieters verteilen, z. B. einen Chat oder eine E-Mail-Anwendung.

   * Gehen Sie wie folgt vor, um den Link direkt aus Adobe Workfront per E-Mail zu senden:

      1. Beginnen Sie im Feld **ODER-E-Mail-Link zu** mit der Eingabe und wählen Sie den Namen Ihres Empfängers aus. Oder geben Sie die E-Mail-Adresse eines externen Benutzers an, für den Sie freigeben möchten.

         >[!NOTE]
         >
         >Wenn bei der Freigabe eines Korrekturabzugs eine Alias-E-Mail angezeigt wird, erstellen Sie keinen neuen Gastbenutzer, indem Sie die ursprüngliche E-Mail eingeben, wenn eine entsprechende Alias-E-Mail vorhanden ist.

      1. Wählen Sie aus den folgenden Optionen aus:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Öffentlichen Link senden</td>
            <td><p>Enthält eine Schaltfläche in der E-Mail-Benachrichtigung, die Benutzende zum Korrekturabzug innerhalb der von ihnen verwendeten Korrekturabzugsansicht weiterleitet und Ansichtszugriff gewährt.</p><p>Wenn <strong>Korrekturabzug über öffentliche URL oder Einbettungs-Code abonnieren</strong> für den Korrekturabzug deaktiviert ist, können sich Benutzende mit ihren Workfront-Anmeldedaten anmelden, um dem Korrekturabzug Kommentare hinzuzufügen. Wenn er aktiviert ist, kann jeder, der seine E-Mail-Adresse und seinen Namen (kein Passwort erforderlich) angibt, den Korrekturabzug signieren und Kommentare hinzufügen.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Download-Link senden</td>
            <td>Enthält eine Schaltfläche in der E-Mail-Benachrichtigung, die Benutzer zu einer Download-Seite weiterleitet, die Dateidetails, Dateinamen und Dateigröße bereitstellt, wobei die Datei inline angezeigt wird. Benutzer können auf der Download-Seite auf den Download-Link klicken, um die Datei herunterzuladen.</td>
           </tr>
           <tr>
            <td role="rowheader">Benutzerdefinierte Nachricht hinzufügen</td>
            <td>Ermöglicht die Angabe eines benutzerdefinierten Betreffs und Textkörpers für die E-Mail-Benachrichtigung.</td>
           </tr>
          </tbody>
         </table>

      1. Klicken Sie auf **Senden**.

         Ihre Empfänger erhalten eine E-Mail-Benachrichtigung mit Informationen zum Testversand und den Schaltflächen, die Sie einbezogen haben.

         ![](assets/proof-share-email-350x87.png)

## Freigeben des Einbettungs-Codes

Sie können einen Korrekturabzug über Einbettungs-Code freigeben, wenn der Korrekturabzugsverantwortliche ihn für diesen konfiguriert hat.

So geben Sie einen Korrekturabzug über den Einbettungs-Code frei:

1. Klicken Sie in der Symbolleiste links neben der Korrekturabzugsansicht auf das Symbol **Freigeben**.

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. Klicken Sie in den **Korrekturabzug freigeben** angezeigten Optionen auf **Einbettungs-Code abrufen** und dann auf **Kopieren**.

## Freigeben eines Korrekturabzugs durch Hinzufügen von Benutzern

Sie können Benutzende zu einem Korrekturabzug hinzufügen, während Sie einen Korrekturabzug überprüfen, wenn Sie über eine der folgenden Berechtigungen verfügen:

* Berechtigungen als Verantwortlicher oder Administrator
* Manager-Berechtigungen und Sie sind der Ersteller oder Inhaber des Korrekturabzugs
* Managerberechtigungen mit der Rolle „Autor oder Moderator - Korrekturabzug“

Wenn der Korrekturabzug über einen automatisierten Workflow verfügt, können Sie den/die Benutzende(n) zu einem einzelnen Schritt hinzufügen. Weitere Informationen finden Sie unter [Automatisierter Workflow - Übersicht](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Standardmäßig fügen Sie dem Korrekturabzug Benutzer hinzu:

* Erhalten Sie eine E-Mail-Benachrichtigung mit einem Link zum Korrekturabzug.
* Kann Genehmigungsentscheidungen für den Korrekturabzug über den Bereich „Startseite“ treffen, wie unter [Genehmigen von Arbeit](../../../../review-and-approve-work/manage-approvals/approving-work.md) beschrieben.
* Proofing muss nicht aktiviert sein, damit der Korrekturabzug überprüft werden kann.

Wenn der automatisierte Workflow aktiviert ist und Sie dem Korrekturabzug einen Benutzer hinzufügen, für den das Proofing nicht in Workfront aktiviert ist, wird innerhalb des automatisierten Workflows ein neuer Schritt erstellt. Der/die Benutzende, den/die Sie hinzufügen, wird automatisch zu dieser neuen Phase hinzugefügt, wenn er/sie den Korrekturabzug zum ersten Mal aufruft. Weitere Informationen finden Sie unter [Automatisierter Workflow - Übersicht](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

So geben Sie einen Korrekturabzug für einzelne Benutzer frei:

1. Klicken Sie in der Symbolleiste links neben der Korrekturabzugsansicht auf das Symbol **Freigeben**.

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Klicken Sie **der** auf der linken Seite auf Empfänger hinzufügen .
1. Geben **unter „Neue Korrekturabzugsempfänger** den Namen eines Benutzers ein, für den Sie den Korrekturabzug freigeben möchten. Klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. (Optional) Ändern Sie alle Reviewer-Optionen rechts neben dem Namen der Person:

   * **Rolle des Korrekturabzugs**: Weitere Informationen finden Sie unter [Rollen von Korrekturabzügen in Workfront Proof verwalten](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Staging**: (nur verfügbar, wenn der Korrekturabzug einen automatisierten Workflow aufweist). Weitere Informationen finden Sie unter  [Übersicht über die automatisierten Workflow-](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **E-Mail-**: Wählen Sie eine der folgenden Optionen, um festzulegen, wie die Person über Aktivitäten im Testversand benachrichtigt werden soll.

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
        <td>Eine E-Mail wird nur dann an den Prüfer gesendet, wenn jemand explizit auf seinen Kommentar antwortet (dies schließt die eigenen Antworten auf seine eigenen Kommentare aus). Das bedeutet, dass, wenn jemand auf dem Korrekturabzug einen neuen Kommentar abgibt, der Prüfer nicht benachrichtigt wird.<p>Diese Einstellung wird für Ihre Kunden auf dem Korrekturabzug empfohlen, damit sie nicht über andere Kommentare zu dem Korrekturabzug benachrichtigt werden und nur über Antworten auf ihre eigenen Kommentare.</p><p>Reviewer mit dieser E-Mail-Warnhinweiseinstellung werden zwar nicht über andere neue Kommentare benachrichtigt, sie können jedoch alle Kommentare zum Korrekturabzug in der Proofing-Anzeige anzeigen.</p><p>Weitere Informationen zu Kommentaren finden Sie unter <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Kommentare zu Korrekturabzügen anzeigen und </a>.</p></td> 
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
        <td>Workfront sendet eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen nur an Tagen, an denen außer Ihrer eigenen Aktivität eine andere Aktivität stattfindet.<p>Dieser Warnhinweis bietet eine gute Möglichkeit, eine Zusammenfassung des Projekts anzuzeigen, ohne im Laufe des Tages durch mehrere Updates überfordert zu werden.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Abteilungsleiter, der den Gesamtfortschritt des Projekts überwachen möchte.</p><p>Weitere Informationen finden Sie unter <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Verwalten von Benachrichtigungen für Kommentare und Entscheidungen zu Korrekturabzügen</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Keine E-Mail</td> 
        <td>Workfront sendet keine E-Mail-Warnungen.<br>Dies ist für Personen nützlich, die einem Korrekturabzug nur zu Referenzzwecken hinzugefügt werden und nicht über Änderungen benachrichtigt werden müssen.<p>Der Systemstandard lautet „Tägliche Zusammenfassung“ (wird auch als „Nicht festgelegt“ angezeigt). Wenn Sie oder Ihre Prüfer keine anderen Änderungen vornehmen, haben alle Ihre Korrekturabzüge diese Einstellung.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Optional) Wiederholen Sie die beiden vorherigen Schritte, um dem Korrekturabzug mehrere Benutzer hinzuzufügen. 
1. (Optional) Legen Sie eine **Frist** für die Prüfer fest (nur verfügbar, wenn der Korrekturabzug keinen automatisierten Workflow hat).
1. (Optional) Wählen Sie **E-Mail-Benachrichtigung an neue Empfänger**, um sie darüber zu informieren, dass Sie sie zum Korrekturabzug hinzugefügt haben.
1. Wenn Sie alle weiteren Benutzenden zum Korrekturabzug hinzugefügt haben, klicken Sie auf **Fertig.**
