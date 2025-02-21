---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow
description: Ein automatisierter Workflow erleichtert die Verwaltung des Überprüfungsprozesses, wenn Ihr Prozess komplex ist oder wenn Sie Inhalte regelmäßig zur Überprüfung an dieselben Personen senden. Der Korrekturabzug wechselt von Schritt zu Schritt und Adobe Workfront benachrichtigt jeden Benutzer, wenn er an der Reihe ist, ihn zu überprüfen. Weitere Informationen zu automatisierten Workflows finden Sie unter Automatisierte Workflows - Übersicht.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow

<!-- Audited: 2/2024 -->

Ein automatisierter Workflow erleichtert die Verwaltung des Überprüfungsprozesses, wenn Ihr Prozess komplex ist oder wenn Sie Inhalte regelmäßig zur Überprüfung an dieselben Personen senden. Der Korrekturabzug wechselt von Schritt zu Schritt und Adobe Workfront benachrichtigt jeden Benutzer, wenn er an der Reihe ist, ihn zu überprüfen. Weitere Informationen zu automatisierten Workflows finden Sie unter [Automatisierter Workflow - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Neu: Beliebig</p><p>Aktueller Plan: Pro oder höher</p><p>Legacy-Plan: Auswählen oder höher</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p><p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem bzw. dem Sie den Korrekturabzug anzeigen möchten, und klicken Sie dann auf die Registerkarte **Dokumente**.
1. Klicken Sie **Neu hinzufügen** > Testversand, laden Sie den Inhalt hoch und bearbeiten Sie dann die unten aufgeführten Abschnitte.

   oder

   Bewegen Sie den Mauszeiger über ein vorhandenes Dokument, klicken Sie dann auf **Korrekturabzug erstellen** > **Erweiterter**) und durchlaufen Sie die unten aufgeführten Abschnitte.

## Konfigurieren der Testversand-Phasen

1. Wählen Sie im Abschnitt Workflow-Typ die Option **Automated**.
1. (Optional) Wenn Sie eine automatisierte Workflow-Vorlage verwenden möchten, die Ihr Workfront-Administrator erstellt und für Sie freigegeben hat, klicken Sie auf **Vorlage hinzufügen** wählen Sie die Vorlage in dem angezeigten Feld aus und klicken Sie dann auf **Vorlage hinzufügen**.

   >[!NOTE]
   >
   >Beachten Sie bei der Verwendung einer automatisierten Workflow-Vorlage Folgendes:
   >   
   >* Die Einstellungen einer automatisierten Workflow-Vorlage bestimmen, was Sie mit dem automatisierten Workflow für einen Korrekturabzug tun können. Wenn zum Beispiel die Schaltfläche Schritt hinzufügen in der Vorlage deaktiviert ist, wird sie nicht angezeigt, wenn Sie mit den Einstellungen des automatisierten Workflows für den Korrekturabzug arbeiten.
   >* Wenn eine Person zu einer Phase in einer automatisierten Workflow-Vorlage hinzugefügt wird, aber auch bereits als Prüferin bzw. Prüfer im Korrekturabzug vorhanden ist, wird sie durch Anwenden der Vorlage von der Phase entfernt. Wenn Sie keinen weiteren Validierungsverantwortlichen zum Schritt hinzufügen, werden Sie in einer Meldung aufgefordert, einen hinzuzufügen.
   >* Ihre Möglichkeit, eine Vorlage für einen automatisierten Workflow zu ändern, hängt von den Vorlageneinstellungen ab, die vom Workfront-Administrator konfiguriert wurden, wie in beschrieben. Wenn die Möglichkeit, die Vorlage zu ändern, deaktiviert ist, kann nur der Besitzer der Vorlage sie ändern.

