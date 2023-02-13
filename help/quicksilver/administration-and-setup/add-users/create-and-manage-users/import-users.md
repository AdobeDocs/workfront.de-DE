---
title: Benutzer importieren
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können Benutzer zur Adobe Workfront-Site importieren, indem Sie Benutzer von einem Netzwerkordnerdienst (z. B. Active Directory oder einem anderen LDAP-Ordner) synchronisieren oder mithilfe einer Tabellenimportdatei importieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# Benutzer importieren

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Anweisungen zum Bearbeiten eines Benutzerprofils in der Adobe Admin Console finden Sie im Abschnitt &quot;Benutzer hinzufügen&quot;im Artikel [Massen-Upload von Benutzern](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) oder wenden Sie sich an Ihren Adobe Admin Console-Administrator.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Sie können Benutzer mithilfe einer Tabellenimportdatei importieren.

Bevor Sie einen neuen Benutzer erstellen, stellen Sie zunächst sicher, dass Sie alle Objekte erstellt haben, die Sie mit dem Benutzer verknüpfen möchten. Wenn Sie beispielsweise keinen Zeitplan erstellt haben, können Sie dem neuen Benutzer keinen Zeitplan zuweisen. Das Feld, mit dem Sie einen Zeitplan mit dem neuen Benutzer verknüpfen, wird nicht im Bildschirm &quot;Neuer Benutzer&quot;angezeigt.

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

## Importieren von Benutzern mithilfe einer Tabellenimportdatei

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).

1. Klicken Sie auf **Neuer Benutzer** Dropdownpfeil und klicken Sie dann auf **Benutzer importieren**.

1. Im **Benutzer importieren** , das angezeigt wird, laden Sie die Beispieldatei herunter und aktualisieren Sie dann die Beispieldatei, um die personenbezogenen Daten Ihres eigenen Benutzers einzuschließen.

   Jede Zeile enthält die folgenden Felder:

   * **Vorname**
   * **Nachname**
   * **E-Mail-Adresse**

      E-Mail-Adressen müssen eindeutig sein.

   * **Zugriffsebene**

      Bei Zugriffsebenen wird zwischen Groß- und Kleinschreibung unterschieden.

   * **SSO Anmelde-ID**

      Dieses Feld ist nur enthalten, wenn SSO in Ihrem System aktiviert ist. Sie müssen in diesem Feld für jeden Benutzer die Föderations-ID hinzufügen. Wenn Sie einen Benutzer auf der Registerkarte &quot;Personen&quot;erstellen, können Sie ein Kennwort für den Benutzer einrichten, wenn Sie es Benutzern ermöglichen möchten, sich ohne einmalige Anmeldung anzumelden. Die Importfunktion ermöglicht es jedoch nicht, die SSO-LOGIN-ID leer zu lassen.

   * Stellen Sie sicher, dass vor oder nach der E-Mail-Adresse eines Benutzers keine zusätzlichen Leerzeichen vorhanden sind.

   Wenn Sie mit einer Zeile fertig sind, sollte sie wie folgt aussehen:

   ![importing-new-users.png](assets/importing-new-users.png)

1. Speichern Sie die Datei an einem Speicherort auf Ihrer Workstation.
1. Klicken **Datei auswählen** im **Benutzer importieren** ankreuzen.

1. Navigieren Sie zur gespeicherten Datei und wählen Sie sie aus.
1. (Optional) Wählen Sie die **Senden einer Einladungs-E-Mail an diesen Benutzer** die Option zum Senden einer E-Mail-Einladung an den Benutzer, die Benachrichtigung, dass ein Workfront-Konto erstellt wurde, und die Aufforderung, sein Kennwort festzulegen.

   Deaktivieren Sie diese Option, wenn Sie das Kennwort für den Benutzer festlegen möchten.

1. Klicken **Import**.

   Oben auf dem Bildschirm erhalten Sie eine Bestätigungsmeldung, dass der Benutzer erfolgreich importiert wurde.
