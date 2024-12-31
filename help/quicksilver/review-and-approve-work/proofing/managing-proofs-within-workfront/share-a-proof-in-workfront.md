---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Freigeben eines Korrekturabzugs in Adobe Workfront
description: Sie können ein Korrekturabzugsdokument in Adobe Workfront freigeben, indem Sie das Dokument freigeben oder Benutzende zum Korrekturabzug hinzufügen.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: aaf5beb8692b2fdbb797ba908796d78b4ee8866c
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# Freigeben eines Korrekturabzugs in Adobe Workfront

Sie können ein Korrekturabzugsdokument in Adobe Workfront freigeben, indem Sie das Dokument freigeben oder Benutzende zum Korrekturabzug hinzufügen.

Wenn Sie den Korrekturabzug freigeben, wie in diesem Artikel erläutert, hat Ihr Empfänger denselben Zugriff auf das Dokument und den Korrekturabzug. Darüber hinaus können Sie vom Empfänger eine Genehmigung für den Testversand anfordern.

>[!TIP]
>
>Sie können einen Korrekturabzug auch über die Proofing-Anzeige freigeben. Anweisungen finden Sie unter [Freigeben eines Korrekturabzugs vom Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

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
   <td role="rowheader">Rolle des Korrekturabzugs</td> 
   <td>Autor oder Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Korrekturabzugs-Link freigeben

Durch die Freigabe eines Korrekturabzugs-Links erhalten Workfront-Benutzer Anzeigezugriff. Benutzende können den Korrekturabzug kommentieren und E-Mail-Benachrichtigungen für den Korrekturabzug mit ihren Workfront-Anmeldedaten abonnieren. Nicht-Proofing-Benutzende können Kommentare abgeben und sich mit einer E-Mail-Adresse und einem Anzeigenamen anmelden.

>[!IMPORTANT]
>
>Die Einstellung Freigabe von Korrekturabzug über öffentliche URL oder Einbettungs-Code zulassen muss aktiviert sein.

1. Wählen Sie das Dokument aus, das den Korrekturabzug enthält, den Sie für Benutzende freigeben möchten.

   Sie können nur ein Dokument auswählen. Sie können den Link für mehrere Dokumente nicht gleichzeitig freigeben.

1. Klicken Sie **Freigeben** > **Korrekturabzugs-Link**.
1. Führen **im angezeigten** (Korrekturabzug) einen der folgenden Schritte aus:

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

## Benutzer zu einem Korrekturabzug hinzufügen

Sie können dem Korrekturabzug jeden Workfront-Benutzer hinzufügen, der über Bearbeitungsrechte für den Korrekturabzug verfügt. Wenn der Korrekturabzug mehrere Phasen umfasst, fügen Sie den/die Benutzende(n) zu einem einzelnen Schritt hinzu

>[!WARNING]
>
>Zusätzlich zu den in diesem Artikel aufgeführten Methoden ist es möglich, Benutzer zu einem Korrekturabzug hinzuzufügen, indem Sie sie in einem Kommentar auf der Registerkarte Aktualisierungen eines vorhandenen Korrekturabzugs taggen. Benutzende, die auf diese Weise zu einem Korrekturabzug hinzugefügt werden, erhalten jedoch keine E-Mail-Benachrichtigung, es sei denn, sie werden erneut getaggt, nachdem sie zum Workflow des Korrekturabzugs hinzugefügt wurden.
>
>Daher empfehlen wir, Benutzende mithilfe einer der unten aufgeführten Methoden und nicht durch Taggen in einem Kommentar zu einem Korrekturabzug hinzuzufügen.
>

>[!NOTE]
>
>Beachten Sie Folgendes, wenn Sie einen alten Workfront-Plan verwenden, in dem das Proofing für einen Benutzer aktiviert und deaktiviert werden kann:
>
>* Für Empfänger muss das Proofing nicht aktiviert sein, damit sie den Korrekturabzug überprüfen können.
>* Wenn der automatisierte Workflow aktiviert ist und Sie dem Korrekturabzug einen Benutzer hinzufügen, für den das Proofing nicht in Workfront aktiviert ist, wird innerhalb des automatisierten Workflows ein neuer Schritt erstellt. Der/die Benutzende, den/die Sie hinzufügen, wird automatisch zu dieser neuen Phase hinzugefügt, wenn er/sie den Korrekturabzug zum ersten Mal aufruft. (Weitere Informationen finden Sie unter [Automatisierter Workflow - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### Benutzer zu einem vorhandenen Korrekturabzug über die Registerkarte Dokumente hinzufügen

1. Wählen Sie das Dokument aus, das den Korrekturabzug enthält, dem Benutzer hinzugefügt werden sollen.
1. Wenn der Korrekturabzug keinen automatisierten Workflow (Phasen) hat, klicken Sie auf das **Mehr**-Symbol in der oberen rechten Ecke des Abschnitts von Schritt 1 und dann im Dropdown-Menü auf **Freigeben**.

   Oder

   Wenn der Korrekturabzug über einen automatisierten Workflow verfügt, klicken Sie auf das Symbol **Mehr** in der oberen rechten Ecke der Phase, in der Sie den Reviewer hinzufügen möchten, und klicken Sie dann **Dropdown-Menü auf** Freigeben.

1. Beginnen Sie im Feld **Diese Version freigeben** unter **Freigeben** mit der Eingabe des Namens oder der E-Mail-Adresse eines Benutzers, für den Sie den Korrekturabzug freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

1. (Optional) Wiederholen Sie diesen Schritt, um dem Korrekturabzug mehrere Benutzer hinzuzufügen.
1. (Optional) Legen Sie eine Frist für die Validierungsverantwortlichen fest.
1. (Optional) Stellen Sie sicher **dass „Personen per E** Mail benachrichtigen“ ausgewählt ist, wenn Sie die Prüfer darüber informieren möchten, dass Sie sie zum Korrekturabzug hinzugefügt haben.
1. (Optional) **Hinzufügen einer benutzerdefinierten Nachricht** zur E-Mail.
1. Wenn Sie alle Reviewer hinzugefügt haben, klicken Sie auf **Freigeben**.

### Hinzufügen von Benutzern zu einem vorhandenen Korrekturabzug über die Proofing-Anzeige

Sie können Benutzer zu einem Korrekturabzug hinzufügen, während Sie einen Korrekturabzug im Web Proofing Viewer und im Desktop Proofing Viewer überprüfen.

Weitere Informationen finden Sie unter [Freigeben eines Korrekturabzugs durch Hinzufügen von Benutzern](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) im Artikel [Freigeben eines Korrekturabzugs über die Korrekturabzugsanzeige](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Bericht zu Proofing-Genehmigungen

Sie können einen Bericht erstellen, der über die in Workfront freigegebenen Proofing-Genehmigungen berichtet. Dieser Bericht enthält die folgenden Informationen zur Genehmigung von Korrekturabzügen in Ihrem System:

* Dokument, das zur Genehmigung eingereicht wurde
* Name der genehmigenden Person
* Korrekturabzug-Version
* Korrekturabzugs-ID
* Erstellungsdatum des Korrekturabzugs

Sie können auf diese Genehmigung zugreifen, wenn Sie einen Bericht auf der Grundlage eines Objekts erstellen, wie in [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.

Weitere Informationen zum Objektbericht für Korrekturabzugsgenehmigungen finden Sie im Abschnitt [Bericht zu Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) in [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Freigegebenen Korrekturabzug genehmigen

Wenn Sie ein(e) Benutzende(r) einem Korrekturabzug hinzufügt und entweder die Rolle Genehmigende Person oder die Rolle Prüfende und genehmigende Person mithilfe eines automatisierten Workflows gewährt, wird die Genehmigungsanfrage im Widget Meine Genehmigungen im Bereich Startseite angezeigt. Sie können dann den Korrekturabzug anzeigen und direkt aus Workfront eine Genehmigungsentscheidung für den Korrekturabzug treffen.

Weitere Informationen zum Treffen von Genehmigungsentscheidungen über das Widget Meine Genehmigungen finden Sie unter [Genehmigen von Arbeit im Bereich „Startseite](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) oder [Genehmigen von Arbeit](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) in [Genehmigen von Arbeit](../../../review-and-approve-work/manage-approvals/approving-work.md).
