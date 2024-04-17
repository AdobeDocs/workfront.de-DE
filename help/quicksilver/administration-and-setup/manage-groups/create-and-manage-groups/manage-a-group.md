---
user-type: administrator
product-area: system-administration;user-management
keywords: manage,group,edit,
navigation-topic: create-and-manage-groups
title: Verwalten einer Gruppe
description: Als Gruppenadministrator können Sie eine Gruppe, die Sie verwalten, im Bereich Gruppen unter Einrichtung verwalten. Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 0afd578ebaa55d911c04a1d08fbcadddc1d05bbc
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 0%

---

# Verwalten einer Gruppe

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

Als Gruppenadministrator können Sie eine Gruppe, die Sie verwalten, im Bereich Gruppen unter Einrichtung verwalten. Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>Wenn Sie als Administrator für eine Gruppe zugewiesen sind, erben Sie die Rolle des Gruppenadministrators für alle Untergruppen, die darunter liegen. Die einzigen Benutzer, die eine Untergruppe verwalten können, sind die Gruppenadministratoren für die oberste Gruppe darüber sowie alle Gruppenadministratoren, die der Untergruppe zugewiesen sind.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Gruppenmitgliedschaften verwalten

Sie können Benutzer und andere Gruppen zu einer von Ihnen verwalteten Gruppe hinzufügen und daraus entfernen. Sie können Gruppenmitglieder auch als Administratoren für die Gruppe zuweisen und die Benutzerprofilinformationen der Gruppenmitglieder verwalten.

