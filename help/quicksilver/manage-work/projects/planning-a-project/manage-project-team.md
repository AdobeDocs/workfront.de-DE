---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Verwalten des Projektteams
description: Das Projektteam besteht aus Benutzern, die mit dem Projekt verknüpft sind. Die Mitglieder des Projektteams werden im Abschnitt Personen des Projekts angezeigt.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '684'
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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Benutzer</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für das Projekt</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Hinzufügen von Benutzern zu einem Projektteam

Wenn Sie Benutzer zum Projektteam hinzufügen, erhalten sie Anzeigeberechtigungen für das Projekt sowie die Aufgaben, Probleme und Dokumente des Projekts. Weitere Informationen finden Sie im Artikel [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Benutzer im Projektteam werden nicht automatisch zu den Tools für die Ressourcenverwaltung des Projekts hinzugefügt.

Sie können dem Projektteam auf folgende Weise Benutzer hinzufügen:

* [Benutzer automatisch zu einem Projektteam hinzufügen](#automatically-add-users-to-a-project-team)
* [Manuelles Hinzufügen von Benutzern zu einem Projektteam](#manually-add-users-to-a-project-team)

### Benutzer automatisch zu einem Projektteam hinzufügen {#automatically-add-users-to-a-project-team}

Die Benutzer, die die folgenden Rollen im Projekt erfüllen, werden automatisch zum Projektteam hinzugefügt und erscheinen beim Erstellen des Projekts im Abschnitt Personen .

* Der Verfasser des Projekts
* Projekteigentümer
* Der Projektsponsor

Benutzer werden auch automatisch zum Projektteam hinzugefügt, wenn sie den folgenden Benutzern zugewiesen sind:

* Aufgaben
* Probleme

### Manuelles Hinzufügen von Benutzern zu einem Projektteam {#manually-add-users-to-a-project-team}

Wenn Benutzer, die keine Rolle im Projekt erfüllen, über bestimmte Aktualisierungen oder Änderungen während der Projektlaufzeit benachrichtigt werden möchten, können Sie sie manuell zum Projektteam hinzufügen.

Weitere Informationen dazu, welche Benachrichtigungen für Benutzer des Projektteams aktiviert werden können, finden Sie unter [In Adobe Workfront verfügbare Ereignisbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Wechseln Sie zu dem Projekt, dem Sie Benutzer hinzufügen möchten.

1. Klicken **Personen** im linken Bereich. Möglicherweise müssen Sie auf **Mehr anzeigen** zuerst.

1. Klicken **Benutzer hinzufügen**.

   Das Dialogfeld Benutzer zum Projektteam hinzufügen wird angezeigt.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. Im **Benutzer hinzufügen** Geben Sie den Namen eines aktiven Workfront-Benutzers ein, den Sie dem Projektteam hinzufügen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.

   Wiederholen Sie diesen Schritt, um dem Projektteam mehrere Benutzer hinzuzufügen. Die Benutzer müssen zur Gruppe gehören, die mit dem Projekt verknüpft ist.

   >[!TIP]
   >
   >* Sie können keine Benutzer hinzufügen, indem Sie ihre Teams, Gruppen, Unternehmen oder Rollen hinzufügen.
   >* Beachten Sie beim Hinzufügen der Benutzer den Avatar, die Primäre Rolle des Benutzers und seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzer müssen mindestens einer Auftragsrolle zugeordnet sein, damit sie beim Hinzufügen angezeigt werden können.
   >
   >  Sie müssen die Einstellung Kontaktinformationen anzeigen auf Ihrer Zugriffsebene aktivieren, damit Benutzer E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Klicken **Hinzufügen**.

   Die Benutzer erhalten Ansichtsberechtigungen für das Projekt und erhalten Benachrichtigungen über das Projekt als Teil des Projektteams.

## Entfernen von Benutzern aus einem Projektteam

Wenn Sie Benutzer aus ihren Rollen im Projekt entfernen, bleiben sie Teil des Projektteams.

Wenn Sie einen Benutzer aus dem Projektteam entfernen und der Benutzer Aufgaben oder Problemen im Projekt zugewiesen ist, wird die Zuweisung des Benutzers zu den nicht abgeschlossenen Aufgaben und Problemen aufgehoben. In diesem Fall kehren die Aufgaben und Probleme zum nicht zugewiesenen Arbeitsbereich im Arbeitslastausgleich zurück.

Benutzer, die abgeschlossenen Aufgaben und Problemen zugewiesen sind, bleiben auch dann zugewiesen, wenn Sie sie aus dem Projektteam entfernen.

Weitere Informationen zum Entfernen von Benutzern aus dem Projektteam finden Sie unter [Entfernen von Benutzern aus Projekten](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
