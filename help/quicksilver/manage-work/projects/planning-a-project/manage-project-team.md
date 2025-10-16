---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Verwalten des Projektteams
description: Das Projektteam besteht aus Benutzern, die mit dem Projekt verknüpft sind. Die Mitglieder des Projektteams werden im Abschnitt Personen des Projekts oder im Abschnitt Personen der Vorlage angezeigt, die zum Erstellen eines Projekts verwendet werden kann.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 2%

---

# Verwalten des Projektteams

<!--take preview and production references out at production - August 7-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>

-->

Das Projektteam besteht aus Benutzern, die mit dem Projekt verknüpft sind. Weitere Informationen finden Sie unter [Übersicht über das Projektteam](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

Die Mitglieder des Projektteams werden im Abschnitt Personen des Projekts angezeigt.

Die Benutzer, die im Abschnitt Personen einer Projektvorlage angezeigt werden, werden zum Projektteam, nachdem das Projekt aus der Vorlage erstellt wurde.

Die folgenden Benutzer werden dem Projekt-Team automatisch für Projekte und Vorlagen hinzugefügt:

* Besitzerin bzw. Besitzer
* Sponsor
* Benutzern, die Aufgaben zugewiesen wurden
* Benutzern, die Problemen zugewiesen sind (nur für ein Projekt)

Benutzer im Projektteam erhalten Benachrichtigungen über das Projekt. Weitere Informationen finden Sie unter [Ereignistypen](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Sie können die Benutzer in den Teams des Projekts und der Vorlage verwalten, indem Sie sie hinzufügen (nur für das Projekt), entfernen oder ihnen eine Aktualisierung senden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
    <p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Vorlagen bearbeiten</p> <p>Anzeigen von oder höherem Zugriff auf Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für ein Projekt oder eine Vorlage</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

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
   <td> <p>Standard </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>View or higher access to Users</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project or to a template</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 



## Manage people on a project

1. Go to the project you want to manage the project team for.

   >[!TIP]
   >
   >You must have users assigned to tasks, issues or as stakeholders on the project to have them display in the People section.

1. Click **People** in the left panel. 

1. Click **Add users**. 

   The **Add users to Project Team** box displays.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In the **Add users** box, begin typing the name of an active Workfront user that you want to add to the project team, then click the name when it appears in the list.

   Repeat this step to add multiple users to the project team. The users must belong to the group associated with the project. 

   >[!TIP]
   >
   >* You cannot add users by adding their teams, groups, companies, or job roles.
   >* As you add the users, notice the avatar, the user's Primary Role, and their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them.
   >
   >  You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Click **Add**.

   The users gain View permissions to the project and receive notifications about the project as part of the project team.

1. (Optional) If you want a user to receive a  notification when their job role is added to a task, issue, or project approval, click inside the **Job Role** column for the user, and select a job role that will be associated with the approval. 

   The users will receive notifications related to the approvals assigned to the selected job role. 

   For more information see the "Role-based approvals" section in the article [Project Team overview](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Select one or several users in the list, then click the **Remove** icon ![Remove icon](assets/remove-icon.png) to remove them from the team. 
 
1. Click **Yes, Remove Selected Users** to confirm and remove the users.

   Users are removed and unassigned from incomplete work items.

   For more information, see the [Considerations for removing users from a project team](#considerations-for-removing-users-from-a-project-team) section in this article.
1. (Optional) To send an update for this project to users, click **Update All** to send the update to everyone on the team

   Or 

   Select one or multiple users in the list, then click **Send Update to User**.

   <!--update screen shot when they fix the bug - the text above the box needs to match the OLD box, below-->

![Update an Benutzerfeld im Projekt senden](assets/send-update-to-user-on-project-box-2025.png)

<!--Old UI for projects but the text above the comment box is right and matches the functionality):
   ![OLD Send update to user on a project](assets/send-update-to-user-on-project-box.png)-->

Das **Update an Benutzer senden** wird geöffnet.

1. Führen Sie einen der folgenden Schritte aus:

   * Für die ausgewählten Benutzer eine Aktualisierung hinzufügen.
   * Klicken Sie auf das Schlosssymbol, um die Aktualisierung für die Benutzer in Ihrer Firma privat zu machen.
   * Taggen Sie zusätzliche Benutzer, um dasselbe Update zu erhalten.
   * Klicken Sie auf **Senden**.

   Die Aktualisierung wird zum Abschnitt **Updates** des Projekts hinzugefügt und alle ausgewählten Benutzer werden als getaggte Benutzer angezeigt.

   Benutzer erhalten möglicherweise eine E-Mail-Benachrichtigung, wenn sie für sie aktiviert sind, und sie erhalten eine In-App-Benachrichtigung über das neue Update.

1. (Optional) Klicken Sie auf **Export**-Symbol ![Export-Symbol](assets/export-icon.png), um die Benutzerliste in eine Datei zu exportieren

   Oder

   Wählen Sie Benutzer aus und klicken Sie dann auf das **Exportieren**-Symbol, um nur bestimmte Benutzer zu exportieren.

## Personen in einer Vorlage verwalten

1. Wechseln Sie zu der Vorlage, für die Sie das Projektteam verwalten möchten.

   >[!TIP]
   >
   >Sie müssen Benutzer haben, die Aufgaben zugewiesen sind, oder als Stakeholder auf der Vorlage, damit sie im Abschnitt Personen angezeigt werden.

1. Klicken Sie **linken** auf „Personen“.

1. Wählen Sie einen oder mehrere Benutzer aus der Liste aus und klicken Sie dann auf das Symbol **Entfernen**, um sie aus dem Team zu entfernen.

1. Klicken Sie **Ja, Ausgewählte Benutzer entfernen**, um die Benutzer zu bestätigen und zu entfernen.

   Benutzer werden aus den Vorlagenaufgaben entfernt und ihre Zuweisung wird aufgehoben.

   Weitere Informationen finden Sie im Abschnitt [Überlegungen zum Entfernen von Benutzern aus einem &#x200B;](#considerations-for-removing-users-from-a-project-team)) in diesem Artikel.

1. (Optional) Um eine Aktualisierung an Benutzer zu senden, klicken Sie auf **Alle aktualisieren**, um die Aktualisierung an alle Benutzer in der Liste zu senden

   Oder

   Wählen Sie einen oder mehrere Benutzer aus der Liste aus und klicken Sie dann auf **Update an Benutzer senden**.

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![Aktualisierung an Benutzerfeld in der Vorlage senden](assets/send-update-to-user-on-template-box.png)

   Das **Update an Benutzer senden** wird geöffnet.

1. Gehen Sie folgendermaßen vor:

   * Für die ausgewählten Benutzer eine Aktualisierung hinzufügen.
   * Klicken Sie **Personen taggen**, um zusätzliche Benutzer zu taggen, damit sie dasselbe Update erhalten.
   * Wählen Sie die Option **Privat für meine Firma** aus, um die Aktualisierung für die Benutzer in Ihrer Firma privat zu machen.
   * Klicken Sie auf **Senden**.

     >[!TIP]
     >
     >Die Einstellung **Privat für meine**) ist nur verfügbar, wenn Ihr Workfront-Profil mit einer Firma verknüpft ist.

   Die Aktualisierung wird zum Abschnitt **Aktualisierungen** des Profils jedes getaggten Benutzers hinzugefügt.

   Benutzer erhalten möglicherweise eine E-Mail-Benachrichtigung, wenn sie für sie aktiviert sind, und sie erhalten eine In-App-Benachrichtigung über das neue Update.

1. Klicken Sie auf **Export**-Symbol ![Export-Symbol](assets/export-icon.png), um die Benutzerliste in eine Datei zu exportieren

   Oder

   Wählen Sie Benutzer aus und klicken Sie dann auf das **Exportieren**-Symbol, um nur bestimmte Benutzer zu exportieren.

## Überlegungen zum Entfernen von Benutzern aus einem Projektteam

Wenn Sie Benutzer aus ihren Rollen im Projekt entfernen, bleiben sie Teil des Projektteams.

Sie müssen sie aus dem Projektteam aus dem Abschnitt Personen des Projekts entfernen, damit sie keine Benachrichtigungen mehr an das Projektteam erhalten.

Wenn Sie einen Benutzer aus dem Projektteam entfernen und der Benutzer Aufgaben oder Problemen im Projekt zugewiesen ist, wird die Zuweisung des Benutzers für die Aufgaben und Probleme aufgehoben, die noch nicht abgeschlossen sind. In diesem Fall kehren die Aufgaben und Probleme zum Bereich Nicht zugewiesene Arbeit im Workload-Balancer zurück.

Benutzer, die abgeschlossenen Aufgaben und Problemen zugewiesen sind, bleiben den Aufgaben und Problemen zugewiesen, selbst wenn Sie sie aus dem Projektteam entfernen.

Die folgenden Benutzer werden aus ihren Rollen im Projekt entfernt, wenn Sie sie aus dem Abschnitt Personen eines Projekts oder einer Vorlage entfernen:

* Benutzern, die noch nicht abgeschlossenen Aufgaben zugewiesen wurden
* Benutzern, die noch nicht vollständig abgewickelten Problemen zugewiesen wurden

Die folgenden Benutzer werden nicht aus ihren Rollen im Projekt entfernt, wenn Sie sie aus dem Abschnitt Personen eines Projekts oder einer Vorlage entfernen:

* Besitzerin bzw. Besitzer
* Sponsor

Weitere Informationen zum Entfernen von Benutzern aus dem Projektteam finden Sie unter [Entfernen von Benutzern aus Projekten](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).

