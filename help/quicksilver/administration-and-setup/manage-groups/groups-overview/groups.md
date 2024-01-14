---
title: Gruppenübersicht
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Ein Workfront-Administrator kann Benutzergruppen erstellen, die mit Ihrer Abteilungsstruktur übereinstimmen. Gruppen sind ähnlich, unterscheiden sich aber von Teams und Unternehmen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: 9c4aa8d1f812299ba6cdcb664b990c1119e3cb31
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Gruppenübersicht

Ein Workfront-Administrator kann Benutzergruppen erstellen, die mit Ihrer Abteilungsstruktur übereinstimmen. Gruppen sind ähnlich, unterscheiden sich aber von Teams und Unternehmen.

Der Workfront-Administrator gewährt Gruppen Zugriff auf die Bereiche der Workfront, in denen sie arbeiten und kommunizieren müssen. Jede Gruppe kann dann ihre Workfront-Informationen wie Benutzer, Vorlagen, benutzerdefinierte Formulare und Projekte von denen anderer Abteilungen trennen.

Für jede Gruppe ist mindestens ein Gruppenadministrator erforderlich. Gruppenadministratoren können die Seite Gruppen verwenden, um ihre Gruppen an einem Ort zu verwalten. Weitere Informationen finden Sie unter [Gruppenadministratoren](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Sie können bis zu 14 Ebenen von Untergruppen unter einer Gruppe erstellen. Weitere Informationen finden Sie unter [Übersicht über Untergruppen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) und [Erstellen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Verwenden von Gruppen zum Organisieren von Benutzern

Als Workfront-Administrator oder Gruppenadministrator können Sie Benutzer Gruppen und Untergruppen zuordnen. Wenn Sie eine Gruppe öffentlich machen, können Benutzer mit einer Planner-Lizenz Benutzer damit verknüpfen. Weitere Informationen zu Gruppenadministratoren und öffentlichen Gruppen finden Sie unter [Gruppe erstellen](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Wenn Sie einen Benutzer erstellen, empfehlen wir, diesen Benutzer der entsprechenden Startseite und anderen Gruppen hinzuzufügen, in denen der Benutzer arbeiten soll. Ein Benutzer kann nur über eine Home Group verfügen, sich jedoch mehreren anderen Gruppen angehören.

Durch die Mitgliedschaft in einer Gruppe erhält der Benutzer Zugriff auf Objekte, die für die Gruppe und die Untergruppen freigegeben sind. Wenn Sie beispielsweise ein Projekt für eine Gruppe freigeben, haben Benutzer in der Gruppe und die Untergruppen der Gruppe Zugriff darauf.

>[!TIP]
>
>Wenn Abteilungen in Ihrer Organisation häufig zusammenarbeiten, um Projekte und die Ressourcen für diese Projekte zu verwalten, ist es möglicherweise nicht erforderlich, Abteilungen in viele kleinere Gruppen zu unterteilen. Einige hochrangige Gruppen könnten am besten funktionieren.

Eine Gruppe kann eine unbegrenzte Anzahl von Benutzern haben.

Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/add-users.md).

## Gewähren des Gruppenzugriffs auf Objekte

Wenn Sie ein Objekt für eine Gruppe freigeben, haben alle Mitglieder dieser Gruppe (einschließlich Mitglieder von Untergruppen) Zugriff auf das Objekt. Weitere Informationen zur Freigabe in Workfront finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Zuordnen einer Gruppe zu einem Objekt

Wenn Sie eines der folgenden Workfront-Objekte erstellen oder bearbeiten, können Sie es mit einer Gruppe verknüpfen:

* **Projekt**: Sie können eine einzelne Gruppe mit einem Projekt verknüpfen, um die Eigentümerschaft des Projekts anzugeben.

  Dadurch werden nicht implizit jedem Mitglied der Gruppe Berechtigungen für das Projekt gewährt. Um Berechtigungen für das Projekt zu erhalten, müssen Benutzer das Projekt für sie freigeben.

  Benutzer können zwar Mitglieder mehrerer Gruppen sein, einem Projekt kann jedoch eine einzelne Gruppe zugeordnet sein. Benutzer aus anderen Gruppen können weiterhin an demselben Projekt arbeiten, wenn das Projekt für sie oder ihre Gruppen freigegeben wurde. Die mit dem Projekt verbundene Gruppe ist in der Regel entweder die Gruppe, die für den Abschluss des Projekts verantwortlich ist, oder die Gruppe, für die das Projekt bereitgestellt wird.

  Anweisungen zum Verknüpfen eines Projekts mit einer Gruppe finden Sie unter [Informationen im Bereich &quot;Projektübersicht&quot;verwalten](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, Programm oder Unternehmen**: Wenn Sie ein Portfolio, Programm oder Unternehmen erstellen oder bearbeiten, können Sie ihm eine einzelne Gruppe zuweisen, um anzugeben, dass die Gruppe für dieses Portfolio verantwortlich ist oder ist. Mit dieser Vereinigung können Administratoren und Benutzer leicht erkennen, an welchen Portfolios, Programmen und Unternehmen ihre Gruppen arbeiten.

  Beispielsweise kann ein Gruppenadministrator alle Portfolios in der Organisation mithilfe einer Liste oder eines Berichts auflisten und in der Spalte Gruppe feststellen, welchen Portfolios seine Gruppe zugewiesen ist.

  >[!NOTE]
  >
  >Die Zuweisung einer Gruppe zu einem Portfolio, Programm oder Unternehmen mit einer Gruppe bedeutet nicht automatisch, dass die Informationen in der Gruppe Zugriff auf die Daten haben. Sie müssen den Zugriff auf die Daten manuell für die Gruppe freigeben, bevor sie sie sehen können.

  Anweisungen finden Sie unter [Erstellen eines Portfolios](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Programm erstellen](../../../manage-work/portfolios/create-and-manage-programs/create-program.md), und [Erstellen und Bearbeiten von Unternehmen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Validierungsprozess**: Sie können einen Genehmigungsprozess für Projekte, Aufgaben und Probleme einer bestimmten Gruppe verfügbar machen. Weitere Informationen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Milestone-Pfad**: Sie können Benutzern in bestimmten Gruppen erlauben, einen Meilensteinpfad für ihre Projekte zu verwenden. Weitere Informationen finden Sie unter [Meilensteinpfad erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Layout-Vorlage**: Sie können den Administratoren einer Gruppe die Berechtigung zum Ändern einer Layout-Vorlage erteilen. Anweisungen finden Sie unter [Administratorzugriff für eine Layoutvorlage gewähren](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Datenblatt-Profil**: Sie können den Administratoren einer Gruppe die Berechtigung zum Ändern eines Timesheet-Profils erteilen. Weitere Informationen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Zeitpläne**: Sie können den Administratoren einer Gruppe die Berechtigung zum Ändern eines Zeitplans erteilen. Weitere Informationen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Teams**: Sie können eine Gruppe mit einem Team verknüpfen, sodass die Administratoren der Gruppen und ihrer Untergruppen diese Teams aus dem Bereich Gruppen anzeigen und verwenden können. Weitere Informationen finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) oder [Team-Einstellungen bearbeiten](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Vorlage**: Sie können einer Projektvorlage eine Gruppe zuweisen. Auf diese Weise können Sie den Prozess zur Projekterstellung optimieren und leichter erkennen und Berichte zu den Gruppen erstellen, deren Projektvorlagen gehören. Weitere Informationen finden Sie im Abschnitt . [Übersicht](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) im Artikel [Bearbeiten von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Kürzlich gelöschte und wiederhergestellte Elemente**: Sie können die zuletzt gelöschten Gruppen anzeigen und verwalten. Weitere Informationen finden Sie unter [Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) und [Anzeigen und Verwalten der kürzlich wiederhergestellten Elemente einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
