---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Benutzer hinzufügen
description: Als Workfront-Administrator oder Benutzer mit vollem Administratorzugriff können Sie Benutzer in Workfront hinzufügen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1132'
ht-degree: 1%

---

# Benutzer hinzufügen

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie Systemadministratoren über die Adobe Admin Console erstellen.
>
>Anweisungen zum Erstellen von Systemadministratoren in der Adobe Admin Console finden Sie unter [Verwalten von Systemadministratoren in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Gruppenadministratoren in Unternehmen, die in Adobe Admin Console integriert wurden, können dieses Verfahren zum Erstellen von Benutzern und zum Senden des Benutzers zur Admin-Genehmigung verwenden.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Sie können Benutzer in Adobe Workfront hinzufügen, indem Sie einzelne Benutzer von Grund auf neu erstellen oder vorhandene Benutzer kopieren.

Informationen zum gleichzeitigen Importieren mehrerer Benutzer finden Sie unter [Benutzer importieren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p><p>Oder</p><p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsebene, die für den Zugriff auf <b>Bearbeiten</b> konfiguriert ist, wobei <b>Erstellen</b> und mindestens eine der beiden Optionen <b>Benutzeradministrator</b> unter <b>Optimieren Ihrer Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png"> aktiviert sind. </p> <p>Wenn von diesen beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)</b> aktiviert ist, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie einen Benutzer hinzufügen, erfassen Sie die unten aufgeführten Informationen über den Benutzer und bestimmen Sie, welche Informationen Sie mit diesem Benutzer verknüpfen möchten:

* Welche personenbezogenen Daten hat der Benutzer? Sie benötigen mindestens Folgendes:

   * Vollständiger Name
   * Ein Benutzername
   * Standardkennwort
   * E-Mail-Adresse

  >[!NOTE]
  >
  >Sie können festlegen, ob Benutzer die Kontaktinformationen anderer Benutzer anzeigen können, indem Sie bei der Angabe der Zugriffsebene für Workfront-Objekte die Einstellung &quot;Benutzeransicht&quot;anpassen. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Wie steht der neue Benutzer im Unternehmen? Hat diese Person direkte Berichte? Wem meldet diese Person?
* Welche berufliche Rolle spielt die Person? Gibt es diese Rolle in Workfront? Gibt es eine Begrenzung für die Zahl der Personen, die diese Aufgabe erfüllen können? Weitere Informationen zum Erstellen von Auftragsrollen finden Sie unter [Erstellen und Verwalten von Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Welche Zugriffsebene sollte der Benutzer haben? Existiert es bereits oder müssen Sie ein neues erstellen? Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* In welcher Startseite sollte dieser Benutzer sein? Sollte die Person in mehr als einer Gruppe sein? Weitere Informationen zu Gruppen finden Sie unter [Gruppenübersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* In welchem Heimteam sollte dieser Benutzer sein? Sollte die Person in mehr als einem Team sein? Weitere Informationen zu Teams finden Sie unter [Übersicht über Teams](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Welche benutzerdefinierten Informationen müssen Sie mit diesem Benutzer verknüpfen?

  Wenn Informationen zu Benutzern in von Ihnen erstellten benutzerdefinierten Feldern erfasst werden, müssen Sie beim Erstellen eines Benutzers über ein benutzerdefiniertes Formular verfügen. Weitere Informationen zu benutzerdefinierten Formularen finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Neuen Benutzer erstellen

{{step-1-to-users}}

1. Klicken Sie auf **Neuer Benutzer > Neuer Benutzer** , um einen Benutzer hinzuzufügen, der noch nicht zu Workfront hinzugefügt wurde.

   Oder

   Klicken Sie auf **Neuer Benutzer > Benutzer importieren** , um Benutzer durch Hochladen einer Tabellenimportdatei hinzuzufügen.

   Wenn Sie Benutzer importieren, müssen Sie diese Schritte nicht fortsetzen. Weitere Informationen finden Sie unter [Benutzer importieren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. Klicken Sie im angezeigten Feld **Neuer Benutzer** auf **Erweiterte Optionen anzeigen** und konfigurieren Sie dann die verfügbaren Optionen, um die Informationen der Person einzugeben.

   Weitere Informationen zu diesen Optionen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Führen Sie einen der folgenden Schritte aus:

   * Lassen Sie **Einladungs-E-Mail an diese Person senden** aktiviert. In diesem Fall erhält der Benutzer eine E-Mail, in der er einem Link folgen kann, um sein eigenes Kennwort für Workfront zu erstellen. Benutzer, die die Einladung in die E-Mail nicht annehmen und ein Workfront-Kennwort erstellen, werden in Workfront als Abgemeldet aufgeführt.
   * Deaktivieren Sie **Senden Sie eine Einladungs-E-Mail an diese Person**, geben Sie dann ein **Kennwort** für die Person ein und bestätigen Sie es in das Feld **Kennwort bestätigen** . Sie müssen dieses Kennwort für den Benutzer außerhalb von Workfront freigeben.

   >[!NOTE]
   >
   >* Wenn Ihr Workfront-Administrator eine SSO-Integration in Workfront aktiviert hat, wird das Feld Nur die SSO-Konfiguration zulassen ausgeblendet, wenn Sie die E-Mail-Einladung deaktivieren. Das Feld Verknüpfungs-ID oder &lt;SSO-Konfiguration> Benutzername bleibt sichtbar.
   >
   * Wenn Ihr Unternehmen in die Admin Console integriert wurde und Sie einen Benutzer über Workfront hinzufügen, haben Sie keine Möglichkeit, eine Einladung per E-Mail zu senden.
   >
   Für bestehende Adobe-Benutzer kann der Benutzer eine E-Mail über die Verfügbarkeit von Workfront erhalten oder auch nicht. Dies ist eine vom Adobe-Administrator kontrollierte Voreinstellung für das Produkt.

1. Klicken Sie auf **Diese Person hinzufügen**.

   Oder

   Klicken Sie auf **Person hinzufügen und einen weiteren starten** , um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.

   >[!NOTE]
   >
   Wenn Sie ein Gruppenadministrator sind, der einen Benutzer zu einer Organisation hinzufügt, die in der Adobe Admin Console integriert wurde, sind die Optionen für diesen Schritt **Benutzer zur Admin-Genehmigung einreichen** und **Zur Genehmigung übermitteln und einen weiteren starten**. Der Benutzer wird in den Status Deaktiviert und Ausstehende Genehmigung erstellt. Ein Workfront-Administrator muss den Benutzer genehmigen, der den Benutzer in Workfront aktiviert und der Adobe Admin Console hinzufügt.

## Kopieren Sie einen Benutzer, um einen neuen zu erstellen

Sie können einen Benutzer durch Kopieren eines vorhandenen Benutzers erstellen.

>[!NOTE]
>
Wenn Sie einen Benutzer auf diese Weise erstellen, werden alle Informationen vom ursprünglichen Benutzer in den neu erstellten Benutzer kopiert, mit Ausnahme der folgenden:
>
* Die Informationen im Abschnitt Persönliche Informationen .
* Beim Anmelden anzeigen: In diesem Feld wird der Standard-Landingtab für die Zugriffsebene ausgewählt.
* Verzeichnisberichte
>

So erstellen Sie einen neuen Benutzer durch Kopieren eines vorhandenen:

{{step-1-to-users}}

1. Wählen Sie den Benutzer aus, den Sie kopieren möchten, und klicken Sie dann auf das Kopiersymbol ![](assets/copy-icon.png).
1. Bearbeiten Sie im angezeigten Feld **Benutzer kopieren** die für den neuen Benutzer verfügbaren Felder.

   Informationen zu allen Feldern, die mit einem Benutzer verknüpft sind, finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Klicken Sie auf **Diese Person hinzufügen**.

   Oder

   Klicken Sie auf **Person hinzufügen und einen weiteren starten** , um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.

Dadurch wird in Workfront ein neues Konto für den Benutzer erstellt.

Wenn Sie die Option zum Senden einer Einladung an den Benutzer ausgewählt haben, sollte dieser eine E-Mail erhalten, über die er einem Link folgen kann, um sein Workfront-Kennwort zu erstellen.

>[!NOTE]
>
Wenn Ihr Unternehmen in die Admin Console integriert wurde und Sie einen Benutzer über Workfront hinzufügen, haben Sie keine Möglichkeit, eine Einladung per E-Mail zu senden.
>
Für bestehende Adobe-Benutzer kann der Benutzer eine E-Mail über die Verfügbarkeit von Workfront erhalten oder auch nicht. Dies ist eine vom Adobe-Administrator kontrollierte Voreinstellung für das Produkt.
