---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Erstellen eines erweiterten Testversands mit einem einfachen Workflow
description: Mit einem einfachen Workflow können mehrere Validierungsverantwortliche einen Testversand durchführen, diese sind jedoch nicht in Phasen unterteilt. Alle hinzugefügten Validierungsverantwortlichen können sofort nach der Erstellung auf den Testversand zugreifen.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1853'
ht-degree: 1%

---

# Erstellen eines erweiterten Testversands mit einem einfachen Workflow

<!-- Audited: 1/2024 -->

Mit einem einfachen Workflow können mehrere Validierungsverantwortliche einen Testversand durchführen, diese sind jedoch nicht in Phasen unterteilt. Alle hinzugefügten Validierungsverantwortlichen können sofort nach der Erstellung auf den Testversand zugreifen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>
   <p>Neu: Beliebig</p>
    <p>Aktueller Plan: Pro oder höher</p>
   <p>Veralteter Plan: Auswählen oder höher</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
    <p>Aktuell: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

+++

## Erstellen eines erweiterten Testversands mit einem einfachen Workflow

1. Wechseln Sie zum Projekt, zur Aufgabe oder zur Ausgabe, an der Sie den Testversand durchführen möchten, und klicken Sie dann auf die Registerkarte **Dokumente** .
1. Klicken Sie auf **Neu hinzufügen** > Testversand , laden Sie den Inhalt hoch und arbeiten Sie dann durch die unten aufgeführten Abschnitte.

   oder

   Bewegen Sie den Mauszeiger über ein vorhandenes Dokument, klicken Sie auf **Testversand erstellen** > **Erweiterter Testversand** und arbeiten Sie durch die folgenden Abschnitte.

## Workflow konfigurieren und Überprüfer hinzufügen

1. Wählen Sie im Abschnitt Workflow-Typ die Option **Einfach**.
1. Geben Sie die Benutzer an, die Sie hinzufügen möchten, und wählen Sie dann eine Proof-Rolle aus.

   ![](assets/new-proof---roles-350x213.png)

1. In der folgenden Tabelle sind alle Rollen und die damit verbundenen Rechte aufgeführt.

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
      <th> <p><strong>Anzeigen eines Testversands</strong> </p> </th> 
      <th> <p><strong>Markups hinzufügen</strong> </p> </th> 
      <th> <p><strong>Kommentare hinzufügen</strong> </p> </th> 
      <th> <p><strong>Eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind</strong> </p> </th> 
      <th> <p><strong>Entscheidungsfindung</strong> </p> </th> 
      <th> <p><strong>Kommentare anderer Benutzer löschen</strong> </p> </th> 
      <th>Kommentare auflösen</th> 
      <th>Anwenden von Aktionen auf Kommentare</th> 
      <th> <p><strong>Testversand bearbeiten</strong> </p> </th> 
      <th>Testversand für andere freigeben</th> 
      <th>Neue Version erstellen</th> 
      <th> <p><strong>Genehmigungsanforderungen im Startbereich anzeigen</strong> </p> </th> 
      <th>Hinzufügen neuer Validierungsverantwortlicher</th> 
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
      <td> <p><strong>Überprüfer und Genehmiger</strong> </p> </td> 
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
      <td> <p><strong>Autor</strong> </p> </td> 
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