1. Konfigurieren Sie die erste Phase des automatisierten Workflows:

   1. (Optional) Wenn Sie einen Namen für das erste Stadium erstellen möchten, klicken Sie auf **Stadium 1** und geben Sie dann den Namen ein.
   1. Fügen Sie im **Empfänger** für die Phase Validierungsverantwortliche zur Phase hinzu.

      >[!NOTE]
      >
      >Beachten Sie Folgendes, wenn Sie Reviewer zu einem Schritt hinzufügen:
      >   
      >* Sie können externe Benutzer zu einem Schritt mit einer E-Mail-Adresse hinzufügen.
      >* Nachdem Sie einen Benutzer zu einem Schritt hinzugefügt haben, können Sie Einstellungen für diesen Benutzer im Korrekturabzug konfigurieren.
      >* Sie können Benutzer direkt in eine andere Phase ziehen oder Benutzer in eine Phase auf dem Diagramm **Phasen** ziehen. Drücken Sie zum Auswählen mehrerer Benutzer Umschalt+Strg (unter Windows) oder Umschalt+Befehl (unter Mac).
      >* Sie können einem Korrekturabzug nur einmal einen Prüfer hinzufügen. Das bedeutet, dass Sie dieselbe Person nicht zu mehr als einem Schritt im Korrekturabzug hinzufügen können.
      >* Prüfer, die nicht zu einer privaten Phase hinzugefügt wurden, können diese Phase nicht im Korrekturabzug oder in Kommentaren sehen, die in dieser Phase gemacht wurden.
      >* Standardmäßig gewährt das Hinzufügen eines Benutzers zu einem Schritt diesem Benutzer Zugriff, um den Korrekturabzug ab dem Zeitpunkt anzuzeigen, zu dem der Korrekturabzug erstellt wird. Ihr Workfront-Administrator kann Benutzende vom Zugriff auf den Korrekturabzug ausschließen, bis der Workflow in das Stadium eintritt, in dem der/die Benutzende hinzugefügt wurde.

   1. Klicken Sie auf **Staging-Einstellungen**.
   1. Klicken Sie auf **Option** Phase aktivieren“, um anzugeben, wie die Phase aktiviert werden soll.

      Im ersten Schritt können Sie nur „Bei **Korrekturabzugs-Erstellung**, **An einem bestimmten Datum und zu einer bestimmten Uhrzeit** oder **Manuell** auswählen.

   1. (Bedingt) Wenn Sie im vorherigen Schritt **An einem bestimmten Datum und zu einer bestimmten Uhrzeit** ausgewählt haben, wählen Sie das Datum und die Uhrzeit für die Aktivierung des Schritts im angezeigten **Aktivieren** aus.

   1. Verwenden Sie eine der folgenden Optionen, um das Stadium weiter zu konfigurieren.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Stadium-Deadline festlegen</td>
         <td><p>Um einen Termin für die Phase festzulegen, klicken Sie auf eine Option in <strong> Dropdown-Liste "</strong>". Führen <strong> dann unter "</strong>" einen der folgenden Schritte aus:</p>
          <ul>
           <li>Bei Auswahl von <strong>Spezifisches Datum festlegen</strong> wählen Sie das gewünschte Datum und die gewünschte Uhrzeit für die Frist aus.</li>
           <li>Bei Auswahl von <strong>Ab Staging-Aktivierungsdatum berechnen</strong> wählen Sie die Anzahl der Werktage, die Sie zum Staging-Aktivierungsdatum hinzufügen möchten, um die Frist zu bestimmen.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Schleusenbühne</td>
         <td>Geben Sie an, wann das Stadium gesperrt werden kann. </td>
        </tr>
        <tr>
         <td role="rowheader">Übertragen von primären Entscheidungsrechten an</td>
         <td><p>Wählen Sie den Primären Entscheidungsträger auf der Bühne aus (nur verfügbar, nachdem Sie mindestens eine Person zur Bühne hinzugefügt haben, die die Rolle einer genehmigenden Person oder höher für Korrekturabzüge hat). Wenn Sie einen Primären Entscheidungsträger auswählen, ist die Option <strong>Nur eine Entscheidung erforderlich</strong> in diesem Schritt deaktiviert.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Nur eine Entscheidung für diese Phase verlangen</td>
         <td>Beendet den gesamten Überprüfungsprozess, wenn einer der Entscheidungsträger eine Entscheidung trifft.<p>Diese Option ist nicht verfügbar, wenn Sie im Dropdownmenü <strong>Primärer Entscheidungsträger</strong> einen Benutzer angegeben haben.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Diese Phase als privat festlegen</td>
         <td>Ermöglicht nur den folgenden Personen, Kommentare und Entscheidungen anzuzeigen, die in dieser Phase getroffen wurden: Supervisoren, Workfront-Administratoren und Workfront Proof-Administratoren</td>
        </tr>
       </tbody>
      </table>

