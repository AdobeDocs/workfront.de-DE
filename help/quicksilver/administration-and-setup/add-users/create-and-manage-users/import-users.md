---
title: Benutzer importieren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können Benutzer zur Adobe Workfront-Site importieren, indem Sie Benutzer von einem Netzwerkordnerdienst (z. B. Active Directory oder einem anderen LDAP-Ordner) synchronisieren oder mithilfe einer Tabellenimportdatei importieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Benutzer importieren

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Sie können Benutzer mithilfe einer Tabellenimportdatei importieren.

Bevor Sie einen neuen Benutzer erstellen, stellen Sie zunächst sicher, dass Sie alle Objekte erstellt haben, die Sie mit dem Benutzer verknüpfen möchten. Wenn Sie beispielsweise keinen Zeitplan erstellt haben, können Sie dem neuen Benutzer keinen Zeitplan zuweisen. Das Feld, mit dem Sie einen Zeitplan mit dem neuen Benutzer verknüpfen, wird nicht im Bildschirm &quot;Neuer Benutzer&quot;angezeigt.

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

## Importieren von Benutzern mithilfe einer Tabellenimportdatei

{{step-1-to-users}}

1. Klicken Sie auf den Dropdown-Pfeil **Neuer Benutzer** und dann auf **Benutzer importieren**.

1. Laden Sie im angezeigten Feld **Benutzer importieren** die Beispieldatei herunter und aktualisieren Sie dann die Beispieldatei, um die personenbezogenen Daten Ihres eigenen Benutzers einzuschließen.

   Jede Zeile enthält die folgenden Felder:

   * **Vorname**
   * **Nachname**
   * **E-Mail-Adresse**

     E-Mail-Adressen müssen eindeutig sein.

   * **Zugriffsebene**

     Bei Zugriffsebenen wird zwischen Groß- und Kleinschreibung unterschieden.

   * **SSO-Anmelde-ID**

     Dieses Feld ist nur enthalten, wenn SSO in Ihrem System aktiviert ist. Sie müssen in diesem Feld für jeden Benutzer die Föderations-ID hinzufügen. Wenn Sie einen Benutzer auf der Registerkarte &quot;Personen&quot;erstellen, können Sie ein Kennwort für den Benutzer einrichten, wenn Sie es Benutzern ermöglichen möchten, sich ohne einmalige Anmeldung anzumelden. Die Importfunktion ermöglicht es jedoch nicht, die SSO-LOGIN-ID leer zu lassen.

   * Stellen Sie sicher, dass vor oder nach der E-Mail-Adresse eines Benutzers keine zusätzlichen Leerzeichen vorhanden sind.

   Wenn Sie mit einer Zeile fertig sind, sollte sie wie folgt aussehen:

   ![importing-new-users.png](assets/importing-new-users.png)

1. Speichern Sie die Datei an einem Speicherort auf Ihrer Workstation.
1. Klicken Sie im Feld **Benutzer importieren** auf **Datei auswählen** .

1. Navigieren Sie zur gespeicherten Datei und wählen Sie sie aus.
1. (Optional) Wählen Sie die Option **Einladungs-E-Mail an diesen Benutzer senden** aus, um eine E-Mail-Einladung an den Benutzer zu senden. Sie werden benachrichtigt, dass ein Workfront-Konto erstellt wurde, und werden aufgefordert, sein Kennwort festzulegen.

   Deaktivieren Sie diese Option, wenn Sie das Kennwort für den Benutzer festlegen möchten.

1. Klicken Sie auf **Importieren**.

   Oben auf dem Bildschirm erhalten Sie eine Bestätigungsmeldung, dass der Benutzer erfolgreich importiert wurde.
