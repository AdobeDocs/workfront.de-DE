---
title: Gruppenadministratoren
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Adobe Workfront-Administratoren in einer großen Organisation mit vielen Abteilungen möchten möglicherweise nicht alle Abteilungen und Gruppen der Organisation innerhalb dieser Abteilungen verwalten. Stattdessen können sie eine Gruppe für jede Abteilung und Untergruppen innerhalb dieser Gruppe erstellen, die jeweils von einem Gruppenadministrator verwaltet werden.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 850e0801511177efc5189258acd9b88234cf59c9
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# Gruppenadministratoren

<!-- Audited: 12/2023 -->

Adobe Workfront-Administratoren in einer großen Organisation mit vielen Abteilungen möchten möglicherweise nicht alle Abteilungen und Gruppen der Organisation innerhalb dieser Abteilungen verwalten. Stattdessen können sie eine Gruppe für jede Abteilung und Untergruppen innerhalb dieser Gruppe erstellen, die jeweils von einem Gruppenadministrator verwaltet werden.

Ein Gruppenadministrator kann die Anforderungen einer Gruppe verwalten, z. B. die Mitgliedschaft im Benutzer, Layoutvorlagen, benutzerdefinierte Daten, Status und Voreinstellungen.

Unter einer Gruppe können bis zu 14 Ebenen von Untergruppen existieren.

>[!NOTE]
>
>Alle Gruppenadministratoren in der Hierarchie über einer Untergruppe verfügen über Administratorrechte für die Verwaltung dieser Untergruppe.