1. So fügen Sie einen weiteren Schritt hinzu und konfigurieren ihn:

   1. Klicken Sie auf **Neues Stadium**.
   1. (Optional) Wenn Sie einen Namen für das erste Stadium erstellen möchten, klicken Sie auf **Stadium 2** (oder **Stadium 3**, **Stadium 4** usw.) und geben Sie dann den Namen ein.

   1. Klicken Sie auf **Phase aktivieren** und wählen Sie dann eine Option aus, um anzugeben, ob die Phase automatisch oder manuell aktiviert werden soll.

      Zusätzlich zu den Optionen **Bei der Erstellung eines Korrekturabzugs**, **An einem bestimmten Datum und zu einer bestimmten Uhrzeit** oder **Manuell** können Sie eine Option auswählen, die von dem abhängt, was im vorherigen Schritt aufgetreten ist:

      ![Aktivieren von Staging-Optionen](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Wenn Sie eine Option Phase aktivieren ausgewählt haben, die von dem abhängt, was im vorherigen Schritt geschehen ist, verwenden Sie die Optionen, die angezeigt werden, um die Aktivierungseinstellung zu konfigurieren.

      Wenn Sie beispielsweise **Wenn sich der Status des vorherigen Schritts ändert** ausgewählt haben, wählen Sie das Feld **Vorheriges** aus und wählen Sie dann den Status im Feld **Status geändert zu** aus.

1. Wiederholen Sie den vorherigen Schritt nach Bedarf, um weitere Stadien hinzuzufügen.

   Wenn Sie dem automatisierten Workflow Stadien hinzufügen, wird auf dem Bildschirm ein Diagramm erstellt, das diese Stadien darstellt:

   ![Stadiendiagramm](assets/stages-diagram-350x213.png)

1. Fahren Sie mit [E-Mail-Einstellungen für den Korrekturabzug konfigurieren](#configure-email-settings-for-the-proof) unten fort.

## E-Mail-Einstellungen für den Testversand konfigurieren {#configure-email-settings-for-the-proof}

1. Wählen Sie im Abschnitt **E-Mail** Benachrichtigung) aus, ob Sie E-Mail-Benachrichtigungen und eine benutzerdefinierte Nachricht an die Benutzerinnen und Benutzer senden möchten, die Sie zuvor in [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](#workflow) in diesem Artikel ausgewählt haben:

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
        <li><strong>Abonnentenrolle</strong> Die Standardrolle für den Korrekturabzug, die allen Reviewern zugewiesen ist, die den Korrekturabzug abonnieren.</li>
        <li><strong>E-Mail-Warnhinweiseinstellungen für Abonnenten:</strong> Der E-Mail-Warnhinweis, der standardmäßig allen Reviewern zugewiesen wird, die den Testversand abonniert haben.</li>
       </ul><p>
        <ul>
         <li><strong>Zugriff auf Korrekturabzug über einen E-Mail-Link erforderlich für</strong> Konfigurieren Sie, ob der Abonnent eine E-Mail mit einem Link zum Korrekturabzug erhält. Sie können zwischen <strong>Keine E-Mail</strong> (für den Zugriff auf den Korrekturabzug ist kein E-Mail-Link erforderlich), <strong>Nur E-Mail-Benachrichtigung über den Korrekturabzug</strong> (der Abonnent erhält einen Link zum Korrekturabzug per E-Mail ohne Bestätigung) oder <strong>E-Mails zur Validierung und </strong> des Korrekturabzugs (der Abonnent erhält einen Link zum Korrekturabzug per E-Mail und muss auf den Link klicken, um auf den Korrekturabzug zuzugreifen. Diese Option dient dazu, sicherzustellen, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, auf die er Zugriff hat).</li>
        </ul><p><strong>Hinweis:</strong> Wenn an die Korrekturabzüge ein automatisierter Workflow angehängt ist, generieren alle Abonnements Bestätigungs-E-Mails an die Testversand-Verantwortlichen, damit diese entscheiden können, zu welchem Schritt die Person hinzugefügt werden soll.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Korrekturabzug erstellen**.

   Workfront erstellt nun einen Korrekturabzug für die ausgewählten Dokumente oder Websites. Je nach Dateigröße und -typ kann die Verzögerungszeit beim Hochladen eines Dokuments variieren. Seien Sie geduldig, da die Generierung größerer Dateien länger dauert. Wenn Sie die Seite verlassen, erstellt Workfront weiterhin die Datei. Die maximale Größe des Datei-Uploads beträgt 4 GB.

1. Klicken Sie nach der Erstellung des Korrekturabzugs auf **Korrekturabzug öffnen**, um die Korrekturabzugsansicht zu starten.

   ![Korrekturabzug öffnen](assets/open-proof-350x132.png)

   Benutzer, für die das Proofing nicht aktiviert ist, können weiterhin das Dokument anzeigen und Kommentare zum [ machen.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
