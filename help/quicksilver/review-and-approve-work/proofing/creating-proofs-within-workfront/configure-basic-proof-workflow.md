---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow
description: Mit einem einfachen Workflow können Sie mehrere Prüfer zu einem Korrekturabzug hinzufügen, sie sind jedoch nicht in Phasen unterteilt. Alle Reviewer, die Sie hinzufügen, können sofort nach der Erstellung auf den Korrekturabzug zugreifen.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1793'
ht-degree: 4%

---

# Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow

<!-- Audited: 1/2024 -->

Mit einem einfachen Workflow können Sie mehrere Prüfer zu einem Korrekturabzug hinzufügen, sie sind jedoch nicht in Phasen unterteilt. Alle Reviewer, die Sie hinzufügen, können sofort nach der Erstellung auf den Korrekturabzug zugreifen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>
   <p>Beliebig</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
    <p>Arbeit oder Plan</p> </td> 
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

## Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem bzw. dem Sie den Korrekturabzug anzeigen möchten, und klicken Sie dann auf die Registerkarte **Dokumente**.
1. Klicken Sie **Neu hinzufügen** > Testversand, laden Sie den Inhalt hoch und bearbeiten Sie dann die unten aufgeführten Abschnitte.

   oder

   Bewegen Sie den Mauszeiger über ein vorhandenes Dokument, klicken Sie dann auf **Korrekturabzug erstellen** > **Erweiterter**) und durchlaufen Sie die unten aufgeführten Abschnitte.

## Konfigurieren des Workflows und Hinzufügen von Reviewern

1. Wählen Sie im Abschnitt Workflow-Typ die Option **Allgemein**.
1. Geben Sie die Benutzer an, die Sie hinzufügen möchten, und wählen Sie dann die Rolle Testversand aus.

   ![Neue Korrekturabzug-Rollen](assets/new-proof---roles-350x213.png)

1. In der folgenden Tabelle sind die einzelnen Rollen und die damit verbundenen Rechte aufgeführt.

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>Korrekturabzug anzeigen</strong> </p> </th> 
      <th> <p><strong>Hinzufügen von Markierungen</strong> </p> </th> 
      <th> <p><strong>Kommentare hinzufügen</strong> </p> </th> 
      <th> <p><strong>Eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind</strong> </p> </th> 
      <th> <p><strong>Entscheidung treffen</strong> </p> </th> 
      <th> <p><strong>Löschen von Kommentaren anderer</strong> </p> </th> 
      <th>Kommentare auflösen</th> 
      <th>Aktionen auf Kommentare anwenden</th> 
      <th> <p><strong>Bearbeiten des Korrekturabzugs</strong> </p> </th> 
      <th>Korrekturabzug für andere freigeben</th> 
      <th>Neue Version erstellen</th> 
      <th> <p><strong>Anzeigen von Genehmigungsanfragen im Bereich „Startseite“</strong> </p> </th> 
      <th>Neue Reviewer hinzufügen</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Schreibgeschützt</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Prüfer</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Genehmigende Person</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Prüfer und genehmigende Person</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>author</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Moderator</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. Benutzende mit neuen Workfront-Plänen können allen Benutzenden im System Autoren- oder Moderatorrollen gewähren. Benutzer mit älteren Plänen können Autoren- oder Moderatorrollen an jeden Benutzer mit einer Proof-Lizenz im System vergeben.
1. (Optional) Wählen Sie bei weiterhin geöffnetem Dropdown-Menü unten im Menü alle verfügbaren zusätzlichen Berechtigungen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Auflösen von Kommentaren und Anwenden von Aktionen </td> 
      <td> <p>Ermöglicht dem Workfront-Benutzer Folgendes:</p> 
       <ul> 
        <li>Lösen Sie einen Kommentar nach der Adressierung auf, wie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Korrekturabzugskommentare auflösen</a> erläutert.</li> 
        <li>Wenden Sie Aktionen auf Kommentare an, wie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Verwenden von Aktionen für Korrekturabzugskommentare</a> erläutert. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Korrekturabzug durch Taggen teilen</td> 
      <td> <p>Ermöglicht dem Prüfer, dem Korrekturabzug beliebige Workfront-Benutzende hinzuzufügen, wie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Freigeben eines Korrekturabzugs durch Benutzende von Tags</a> beschrieben.</p> <p>Hinweis:  <p>Wenn diese beiden Optionen nicht verfügbar (abgeblendet) sind, verfügt der Benutzer bereits über ein Berechtigungsprofil, das das Auflösen von Kommentaren, das Anwenden von Aktionen auf Kommentare und das Tagging von Benutzern ermöglicht. </p> <p>Wenn die Optionen nicht angezeigt werden, ist die hinzugefügte Person kein Workfront-Lizenzinhaber.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Wiederholen Sie die Schritte 1 bis 3 für alle anderen Benutzer, die Sie dem Korrekturabzug hinzugefügt haben.
