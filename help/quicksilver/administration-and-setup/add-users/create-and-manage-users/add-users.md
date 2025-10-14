---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Benutzende hinzufügen
description: Als Workfront-Admin oder Benutzende mit vollem Administratorzugriff können Sie Benutzende in Workfront hinzufügen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 3%

---

# Benutzer hinzufügen

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>* **Wenn Ihre Organisation in die Adobe Admin Console integriert wurde, müssen Sie Systemadministratoren über die Adobe Admin Console erstellen.**
>
>   Anweisungen zum Erstellen von Systemadministratoren in der Adobe Admin Console finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>   Gruppenadministratoren in Organisationen, die in die Adobe Admin Console integriert wurden, können mit diesem Verfahren Benutzende erstellen und diese zur Genehmigung durch den Administrator einreichen.
>
>   Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
>* **Wenn Ihr Unternehmen Single Sign-on (SSO) verwendet** empfehlen wir, Benutzer zu erstellen und sie Workfront in Adobe Admin Console zuzuweisen. Das Erstellen dieser Benutzenden in Workfront ist möglich. Abhängig von der Konfiguration der Admin Console Ihres Unternehmens kann es jedoch zu Problemen bei der Übertragung dieser Informationen an die Adobe Admin Console kommen.
>  &#x200B;>   Nachdem Sie den Benutzer in der Adobe Admin Console erstellt haben, können Sie die Benutzerinformationen in der Workfront konfigurieren, z. B. das Zuweisen von Rollen, Gruppen, Teams und Zugriffsebenen.
>* **Wenn Ihr Unternehmen kein Single Sign-on (SSO) verwendet** können Sie Benutzende, die keine Systemadministratoren sind, direkt in Workfront hinzufügen. Es ist möglich, Benutzende in der Adobe Admin Console hinzuzufügen. Durch das Hinzufügen in der Workfront können Sie jedoch deren Zugriffsebene beim Erstellen festlegen, was Ihnen Zeit sparen kann.



Sie können Benutzende in Adobe Workfront hinzufügen, indem Sie einzelne Benutzende von Grund auf neu erstellen oder indem Sie bestehende Benutzende kopieren.