1. Benutzer mit neuen Workfront-Plänen können allen Benutzern im System Autoren- oder Moderatorrollen zuweisen. Benutzer mit älteren Plänen können Autoren- oder Moderatorrollen jedem Benutzer mit einer Testversandlizenz im System zuweisen.
1. (Optional) Wenn das Dropdown-Menü noch geöffnet ist, wählen Sie alle zusätzlichen Berechtigungen aus, die unten im Menü verfügbar sind:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kommentare auflösen und Aktionen anwenden </td> 
      <td> <p>Ermöglicht dem Workfront-Benutzer Folgendes:</p> 
       <ul> 
        <li>Beheben Sie einen Kommentar, nachdem er bearbeitet wurde, wie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Testversand-Kommentare auflösen</a> beschrieben.</li> 
        <li>Wenden Sie Aktionen auf Kommentare an, wie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Aktionen für Testkommentare verwenden</a> beschrieben. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Korrekturabzug durch Taggen teilen</td> 
      <td> <p>Ermöglicht dem Validierer das Hinzufügen eines beliebigen Workfront-Benutzers zum Testversand, wie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Benutzer taggen, um einen Testversand freizugeben</a> beschrieben.</p> <p>Hinweis:  <p>Wenn diese beiden Optionen nicht verfügbar sind (abgeblendet), verfügt der Benutzer bereits über ein Berechtigungsprofil, das das Auflösen von Kommentaren, das Anwenden von Aktionen auf Kommentare und das Taggen von Benutzern ermöglicht. </p> <p>Wenn die Optionen nicht angezeigt werden, ist die hinzugefügte Person kein Workfront-Lizenzinhaber.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Wiederholen Sie die Schritte 1 bis 3 für alle anderen Benutzer, die Sie zum Testversand hinzugefügt haben.
1. Wählen Sie für jeden Benutzer, für den Sie eine Freigabe durchführen, in der Dropdown-Liste **E-Mail-Warnungen** den Typ der E-Mail-Warnungen aus, die dieser Benutzer erhält, wenn er Kommentare und Entscheidungen zum Testversand trifft:

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