1. Wählen Sie für jeden Benutzer, den Sie freigeben, in der Dropdown-Liste **E-Mail** den E-Mail-Warnhinweistyp aus, den dieser Benutzer erhält, wenn Benutzer Kommentare zum Korrekturabzug eingeben und Entscheidungen treffen:

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

1. Fahren Sie mit [E-Mail-Einstellungen für den Korrekturabzug konfigurieren](#configure-email-settings-for-the-proof) unten fort.

## E-Mail-Einstellungen für den Testversand konfigurieren {#configure-email-settings-for-the-proof}

1. Wählen Sie im Abschnitt **E-Mail** Benachrichtigung) aus, ob Sie E-Mail-Benachrichtigungen und eine benutzerdefinierte Nachricht an die Benutzerinnen und Benutzer senden möchten, die Sie zuvor in [Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow](#workflow) in diesem Artikel ausgewählt haben:

   <table>
   <tbody>
   <tr>
   <td>Empfänger über diesen Korrekturabzug benachrichtigen</td>
   <td>Wählen Sie diese Option, um Benutzern eine E-Mail-Benachrichtigung zu senden. Wenn <strong>Einfache Freigabe</strong> im Abschnitt <strong>Workflow</strong> ausgewählt ist, wird bei der Erstellung des Korrekturabzugs eine E-Mail-Benachrichtigung gesendet. Wenn <strong>Automatisierter Workflow</strong> im Abschnitt <strong>Workflow</strong> ausgewählt ist, wird eine E-Mail-Benachrichtigung gesendet, wenn der Korrekturabzug in den Schritt des automatisierten Workflows eintritt, mit dem der Benutzer verknüpft ist.</td>
   </tr>
   <tr>
   <td>Benutzerdefinierte Nachricht hinzufügen</td>
   <td>Wählen Sie diese Option, um eine benutzerdefinierte Nachricht in die Benachrichtigung aufzunehmen. Sie können einen Betreff und einen Nachrichtentext angeben. Der Nachrichtentext kann Rich-Text-Formatierungen wie fett, Aufzählungszeichen und Hyperlinks enthalten.</td>
   </tr>
   </tbody>
   </table>


1. Fahren Sie mit [Testversandeinstellungen konfigurieren](#configure-proof-settings) unten fort.

## Konfigurieren der Einstellungen für Korrekturabzüge {#configure-proof-settings}

1. Wählen Sie **Abschnitt** Korrekturabzugseinstellungen“ eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anmeldung verlangen - Korrekturabzug kann nur für andere Benutzer freigegeben werden</td> 
      <td>Wenn diese Option deaktiviert ist (Standard), kann jeder Benutzer mit der URL den Korrekturabzug anzeigen. <br>Wenn diese Option ausgewählt ist:
       <ul>
        <li>Nur Workfront Proof-Benutzende können den Korrekturabzug anzeigen.</li>
        <li>Benutzende können sich nur dann beim Korrekturabzug anmelden, wenn sie zum Korrekturabzug hinzugefügt wurden.</li>
        <li>Abonnements können nicht aktiviert werden.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Für diesen Korrekturabzug ist nur eine Entscheidung erforderlich</td> 
      <td>Wenn diese Option ausgewählt ist, wird die Überprüfung abgeschlossen, nachdem einer der Entscheidungsträger seine Entscheidung getroffen hat.<br>Diese Option ist standardmäßig deaktiviert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidungen müssen elektronisch signiert werden</td> 
      <td>Benutzer müssen ihren Benutzernamen und ihr Kennwort angeben, wenn sie sich für einen Korrekturabzug entscheiden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Korrekturabzug sperren, wenn alle erforderlichen Entscheidungen getroffen werden</td> 
      <td>Wenn diese Einstellung aktiviert ist, wird der Status des Korrekturabzugs gesperrt, nachdem alle Entscheidungen getroffen wurden. Der Status wird automatisch von entsperrt in gesperrt geändert, wenn die endgültige genehmigende Person ihre Entscheidung trifft.<br>Diese Option ist standardmäßig deaktiviert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Originaldatei herunterladen</td> 
      <td>Wenn diese Option ausgewählt ist, können Prüfer die Originaldatei, aus der der Korrekturabzug erstellt wurde, herunterladen.<br>Wenn diese Option deaktiviert ist, ist das Download-Symbol nicht mehr sichtbar.<br>Diese Option ist standardmäßig aktiviert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Korrekturabzug über öffentliche URL oder eingebetteten Code freigeben</td> 
      <td>Wenn diese Option ausgewählt ist, kann der Korrekturabzug über eine öffentliche URL oder einen Einbettungs-Code freigegeben werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Testversand über öffentliche URL oder Einbettungs-Code abonnieren</td> 
      <td>Wenn diese Option ausgewählt ist, können Personen, die dem Korrekturabzug nicht explizit hinzugefügt wurden, den Korrekturabzug abonnieren. Der Person, die den Korrekturabzug abonniert, wird die Rolle und die E-Mail-Adresse zugewiesen, die Sie in den folgenden Einstellungen definieren:
       <ul>
        <li><strong>Abonnentenrolle</strong> Die Standardrolle für den Korrekturabzug, die allen Reviewern zugewiesen ist, die den Korrekturabzug abonnieren. </li>
        <li><strong>E-Mail-Warnhinweiseinstellungen für Abonnenten:</strong> Der E-Mail-Warnhinweis, der standardmäßig allen Reviewern zugewiesen wird, die den Testversand abonniert haben.</li>
       </ul><p>
        <ul>
         <li><strong>Zugriff auf Korrekturabzug über einen E-Mail-Link erforderlich für</strong> Konfigurieren Sie, ob der Abonnent eine E-Mail mit einem Link zum Korrekturabzug erhält. Sie können zwischen <strong>Keine E-Mail</strong> (für den Zugriff auf den Korrekturabzug ist kein E-Mail-Link erforderlich), <strong>Nur E-Mail-Benachrichtigung über den Korrekturabzug</strong> (der Abonnent erhält einen Link zum Korrekturabzug per E-Mail ohne Bestätigung) oder <strong>E-Mails zur Validierung und </strong> des Korrekturabzugs (der Abonnent erhält einen Link zum Korrekturabzug per E-Mail und muss auf den Link klicken, um auf den Korrekturabzug zuzugreifen. Diese Option dient dazu, sicherzustellen, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, auf die er Zugriff hat).</li>
        </ul><p>Hinweis:  Wenn an die Korrekturabzüge ein automatisierter Workflow angehängt ist, generieren alle Abonnements Bestätigungs-E-Mails an die Verantwortlichen des Korrekturabzugs, damit sie entscheiden können, zu welchem Schritt die Person hinzugefügt werden soll.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Korrekturabzug erstellen**.

   Workfront erstellt nun einen Korrekturabzug für die ausgewählten Dokumente oder Websites. Je nach Dateigröße und -typ kann die Verzögerungszeit beim Hochladen eines Dokuments variieren. Seien Sie geduldig, da die Generierung größerer Dateien länger dauert. Wenn Sie die Seite verlassen, erstellt Workfront weiterhin die Datei. Die maximale Größe des Datei-Uploads beträgt 4 GB.

1. Klicken Sie nach der Erstellung des Korrekturabzugs auf **Korrekturabzug öffnen**, um die Korrekturabzugsansicht zu starten.

   ![Korrekturabzug öffnen](assets/open-proof-350x132.png)

   Benutzer, für die das Proofing nicht aktiviert ist, können weiterhin das Dokument anzeigen und Kommentare zum Korrekturabzug abgeben.