Informationen zum gleichzeitigen Importieren mehrerer Benutzer finden Sie unter [Benutzer importieren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p><p>Oder</p><p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie einen Benutzer hinzufügen, sammeln Sie die unten aufgeführten Informationen zum Benutzer und bestimmen Sie, welche Informationen Sie mit diesem Benutzer verknüpfen möchten:

* Wie lauten die personenbezogenen Daten des Benutzers? Sie benötigen mindestens Folgendes:

   * Vollständiger Name
   * Ein Benutzername
   * Standardkennwort
   * E-Mail-Adresse

  >[!NOTE]
  >
  >Sie können bestimmen, ob Benutzer die Kontaktinformationen anderer Benutzer anzeigen können, indem Sie die Einstellung „Benutzeransicht“ optimieren, wenn Sie Zugriffsebenen für Workfront-Objekte angeben. Weitere Informationen finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Welche Position hat der neue Benutzer innerhalb des Unternehmens? Hat diese Person direkt unterstellte Mitarbeiter? Wem berichtet diese Person?
* Welche Aufgabengebiete hat die Person? Gibt es dieses Aufgabengebiet in Workfront? Gibt es eine Begrenzung für die Anzahl der Personen, die dieses Aufgabengebiet ausfüllen können? Informationen zum Erstellen von Aufgabengebieten finden Sie unter [Erstellen und Verwalten von &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)).
* Welche Zugriffsebene sollte der Benutzer haben? Ist es bereits vorhanden oder muss ein neues erstellt werden? Weitere Informationen finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* In welcher Hauptgruppe sollte sich dieser Benutzer befinden? Sollte die Person in mehr als einer Gruppe sein? Informationen zu Gruppen finden Sie unter [Gruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* In welchem Haupt-Team sollte sich dieser Benutzer befinden? Sollte die Person in mehr als einem Team sein? Informationen zu Teams finden Sie unter [Teams - Übersicht](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Welche benutzerdefinierten Informationen müssen Sie mit diesem Benutzer verknüpfen?

  Wenn Informationen über Benutzer in benutzerdefinierten Feldern erfasst werden, die Sie erstellt haben, müssen Sie beim Erstellen eines Benutzers über ein benutzerdefiniertes Formular verfügen. Informationen zu benutzerdefinierten Formularen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Neuerstellen von Benutzern

{{step-1-to-users}}

1. Klicken Sie **Neuer Benutzer > Neuer Benutzer**, um einen Benutzer hinzuzufügen, der noch nicht zu Workfront hinzugefügt wurde.

   Oder

   Klicken Sie auf **Neuer Benutzer > Benutzer importieren**, um Benutzer hinzuzufügen, indem Sie eine Tabellenimportdatei hochladen.

   Wenn Sie Benutzende importieren, müssen Sie diese Schritte nicht fortsetzen. Weitere Informationen finden Sie unter [Benutzer importieren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. Klicken Sie im **Neuer Benutzer** auf **Erweiterte Optionen anzeigen** und konfigurieren Sie dann die verfügbaren Optionen, um die Informationen der Person einzugeben.

   Weitere Informationen zu diesen Optionen finden [&#x200B; unter „Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Führen Sie einen der folgenden Schritte aus:

   * Lassen Sie **Einladungs-E-Mail an diese Person senden** aktiviert. In diesem Fall erhält der Benutzer eine E-Mail, in der er einem Link folgen kann, um sein eigenes Kennwort für Workfront zu erstellen. Benutzer, die die E-Mail-Einladung nicht annehmen und ein Workfront-Kennwort erstellen, werden in Workfront als Nicht registriert aufgeführt.
   * Deaktivieren Sie **Einladungs-E-Mail an diese Person senden** und geben Sie dann ein **Kennwort** für die Person ein und bestätigen Sie es im Feld **Kennwort bestätigen**. Sie müssen dieses Kennwort für Benutzer außerhalb von Workfront freigeben.

   >[!NOTE]
   >
   >* Wenn Ihr Workfront-Administrator eine SSO-Integration mit Workfront aktiviert hat, wird das Feld Nur &lt;SSO-Konfiguration>-Authentifizierung zulassen ausgeblendet, wenn Sie die E-Mail-Einladung deaktivieren. Das Feld Federation-ID oder &lt;SSO Configuration> Benutzername bleibt sichtbar.
   >
   >* Wenn Ihre Organisation in die Admin Console integriert wurde und Sie eine Benutzerin bzw. einen Benutzer über Workfront hinzufügen, haben Sie keine Möglichkeit, eine E-Mail-Einladung zu senden.
   >
   >   Bestehende Adobe-Benutzende erhalten möglicherweise eine E-Mail, in der sie darauf hingewiesen werden, dass Workfront verfügbar ist. Dies ist eine Voreinstellung, die vom Adobe-Administrator für das Produkt gesteuert wird.

1. Klicken Sie **Diese Person hinzufügen**.

   Oder

   Klicken Sie auf **Person hinzufügen und eine weitere starten**, um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.

   >[!NOTE]
   >
   >* Wenn Sie Gruppenadministrator sind und Benutzer zu einer Organisation hinzufügen, die in die Adobe Admin Console integriert wurde, lauten die Optionen für diesen Schritt **Benutzer zur Genehmigung durch den Administrator einreichen** und **Zur Genehmigung einreichen und einen anderen starten**. Der Benutzer wird mit dem Status Deaktiviert und Ausstehende Genehmigung erstellt.
   > 
   >* Wenn der Benutzer den Status Deaktiviert und Ausstehende Genehmigung nicht innerhalb weniger Minuten verlässt und durch eine Bildschirmaktualisierung das Abzeichen Ausstehende Genehmigung nicht entfernt wird, können Sie den Benutzer manuell genehmigen.
   >
   >   1. Navigieren Sie zu Einstellungen > Benutzer.
   >   1. Wählen Sie die Benutzenden in der Benutzerliste aus.
   >   1. Klicken Sie auf das Dreipunkt-Menü in der Listenüberschrift.
   >   1. Wählen Sie **Genehmigen** aus.
   >   1. Aktualisieren Sie die Seite nach einigen Minuten.


## Kopieren eines Benutzers zum Erstellen eines neuen

Sie können einen Benutzer erstellen, indem Sie einen vorhandenen Benutzer kopieren.

>[!NOTE]
>
>Wenn Sie einen Benutzer auf diese Weise erstellen, werden alle Informationen vom ursprünglichen Benutzer an den neu erstellten Benutzer kopiert, mit Ausnahme der folgenden:
>
>* Die Informationen im Abschnitt Persönliche Informationen .
>* Beim Anmelden anzeigen: Hier ist die Standardregisterkarte für die Zugriffsebene ausgewählt.
>* Verzeichnisberichte
>

So erstellen Sie einen neuen Benutzer durch Kopieren eines vorhandenen Benutzers:

{{step-1-to-users}}

1. Wählen Sie den Benutzer aus, den Sie kopieren möchten, und klicken Sie dann auf das Symbol „Kopieren![&#x200B; „Kopieren](assets/copy-icon.png).
1. Bearbeiten Sie im **Benutzer kopieren** angezeigten Feld die für den neuen Benutzer verfügbaren Felder.

   Informationen zu allen mit einem Benutzer verknüpften Feldern finden Sie unter [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Klicken Sie **Diese Person hinzufügen**.

   Oder

   Klicken Sie auf **Person hinzufügen und eine weitere starten**, um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.

Dadurch wird ein neues Konto in Workfront für den Benutzer erstellt.

Wenn Sie die Option zum Senden einer Einladung an den Benutzer ausgewählt haben, sollte dieser eine E-Mail erhalten, über die er einem Link folgen kann, um sein Workfront-Kennwort zu erstellen.

>[!NOTE]
>
>Wenn Ihre Organisation in die Admin Console integriert wurde und Sie eine Benutzerin bzw. einen Benutzer über Workfront hinzufügen, haben Sie keine Möglichkeit, eine E-Mail-Einladung zu senden.
>
>Bestehende Adobe-Benutzende erhalten möglicherweise eine E-Mail, in der sie darauf hingewiesen werden, dass Workfront verfügbar ist. Dies ist eine Voreinstellung, die vom Adobe-Administrator für das Produkt gesteuert wird.
