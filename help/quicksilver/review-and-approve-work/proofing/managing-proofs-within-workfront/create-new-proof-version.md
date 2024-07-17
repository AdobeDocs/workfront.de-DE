---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Erstellen einer neuen Testversion
description: Das Verwalten von Feedback über mehrere Versionen oder Revisionen eines Werkes hinweg kann eine große Herausforderung sein. Workfront vereinfacht diesen Vorgang, indem Sie mehrere Testversionen erstellen und vergleichen können.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1723'
ht-degree: 0%

---

# Erstellen einer neuen Testversion

Das Verwalten von Feedback über mehrere Versionen oder Revisionen eines Werkes hinweg kann eine große Herausforderung sein. Workfront vereinfacht diesen Vorgang, indem Sie mehrere Testversionen erstellen und vergleichen können.

Beachten Sie beim Erstellen einer neuen Testversand-Version die folgenden Informationen:

* Sie können einem Benutzer Berechtigungen erteilen, eine Version, aber keine andere anzuzeigen. Wenn Sie hingegen eine spätere Version für einen Benutzer freigeben, kann dieser Benutzer frühere Versionen nur sehen, wenn Sie zurückgehen und dem Benutzer explizit Zugriff auf diese vorherigen Versionen gewähren.
* Um eine neue Version eines Testversands zu erstellen, benötigen Sie die Berechtigung zum Bearbeiten des Testversands.

  Weitere Informationen dazu, wer für einen Testversand Bearbeitungsrechte besitzt, finden Sie unter [Verwalten von Proof-Rollen in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) und [Proof Permissions Profiles in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) .

  Informationen zum Freigeben von Testversandversionen finden Sie unter  [Freigeben eines Testversands in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Wenn in Adobe Workfront ein Testversand erstellt wird, müssen alle neuen Versionen, die für diesen Testversand erstellt wurden, auch in Workfront erstellt werden. Es ist nicht möglich, in Workfront Proof eine neue Testversion zu erstellen, wenn dieser Testversand in Workfront erstellt wurde.

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

## Erstellen einer neuen Testversion in Workfront

Es gibt mehrere Möglichkeiten, eine neue Testversion in Workfront hochzuladen. Die Standardeinstellungen für den Testversand können je nach gewählter Methode von der vorherigen Version übernommen werden oder nicht:

* **Testsendungen beim Hochladen von Dokumenten automatisch generieren**: Die Standardeinstellungen für den Testversand werden nicht übernommen. Wenn Sie diese Einstellung in Ihrem Benutzerprofil aktiviert haben, werden die standardmäßigen Testversandeinstellungen beim Ziehen einer neuen Version nicht übernommen.
* **Erstellen Sie einen Testversand > Einfach**: Die Standardeinstellungen für den Testversand werden nicht übernommen. Wenn Sie bei der Erstellung einer neuen Testversand-Version die Option Einfach auswählen, werden die standardmäßigen Testversandeinstellungen nicht von der vorherigen Version übernommen.
* **Neu hinzufügen > Version > Testversand**: Die standardmäßigen Testversandeinstellungen werden von der vorherigen Version übernommen.
* **Testversand erstellen > Erweitert**: Die standardmäßigen Testversandeinstellungen werden von der vorherigen Version übernommen.

  <table>
  <tbody>
  <tr>
  <td>Beim Hochladen von Dokumenten automatisch Korrekturabzüge generieren</td>
  <td>Die Standardeinstellungen für den Testversand werden nicht übernommen. Wenn Sie diese Einstellung in Ihrem Benutzerprofil aktiviert haben, werden die standardmäßigen Testversandeinstellungen beim Ziehen einer neuen Version nicht übernommen.</td>
  </tr>
  <tr>
  <td>Testversand erstellen &gt; Einfach</td>
  <td>Die Standardeinstellungen für den Testversand werden nicht übernommen. Wenn Sie bei der Erstellung einer neuen Testversand-Version die Option Einfach auswählen, werden die standardmäßigen Testversandeinstellungen nicht von der vorherigen Version übernommen.</td>
  </tr>
  <tr>
  <td>Neu hinzufügen &gt; Version &gt; Testversand</td>
  <td>Die Standardeinstellungen für den Testversand werden von der vorherigen Version übernommen.</td>
  </tr>
  <tr>
  <td>Testversand erstellen &gt; Erweitert</td>
  <td>Die Standardeinstellungen für den Testversand werden von der vorherigen Version übernommen.</td>
  </tr>
  </tbody>
  </table>




So erstellen Sie eine neue Version eines Testversands:

1. Öffnen Sie die Dokumentliste mit dem Testversand.
1. Ziehen Sie aus dem Dateisystem Ihres Computers eine neue Datei auf den Testversand.

   Oder

   Wählen Sie die Zeile aus, in der der Testversand aufgelistet ist, klicken Sie auf **Neu hinzufügen** > **Version** und dann auf die Option, mit der Sie die neue Version des Testversands hinzufügen möchten.

   ![](assets/add-new-version-350x185.png)

## Erstellen Sie eine neue Testversion aus dem Testversand-Viewer (nur Workfront Proof).

Wenn Sie die eigenständige Workfront Proof verwenden, können Sie eine neue Testversion erstellen, die eine einzelne Datei oder Weberfassung enthält. 

>[!NOTE]
>
>Wenn Ihr Konto einen Enterprise-Plan hat und Sie mehrere Dateien oder Web-Captures hochladen, werden diese automatisch zu einer neuen Version zusammengefasst. Weitere Informationen finden Sie unter [Erstellen eines mehrseitigen Testversands](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) .

So erstellen Sie eine neue Testversion in Workfront Proof:

1. Öffnen Sie den Testversand.
1. Klicken Sie oben links auf das Dropdownmenü **Version** und dann im angezeigten Feld auf **+ Neue Version** .

   Auf der angezeigten Seite **Neue Testversand-Version von** werden alle validierungsverantwortlichen Benutzer der vorherigen Version angezeigt, einschließlich ihrer Rollen und E-Mail-Benachrichtigungseinstellungen. Sie können die Rollen und Benachrichtigungen bestehender Validierungsverantwortlicher einfach bearbeiten oder vorhandene Validierer aus der neuen Version auf dieser Seite entfernen.

1. Laden Sie unter **Dateien hinzufügen** eine Datei als neue Version des Testversands hoch, indem Sie sie per Drag-and-Drop von Ihrem Computer ziehen oder auf **Durchsuchen** klicken und die gewünschte Datei auswählen. Sie können einen **Testversand-Namen** für die Version eingeben oder dieses Feld leer lassen, um denselben Dateinamen mit einer Versionsnummer zu verwenden, die am Ende hinzugefügt wird.

   Oder

   Erfassen Sie eine Webseite als neue Version des Testversands, indem Sie eine URL eingeben.

   >[!NOTE]
   >
   >Drag &amp; Drop ist nur bei Browsern verfügbar, die HTML 5 vollständig unterstützen. Hiervon ausgenommen sind Internet Explorer 7 bis 9 und Safari.

1. Nehmen Sie unter **Workflow** eine der folgenden Änderungen vor, um die Validierer für diese Version des Testversands anzugeben.

   Überprüfer aus der vorherigen Version werden durch die von Ihnen hinzugefügten Überprüfer ersetzt.

   * Ändern Sie den **Inhaber** der Version in einen anderen Benutzer in Ihrem Konto.\
     Weitere Informationen zu Berechtigungen für Inhaber finden Sie unter [Profile für Testberechtigungen in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Fügen Sie der Version mithilfe des Kontaktnamen oder der E-Mail-Adresse **Typ ein Empfängerfeld** hinzu. Sie können für jeden Empfänger eine **Proof role** und einen **E-Mail-Warnungen**-Typ angeben.

     Informationen zum Hinzufügen von Gruppen zum Testversand finden Sie unter  [Gruppen zu einem Testversand hinzufügen](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). Weitere Informationen zu Rollen finden Sie unter [Verwalten von Proof-Rollen in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Wenn der Ersteller oder Eigentümer  Wenn für den Testversand die Option [E-Mail vom Typ Testversand](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) standardmäßig deaktiviert ist (in den persönlichen Einstellungen), erhalten diese keine E-Mails vom Typ Testversand oder Neuer Testversand, selbst wenn auf der Seite Neuer Testversand die Option Personen per E-Mail benachrichtigen aktiviert ist. Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie unter [E-Mail-Benachrichtigungseinstellungen in Workfront Proof konfigurieren](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). Siehe auch [Die E-Mail zum Testversand](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) und [Neue Testversand-E-Mail](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Legen Sie eine Testversand-Deadline für die Version fest.
   * Bewegen Sie den Mauszeiger über den Namen eines Validierers, um alle Entscheidungen anzuzeigen, die er in einer früheren Version getroffen hat.

1. Führen Sie unter **E-Mail-Benachrichtigung** einen der folgenden Schritte aus:

   * Geben Sie an, ob Sie die Validierungsverantwortlichen über die neue Version informieren möchten.\
     Ihre Auswahl wird im Abschnitt Aktivität auf der Seite Testversand-Details protokolliert. Weitere Informationen finden Sie unter [Verwalten von Testversanddetails in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Fügen Sie einen benutzerdefinierten Betreff und eine Nachricht hinzu.

1. Führen Sie im Abschnitt **Organisation** einen der folgenden Schritte aus: 

   * Anwenden eines oder mehrerer Tags auf den Testversand. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Tags in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
     Beachten Sie, dass Tags auch von der vorherigen Version des Testversands übernommen werden. Wenn Sie der neuen Version ein neues Tag hinzufügen, werden auch frühere Versionen mit Tags versehen.

   * Fügen Sie die Version einem Ordner hinzu. Weitere Informationen finden Sie unter [Verwalten von Ordnern in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) . Der Ordner wird aus der vorherigen Version des Testversands kopiert. Wenn Sie einen anderen Ordner auswählen, wird der gesamte Testversand (alle Versionen) verschoben.

   * Rechnungsadministratoren und Administratoren können das Ordnerfeld für das gesamte Konto auf der Registerkarte Einstellungen obligatorisch machen. Weitere Informationen finden Sie unter .

1. Nehmen Sie unter Testversandeinstellungen eine der folgenden Änderungen vor:

   * Anmeldung beim Testversand erforderlich
   * Elektronische Signaturen für den Testversand erforderlich (nur Enterprise-Plan)
   * Sperren des Testversands bei allen Entscheidungen
   * Herunterladen der Originaldatei zulassen oder blockieren
   * Öffentliche Freigabe des Testversands, einschließlich Einstellungen für die öffentliche Freigabe
   * Testversand-Anmeldung\
     Die in diesem Abschnitt vorgenommenen Auswahlen werden auf der Seite Testversand-Details angezeigt (auf der einige Felder bearbeitet werden können). Weitere Informationen finden Sie unter [Verwalten von Testversanddetails in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## Über die Nachricht &quot;Neue Version&quot;

Wenn in der vorherigen Version des Testversands ein benutzerdefinierter Betreff/eine benutzerdefinierte Nachricht enthalten war, wird diese standardmäßig auf der Seite Neue Version angezeigt. Sie können:

* Bearbeiten Sie den Betreff und die Nachricht.
* Deaktivieren Sie das Feld Personen per E-Mail benachrichtigen , d. h., Ihre Prüfer erhalten keine E-Mail, um ihnen mitzuteilen, dass sie über eine neue Version verfügen, die überprüft werden soll.

  >[!NOTE]
  >
  > Dies wird durch benutzerdefinierte Standardbetreff/Standardnachricht, die in Ihren persönlichen Einstellungen gespeichert sind, nicht beeinträchtigt.

Wenn Sie einen Standardbetreff und eine Standardnachricht in Ihren persönlichen Einstellungen gespeichert haben, wirkt sich dies auf die Nachricht aus, die standardmäßig auf der Seite Neue Version angezeigt wird:

* Wenn Sie Ihre validierungsverantwortlichen Benutzer per E-Mail über die vorherige Testversand-Version mit der Standard-E-Mail informieren möchten (z. B. kein benutzerspezifischer Betreff/keine benutzerdefinierte Nachricht), wird Ihr standardmäßiger benutzerdefinierter Betreff/Ihre benutzerdefinierte Nachricht (Ihre persönlichen Einstellungen) auf der Seite Neue Version angezeigt. Sie können dann den benutzerdefinierten Betreff und die Nachricht bearbeiten oder die Auswahl des Felds Personen per E-Mail benachrichtigen aufheben (d. h., Ihre Prüfer erhalten keine E-Mail, um ihnen mitzuteilen, dass sie eine neue Version zur Überprüfung haben).
* Wenn Sie Ihre Validierungsverantwortlichen nicht per E-Mail über die frühere Testversand-Version informieren möchten (z. B. keine standardmäßige oder benutzerdefinierte E-Mail), enthält die Seite &quot;Neue Version&quot;standardmäßig keine Nachricht. Um Ihre Validierungsverantwortlichen über die neue Version zu informieren, klicken Sie auf den Link Nachricht senden , der Ihren standardmäßigen benutzerdefinierten Betreff/Ihre standardmäßige Nachricht anzeigt (entsprechend Ihren persönlichen Einstellungen). Sie können dann bei Bedarf den benutzerdefinierten Betreff und die Nachricht bearbeiten.

Wenn Sie keinen Standardbetreff und keine Standardnachricht in Ihren persönlichen Einstellungen gespeichert haben, wird Folgendes auf der Seite Neue Version angezeigt:

* Wenn Sie Ihre validierungsverantwortlichen Benutzer per E-Mail über die vorherige Testversand-Version mit der Standard-E-Mail benachrichtigen möchten (z. B. kein benutzerspezifischer Betreff/keine benutzerdefinierte Nachricht), wird die Option Personen per E-Mail benachrichtigen standardmäßig auf der Seite Neue Version ausgewählt. Um eine benutzerdefinierte Nachricht hinzuzufügen, klicken Sie auf den Link.
* Wenn Sie Ihre Validierungsverantwortlichen nicht per E-Mail über die frühere Testversand-Version informieren möchten (z. B. keine standardmäßige oder benutzerdefinierte E-Mail), enthält die Seite &quot;Neue Version&quot;standardmäßig keine Nachricht. Klicken Sie auf den Link Nachricht senden , um die Validierungsverantwortlichen über die neue Version zu informieren. Sie können dann einen benutzerdefinierten Betreff und eine Nachricht hinzufügen, indem Sie auf den Link Benutzerdefinierte Nachricht hinzufügen klicken.
