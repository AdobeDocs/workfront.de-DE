---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Verwalten des Projektteams
description: Das Projektteam besteht aus Benutzern, die mit dem Projekt verknüpft sind. Die Mitglieder des Projektteams werden im Abschnitt Personen des Projekts oder im Abschnitt Personen der Vorlage angezeigt, die zum Erstellen eines Projekts verwendet werden kann.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: a00776ecd9f8dc14b9dce14ce9463c2bb709a363
workflow-type: tm+mt
source-wordcount: '1399'
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

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen. 

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
   <td> <p>Standard </p>
    <p>Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Vorlagen bearbeiten</p> <p>Anzeigen von oder höherem Zugriff auf Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für ein Projekt oder eine Vorlage</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
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

*To find out what plan, license type, or access you have, contact your Workfront administrator.-->

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

## Personen in einem Projekt verwalten

1. Wechseln Sie zu dem Projekt, für das Sie das Projektteam verwalten möchten.

   >[!TIP]
   >
   >Sie müssen Benutzer bzw. Benutzerinnen, die Aufgaben, Problemen oder als Stakeholder im Projekt zugewiesen sind, haben, damit sie im Abschnitt Personen angezeigt werden.

1. Klicken Sie **linken** auf „Personen“.

1. Klicken Sie **Benutzer hinzufügen**.

   Das **Benutzer zum Projektteam hinzufügen** wird angezeigt.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. Geben **in das Feld &quot;** hinzufügen“ den Namen eines aktiven Workfront-Benutzers ein, den Sie dem Projektteam hinzufügen möchten. Klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Wiederholen Sie diesen Schritt, um dem Projekt-Team mehrere Benutzer hinzuzufügen. Die Benutzer müssen zu der mit dem Projekt verknüpften Gruppe gehören.

   >[!TIP]
   >
   >* Sie können keine Benutzer hinzufügen, indem Sie deren Teams, Gruppen, Unternehmen oder Aufgabengebiete hinzufügen.
   >* Beachten Sie beim Hinzufügen der Benutzer den Avatar, die Primäre Rolle des Benutzers und seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.
   >
   >  Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter [Gewähren des Benutzerzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. Klicken Sie auf **Hinzufügen**.

   Die Benutzer erhalten Ansichtsberechtigungen für das Projekt und erhalten als Teil des Projektteams Benachrichtigungen über das Projekt.

1. (Optional) Wenn ein(e) Benutzende(r) eine Benachrichtigung erhalten soll, wenn sein/ihr Aufgabengebiet zu einer Aufgaben-, Problem- oder Projektgenehmigung hinzugefügt wird, klicken Sie in die Spalte **Aufgabengebiet** für den/die Benutzende und wählen Sie ein Aufgabengebiet aus, das mit der Genehmigung verknüpft werden soll.

   Die Benutzer erhalten Benachrichtigungen im Zusammenhang mit den Genehmigungen, die dem ausgewählten Aufgabengebiet zugewiesen wurden.

   Weitere Informationen finden Sie im Abschnitt „Rollenbasierte Genehmigungen“ im Artikel [Projektteam - Übersicht](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md).

1. Wählen Sie einen oder mehrere Benutzer aus der Liste aus und klicken Sie dann auf das Symbol **Entfernen** ![Symbol entfernen](assets/remove-icon.png), um sie aus dem Team zu entfernen.

1. Klicken Sie **Ja, Ausgewählte Benutzer entfernen**, um die Benutzer zu bestätigen und zu entfernen.

   Benutzer werden aus unvollständigen Arbeitselementen entfernt und deren Zuweisung aufgehoben.

   Weitere Informationen finden Sie im Abschnitt [Überlegungen zum Entfernen von Benutzern aus einem ](#considerations-for-removing-users-from-a-project-team)) in diesem Artikel.
1. (Optional) Um eine Aktualisierung für dieses Projekt an Benutzer zu senden, klicken Sie auf **Alle aktualisieren** um die Aktualisierung an alle Mitglieder des Teams zu senden

   Oder

   Wählen Sie einen oder mehrere Benutzer aus der Liste aus und klicken Sie dann auf **Update an Benutzer senden**.

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

   Weitere Informationen finden Sie im Abschnitt [Überlegungen zum Entfernen von Benutzern aus einem ](#considerations-for-removing-users-from-a-project-team)) in diesem Artikel.

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

