---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Erstellen oder Bearbeiten eines automatisierten Workflows für einen vorhandenen Korrekturabzug
description: Automatisierte Workflows erleichtern die Verwaltung des Überprüfungsprozesses, wenn Ihr Prozess komplex ist oder Sie regelmäßig Inhalte zur Überprüfung an dieselben Personengruppen senden. Wenn Sie einen Korrekturabzug mit einem automatisierten Workflow erstellen, wechselt der Korrekturabzug von einer Phase zur nächsten bis zur endgültigen Genehmigung. Die Teilnehmer werden benachrichtigt, wenn sie an der Reihe sind, das Dokument zu überprüfen.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 1%

---

# Erstellen oder Bearbeiten eines automatisierten Workflows für einen vorhandenen Korrekturabzug

Automatisierte Workflows erleichtern die Verwaltung des Überprüfungsprozesses, wenn Ihr Prozess komplex ist oder Sie regelmäßig Inhalte zur Überprüfung an dieselben Personengruppen senden. Wenn Sie einen Korrekturabzug mit einem automatisierten Workflow erstellen, wechselt der Korrekturabzug von einer Phase zur nächsten bis zur endgültigen Genehmigung. Die Teilnehmer werden benachrichtigt, wenn sie an der Reihe sind, das Dokument zu überprüfen.