Informationen zum Erstellen und Verwalten von Gruppen finden Sie unter [Gruppe erstellen](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) und [Verwalten einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Siehe auch [Übersicht über Untergruppen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Gruppenadministratoren bestimmen

Jede Gruppe der obersten Ebene muss über mindestens einen Gruppenadministrator verfügen. Ein Workfront-Administrator oder -Administrator einer Gruppe kann den Untergruppen der Gruppe Gruppenadministratoren zuweisen, dies ist jedoch nicht erforderlich. Weitere Informationen finden Sie unter [Gruppe erstellen](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Wenn Sie Workfront-Administrator sind, sollten Sie Folgendes tun, bevor Sie Benutzer als Gruppenadministratoren festlegen:

* Notieren Sie sich die aktuelle Anzahl von Workfront-Administratoren in Ihrem System.
* Notieren Sie sich die Anzahl der Gruppen, die Sie in Ihrem System haben.
* Bestimmen Sie, ob Sie die Zugriffsebene einiger Workfront-Administratoren ändern und diese stattdessen als Gruppenadministratoren festlegen können.

  Weitere Informationen zu den Funktionen von Gruppenadministratoren finden Sie unter [Aufgaben, die von Gruppenadministratoren ausgeführt werden](#tasks-done-by-group-administrators) in diesem Artikel.

* Bestimmen Sie, ob Gruppenadministratoren sich als andere Benutzer anmelden können sollen oder ob sie die Passwörter für Benutzer in den von Ihnen verwalteten Gruppen zurücksetzen möchten. Zur Durchführung dieser Aufgaben ist zusätzlicher Zugriff erforderlich, wie unten beschrieben unter [Für Gruppenadministratoren benötigter Zugriff](#access-needed-for-group-administrators).
* Für eine bessere Benutzerverwaltung sollten Sie die folgenden Objekte mit Gruppen oder Untergruppen anstelle von Benutzern verknüpfen:

   * Layoutvorlagen
   * Zeitpläne
   * Arbeitszeittabellen-Profile

## Für Gruppenadministratoren benötigter Zugriff {#access-needed-for-group-administrators}

Jeder Gruppenadministrator muss

* Eine Planungslizenz im aktuellen Preis- und Verpackungsmodell
* Eine Standardlizenz im neuen Preis- und Verpackungsmodell

Es wird empfohlen, dass Gruppenadministratoren Zugriff auf die Option Bearbeiten haben, damit sie die folgenden Aufgaben ausführen können:

* Melden Sie sich als andere Benutzer in den von ihnen verwalteten Gruppen und Untergruppen an.
* Setzen Sie das Kennwort eines anderen Benutzers in den von ihm verwalteten Gruppen zurück.

>[!IMPORTANT]
>
>Gruppenadministratoren müssen einen höheren Zugriff haben als sie verwalten. Andernfalls können sie niedrigere Zugriffsebenen nicht anzeigen oder ändern.
>Anweisungen zur Gewährung dieses Zugriffs finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Für einen Gruppenadministrator, der Benutzern in Gruppen und Untergruppen Zeitleistenprofile zuweisen muss, empfehlen wir außerdem Administratorzugriff auf Zeitpläne und Stunden. Anweisungen zur Gewährung dieses Zugriffs finden Sie unter [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Aufgaben, die von Gruppenadministratoren ausgeführt werden {#tasks-done-by-group-administrators}

Als Gruppenadministrator können Sie die unten beschriebenen Aufgaben ausführen, um die von Ihnen überwachten Gruppen zu verwalten. Einige davon entsprechen den Fähigkeiten, die einem Workfront-Administrator geboten werden.

>[!NOTE]
>
>Im neuen Preis- und Verpackungsmodell müssen Sie über einen Prime-Plan oder höher verfügen, um Folgendes durchführen zu können:
>
> * Gruppenereignisbenachrichtigungen erstellen
> * Gruppenprojektvoreinstellungen konfigurieren
> * Konfigurieren von Gruppenaufgaben- und Problemeinstellungen
> * Konfiguration der Untergruppenvoreinstellungen entsperren
> * Voreinstellungen für Gruppenzeitpläne und -zeiten
> * Zeitblatt und Stunde entsperren

### Gruppenmitglieder verwalten {#manage-group-members}

* Erstellen, bearbeiten und löschen Sie Untergruppen innerhalb der von Ihnen verwalteten Gruppen und Untergruppen. Anweisungen finden Sie unter [Erstellen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Fügen Sie alle Benutzer, für die Sie Zugriff auf die Bearbeitung haben, zu Ihren Gruppen und Untergruppen hinzu. Oder fügen Sie Benutzer Gruppen und Untergruppen hinzu, indem Sie ihre Profile bearbeiten.

  Sie können die Felder im Profil eines Gruppenmitglieds auch aktualisieren, wenn Sie die Berechtigung Benutzeradministrator (Gruppenbenutzer) in Ihrer Zugriffsebene aktiviert haben.

  Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Workfront-Administratoren können Änderungen an Gruppenmitgliedschaften überschreiben, die von einem Gruppenadministrator vorgenommen wurden.

* Setzen Sie Kennwörter für Benutzer zurück, die Mitglieder der von Ihnen verwalteten Gruppen sind. Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Melden Sie sich als Benutzer an, die Mitglieder der von Ihnen verwalteten Gruppen sind. Weitere Informationen finden Sie unter [Melden Sie sich als anderer Benutzer an](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Zeigen Sie die Anzahl der verfügbaren Lizenzen für Ihre Gruppe und die Untergruppen darunter an. Weitere Informationen finden Sie unter [Verwalten der verfügbaren Lizenzen in Ihrem System](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Verwalten von Gruppenobjekten {#manage-group-objects}

* Erstellen Sie Layoutvorlagen auf Gruppenebene und verknüpfen Sie sie mit den von Ihnen verwalteten Gruppen und Untergruppen. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Erstellen Sie auf Gruppenebene erstellte Zeitleistenprofile, verknüpfen Sie sie mit Benutzern und Gruppen, die Sie verwalten, und generieren Sie manuell Timesheets. Weitere Informationen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Timesheet-Profilen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Erstellen und bearbeiten Sie ohne Administratorzugriff auf die Validierungsprozesse Validierungsprozesse für die von Ihnen verwalteten Gruppen und Untergruppen. Weitere Informationen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Informationen zum administrativen Zugriff auf Genehmigungsprozesse finden Sie unter [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Erstellen Sie Zeitpläne und verknüpfen Sie sie mit einer von Ihnen verwalteten Gruppe. Weitere Informationen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Verwalten Sie ein Team, das einer von Ihnen verwalteten Gruppe zugewiesen ist, ohne Mitglied des Teams zu sein. Erstellen Sie außerdem einen Teambericht basierend auf dem Feld Gruppe , um zu ermitteln, welcher Gruppe ein bestimmtes Team zugewiesen ist. Weitere Informationen finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Stellen Sie ein Projekt, das mit einer von Ihnen verwalteten Gruppe verknüpft ist, zusammen mit allen Aufgaben, Problemen oder Dokumenten, die mit dem Projekt verknüpft sind, wieder her. Weitere Informationen finden Sie unter [Gelöschte Elemente wiederherstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Verwalten von Gruppenvoreinstellungen und Tools {#manage-group-preferences-and-tools}

* Wenn eine Voreinstellung für ein Projekt, eine Aufgabe oder ein Problem oder eine Voreinstellung für Timesheets und Stunden für Gruppen im gesamten System entsperrt wird, bearbeiten Sie diese Voreinstellung für die von Ihnen verwalteten Gruppen. Diese Voreinstellungen wirken sich auf Projekt-, Aufgaben- und Problemverhalten aus. Weitere Informationen finden Sie unter folgenden Themen:

   * [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Erstellen und bearbeiten Sie Gruppenstatus für von Ihnen verwaltete Gruppen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Konfigurieren Sie eine Ereignisbenachrichtigung für von Ihnen verwaltete Gruppen. Dies ist erst möglich, wenn ein Workfront-Administrator die Möglichkeit freischaltet, Ereignisbenachrichtigungen für Gruppen im gesamten System zu konfigurieren. Weitere Informationen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
