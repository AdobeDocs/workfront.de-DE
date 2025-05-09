---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Verwalten des Projektteams
description: Das Projektteam besteht aus Benutzern, die mit dem Projekt verknüpft sind. Die Mitglieder des Projektteams werden im Abschnitt Personen des Projekts angezeigt.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Verwalten des Projektteams

Das Projektteam besteht aus Benutzern, die mit dem Projekt verknüpft sind. Die Mitglieder des Projektteams werden im Abschnitt Personen des Projekts angezeigt.

## Zugriffsanforderungen

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Anzeigen von oder höherem Zugriff auf Benutzer</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Hinzufügen von Benutzern zu einem Projektteam

Wenn Sie Benutzer zum Projektteam hinzufügen, erhalten diese Ansichtsberechtigungen für das Projekt sowie für die Aufgaben, Probleme und Dokumente des Projekts. Weitere Informationen finden Sie im Artikel [Projektteam - Übersicht](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Benutzer des Projektteams werden nicht automatisch zu den Ressourcenverwaltungs-Tools für das Projekt hinzugefügt.

Sie können Benutzer wie folgt zum Projekt-Team hinzufügen:

* [Benutzer automatisch einem Projektteam hinzufügen](#automatically-add-users-to-a-project-team)
* [Manuelles Hinzufügen von Benutzern zu einem Projektteam](#manually-add-users-to-a-project-team)

### Benutzer automatisch einem Projektteam hinzufügen {#automatically-add-users-to-a-project-team}

Die Benutzer, die die folgenden Rollen im Projekt erfüllen, werden automatisch zum Projektteam hinzugefügt und erscheinen im Abschnitt Personen , wenn das Projekt erstellt wird:

* Der Ersteller des Projekts
* Der Projektbesitzer
* Der Projektsponsor

Benutzer werden auch automatisch zum Projekt-Team hinzugefügt, wenn sie Folgendem zugewiesen sind:

* Aufgaben
* Probleme

### Manuelles Hinzufügen von Benutzern zu einem Projektteam {#manually-add-users-to-a-project-team}

Wenn Benutzer, die keine Rolle im Projekt erfüllen, über bestimmte Aktualisierungen oder Änderungen während der Laufzeit des Projekts benachrichtigt werden möchten, können Sie sie manuell zum Projektteam hinzufügen.

Weitere Informationen dazu, welche Benachrichtigungen für Benutzende im Projektteam aktiviert werden können, finden Sie unter [Typen von Ereignisbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Gehen Sie zu dem Projekt, dem Benutzer hinzugefügt werden sollen.

1. Klicken Sie **linken** auf „Personen“.

1. Klicken Sie **Benutzer hinzufügen**.

   Das Dialogfeld Benutzer zum Projektteam hinzufügen wird angezeigt.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. Geben **in das Feld &quot;** hinzufügen“ den Namen eines aktiven Workfront-Benutzers ein, den Sie dem Projektteam hinzufügen möchten. Klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   Wiederholen Sie diesen Schritt, um dem Projekt-Team mehrere Benutzer hinzuzufügen. Die Benutzer müssen zu der mit dem Projekt verknüpften Gruppe gehören.

   >[!TIP]
   >
   >* Sie können keine Benutzer hinzufügen, indem Sie deren Teams, Gruppen, Unternehmen oder Aufgabengebiete hinzufügen.
   >* Beachten Sie beim Hinzufügen der Benutzer den Avatar, die Primäre Rolle des Benutzers und seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.
   >
   >  Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Benutzerzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Klicken Sie **Hinzufügen**.

   Die Benutzer erhalten Ansichtsberechtigungen für das Projekt und erhalten als Teil des Projektteams Benachrichtigungen über das Projekt.

## Entfernen von Benutzern aus einem Projektteam

Wenn Sie Benutzer aus ihren Rollen im Projekt entfernen, bleiben sie Teil des Projektteams.

Wenn Sie einen Benutzer aus dem Projektteam entfernen und der Benutzer Aufgaben oder Problemen im Projekt zugewiesen ist, wird die Zuweisung des Benutzers für die Aufgaben und Probleme aufgehoben, die noch nicht abgeschlossen sind. In diesem Fall kehren die Aufgaben und Probleme zum Bereich Nicht zugewiesene Arbeit im Workload-Balancer zurück.

Benutzer, die abgeschlossenen Aufgaben und Problemen zugewiesen sind, bleiben auch dann zugewiesen, wenn Sie sie aus dem Projektteam entfernen.

Weitere Informationen zum Entfernen von Benutzern aus dem Projektteam finden Sie unter [Entfernen von Benutzern aus Projekten](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
