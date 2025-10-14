---
user-type: administrator
product-area: system-administration;user-management
keywords: verwalten,gruppieren,bearbeiten,
navigation-topic: create-and-manage-groups
title: Verwalten einer Gruppe
description: Als Gruppenadministrator können Sie eine Gruppe, die Sie verwalten, über den Bereich Gruppen im Setup verwalten. Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 0%

---

# Verwalten einer Gruppe

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

Als Gruppenadministrator können Sie eine Gruppe, die Sie verwalten, über den Bereich Gruppen im Setup verwalten. Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>Wenn Sie als Administrator für eine Gruppe zugewiesen werden, übernehmen Sie die Rolle des Gruppenadministrators für alle Untergruppen, die sich unter dieser Gruppe befinden. Die einzigen Benutzer, die eine Untergruppe verwalten können, sind die Gruppenadministratoren für die oberste Gruppe darüber und alle Gruppenadministratoren, die der Untergruppe zugewiesen sind.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verwalten von Gruppenmitgliedschaften

Sie können Benutzer und andere Gruppen zu einer Gruppe, die Sie verwalten, hinzufügen und daraus entfernen. Sie können Gruppenmitglieder auch als Administratoren für die Gruppe zuweisen und die Benutzerprofilinformationen von Gruppenmitgliedern verwalten.

