---
title: Gruppen - Übersicht
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Ein Workfront-Administrator kann Benutzergruppen erstellen, die mit Ihrer Abteilungsstruktur übereinstimmen. Gruppen ähneln Teams und Unternehmen, unterscheiden sich aber von ihnen.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Gruppen - Übersicht

<!-- Audited: 01/2024 -->

Ein Workfront-Administrator kann Benutzergruppen erstellen, die mit Ihrer Abteilungsstruktur übereinstimmen. Gruppen ähneln Teams und Unternehmen, unterscheiden sich aber von ihnen.

Der Workfront-Administrator gewährt Gruppen Zugriff auf die Workfront-Bereiche, in denen sie arbeiten und kommunizieren müssen. Jede Gruppe kann dann ihre Workfront-Informationen wie Benutzer, Vorlagen und benutzerdefinierte Formulare sowie Projekte getrennt von denen anderer Abteilungen aufbewahren.

Für jede Gruppe ist mindestens ein Gruppenadministrator erforderlich. Gruppenadministratoren können die Seite „Gruppen“ verwenden, um ihre Gruppen an einem Ort zu verwalten. Weitere Informationen finden Sie unter [Gruppenadministratoren](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Sie können bis zu 14 Ebenen von Untergruppen unter einer Gruppe erstellen. Weitere Informationen finden Sie unter [Übersicht über Untergruppen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) und [Erstellen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Verwenden von Gruppen zum Organisieren von Benutzern

Als Workfront-Administrator oder Gruppenadministrator können Sie Benutzende mit Gruppen und Untergruppen verknüpfen. Wenn Sie eine Gruppe öffentlich machen, können Benutzende mit einer Standard- (neuen) oder Plan- (aktuellen) Lizenz ihr Benutzende zuordnen. Weitere Informationen zu Gruppenadministratoren und öffentlichen Gruppen finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Wenn Sie einen Benutzer erstellen, empfehlen wir, diesen Benutzer der entsprechenden Hauptgruppe und anderen Gruppen hinzuzufügen, in denen der Benutzer arbeiten soll. Ein Benutzer kann nur über eine Hauptgruppe verfügen, sich jedoch mehreren anderen Gruppen anschließen.

Die Mitgliedschaft in einer Gruppe ermöglicht Benutzenden den Zugriff auf Objekte, die für die Gruppe und die Untergruppen freigegeben sind. Wenn Sie beispielsweise ein Projekt für eine Gruppe freigeben, haben Benutzende in der Gruppe und deren Untergruppen Zugriff darauf.

>[!TIP]
>
>Wenn Abteilungen in Ihrem Unternehmen häufig zusammenarbeiten, um Projekte und die Ressourcen für diese Projekte zu verwalten, ist es möglicherweise nicht erforderlich, Abteilungen in viele kleinere Gruppen zu unterteilen. Einige hochrangige Gruppen funktionieren vielleicht am besten.

Eine Gruppe kann eine unbegrenzte Anzahl von Benutzern haben.

Weitere Informationen zum Erstellen neuer Benutzer finden Sie unter [Benutzer hinzufügen](../../../administration-and-setup/add-users/add-users.md).

## Gewähren von Gruppenzugriff auf Objekte

Wenn Sie ein Objekt für eine Gruppe freigeben, haben alle Mitglieder dieser Gruppe (einschließlich der Mitglieder von Untergruppen) Zugriff auf das Objekt. Weitere Informationen zur Freigabe in Workfront finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Gruppe mit einem Objekt verknüpfen

Wenn Sie eines der folgenden Workfront-Objekte erstellen oder bearbeiten, können Sie es mit einer Gruppe verknüpfen:

* **Projekt**: Sie können eine einzelne Gruppe mit einem Projekt verknüpfen, um anzugeben, wer Eigentümer des Projekts ist.

  Dadurch werden den einzelnen Mitgliedern der Gruppe nicht implizit Rechte am Projekt gewährt. Damit Benutzer über Rechte für das Projekt verfügen, muss das Projekt für sie freigegeben sein.

  Während Benutzende Mitglieder mehrerer Gruppen sein können, kann einem Projekt eine einzelne Gruppe zugeordnet sein. Benutzer aus anderen Gruppen können weiterhin am selben Projekt arbeiten, wenn das Projekt für sie oder ihre Gruppen freigegeben wurde. Die mit dem Projekt verknüpfte Gruppe ist in der Regel entweder die Gruppe, die für die Fertigstellung des Projekts verantwortlich ist, oder die Gruppe, für die das Projekt bereitgestellt wird.

  Anweisungen zum Verknüpfen eines Projekts mit einer Gruppe finden Sie unter [Verwalten von Informationen im Bereich Projektübersicht](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, Programm oder Unternehmen**: Wenn Sie ein Portfolio, ein Programm oder ein Unternehmen erstellen oder bearbeiten, können Sie ihm eine einzelne Gruppe zuweisen, um anzugeben, dass die Gruppe Eigentümer oder verantwortlich für sie ist. Durch diese Verknüpfung können Administratoren und Benutzer leicht erkennen, an welchen Portfolios, Programmen und Unternehmen ihre Gruppen arbeiten.

  Beispielsweise kann ein Gruppenadministrator alle Portfolios in der Organisation mithilfe einer Liste oder eines Berichts auflisten und in der Spalte Gruppe notieren, welche Portfolios seiner Gruppe zugewiesen sind.

  >[!NOTE]
  >
  >Wenn Sie einer Gruppe ein Portfolio, ein Programm oder ein Unternehmen mit einer Gruppe zuweisen, bedeutet dies nicht automatisch, dass die Informationen in dieser Gruppe Zugriff auf die Daten der Gruppe haben. Sie müssen den Zugriff auf die Daten manuell für die Gruppe freigeben, bevor sie sie sehen können.

  Anweisungen finden Sie unter [Portfolio erstellen](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Programm erstellen](../../../manage-work/portfolios/create-and-manage-programs/create-program.md) und [Firmen erstellen und bearbeiten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Genehmigungsprozess**: Sie können einen Genehmigungsprozess für Projekte, Aufgaben und Probleme einer bestimmten Gruppe verfügbar machen. Weitere Informationen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Meilensteinpfad**: Sie können Benutzern in bestimmten Gruppen die Verwendung eines Meilensteinpfads für ihre Projekte erlauben. Weitere Informationen finden Sie unter [Meilensteinpfad erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Layout-Vorlage**: Sie können den Administratoren einer Gruppe die Berechtigung zum Ändern einer Layout-Vorlage erteilen. Anweisungen finden Sie unter [Gewähren des Administratorzugriffs für eine Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Arbeitszeittabellen-**: Sie können den Administratoren einer Gruppe die Berechtigung erteilen, ein Arbeitszeittabellen-Profil zu ändern. Weitere Informationen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Zeitpläne**: Sie können den Administratoren einer Gruppe die Berechtigung erteilen, einen Zeitplan zu ändern. Weitere Informationen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Teams**: Sie können eine Gruppe mit einem Team verknüpfen, damit die Administratoren der Gruppen und deren Untergruppen diese Teams im Bereich Gruppen anzeigen und mit ihnen arbeiten können. Weitere Informationen finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) oder [Teameinstellungen bearbeiten](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Vorlage**: Sie können einer Projektvorlage eine Gruppe zuweisen. Auf diese Weise können Sie den Prozess der Projekterstellung optimieren und einfacher identifizieren, welche Gruppen welche Projektvorlagen besitzen, und Berichte dazu erstellen. Weitere Informationen finden Sie im Abschnitt [Übersicht](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) im Artikel [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Kürzlich gelöschte und wiederhergestellte Elemente**: Sie können die kürzlich gelöschten Gruppen anzeigen und verwalten. Weitere Informationen finden Sie unter [Anzeigen und Verwalten der kürzlich gelöschten Elemente einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) und [Anzeigen und Verwalten der kürzlich wiederhergestellten Elemente einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