Anweisungen finden Sie unter [Gruppenmitgliedschaften anzeigen und verwalten](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Details einer Gruppe verwalten

Sie können die Seite Gruppendetails für eine von Ihnen verwaltete Gruppe oder Untergruppe anzeigen und bearbeiten. Diese Seite enthält eine Beschreibung der Gruppe, die Namen des Business Leaders und der Gruppenadministratoren sowie eine Option, mit der Sie die Gruppe und alle zugehörigen Untergruppen öffentlich oder privat machen können. Wenn Sie auf Ihre Zugriffsebene benutzerdefinierte Formulare verwalten können, können Sie ein benutzerdefiniertes Formular an eine Gruppe anhängen.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Anweisungen finden Sie unter [Details einer Gruppe anzeigen und verwalten](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Bearbeiten, Kopieren oder Löschen einer Gruppe

Ohne die Hauptseite einer Gruppe zu verlassen, die Sie anzeigen, können Sie die Gruppe schnell bearbeiten, kopieren oder löschen.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **Gruppen**.

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Wählen Sie die Gruppe aus und klicken Sie auf Bearbeiten . ![](assets/edit-icon.png), Kopie ![](assets/copy-icon.png)oder Löschen ![](assets/delete.png) Symbol.

   Wenn Sie Informationen zur Verwendung des angezeigten Felds benötigen, sehen Sie sich eine der folgenden Möglichkeiten an:

   * **Bearbeiten**: [Details einer Gruppe anzeigen und verwalten](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Kopieren**: [Erstellen einer Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) im Artikel [Gruppe erstellen](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Löschen**: [Gruppe löschen](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Konfigurieren von Projekt-, Aufgaben- und Problemeinstellungen für eine Gruppe

Wenn Sie Gruppenadministrator sind und Ihre Gruppe andere Einstellungen für Projekt, Aufgabe und Ausgabe als auf Systemebene festgelegt benötigen, können Sie den Workfront-Administrator bitten, eine Voreinstellung für alle Gruppen in der Organisation zu entsperren. Nachdem die Sperre aufgehoben wurde, können Sie sie (und Gruppenadministratoren für alle anderen Gruppen) für die von Ihnen verwalteten Gruppen konfigurieren.

Anweisungen finden Sie unter [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und  [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Untergruppen auflisten, hinzufügen und konfigurieren

Unter einer von Ihnen verwalteten Gruppe können Sie Untergruppen erstellen, anzeigen, bearbeiten, kopieren, umbenennen, exportieren und löschen.

## Ereignisbenachrichtigungen für eine Gruppe konfigurieren

Wenn ein Workfront-Administrator die Möglichkeit freischaltet, Ereignisbenachrichtigungen für die Gruppen in Ihrem Unternehmen zu konfigurieren, können Sie sie für eine von Ihnen verwaltete Gruppe konfigurieren. Anweisungen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Erstellen und Anpassen von Status für eine Gruppe

Als Gruppenadministrator können Sie benutzerdefinierte Status für eine von Ihnen verwaltete Gruppe der obersten Ebene erstellen. Dies gibt Ihrer Gruppe Autonomie und hilft, Dutzende unternehmensweiter benutzerdefinierter Status zu eliminieren. (Ein Workfront-Administrator kann dies auch für jede Gruppe tun.)

Sie können auch den Systemstatus für eine Gruppe der obersten Ebene anpassen, wenn ein Workfront-Administrator sie so konfiguriert hat, dass sie angepasst werden können.

Anweisungen finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Arbeiten mit Projekten einer Gruppe

Wenn Sie im Bereich Gruppen unter Einrichtung die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen, können Sie mit Projekten Folgendes tun:

* Auflisten und Bearbeiten (Bearbeiten, Kopieren, Löschen und Exportieren) der Projekte, die mit der Gruppe und ihren Untergruppen verknüpft sind und für Sie freigegeben wurden
* Neues Projekt für die Gruppe erstellen

Anweisungen finden Sie unter [Erstellen und Ändern von Gruppenprojekten](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Validierungsprozesse einer Gruppe anzeigen und verwalten

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die Genehmigungsprozesse anzeigen und bearbeiten, auf die die Administratoren der Gruppe oder einer ihrer Untergruppen Administratorzugriff haben.

Anweisungen finden Sie unter [Validierungsprozesse auf Gruppenebene](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Layout-Vorlagen einer Gruppe anzeigen und verwalten

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich &quot;Gruppen&quot;verwalten, können Sie die Layout-Vorlage anzeigen und verwenden, auf die die Administratoren der Gruppe oder einer ihrer Untergruppen administrativen Zugriff haben.

Anweisungen finden Sie unter [Erstellen und Ändern von Gruppenlayoutvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Zeitpläne von Gruppenmitgliedern anzeigen und verwalten

Ein Gruppenadministrator, der einen Zeitplan für eine Gruppe erstellt, muss die Gruppe angeben, deren Administratoren den Zeitplan verwalten. Normalerweise handelt es sich hierbei um die Gruppe, für die der Zeitplan erstellt wird. Es kann sich jedoch um eine andere Gruppe handeln, wenn der Gruppenadministrator mehrere Gruppen verwaltet und stattdessen eine der anderen angibt.

Wenn Sie die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen und die Gruppe als Gruppe bestimmt ist, deren Administratoren einen Zeitplan bearbeiten können, können Sie den Zeitplan auf der Seite der Gruppe anzeigen und verwalten.

Anweisungen finden Sie unter [Erstellen und Ändern der Zeitpläne einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Anzeigen und Verwalten von Profilen der Gruppenmitglieder

Wenn Sie sich die Hauptseite einer von Ihnen verwalteten Gruppe ansehen, können Sie die Timesheet-Profile verwalten, für die Sie und die anderen Administratoren der Gruppe - oder einer ihrer Untergruppen - über die Berechtigung zum Bearbeiten verfügen. Anweisungen finden Sie unter [Erstellen und Verwalten von Timesheet-Profilen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Mitglieder einer Gruppe anzeigen und verwalten

Wenn Sie die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen, können Sie alle Benutzer in den Untergruppen der Gruppe anzeigen und verwalten. Anweisungen finden Sie unter [Anzeigen und Verwalten von Untergruppenmitgliedern](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Anzeigen und Verwalten von Teams einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie Teams anzeigen und mit dieser Gruppe oder einer ihrer Untergruppen zusammenarbeiten.

Anweisungen finden Sie unter [Erstellen und Ändern von Teams einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Anzeigen und Verwalten von Unternehmen einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit der Gruppe oder einer ihrer Untergruppen verbundene Unternehmen anzeigen und zusammenarbeiten. Anweisungen finden Sie unter [Erstellen und Ändern von Unternehmen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Anzeigen und Verwalten der Portfolios und Programme einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich &quot;Gruppen&quot;verwalten, können Sie Portfolios und Programme anzeigen und bearbeiten, wenn beide der folgenden Punkte zutreffen:

* Sie sind mit der angezeigten Gruppe oder einer ihrer Untergruppen verknüpft.
* Sie sind berechtigt, sie anzuzeigen, weil Sie sie erstellt oder für Sie freigegeben haben

Anweisungen finden Sie unter [Erstellen und Ändern von Gruppenprojekten](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) und [Erstellen, Ändern und Anzeigen von Programmen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Gruppe deaktivieren oder reaktivieren

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Sie können eine Gruppe in ihrem standardmäßigen aktiven Status belassen oder deaktivieren.

Die Deaktivierung einer Gruppe kann nützlich sein, wenn sie derzeit nicht verwendet wird, da Benutzer sie nicht mehr in Typ-Ahead-Feldern sehen, wenn sie nach einer Gruppe suchen, die sie mit einem anderen Objekt verknüpfen möchten.

Anweisungen zum Aktivieren oder Aktivieren einer Gruppe finden Sie unter [Gruppe deaktivieren oder reaktivieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
