---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Freigeben eines Testversands aus dem Testversand-Viewer
description: Sie können einen Testversand aus dem Testversand-Viewer freigeben, wenn die Freigabe vom Testversand-Eigentümer oder -Ersteller aktiviert wurde.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1501'
ht-degree: 0%

---

# Freigeben eines Testversands aus dem Testversand-Viewer

Sie können einen Testversand aus dem Testversand-Viewer freigeben, wenn die Freigabe vom Testversand-Eigentümer oder -Ersteller aktiviert wurde.

>[!IMPORTANT]
>
>Die Einstellung Freigeben eines Testversands über öffentliche URLs oder Einbettungscodes zulassen muss aktiviert sein.

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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## URL freigeben

Sie können einen Testversand über eine URL freigeben, wenn der Eigentümer den Testversand für die Freigabe konfiguriert hat. Testversand-Inhaber können die Freigabeeinstellungen jederzeit aktualisieren. Weitere Informationen finden Sie unter [Testversand-Einstellungen bearbeiten](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Wenn das Menü mit dem linken Symbol nicht angezeigt wird, klicken Sie auf das Symbol **Menü** in der oberen linken Ecke des Testversand-Viewers.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. Klicken Sie im linken Symbolmenü des Testversand-Viewers auf das Symbol **Freigeben** .

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. Stellen Sie sicher, dass in den angezeigten Optionen **Testversand freigeben** die Option **Freigebbaren Link abrufen** ausgewählt ist.

1.  Führen Sie einen der folgenden Schritte aus:

   * Um den Link in die Zwischenablage zu kopieren, klicken Sie auf **Link kopieren**.

     Sie können den Link nun über ein Tool eines Drittanbieters verteilen, z. B. einen Chat oder eine E-Mail-Anwendung.

   * Gehen Sie wie folgt vor, um den Link direkt von Adobe Workfront per E-Mail zu versenden:

      1. Geben Sie im Feld **Oder email link to** den Namen Ihres Empfängers ein und wählen Sie ihn aus. Oder geben Sie die E-Mail-Adresse eines externen Benutzers an, für den Sie freigeben möchten.

         >[!NOTE]
         >
         >Wenn bei der Freigabe eines Testversands eine Alias-E-Mail angezeigt wird, erstellen Sie keinen neuen Gastbenutzer, indem Sie die ursprüngliche E-Mail eingeben, sofern eine Alias-E-Mail vorhanden ist.

      1. Wählen Sie aus den folgenden Optionen aus:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Öffentlichen Link senden</td>
            <td><p>Enthält eine Schaltfläche in der E-Mail-Benachrichtigung, über die Benutzer zum Testversand innerhalb des von ihnen verwendeten Testversand-Viewers weitergeleitet werden und der Zugriff auf die Ansicht gewährt wird.</p><p>Wenn <strong>Testversand über öffentliche URL oder Einbettungscode abonnieren</strong> für den Testversand deaktiviert ist, können sich die Benutzer mit ihren Workfront-Anmeldedaten anmelden, um dem Testversand Kommentare hinzuzufügen. Ist diese Option aktiviert, kann jeder, der seine E-Mail-Adresse und seinen Namen (kein Passwort erforderlich) angibt, den Testversand signieren und Kommentare hinzufügen.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Downloadlink senden</td>
            <td>Enthält eine Schaltfläche in der E-Mail-Benachrichtigung, über die Benutzer zu einer Download-Seite weitergeleitet werden, auf der Dateidetails, Dateiname und Dateigröße sowie die Datei inline angezeigt werden. Benutzer können auf der Downloadseite auf den Link Download klicken, um die Datei herunterzuladen.</td>
           </tr>
           <tr>
            <td role="rowheader">Benutzerdefinierte Nachricht hinzufügen</td>
            <td>Hiermit können Sie einen benutzerdefinierten Betreff und Text für die E-Mail-Benachrichtigung angeben.</td>
           </tr>
          </tbody>
         </table>

      1. Klicken Sie auf **Senden**.

         Ihre Empfänger erhalten eine E-Mail-Benachrichtigung mit Informationen zum Testversand und den von Ihnen ausgewählten Schaltflächen.

         ![](assets/proof-share-email-350x87.png)

## Freigeben des Einbettungscodes

Sie können einen Testversand über Einbettungscode freigeben, wenn der Testversand-Besitzer ihn dafür konfiguriert hat.

So geben Sie einen Testversand über den Einbettungscode frei:

1. Klicken Sie in der Symbolleiste links neben dem Testversand-Viewer auf das Symbol **Freigeben** .

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. Klicken Sie in den angezeigten Optionen **Testversand freigeben** auf **Einbettungscode abrufen** und dann auf **Kopieren**.

## Freigeben eines Testversands durch Hinzufügen von Benutzern

Sie können bei der Überprüfung eines Testversands Benutzer zu einem Testversand hinzufügen, wenn Sie über eine der folgenden Berechtigungen verfügen:

* Supervisor- oder Administratorberechtigungen
* Manager-Berechtigungen und Sie sind der Ersteller oder Eigentümer des Testversands
* Manager-Berechtigungen mit der Rolle Autor- oder Moderator-Testversand

Wenn der Testversand über einen automatisierten Workflow verfügt, können Sie den Benutzer einer einzelnen Phase hinzufügen. Weitere Informationen finden Sie unter [Überblick über den automatisierten Workflow](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Standardmäßig werden Benutzer, die Sie zum Testversand hinzufügen, wie folgt bewertet:

* Erhalten Sie eine E-Mail-Benachrichtigung mit einem Link zum Testversand.
* Kann Genehmigungsentscheidungen für den Testversand vom Home- oder Arbeitsbereich treffen, wie in [Validieren der Arbeit](../../../../review-and-approve-work/manage-approvals/approving-work.md) beschrieben.
* Die Testversandfunktion muss nicht aktiviert sein, damit der Testversand überprüft werden kann.

Wenn der automatisierte Workflow aktiviert ist und Sie einen Benutzer zum Testversand hinzufügen, für den die Testversand-Funktion in Workfront nicht aktiviert ist, wird im automatisierten Workflow eine neue Phase erstellt. Der Benutzer, den Sie hinzufügen, wird automatisch zu dieser neuen Phase hinzugefügt, wenn er den Testversand zum ersten Mal anzeigt. Weitere Informationen finden Sie unter [Überblick über den automatisierten Workflow](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

So geben Sie einen Testversand für einzelne Benutzer frei:

1. Klicken Sie in der Symbolleiste links neben dem Testversand-Viewer auf das Symbol **Freigeben** .

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Klicken Sie links in der Liste auf **Empfänger hinzufügen** .
1. Geben Sie unter **Neue Testversand-Empfänger** den Namen eines Benutzers ein, für den Sie den Testversand freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. (Optional) Ändern Sie alle Überprüfungsoptionen rechts neben dem Namen der Person:

   * **Proof role**: Weitere Informationen finden Sie unter [Verwalten von Proof Roles in Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Staging**: (Nur verfügbar, wenn der Testversand einen automatisierten Workflow aufweist). Weitere Informationen finden Sie unter  [Übersicht über die automatisierten Workflow-Phasen](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **E-Mail-Warnungen**: Wählen Sie eine der folgenden Optionen aus, um festzulegen, wie die Person über die Aktivität beim Testversand benachrichtigt wird.

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
        <td>Eine E-Mail wird nur dann an den Validierer gesendet, wenn jemand explizit auf seinen Kommentar antwortet (dabei werden eigene Antworten auf eigene Kommentare ausgeschlossen). Das bedeutet, dass der Validierer nicht benachrichtigt wird, wenn jemand, der den Testversand durchführt, einen neuen Kommentar abgibt.<p>Diese Einstellung wird Ihren Kunden empfohlen, den Testversand durchzuführen, damit sie über keine weiteren Kommentare zum Testversand informiert und nur über Antworten auf ihre eigenen Kommentare informiert werden.</p><p>validierungsverantwortliche Benutzer mit dieser E-Mail-Warnungseinstellung werden zwar nicht über andere neue Kommentare benachrichtigt, können aber dennoch alle Kommentare zum Testversand im Testversand-Viewer anzeigen.</p><p>Informationen zu Kommentaren finden Sie unter <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Anzeigen und Antworten auf Testkommentare</a>.</p></td> 
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
        <td>Workfront sendet eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen, die nur an Tagen aufgelistet sind, an denen neben Ihrer eigenen Aktivität Aktivitäten stattfinden.<p>Mit diesem Warnhinweis können Sie eine Zusammenfassung des Projekts anzeigen, ohne über den gesamten Tag hinweg durch mehrere Aktualisierungen überlastet zu sein.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Abteilungsleiter, der den Gesamtfortschritt des Projekts überwachen möchte.</p><p>Weitere Informationen finden Sie unter <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Benachrichtigungen für Testversand-Kommentare und -Entscheidungen verwalten</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Keine E-Mail</td> 
        <td>Workfront sendet keine E-Mail-Warnungen.<br>Dies ist für eine Person nützlich, die einem Testversand nur zu Referenzzwecken hinzugefügt wird und nicht über Änderungen benachrichtigt werden muss.<p>Der Systemstandard lautet Tägliche Zusammenfassung (wird auch als Nicht festgelegt angesehen). Wenn Sie oder Ihre Validierer keine anderen Änderungen vornehmen, haben alle Testsendungen diese Einstellung.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Optional) Wiederholen Sie die beiden vorherigen Schritte, um dem Testversand mehrere Benutzer hinzuzufügen. 
1. (Optional) Legen Sie eine **Deadline** für die Überprüfer fest (nur verfügbar, wenn der Testversand keinen automatisierten Workflow aufweist).
1. (Optional) Wählen Sie **E-Mail-Benachrichtigung an neue Empfänger senden** aus, um ihnen mitzuteilen, dass Sie sie zum Testversand hinzugefügt haben.
1. Wenn Sie alle Benutzer zum Testversand hinzugefügt haben, klicken Sie auf **Fertig** .
