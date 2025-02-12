---
title: Benutzer importieren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können Benutzende in die Adobe Workfront-Site importieren, indem Sie sie mit einem Netzwerkverzeichnisdienst (z. B. Active Directory oder einem anderen LDAP-Ordner) synchronisieren, oder Sie können Benutzende mithilfe einer Tabellenimportdatei importieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '485'
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

Bevor Sie einen neuen Benutzer erstellen, stellen Sie zunächst sicher, dass Sie alle Objekte erstellt haben, die Sie mit dem Benutzer verknüpfen möchten. Wenn Sie beispielsweise keinen Zeitplan erstellt haben, können Sie dem neuen Benutzer keinen Zeitplan zuweisen. Das Feld, mit dem Sie dem neuen Benutzer einen Zeitplan zuordnen, wird nicht im Bildschirm „Neuer Benutzer“ angezeigt.

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

## Importieren von Benutzenden mit einer Tabellenkalkulationsimportdatei

{{step-1-to-users}}

1. Klicken Sie auf **Dropdown** Pfeil „Neuer Benutzer“ und dann auf **Benutzer importieren**.

1. Laden **im angezeigten** „Benutzer importieren“ die Beispieldatei herunter und aktualisieren Sie dann die Beispieldatei, um die persönlichen Informationen Ihrer eigenen Benutzer einzuschließen.

   Jede Zeile enthält die folgenden Felder:

   * **Vorname**
   * **Nachname**
   * **E-Mail-**

     E-Mail-Adressen müssen eindeutig sein.

   * **Zugriffsebene**

     Bei Zugriffsebenen wird zwischen Groß- und Kleinschreibung unterschieden.

   * **SSO Anmelde-ID**

     Dieses Feld ist nur enthalten, wenn SSO in Ihrem System aktiviert ist. Sie müssen für jeden Benutzer die Federation ID in diesem Feld hinzufügen. Wenn Sie einen Benutzer über die Registerkarte Personen erstellen, können Sie ein Kennwort für den Benutzer einrichten, wenn Sie Benutzern die Anmeldung ohne SSO ermöglichen möchten. Die Importfunktion erlaubt es jedoch nicht, die SSO-ANMELDE-ID leer zu lassen.

   * Stellen Sie sicher, dass vor oder nach der E-Mail-Adresse eines Benutzers keine zusätzlichen Leerzeichen vorhanden sind.

   Wenn Sie mit einer Zeile fertig sind, sollte sie wie folgt aussehen:

   ![import-new-users.png](assets/importing-new-users.png)

1. Speichern Sie die Datei an einem Speicherort auf Ihrer Workstation.
1. Klicken Sie **Feld** Benutzer importieren **auf „Datei**&quot;.

1. Navigieren Sie zu und wählen Sie die Datei aus, die Sie gespeichert haben.
1. (Optional) Wählen Sie die Option **Einladungs-E-Mail an diesen Benutzer senden**, um dem Benutzer eine E-Mail-Einladung zu senden, in der er darüber informiert wird, dass ein Workfront-Konto erstellt wurde, und in der er aufgefordert wird, sein Kennwort festzulegen.

   Deaktivieren Sie diese Option, wenn Sie das Kennwort für den Benutzer festlegen möchten.

1. Klicken Sie **Importieren**.

   Sie erhalten oben im Bildschirm eine Bestätigungsmeldung, dass der Benutzer erfolgreich importiert wurde.