1. Fahren Sie mit [E-Mail-Einstellungen für den Testversand konfigurieren](#configure-email-settings-for-the-proof) weiter unten.

## E-Mail-Einstellungen für den Testversand konfigurieren {#configure-email-settings-for-the-proof}

1. Wählen Sie im Abschnitt **E-Mail-Benachrichtigung** aus, ob Sie E-Mail-Benachrichtigungen und eine benutzerdefinierte Nachricht an die Benutzer senden möchten, die Sie zuvor in [Erstellen eines erweiterten Testversands mit einem einfachen Workflow](#workflow) ausgewählt haben:

   <table>
   <tbody>
   <tr>
   <td>Empfänger über diesen Testversand informieren</td>
   <td>Wählen Sie diese Option, um eine E-Mail-Benachrichtigung an Benutzer zu senden. Wenn im Abschnitt <strong>Workflow</strong> die Option <strong>Grundlegende Freigabe</strong> ausgewählt ist, wird bei der Erstellung des Testversands eine E-Mail-Benachrichtigung gesendet. Wenn im Abschnitt <strong>Workflow</strong> die Option <strong>Automatisierter Workflow</strong> ausgewählt ist, wird eine E-Mail-Benachrichtigung gesendet, wenn der Testversand in die Phase des automatisierten Workflows gelangt, mit der der Benutzer verknüpft ist.</td>
   </tr>
   <tr>
   <td>Benutzerdefinierte Nachricht hinzufügen</td>
   <td>Wählen Sie diese Option aus, um eine benutzerdefinierte Nachricht in die Benachrichtigung einzuschließen. Sie können einen Betreff und einen Nachrichtentext angeben. Der Nachrichtentext kann Rich-Text-Formatierungen wie Fett, Aufzählungszeichen und Hyperlinks enthalten.</td>
   </tr>
   </tbody>
   </table>


1. Fahren Sie mit [Konfigurieren Sie die Testversandeinstellungen](#configure-proof-settings) weiter unten.

## Konfigurieren der Testversandeinstellungen {#configure-proof-settings}

1. Wählen Sie im Abschnitt **Testversandeinstellungen** eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anmeldung erforderlich - Testversand kann nur für andere Benutzer freigegeben werden</td> 
      <td>Wenn diese Option deaktiviert ist (Standard), kann jeder mit der URL den Testversand anzeigen. <br>Wenn diese Option ausgewählt ist:
       <ul>
        <li>Nur Workfront Proof-Benutzer können den Testversand anzeigen.</li>
        <li>Benutzer können sich nur dann beim Testversand anmelden, wenn sie zum Testversand hinzugefügt wurden.</li>
        <li>Abonnements können nicht aktiviert werden.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur eine Entscheidung für diesen Testversand erforderlich</td> 
      <td>Wenn diese Option ausgewählt ist, wird die Überprüfung abgeschlossen, nachdem einer der Entscheidungsträger seine Entscheidung getroffen hat.<br>Diese Option ist standardmäßig deaktiviert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidungen müssen elektronisch signiert werden</td> 
      <td>Benutzer müssen ihren Benutzernamen und ihr Kennwort zum Zeitpunkt der Entscheidung über einen Testversand angeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sperren des Testversands, wenn alle erforderlichen Entscheidungen getroffen werden</td> 
      <td>Wenn diese Einstellung aktiviert ist, wird der Testversandstatus gesperrt, nachdem alle Entscheidungen getroffen wurden. Der Status wird automatisch von entsperrt in gesperrt geändert, wenn der endgültige Genehmiger seine Entscheidung trifft.<br>Diese Option ist standardmäßig deaktiviert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Originaldatei herunterladen</td> 
      <td>Wenn diese Option aktiviert ist, können die validierungsverantwortlichen Benutzer die Originaldatei herunterladen, aus der der Testversand erstellt wurde.<br>Wenn diese Option deaktiviert ist, ist das Symbol Herunterladen nicht mehr sichtbar.<br>Diese Option ist standardmäßig aktiviert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Freigeben des Testversands über eine öffentliche URL oder einen Einbettungscode</td> 
      <td>Wenn diese Option aktiviert ist, kann der Testversand über eine öffentliche URL oder einen Einbettungscode freigegeben werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Testversand über öffentliche URL oder Einbettungscode abonnieren</td> 
      <td>Wenn diese Option aktiviert ist, können Personen, die dem Testversand nicht explizit hinzugefügt wurden, den Testversand abonnieren. Die Person, die den Testversand abonniert, erhält die Rolle und E-Mail, die Sie in den folgenden Einstellungen definieren:
       <ul>
        <li><strong>Abonnentenrolle:</strong> Die Standardrolle für den Testversand, die allen Validierern zugewiesen ist, die den Testversand abonnieren. </li>
        <li><strong>E-Mail-Warnhinweiseinstellungen für Abonnenten:</strong> Der Standard-E-Mail-Warnhinweis, der allen Validierern zugewiesen wird, die den Testversand abonnieren.</li>
       </ul><p>
        <ul>
         <li><strong> Nachweis des Zugriffs über einen E-Mail-Link erforderlich:</strong> Konfigurieren Sie, ob der Abonnent eine E-Mail mit einem Link zum Testversand erhält. Sie können "<strong>Keine E-Mail</strong>"(für den Testversand ist kein E-Mail-Link erforderlich), "<strong>Nur E-Mail-Testversand</strong>"(Abonnenten erhalten einen Link zum Testversand per E-Mail ohne Überprüfung) oder "<strong>E-Mail-Benachrichtigung zur Validierung und zum Testversand</strong>"(Abonnenten erhalten per E-Mail einen Link und müssen auf den Link klicken, um einen Testversand anzuzeigen). Diese Option dient dazu, um sicherzustellen, dass die richtige E-Adresse angegeben wird , auf die sie Zugriff haben).</li>
        </ul><p>Hinweis:  Wenn die Testsendungen den automatisierten Workflow angehängt haben, generieren alle Abonnements Bestätigungs-E-Mails an die Testversand-Inhaber, sodass diese entscheiden können, zu welcher Stufe die Person hinzugefügt werden soll.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Testversand erstellen**.

   Workfront beginnt mit der Erstellung eines Testversands der ausgewählten Dokumente oder Websites. Je nach Dateigröße und Typ kann die Zeitverzögerung beim Hochladen von Dokumenten variieren. Seien Sie geduldig, da die Erzeugung größerer Dateien länger dauert. Sie können von der Seite weg navigieren und Workfront generiert weiterhin Ihre -Datei. Die maximale Größe für den Datei-Upload beträgt 4 GB.

1. Nachdem der Testversand erstellt wurde, klicken Sie auf **Testversand öffnen** , um den Testversand-Viewer zu starten.

   ![](assets/open-proof-350x132.png)

   Benutzer, für die die Testversandfunktion nicht aktiviert wurde, können das Dokument weiterhin ansehen und Kommentare zum Testversand abgeben.