Anweisungen finden Sie [Anzeigen und Verwalten der Gruppenmitgliedschaften](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Verwalten der Details einer Gruppe

Sie können die Seite „Gruppendetails“ für eine von Ihnen verwaltete Gruppe oder Untergruppe anzeigen und bearbeiten. Diese Seite enthält eine Beschreibung der Gruppe, die Namen des Business Leaders und der Gruppenadministratoren sowie eine Option, mit der Sie die Gruppe und alle ihre Untergruppen öffentlich oder privat machen können. Und wenn Sie mit Ihrer Zugriffsebene benutzerdefinierte Formulare verwalten können, können Sie ein benutzerdefiniertes Formular an eine Gruppe anhängen.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Anweisungen finden Sie [Anzeigen und Verwalten der Details einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Bearbeiten, Kopieren oder Löschen einer Gruppe

Sie können die Gruppe schnell bearbeiten, kopieren oder löschen, ohne die Hauptseite einer Gruppe zu verlassen, die Sie gerade anzeigen.

{{step-1-to-setup}}

1. Klicken Sie **Gruppen**.

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Wählen Sie die Gruppe aus und klicken Sie dann auf das Symbol ![Bearbeiten](assets/edit-icon.png), das Symbol ![Kopieren](assets/copy-icon.png) oder das Symbol ![Löschen](assets/delete.png).

   Wenn Sie Informationen zur Verwendung des angezeigten Felds benötigen, sehen Sie sich eine der folgenden Vorgehensweisen an:

   * **Bearbeiten**: [Anzeigen und Verwalten der Details einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Kopieren**: [Erstellen einer Gruppe auf oberster Ebene durch Kopieren einer vorhandenen Gruppe oder &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) im Artikel [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Löschen**: [Löschen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Konfigurieren von Projekt-, Aufgaben- und Problem-Voreinstellungen für eine Gruppe

Wenn Sie Gruppenadministrator sind und Ihre Gruppe andere Einstellungen für Projekte, Aufgaben und Probleme benötigt als die auf Systemebene festgelegten, können Sie den Workfront-Administrator bitten, eine Voreinstellung für alle Gruppen im Unternehmen zu entsperren. Nachdem er entsperrt wurde, können Sie (und Gruppenadministratoren für alle anderen Gruppen) ihn für die von Ihnen verwalteten Gruppen konfigurieren.

Anweisungen finden Sie unter [Projektvoreinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Aufgaben- und Problemvoreinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Auflisten, Hinzufügen und Konfigurieren von Untergruppen

Unter einer von Ihnen verwalteten Gruppe können Sie Untergruppen erstellen, anzeigen, bearbeiten, kopieren, umbenennen, exportieren und löschen.

## Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe

Wenn ein Workfront-Administrator die Möglichkeit zur Konfiguration von Ereignisbenachrichtigungen für die Gruppen in Ihrem Unternehmen freigibt, können Sie diese für eine von Ihnen verwaltete Gruppe konfigurieren. Anweisungen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Erstellen und Anpassen von Status für eine Gruppe

Als Gruppenadministrator können Sie benutzerdefinierte Status für eine von Ihnen verwaltete Gruppe auf oberster Ebene erstellen. Dies verleiht Ihrer Gruppe Autonomie und trägt dazu bei, die Notwendigkeit für Dutzende von unternehmensweiten benutzerdefinierten Status zu beseitigen. (Ein Workfront-Administrator kann dies auch für jede Gruppe tun.)

Sie können auch den Systemstatus für eine Gruppe auf oberster Ebene anpassen, wenn ein Workfront-Administrator sie so konfiguriert hat, dass sie eine Anpassung ermöglicht.

Anweisungen finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Arbeiten mit Projekten einer Gruppe

Wenn Sie im Bereich Gruppen unter Setup die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen, können Sie mit Projekten die folgenden Aktionen durchführen:

* Auflisten und Bearbeiten (Bearbeiten, Kopieren, Löschen und Exportieren) der Projekte, die mit der Gruppe und ihren Untergruppen verknüpft sind und für Sie freigegeben wurden
* Erstellen eines neuen Projekts für die Gruppe

Anweisungen finden Sie [Erstellen und Ändern der Projekte einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Genehmigungsprozesse einer Gruppe anzeigen und verwalten

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die Genehmigungsprozesse anzeigen und damit arbeiten, für die die Administratoren der Gruppe oder einer ihrer Untergruppen administrativen Zugriff haben.

Anweisungen finden Sie [Genehmigungsprozesse auf Gruppenebene](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Layoutvorlagen einer Gruppe anzeigen und verwalten

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die Layout-Vorlage anzeigen und mit ihr arbeiten, für die die Administratoren der Gruppe oder eine ihrer Untergruppen administrativen Zugriff haben.

Anweisungen finden Sie unter [Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Anzeigen und Verwalten der Zeitpläne von Gruppenmitgliedern

Ein Gruppenadministrator, der einen Zeitplan für eine Gruppe erstellt, muss die Gruppe angeben, deren Administratoren den Zeitplan verwalten sollen. Normalerweise ist dies die Gruppe, für die der Zeitplan erstellt wird. Es kann sich jedoch auch um eine andere Gruppe handeln, wenn der Gruppenadministrator mehrere Gruppen verwaltet und stattdessen eine der anderen angibt.

Wenn Sie die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen und die Gruppe als diejenige definiert ist, deren Administratoren einen Zeitplan bearbeiten können, können Sie den Zeitplan auf der Seite der Gruppe anzeigen und verwalten.

Anweisungen finden Sie [Erstellen und Ändern der Zeitpläne einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Anzeigen und Verwalten der Arbeitszeittabellen-Profile von Gruppenmitgliedern

Wenn Sie die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen, können Sie die Arbeitszeittabellen-Profile verwalten, zu deren Bearbeitung Sie und die anderen Administratoren der Gruppe - oder einer ihrer Untergruppen - berechtigt sind. Anweisungen finden Sie [Erstellen und Verwalten der Arbeitszeittabellen-Profile einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Anzeigen und Verwalten der Untergruppenmitglieder einer Gruppe

Wenn Sie die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen, können Sie alle Benutzenden in den Untergruppen der Gruppe anzeigen und verwalten. Anweisungen finden Sie unter [Anzeigen und Verwalten von Untergruppenmitgliedern](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Anzeigen und Verwalten der Teams einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit Teams arbeiten, die der Gruppe oder einer ihrer Untergruppen zugeordnet sind.

Anweisungen finden Sie [Erstellen und Ändern der Teams einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Anzeigen und Verwalten der Unternehmen einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit Unternehmen arbeiten, die mit der Gruppe oder einer ihrer Untergruppen verknüpft sind. Anweisungen finden Sie [Erstellen und Ändern der Unternehmen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Portfolios und Programme einer Gruppe anzeigen und verwalten

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie Portfolios und Programme anzeigen und mit ihnen arbeiten, wenn die beiden folgenden Bedingungen erfüllt sind:

* Sie sind mit der angezeigten Gruppe oder einer ihrer Untergruppen verknüpft
* Sie sind berechtigt, sie anzuzeigen, weil Sie sie erstellt haben oder sie für Sie freigegeben wurden

Anweisungen finden Sie unter [Erstellen und Ändern der Projekte einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) und [Erstellen, Ändern und Anzeigen der Programme einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Deaktivieren oder Reaktivieren einer Gruppe

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Sie können eine Gruppe in ihrem standardmäßigen aktiven Status belassen oder deaktivieren.

Das Deaktivieren einer Gruppe kann nützlich sein, wenn sie derzeit nicht verwendet wird, da sie in Feldern mit automatischer Textvervollständigung nicht mehr angezeigt wird, wenn nach einer Gruppe gesucht wird, die mit einem anderen Objekt verknüpft werden soll.

Anweisungen, wie Sie eine Gruppe inaktiv oder aktiv machen, finden Sie unter [Deaktivieren oder Reaktivieren einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
