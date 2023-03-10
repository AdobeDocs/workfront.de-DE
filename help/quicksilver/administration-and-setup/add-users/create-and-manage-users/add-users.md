---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Benutzer hinzufügen
description: Als Workfront-Administrator oder Benutzer mit vollem Administratorzugriff können Sie Benutzer in Workfront hinzufügen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Benutzer hinzufügen

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Anweisungen zum Hinzufügen eines Benutzers in Adobe Admin Console:
>
>* Siehe [Erstellen von Benutzern in Workfront mit Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* Siehe Abschnitt &quot;Benutzer hinzufügen&quot;im Artikel [Benutzer einzeln verwalten](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Wenden Sie sich an Ihren Adobe Admin Console-Administrator.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Sie können Benutzer in Adobe Workfront hinzufügen, indem Sie einzelne Benutzer von Grund auf neu erstellen oder vorhandene Benutzer kopieren.

Informationen dazu, wie Sie mehrere Benutzer gleichzeitig importieren, finden Sie unter [Benutzer importieren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsstufe konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens eines der beiden <b>Benutzer-Admin</b> Optionen aktiviert unter <b>Einstellungen anpassen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie ein Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> <p>Weitere Informationen zum <b>Benutzer</b> auf einer Zugriffsebene festzulegen, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

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
* Welche berufliche Rolle spielt die Person? Gibt es diese Rolle in Workfront? Gibt es eine Begrenzung für die Zahl der Personen, die diese Aufgabe erfüllen können? Weitere Informationen zum Erstellen von Auftragsrollen finden Sie unter [Erstellen und Verwalten von Vorgangsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Welche Zugriffsebene sollte der Benutzer haben? Existiert es bereits oder müssen Sie ein neues erstellen? Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* In welcher Startseite sollte dieser Benutzer sein? Sollte die Person in mehr als einer Gruppe sein? Weitere Informationen zu Gruppen finden Sie unter [Gruppenübersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* In welchem Heimteam sollte dieser Benutzer sein? Sollte die Person in mehr als einem Team sein? Weitere Informationen zu Teams finden Sie unter [Teams - Übersicht](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Welche benutzerdefinierten Informationen müssen Sie mit diesem Benutzer verknüpfen?

   Wenn Informationen zu Benutzern in von Ihnen erstellten benutzerdefinierten Feldern erfasst werden, müssen Sie beim Erstellen eines Benutzers über ein benutzerdefiniertes Formular verfügen. Informationen zu benutzerdefinierten Formularen finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Neuen Benutzer erstellen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).

1. Klicken **Neuer Benutzer > Neuer Benutzer** , um einen Benutzer hinzuzufügen, der noch nicht zu Workfront hinzugefügt wurde.

   Oder

   Klicken **Neuer Benutzer > Benutzer importieren** , um Benutzer durch Hochladen einer Datei für den Tabellenimport hinzuzufügen.

   Wenn Sie Benutzer importieren, müssen Sie diese Schritte nicht fortsetzen. Weitere Informationen finden Sie unter [Benutzer importieren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. Im **Neuer Benutzer** wird angezeigt, klicken Sie auf **Erweiterte Optionen anzeigen** und konfigurieren Sie dann die verfügbaren Optionen, um die Informationen der Person einzugeben.

   Weitere Informationen zu diesen Optionen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Führen Sie einen der folgenden Schritte aus:

   * Urlaub **Eine Einladungs-E-Mail an diese Person senden** aktiviert. In diesem Fall erhält der Benutzer eine E-Mail, in der er einem Link folgen kann, um sein eigenes Kennwort für Workfront zu erstellen. Benutzer, die die Einladung in die E-Mail nicht annehmen und ein Workfront-Kennwort erstellen, werden in Workfront als Abgemeldet aufgeführt.
   * Deaktivieren **Eine Einladungs-E-Mail an diese Person senden**, und geben Sie dann eine **Passwort** für die Person und bestätigen Sie sie im **Kennwort bestätigen** ankreuzen. Sie müssen dieses Kennwort für den Benutzer außerhalb von Workfront freigeben.

   >[!NOTE]
   >
   >Wenn Ihr Workfront-Administrator eine SSO-Integration in Workfront aktiviert hat, dann ist die Option Nur erlauben &lt;sso configuration=&quot;&quot;> Das Authentifizierungsfeld ist ausgeblendet, wenn Sie die Einladung in eine E-Mail deaktivieren. Die Föderation-ID oder &lt;sso configuration=&quot;&quot;> Das Feld &quot;Benutzername&quot;bleibt sichtbar.

   >[!NOTE]
   Wenn Ihr Unternehmen in die Admin Console integriert wurde und Sie einen Benutzer über Workfront hinzufügen, haben Sie keine Möglichkeit, eine Einladung per E-Mail zu senden.
   Der Admin Console werden neue Adobe-Benutzer hinzugefügt und die Admin Console sendet eine E-Mail, um sie aufzufordern, den Registrierungsprozess abzuschließen. Alle Benutzer müssen den Registrierungsprozess abschließen, um auf ein beliebiges Adobe-System zugreifen zu können.
   Für bestehende Benutzer der Adobe kann der Benutzer eine E-Mail über die Verfügbarkeit von Workfront erhalten oder auch nicht. Dies ist eine vom Produktadministrator verwaltete Voreinstellung.

1. Klicken **Diesen Benutzer hinzufügen**.

   Oder

   Klicken **Benutzer hinzufügen und einen weiteren Benutzer starten** , um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.

## Benutzer kopieren, um einen neuen zu erstellen

Sie können einen Benutzer erstellen, indem Sie einen vorhandenen Benutzer kopieren.

>[!NOTE]
Wenn Sie einen Benutzer auf diese Weise erstellen, werden alle Informationen vom ursprünglichen Benutzer in den neu erstellten Benutzer kopiert, mit Ausnahme der folgenden:
* Die Informationen im Abschnitt &quot;Persönliche Informationen&quot;.
* Wenn ich mich anmelde, zeigen Sie Folgendes an: In diesem Feld wird der Standard-Landingtab für die Zugriffsebene ausgewählt.
* Verzeichnisberichte
>


So erstellen Sie einen neuen Benutzer durch Kopieren eines vorhandenen:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).
1. Wählen Sie den Benutzer aus, den Sie kopieren möchten, und klicken Sie dann auf das Symbol Kopieren . ![](assets/copy-icon.png).
1. Im **Neuer Benutzer** die Felder, die für den neuen Benutzer verfügbar sind, bearbeiten.

   Informationen zu allen Feldern, die mit einem Benutzer verknüpft sind, finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Klicken **Diesen Benutzer hinzufügen**.

   Oder

   Klicken **Benutzer hinzufügen und einen weiteren Benutzer starten** , um den neuen Benutzer zu speichern und einen weiteren hinzuzufügen.

Dadurch wird in Workfront ein neues Konto für den Benutzer erstellt.

Wenn Sie die Option zum Senden einer Einladung an den Benutzer ausgewählt haben, sollte dieser eine E-Mail erhalten, über die er einem Link folgen kann, um sein Workfront-Kennwort zu erstellen.

>[!NOTE]
Wenn Ihr Unternehmen in die Admin Console integriert wurde und Sie einen Benutzer über Workfront hinzufügen, haben Sie keine Möglichkeit, eine Einladung per E-Mail zu senden.
Der Admin Console werden neue Adobe-Benutzer hinzugefügt und die Admin Console sendet eine E-Mail, um sie aufzufordern, den Registrierungsprozess abzuschließen. Alle Benutzer müssen den Registrierungsprozess abschließen, um auf ein beliebiges Adobe-System zugreifen zu können.
Für bestehende Benutzer der Adobe kann der Benutzer eine E-Mail über die Verfügbarkeit von Workfront erhalten oder auch nicht. Dies ist eine vom Produktadministrator verwaltete Voreinstellung.
