---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Erstellen oder Bearbeiten eines automatisierten Workflows für einen vorhandenen Testversand
description: Automatisierte Workflows erleichtern die Verwaltung des Überprüfungsprozesses, wenn Ihr Prozess komplex ist oder Sie regelmäßig Inhalte zur Überprüfung an dieselben Personengruppen senden. Wenn Sie einen Testversand mit einem automatisierten Workflow erstellen, wechselt der Testversand von Phase zu Phase bis zur endgültigen Genehmigung. Teilnehmer werden benachrichtigt, wenn sie an der Reihe sind, das Dokument zu überprüfen.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 1%

---

# Erstellen oder Bearbeiten eines automatisierten Workflows für einen vorhandenen Testversand

Automatisierte Workflows erleichtern die Verwaltung des Überprüfungsprozesses, wenn Ihr Prozess komplex ist oder Sie regelmäßig Inhalte zur Überprüfung an dieselben Personengruppen senden. Wenn Sie einen Testversand mit einem automatisierten Workflow erstellen, wechselt der Testversand von Phase zu Phase bis zur endgültigen Genehmigung. Teilnehmer werden benachrichtigt, wenn sie an der Reihe sind, das Dokument zu überprüfen.

Informationen zum Erstellen eines automatisierten Workflows für einen neuen Testversand finden Sie unter [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Erstellen oder bearbeiten Sie einen automatisierten Workflow für einen vorhandenen Testversand:

1. Bewegen Sie den Mauszeiger über das Dokument im Bereich &quot;Dokumente&quot;und klicken Sie dann auf &quot;Testversand-Workflow&quot;.

   Oder

   Wenn Sie den Testversand im Testversand-Viewer überprüfen, klicken Sie im linken Bedienfeld auf **Workflow** ![](assets/workflow-icon-proofing-viewer.png) und dann auf das Bearbeitungssymbol ![](assets/edit-icon-proofing-viewer.png) , um die Einstellungen für den automatisierten Workflow für den Testversand zu öffnen.

1. (Bedingt) Wenn der Testversand derzeit einen einfachen Workflow (ohne Phasen) verwendet, klicken Sie im angezeigten Bildschirm auf **In automatisierten Workflow konvertieren** .

   >[!NOTE]
   >
   >Sie können den ersten Schritt nicht bearbeiten, wenn Sie von einem einfachen Workflow in einen automatisierten Workflow konvertieren. Sie können jedoch neue Phasen hinzufügen und konfigurieren.

1. (Bedingt) Um eine Vorlage für einen automatisierten Workflow zu verwenden, die Ihr Adobe Workfront-Administrator erstellt und für Sie freigegeben hat, klicken Sie auf **Vorlage hinzufügen**, wählen Sie die Vorlage im angezeigten Feld aus und klicken Sie dann auf **Vorlage hinzufügen**.

   Weitere Informationen finden Sie unter [Über die Verwendung von Vorlagen für automatisierte Workflows](#about-using-automated-workflow-templates) in diesem Artikel.

1. Fügen Sie dem automatisierten Workflow eine Bühne hinzu:

   1. Klicken Sie oben rechts auf **Neue Phase**.
   1. Geben Sie in das angezeigte Feld einen **Namen** für die Bühne ein.
   1. (Optional) Legen Sie einen Termin für die Phase fest.
   1. Wählen Sie im Abschnitt **Phase aktivieren** aus, wie die Bühne aktiviert werden soll:


      <table>
      <tbody>
      <tr>
      <td><strong>Erstellen eines Testversands</strong></td>
      <td>Die Bühne wird automatisch aktiviert, da der Testversand bereits erstellt wurde.</td>
      </tr>
      <tr>
      <td><strong>Nach Ablauf der Frist für die vorige Phase</strong></td>
      <td>Klicken Sie in der Dropdownliste <strong>Übergeordnete Phase</strong> auf die vorherige Phase .</td>
      </tr>
      <tr>
      <td><strong>An einem bestimmten Datum und zu einer bestimmten Uhrzeit</strong></td>
      <td>Klicken Sie auf das Feld <strong>An</strong> , um das Datum auszuwählen, und klicken Sie dann auf das Feld rechts, um die Zeit auszuwählen.</td>
      </tr>
      <tr>
      <td><strong>Alle Entscheidungen werden mit Änderungen in der übergeordneten Phase genehmigt oder genehmigt</strong></td>
      <td>Klicken Sie in der Dropdownliste <strong>Übergeordnete Phase</strong> auf die übergeordnete Phase.</td>
      </tr>
      <tr>
      <td><strong>Alle Entscheidungen werden in der übergeordneten Phase genehmigt</strong></td>
      <td>Klicken Sie in der Dropdownliste <strong>Übergeordnete Phase</strong> auf die übergeordnete Phase.</td>
      </tr>
      <tr>
      <td><strong>Alle Entscheidungen werden getroffen</strong></td>
      <td>Klicken Sie in der Dropdownliste <strong>Übergeordnete Phase</strong> auf die übergeordnete Phase.</td>
      </tr>
      </tbody>
      </table>


   1. Geben Sie einen Kontaktnamen oder eine E-Mail-Adresse ein und konfigurieren Sie Einstellungen für Prüfer für die Phase.

      Informationen zum Hinzufügen von Validierungsverantwortlichen finden Sie unter [Über das Hinzufügen von Validierern zu einer Phase](#about-adding-reviewers-to-a-stage) in diesem Artikel.

   1. Verwenden Sie eine der folgenden Optionen, um die Phase weiter zu konfigurieren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Deadline options</strong> </td>
         <td><p>Um einen Termin für die Phase festzulegen, klicken Sie auf eine Option in der Dropdownliste <strong>Deadline-Optionen</strong> . Führen Sie dann unter <strong>Deadline</strong> einen der folgenden Schritte aus:</p>
          <ul>
           <li>Wenn Sie <strong>Bestimmtes Datum festlegen</strong> auswählen: Wählen Sie das gewünschte Datum und die gewünschte Uhrzeit für die Frist aus.</li>
           <li>Wenn Sie "<strong>Von der Staging-Aktivierungsdatum berechnen</strong>": Wählen Sie die Anzahl der Geschäftstage aus, die Sie zum Staging-Aktivierungsdatum hinzufügen möchten, um den Termin zu bestimmen.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Bühne sperren</td>
         <td>Geben Sie an, wann die Bühne gesperrt werden kann. </td>
        </tr>
        <tr>
         <td role="rowheader">Primärer Entscheidungsträger</td>
         <td><p>Wählen Sie den Primären Entscheidungsträger auf der Bühne aus (der nur verfügbar ist, wenn Sie mindestens eine Person zur Bühne hinzufügen, die die Rolle "Genehmiger"oder höher besitzt). Wenn Sie einen Primären Entscheidungsträger auswählen, ist die Option <strong>Nur eine Entscheidung erforderlich</strong> in dieser Phase deaktiviert.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Nur eine Entscheidung erforderlich</td>
         <td>Beendet den gesamten Überprüfungsprozess, wenn einer der Entscheidungsträger eine Entscheidung trifft.<p>Diese Option ist nicht verfügbar, wenn Sie einen Benutzer im Dropdownmenü <strong>Primärer Entscheidungsträger</strong> ausgewählt haben.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Private Bühne</td>
         <td>Ermöglicht nur den folgenden Personen die Anzeige von Kommentaren und Entscheidungen, die in dieser Phase getroffen wurden: Supervisoren, Adobe Workfront-Administratoren und Workfront Proof-Administratoren</td>
        </tr>
        <tr>
         <td role="rowheader">Personen per E-Mail benachrichtigen</td>
         <td>Warnt die validierungsverantwortlichen Benutzer mit einer E-Mail-Benachrichtigung an, wenn sie an der Reihe sind, an einem Testversand zu arbeiten.</td>
        </tr>
       </tbody>
      </table>

   1. Klicken Sie auf **Phase hinzufügen**.

1. Wiederholen Sie den vorherigen Schritt nach Bedarf, um weitere Phasen hinzuzufügen.

   Wenn Sie dem automatisierten Workflow Bühnen hinzufügen, wird ein Diagramm auf dem Bildschirm angezeigt, um sie darzustellen:

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Wenn Sie alle Bühnen hinzugefügt haben, klicken Sie auf **Fertig**.

## Über die Verwendung automatisierter Workflow-Vorlagen {#about-using-automated-workflow-templates}

Beachten Sie Folgendes, wenn Sie eine Vorlage für einen automatisierten Workflow verwenden:

1. Die Einstellungen einer Automated Workflow-Vorlage bestimmen, was Sie mit dem automatisierten Workflow für einen Testversand tun können. Wenn beispielsweise die Schaltfläche Phase hinzufügen in der Vorlage deaktiviert ist, ist sie nicht sichtbar, wenn Sie mit den Einstellungen für den automatisierten Workflow für den Testversand arbeiten.
1. Wenn eine Person in einer Vorlage für einen automatisierten Workflow zu einer Nutzung hinzugefügt, aber bereits als Validierer für den Testversand vorhanden ist, wird der Validierer durch Anwendung der Vorlage aus der Bühne entfernt. Wenn Sie keinen weiteren Validierer zur Bühne hinzufügen, werden Sie in einer Meldung aufgefordert, einen hinzuzufügen.
1. Ihre Fähigkeit, eine Vorlage für einen automatisierten Workflow zu ändern, hängt von den vom Workfront-Administrator konfigurierten Vorlageneinstellungen ab, wie in beschrieben. Wenn die Möglichkeit zur Änderung der Vorlage deaktiviert ist, kann sie nur vom Inhaber der Vorlage geändert werden.

## Über das Hinzufügen von Validierern zu einer Phase {#about-adding-reviewers-to-a-stage}

Beachten Sie beim Hinzufügen von Validierern zu einer Phase Folgendes:

* Nachdem Sie einen Benutzer zu einer Bühne hinzugefügt haben, können Sie Einstellungen für diesen Benutzer für den Testversand konfigurieren, z. B. die Rolle des Testversands und etwaige zusätzliche Berechtigungen, die dieser Benutzer erhalten sollte, sowie den Typ der E-Mail-Warnungen, die er erhalten wird, wenn er zu einem Testversand Kommentare und Entscheidungen trifft.
* Sie können einen oder mehrere Benutzer von einer Phase auf eine andere ziehen. Sie können Benutzer direkt in eine andere Bühne ziehen oder Benutzer auf eine Bühne im Diagramm **Phasen** ziehen. Um mehrere Benutzer auszuwählen, drücken Sie Umschalt+Strg (unter Windows) bzw. Umschalt+Befehl (unter Mac).
* Sie können einen Validierer nur einmal zu einem Testversand hinzufügen. Das bedeutet, dass Sie dieselbe Person nicht mehr als einer Testphase hinzufügen können.
* Prüfer, die nicht zu einer privaten Bühne hinzugefügt wurden, können diese Phase nicht auf dem Testversand oder den Kommentaren sehen, die in dieser Phase abgegeben wurden.
* Wenn ein Benutzer zu einer Phase hinzugefügt wird, erhält dieser Benutzer standardmäßig Zugriff auf den Testversand ab der Erstellung des Testversands.

  Ihr Workfront-Administrator kann den Zugriff auf den Testversand einschränken, bis der Workflow in die Phase gelangt, in der der Benutzer hinzugefügt wurde. Weitere Informationen finden Sie unter  in .
