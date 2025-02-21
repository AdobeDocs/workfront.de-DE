---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Erstellen einer neuen Version eines Korrekturabzugs
description: Das Verwalten des Feedbacks über mehrere Versionen oder Revisionen eines Arbeitsstücks kann eine große Herausforderung sein. Workfront vereinfacht diesen Prozess, da Sie mehrere Versionen eines Korrekturabzugs erstellen und vergleichen können.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1737'
ht-degree: 0%

---

# Erstellen einer neuen Version eines Korrekturabzugs

Das Verwalten des Feedbacks über mehrere Versionen oder Revisionen eines Arbeitsstücks kann eine große Herausforderung sein. Workfront vereinfacht diesen Prozess, da Sie mehrere Versionen eines Korrekturabzugs erstellen und vergleichen können.

Beachten Sie beim Erstellen einer neuen Version eines Korrekturabzugs die folgenden Informationen:

* Sie können Benutzenden die Berechtigung erteilen, eine Version zu sehen, aber keine andere. Wenn Sie dagegen eine spätere Version für einen Benutzer freigeben, kann dieser Benutzer frühere Versionen nur sehen, wenn Sie zurückgehen und dem Benutzer explizit Zugriff auf diese früheren Versionen gewähren.
* Um eine neue Version eines Korrekturabzugs zu erstellen, benötigen Sie Bearbeitungsrechte für den Korrekturabzug.

  Workfront Proof Weitere Informationen [, wer Bearbeitungsrechte für einen Korrekturabzug hat, finden Sie unter ](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)Verwalten von Korrekturabzugsberechtigungsprofilen in [Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

  Informationen zur Freigabe von Korrekturabzugsversionen finden Sie unter  [Freigeben eines Korrekturabzugs in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Wenn ein Korrekturabzug in Adobe Workfront erstellt wird, müssen alle neuen Versionen, die für diesen Korrekturabzug erstellt werden, auch in Workfront erstellt werden. Sie können keine neue Version eines Korrekturabzugs in Workfront Proof erstellen, wenn dieser Korrekturabzug in Workfront erstellt wurde.

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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Erstellen einer neuen Version eines Korrekturabzugs in Workfront

Es gibt mehrere Möglichkeiten, eine neue Korrekturabzugsversion in Workfront hochzuladen. Die standardmäßigen Korrekturabzugseinstellungen werden je nach ausgewählter Methode von der vorherigen Version übernommen oder nicht.

* **Beim Hochladen von Dokumenten automatisch Korrekturabzüge generieren**: Die Standardeinstellungen für Korrekturabzüge werden nicht übernommen. Wenn Sie diese Einstellung in Ihrem Benutzerprofil aktiviert haben, werden die Standardeinstellungen für Korrekturabzüge nicht übernommen, wenn Sie eine neue Version per Drag-and-Drop verschieben.
* **Korrekturabzug erstellen > Einfach**: Die Standardeinstellungen für Korrekturabzüge werden nicht übernommen. Wenn Sie beim Erstellen einer neuen Korrekturabzugsversion Einfach auswählen, werden die standardmäßigen Korrekturabzugseinstellungen nicht von der vorherigen Version übernommen.
* **Neu hinzufügen > Version > Korrekturabzug**: Die Standardeinstellungen für Korrekturabzüge werden von der vorherigen Version übernommen.
* **Korrekturabzug erstellen > Erweitert**: Die Standardeinstellungen für Korrekturabzüge werden von der vorherigen Version übernommen.

  <table>
  <tbody>
  <tr>
  <td>Beim Hochladen von Dokumenten automatisch Korrekturabzüge generieren</td>
  <td>Die Standardeinstellungen für Korrekturabzüge werden nicht übernommen. Wenn Sie diese Einstellung in Ihrem Benutzerprofil aktiviert haben, werden die Standardeinstellungen für Korrekturabzüge nicht übernommen, wenn Sie eine neue Version per Drag-and-Drop verschieben.</td>
  </tr>
  <tr>
  <td>Korrekturabzug erstellen &gt; Einfach</td>
  <td>Die Standardeinstellungen für Korrekturabzüge werden nicht übernommen. Wenn Sie beim Erstellen einer neuen Korrekturabzugsversion Einfach auswählen, werden die standardmäßigen Korrekturabzugseinstellungen nicht von der vorherigen Version übernommen.</td>
  </tr>
  <tr>
  <td>Neu hinzufügen &gt; Version &gt; Testversand</td>
  <td>Die Standardeinstellungen für Korrekturabzüge werden von der vorherigen Version übernommen.</td>
  </tr>
  <tr>
  <td>Korrekturabzug erstellen &gt; Erweitert</td>
  <td>Die Standardeinstellungen für Korrekturabzüge werden von der vorherigen Version übernommen.</td>
  </tr>
  </tbody>
  </table>




Erstellen einer neuen Version eines Korrekturabzugs:

1. Öffnen Sie die Dokumentliste, die den Korrekturabzug enthält.
1. Ziehen Sie aus dem Dateisystem Ihres Computers eine neue Datei per Drag-and-Drop über den Korrekturabzug.

   Oder

   Wählen Sie die Zeile aus, in der der Korrekturabzug aufgeführt ist **klicken Sie auf „Neu hinzufügen** > **Version** und klicken Sie dann auf die Option, die Sie zum Hinzufügen der neuen Version des Korrekturabzugs verwenden möchten.

   ![Neue Version hinzufügen](assets/add-new-version-350x185.png)

## Erstellen einer neuen Version eines Korrekturabzugs über die Proofing-Anzeige (nur Workfront Proof)

Wenn Sie die eigenständige Workfront Proof verwenden, können Sie eine neue Version eines Korrekturabzugs erstellen, der eine einzelne Datei oder ein Web-Capture enthält. 

>[!NOTE]
>
>Wenn für Ihr Konto ein Unternehmensabo erstellt wurde und Sie mehrere Dateien oder Web-Aufnahmen hochladen, werden diese automatisch in einer neuen Version kombiniert. Weitere Informationen finden [ unter „Erstellen eines mehrseitigen ](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)&quot;.

So erstellen Sie eine neue Version eines Korrekturabzugs in Workfront Proof:

1. Öffnen Sie den Korrekturabzug.
1. Klicken Sie auf **Dropdown** Menü „Version“ in der oberen linken Ecke und klicken Sie dann in **angezeigten Feld auf**+ Neue Version .

   Auf der Seite **Neue Korrekturabzugsversion von** werden alle validierungsverantwortlichen Benutzer aus der vorherigen Version angezeigt, einschließlich ihrer Rollen und E-Mail-Benachrichtigungseinstellungen. Sie können auf dieser Seite einfach die Rollen und Benachrichtigungen vorhandener Reviewer bearbeiten oder vorhandene Reviewer aus der neuen Version entfernen.

1. Laden **unter &quot;** hinzufügen“ eine Datei als neue Version des Korrekturabzugs hoch, indem Sie sie von Ihrem Computer ziehen und ablegen oder auf **Durchsuchen** klicken und die gewünschte Datei auswählen. Sie können einen **Korrekturabzugsnamen** für die Version eingeben oder dieses Feld leer lassen, um denselben Dateinamen mit einer Versionsnummer am Ende hinzuzufügen.

   Oder

   Erfassen Sie eine Web-Seite als neue Version des Korrekturabzugs, indem Sie eine URL eingeben.

   >[!NOTE]
   >
   >Drag-and-Drop ist nur bei Browsern verfügbar, die HTML5 vollständig unterstützen. Ausgeschlossen sind Internet Explorer 7 bis 9 und Safari.

1. Führen **unter** Workflow“ eine der folgenden Änderungen durch, um die Reviewer für diese Version des Korrekturabzugs anzugeben.

   Reviewer aus der vorherigen Version werden durch die von Ihnen hinzugefügten Reviewer ersetzt.

   * Ändern Sie den **Inhaber** der Version in einen anderen Benutzer in Ihrem Konto.\
     Informationen zu Eigentümerberechtigungen finden Sie unter [Profile für Korrekturabzugsberechtigungen in Workfront Proof](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Fügen Sie mithilfe von **Kontaktnamen oder E-Mail-Adresse eingeben, um ein Empfängerfeld hinzuzufügen** Validierungsverantwortliche zur Version hinzu. Sie können für jeden Empfänger eine **Rolle** Korrekturabzugs) und einen Typ **E-Mail** Warnhinweise“ angeben.

     Informationen zum Hinzufügen von Gruppen zum Korrekturabzug finden Sie unter  [Gruppen zu einem Korrekturabzug hinzufügen](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). Informationen zu Rollen finden Sie unter [Verwalten von Korrekturabzugsrollen in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Wenn der Ersteller oder Besitzer von  Wenn für den Korrekturabzug [Die E-Mail zu Korrekturabzügen erstellt](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) standardmäßig deaktiviert ist (in den persönlichen Einstellungen), erhalten sie keine E-Mails zu Korrekturabzügen oder neuen Korrekturabzügen, selbst wenn das Kontrollkästchen Personen per E-Mail benachrichtigen auf der Seite Neuer Korrekturabzug aktiviert ist. Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie unter [Konfigurieren von E-Mail-Benachrichtigungseinstellungen in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). Siehe auch [E-Mail zu Korrekturabzug erstellt](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) und [Neue Korrekturabzugs-E-Mail](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * Legen Sie eine Frist für den Korrekturabzug für die Version fest.
   * Bewegen Sie den Mauszeiger über den Namen eines Reviewers, um alle Entscheidungen anzuzeigen, die er oder sie bezüglich einer früheren Version getroffen hat.

1. Führen **unter „E** Mail-Benachrichtigung“ einen der folgenden Schritte aus:

   * Geben Sie an, ob Sie die Validierungsverantwortlichen über die neue Version informieren möchten.\
     Ihre Auswahl wird im Abschnitt Aktivität der Seite mit den Korrekturabzugsdetails protokolliert. Weitere Informationen finden Sie unter [Verwalten von Korrekturabzugsdetails in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Fügen Sie einen benutzerdefinierten Betreff und eine Nachricht hinzu.

1. Führen Sie **Abschnitt** Organisation“ einen der folgenden Schritte aus: 

   * Wenden Sie ein oder mehrere Tags auf den Korrekturabzug an. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Tags in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
     Beachten Sie, dass Tags auch von der vorherigen Version des Korrekturabzugs übernommen werden. Wenn Sie der neuen Version ein neues Tag hinzufügen, werden auch frühere Versionen mit Tags versehen.

   * Fügen Sie die Version einem Ordner hinzu. Weitere [ finden Sie unter ](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) in Workfront Proof verwalten . Der Ordner wird aus der vorherigen Version des Korrekturabzugs kopiert. Wenn Sie einen anderen Ordner auswählen, wird der gesamte Korrekturabzug (alle Versionen) verschoben.

   * Rechnungsadministratoren und -administratoren können auf der Registerkarte Einstellungen das Feld Ordner für das gesamte Konto als Pflichtfeld festlegen. Weitere Informationen finden Sie unter.

1. Nehmen Sie unter Testversandeinstellungen eine der folgenden Änderungen vor:

   * Anmeldung beim Korrekturabzug verlangen
   * Elektronische Signaturen für den Testversand verlangen (nur Enterprise-Plan)
   * Korrekturabzug bei allen Entscheidungen sperren
   * Download der Originaldatei zulassen oder blockieren
   * Öffentliche Freigabe des Korrekturabzugs, einschließlich öffentlicher Freigabeeinstellungen
   * Testversand-Abonnement\
     Die in diesem Abschnitt vorgenommenen Auswahlen werden auf der Seite Korrekturabzugsdetails angezeigt (wo einige Felder bearbeitet werden können). Weitere Informationen finden Sie unter [Verwalten von Korrekturabzugsdetails in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

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

## Über die Nachricht Neue Version

Wenn in der vorherigen Version des Korrekturabzugs ein benutzerdefinierter Betreff/eine benutzerdefinierte Nachricht enthalten war, wird sie/sie standardmäßig auf der Seite „Neue Version“ angezeigt. Sie können:

* Bearbeiten Sie den Betreff und die Nachricht.
* Deaktivieren Sie das Kontrollkästchen Personen per E-Mail benachrichtigen. Das bedeutet, dass keine E-Mail an Ihre Prüfer gesendet wird, um sie darüber zu informieren, dass sie eine neue Version zur Überprüfung haben.

  >[!NOTE]
  >
  >Dies wird durch keinen in Ihren persönlichen Einstellungen gespeicherten benutzerdefinierten Betreff/keine Nachricht beeinflusst.

Wenn Sie einen Standardbetreff und eine Standardnachricht in Ihren persönlichen Einstellungen gespeichert haben, wirkt sich dies auf die standardmäßig auf der Seite Neue Version angezeigte Nachricht aus:

* Wenn Sie sich dafür entschieden haben, Ihre Prüfer per E-Mail über die vorherige Version des Korrekturabzugs mithilfe der Standard-E-Mail zu benachrichtigen (z. B. ohne benutzerdefinierten Betreff/benutzerdefinierte Nachricht), wird Ihr standardmäßiger benutzerdefinierter Betreff/Ihre benutzerdefinierte Nachricht (Ihre persönlichen Einstellungen) auf der Seite Neue Version angezeigt. Sie können dann den benutzerdefinierten Betreff und die Nachricht bearbeiten oder das Kontrollkästchen Personen per E-Mail benachrichtigen deaktivieren (d. h. Ihre Prüfer erhalten keine E-Mail, um sie darüber zu informieren, dass sie eine neue Version zur Überprüfung haben).
* Wenn Sie sich dafür entschieden haben, Ihre Prüfer nicht per E-Mail über die vorherige Version des Korrekturabzugs zu benachrichtigen (z. B. keine Standard- oder benutzerdefinierte E-Mail), enthält die Seite Neue Version standardmäßig keine Nachricht. Um Ihre Validierungsverantwortlichen über die neue Version zu informieren, klicken Sie auf den Link Nachricht senden , wodurch der Standardbetreff bzw. die Standardnachricht (gemäß Ihren persönlichen Einstellungen) angezeigt wird. Bei Bedarf können Sie dann den benutzerdefinierten Betreff und die Nachricht bearbeiten.

Wenn Sie in Ihren persönlichen Einstellungen keinen Standardbetreff und keine Standardnachricht gespeichert haben, wird Folgendes auf der Seite Neue Version angezeigt:

* Wenn Sie entschieden haben, Ihre Prüfer per E-Mail über die vorherige Version des Korrekturabzugs mit der Standard-E-Mail zu benachrichtigen (z. B. ohne benutzerdefinierten Betreff/Nachricht), wird die Option Personen per E-Mail benachrichtigen auf der Seite Neue Version standardmäßig ausgewählt. Um eine benutzerdefinierte Nachricht hinzuzufügen, klicken Sie auf den Link.
* Wenn Sie sich dafür entschieden haben, Ihre Prüfer nicht per E-Mail über die vorherige Version des Korrekturabzugs zu benachrichtigen (z. B. keine Standard- oder benutzerdefinierte E-Mail), enthält die Seite Neue Version standardmäßig keine Nachricht. Um Ihre Validierungsverantwortlichen über die neue Version zu informieren, klicken Sie auf den Link Nachricht senden . Sie können dann einen benutzerdefinierten Betreff und eine benutzerdefinierte Nachricht hinzufügen, indem Sie auf den Link Benutzerdefinierte Nachricht hinzufügen klicken.