Informationen zum Erstellen eines automatisierten Workflows für einen neuen Korrekturabzug finden Sie unter [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Erstellen oder bearbeiten Sie einen automatisierten Workflow für einen vorhandenen Korrekturabzug:

1. Bewegen Sie den Mauszeiger über das Dokument im Bereich Dokumente und klicken Sie dann auf Proofing-Workflow.

   Oder

   Wenn Sie den Korrekturabzug im Proofing Viewer ansehen, klicken Sie im linken ](assets/workflow-icon-proofing-viewer.png) auf **Workflow** ![Workflow-Symbol und dann auf das Symbol „Bearbeiten![Symbol „Bearbeiten“](assets/edit-icon-proofing-viewer.png), um die automatisierten Workflow-Einstellungen für den Korrekturabzug zu öffnen.

1. (Bedingt) Wenn für den Korrekturabzug derzeit ein einfacher Workflow (ohne Phasen) verwendet wird, klicken Sie im angezeigten **auf In automatisierten Workflow**.

   >[!NOTE]
   >
   >Sie können die erste Phase nicht bearbeiten, wenn Sie von einem einfachen Workflow in einen automatisierten Workflow konvertieren. Sie können jedoch neue Phasen hinzufügen und konfigurieren.

1. (Bedingt) Um eine automatisierte Workflow-Vorlage zu verwenden, die Ihr Adobe Workfront-Administrator erstellt und für Sie freigegeben hat, klicken Sie auf **Vorlage hinzufügen** wählen Sie die Vorlage in dem angezeigten Feld aus und klicken Sie dann auf **Vorlage hinzufügen**.

   Weitere Informationen finden Sie unter [Über die Verwendung automatisierter Workflow-Vorlagen](#about-using-automated-workflow-templates) in diesem Artikel.

1. Fügen Sie dem automatisierten Workflow einen Schritt hinzu:

   1. Klicken Sie **Neue Phase** in der oberen rechten Ecke.
   1. Geben Sie in das sich öffnende Feld einen **Namen** für die Phase ein.
   1. (Optional) Legen Sie eine Frist für die Phase fest.
   1. Wählen Sie im **Phase aktivieren**, wie die Phase aktiviert werden soll:


      <table>
      <tbody>
      <tr>
      <td><strong>Bei der Erstellung eines Korrekturabzugs</strong></td>
      <td>Der Schritt wird automatisch aktiviert, da der Korrekturabzug bereits erstellt wurde.</td>
      </tr>
      <tr>
      <td><strong>Nach Ablauf der Frist für die vorige Phase</strong></td>
      <td>Klicken Sie auf das vorherige Stadium in der Dropdown<strong>Liste Übergeordnetes </strong> .</td>
      </tr>
      <tr>
      <td><strong>An einem bestimmten Datum und zu einer bestimmten Uhrzeit</strong></td>
      <td>Klicken Sie auf das <strong>Ein</strong>-Feld, um das Datum auszuwählen, und klicken Sie dann auf das Feld rechts, um die Zeit auszuwählen.</td>
      </tr>
      <tr>
      <td><strong>Alle Entscheidungen werden in der übergeordneten Phase genehmigt oder mit Änderungen genehmigt</strong></td>
      <td>Klicken Sie auf das übergeordnete Stadium in der <strong>Übergeordnetes Stadium</strong> Dropdown-Liste.</td>
      </tr>
      <tr>
      <td><strong>Alle Entscheidungen werden in der übergeordneten Phase genehmigt</strong></td>
      <td>Klicken Sie auf das übergeordnete Stadium in der <strong>Übergeordnetes Stadium</strong> Dropdown-Liste.</td>
      </tr>
      <tr>
      <td><strong>Alle Entscheidungen werden getroffen</strong></td>
      <td>Klicken Sie auf das übergeordnete Stadium in der <strong>Übergeordnetes Stadium</strong> Dropdown-Liste.</td>
      </tr>
      </tbody>
      </table>


   1. Geben Sie einen Kontaktnamen oder eine E-Mail-Adresse ein und konfigurieren Sie die Einstellungen für Validierungsverantwortliche für das Stadium.

      Informationen zum Hinzufügen von Reviewern finden Sie unter [Informationen zum Hinzufügen von Reviewern zu ](#about-adding-reviewers-to-a-stage) in diesem Artikel.

   1. Verwenden Sie eine der folgenden Optionen, um das Stadium weiter zu konfigurieren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Fristoptionen</strong> </td>
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
         <td role="rowheader">Primärer Entscheidungsträger</td>
         <td><p>Wählen Sie den Primären Entscheidungsträger auf der Bühne aus (nur verfügbar, nachdem Sie mindestens eine Person zur Bühne hinzugefügt haben, die die Rolle einer genehmigenden Person oder höher für Korrekturabzüge hat). Wenn Sie einen Primären Entscheidungsträger auswählen, ist die Option <strong>Nur eine Entscheidung erforderlich</strong> in diesem Schritt deaktiviert.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Nur eine Entscheidung erforderlich</td>
         <td>Beendet den gesamten Überprüfungsprozess, wenn einer der Entscheidungsträger eine Entscheidung trifft.<p>Diese Option ist nicht verfügbar, wenn Sie im Dropdown-Menü <strong>Primärer Entscheidungsträger</strong> einen Benutzer angegeben haben.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Private Bühne</td>
         <td>Ermöglicht nur den folgenden Personen, Kommentare und Entscheidungen anzuzeigen, die in dieser Phase getroffen wurden: Supervisoren, Adobe Workfront-Administratoren und Workfront Proof-Administratoren</td>
        </tr>
        <tr>
         <td role="rowheader">Personen per E-Mail benachrichtigen</td>
         <td>Benachrichtigt Prüfer mit einer E-Mail-Benachrichtigung, wenn sie an der Reihe sind, den Korrekturabzug zu bearbeiten.</td>
        </tr>
       </tbody>
      </table>

   1. Klicken Sie **Phase hinzufügen**.

1. Wiederholen Sie den vorherigen Schritt nach Bedarf, um weitere Stadien hinzuzufügen.

   Wenn Sie dem automatisierten Workflow Stadien hinzufügen, wird auf dem Bildschirm ein Diagramm erstellt, das diese Stadien darstellt:

   ![Workflow-](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Wenn Sie alle Schritte hinzugefügt haben, klicken Sie auf **Fertig**.

## Über die Verwendung automatisierter Workflow-Vorlagen {#about-using-automated-workflow-templates}

Beachten Sie bei der Verwendung einer automatisierten Workflow-Vorlage Folgendes:

1. Die Einstellungen einer automatisierten Workflow-Vorlage bestimmen, was Sie mit dem automatisierten Workflow für einen Korrekturabzug tun können. Wenn zum Beispiel die Schaltfläche Schritt hinzufügen in der Vorlage deaktiviert ist, wird sie nicht angezeigt, wenn Sie mit den Einstellungen des automatisierten Workflows für den Korrekturabzug arbeiten.
1. Wenn eine Person zu einer Phase in einer automatisierten Workflow-Vorlage hinzugefügt wird, aber auch bereits als Prüferin bzw. Prüfer im Korrekturabzug vorhanden ist, wird sie durch Anwenden der Vorlage von der Phase entfernt. Wenn Sie keinen weiteren Validierungsverantwortlichen zum Schritt hinzufügen, werden Sie in einer Meldung aufgefordert, einen hinzuzufügen.
1. Ihre Möglichkeit, eine Vorlage für einen automatisierten Workflow zu ändern, hängt von den Vorlageneinstellungen ab, die vom Workfront-Administrator konfiguriert wurden, wie in beschrieben. Wenn die Möglichkeit, die Vorlage zu ändern, deaktiviert ist, kann nur der Besitzer der Vorlage sie ändern.

## Über das Hinzufügen von Validierungsverantwortlichen zu einem Schritt {#about-adding-reviewers-to-a-stage}

Beachten Sie Folgendes, wenn Sie Reviewer zu einem Schritt hinzufügen:

* Nachdem Sie einen Benutzer zu einem Schritt hinzugefügt haben, können Sie Einstellungen für diesen Benutzer im Korrekturabzug konfigurieren, z. B. die Rolle des Korrekturabzugs und alle zusätzlichen Berechtigungen, die er haben sollte, sowie den Typ der E-Mail-Warnungen, die er erhalten soll, wenn Personen Kommentare zum Korrekturabzug abgeben und Entscheidungen dazu treffen.
* Sie können einen oder mehrere Benutzer von einem Schritt in einen anderen ziehen. Sie können Benutzer direkt in eine andere Phase ziehen oder Benutzer in eine Phase auf dem Diagramm **Phasen** ziehen. Drücken Sie zum Auswählen mehrerer Benutzer Umschalt+Strg (unter Windows) oder Umschalt+Befehl (unter Mac).
* Sie können einem Korrekturabzug nur einmal einen Prüfer hinzufügen. Das bedeutet, dass Sie dieselbe Person nicht zu mehr als einem Schritt im Korrekturabzug hinzufügen können.
* Prüfer, die nicht zu einer privaten Phase hinzugefügt wurden, können diese Phase nicht im Korrekturabzug oder in Kommentaren sehen, die in dieser Phase gemacht wurden.
* Standardmäßig gewährt das Hinzufügen eines Benutzers zu einem Schritt diesem Benutzer Zugriff, um den Korrekturabzug ab dem Zeitpunkt anzuzeigen, zu dem der Korrekturabzug erstellt wird.

  Ihr Workfront-Administrator kann Benutzende vom Zugriff auf den Korrekturabzug ausschließen, bis der Workflow in das Stadium eintritt, in dem der/die Benutzende hinzugefügt wurde. Weitere Informationen finden Sie unter  in .
