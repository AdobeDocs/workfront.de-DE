---
title: Gruppenadministratoren
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Adobe Workfront-Administratoren in einem großen Unternehmen mit vielen Abteilungen möchten möglicherweise nicht alle Abteilungen und Gruppen innerhalb dieser Abteilungen verwalten. Stattdessen können sie für jede Abteilung und jede Untergruppe innerhalb dieser Gruppe eine Gruppe erstellen, die jeweils von einem Gruppenadministrator verwaltet werden.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 1%

---

# Gruppenadmins

<!-- Audited: 12/2023 -->

Adobe Workfront-Administratoren in einem großen Unternehmen mit vielen Abteilungen möchten möglicherweise nicht alle Abteilungen und Gruppen innerhalb dieser Abteilungen verwalten. Stattdessen können sie für jede Abteilung und jede Untergruppe innerhalb dieser Gruppe eine Gruppe erstellen, die jeweils von einem Gruppenadministrator verwaltet werden.

Ein Gruppenadministrator bzw. eine Gruppenadministratorin kann die Anforderungen einer Gruppe verwalten, z. B. Benutzermitgliedschaft, Layoutvorlagen, benutzerdefinierte Daten, Status und Voreinstellungen.

Es können bis zu 14 Untergruppenebenen in einer Gruppe vorhanden sein.

>[!NOTE]
>
>Alle Gruppenadministratoren in der Hierarchie über einer Untergruppe verfügen über Administratorrechte zum Verwalten dieser Untergruppe.

Informationen zum Erstellen und Verwalten von Gruppen finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) und [Verwalten einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Siehe auch [Untergruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Bestimmen von Gruppenadministratoren

Jede Gruppe der obersten Ebene muss mindestens einen Gruppenadministrator haben. Ein Workfront-Administrator oder Administrator einer Gruppe kann den Untergruppen der Gruppe Gruppenadministratoren zuweisen. Dies ist jedoch nicht erforderlich. Weitere Informationen finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Wenn Sie Workfront-Administrator sind, empfehlen wir, Folgendes zu tun, bevor Sie Benutzende als Gruppenadministratoren festlegen:

* Notieren Sie sich die aktuelle Anzahl von Workfront-Administratoren in Ihrem System.
* Notieren Sie sich die Anzahl der Gruppen, die Sie in Ihrem System haben.
* Ermitteln Sie, ob Sie die Zugriffsebene einiger Workfront-Administratoren ändern und sie stattdessen als Gruppenadministratoren festlegen können.

  Weitere Informationen zu den Funktionen von Gruppenadministratoren finden Sie unter [Aufgaben von &#x200B;](#tasks-done-by-group-administrators) in diesem Artikel.

* Legen Sie fest, ob Gruppenadministratoren in der Lage sein sollen, sich als andere Benutzer anzumelden, oder die Passwörter für Benutzer in den von Ihnen verwalteten Gruppen zurücksetzen können. Für diese Aufgaben ist zusätzlicher Zugriff erforderlich, wie unten unter [Zugriff für Gruppenadministratoren erforderlich](#access-needed-for-group-administrators) beschrieben.
* Für eine bessere Benutzerverwaltung sollten Sie ggf. Gruppen oder Untergruppen anstelle von Benutzern den folgenden Objekten zuweisen:

   * Layoutvorlagen
   * Zeitpläne
   * Arbeitszeittabellen-Profile

## Zugriff für Gruppenadministratoren erforderlich {#access-needed-for-group-administrators}

Jeder Gruppenadministrator muss über Folgendes verfügen

* Eine Planlizenz im aktuellen Preis- und Verpackungsmodell
* Eine Standardlizenz im neuen Preis- und Verpackungsmodell

Es wird empfohlen, dass Gruppenadministratoren Bearbeitungszugriff auf Benutzer haben, damit sie die folgenden Aufgaben ausführen können:

* Melden Sie sich als andere Benutzer in den von ihnen verwalteten Gruppen und Untergruppen an.
* Setzt das Kennwort eines anderen Benutzers in den von ihm verwalteten Gruppen zurück.

>[!IMPORTANT]
>
>Gruppenadministratoren müssen höhere Zugriffsrechte als die von ihnen verwalteten haben. Andernfalls können sie niedrigere Zugriffsebenen nicht anzeigen oder ändern.
>&#x200B;>Anweisungen zum Gewähren dieses Zugriffs finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Für einen Gruppenadministrator, der Benutzern in ihren Gruppen und Untergruppen Arbeitszeittabellen-Profile zuweisen muss, empfehlen wir außerdem den administrativen Zugriff auf Arbeitszeittabellen und Stunden. Anweisungen zum Gewähren dieses Zugriffs finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Aufgaben von Gruppenadministratoren {#tasks-done-by-group-administrators}

Als Gruppenadministrator können Sie die unten beschriebenen Aufgaben ausführen, um die von Ihnen überwachten Gruppen zu verwalten. Einige dieser Funktionen entsprechen den Funktionen, die ein Workfront-Administrator bietet.

>[!NOTE]
>
>Im neuen Preis- und Verpackungsmodell benötigen Sie einen Prime-Plan oder höher, um Folgendes durchzuführen:
>
> * Erstellen von Gruppenereignis-Benachrichtigungen
> * Gruppenprojekteinstellungen konfigurieren
> * Voreinstellungen für Gruppenaufgaben und -Anfragen konfigurieren
> * Konfiguration von Untergruppeneinstellungen entsperren
> * Arbeitszeittabelle und Stundeneinstellungen gruppieren
> * Arbeitszeittabelle und Stundeneinstellungen entsperren

### Gruppenmitglieder verwalten {#manage-group-members}

* Erstellen, Bearbeiten und Löschen von Untergruppen innerhalb der von Ihnen verwalteten Gruppen und Untergruppen. Anweisungen finden Sie unter [Erstellen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Fügen Sie alle Benutzer, für die Sie Bearbeitungszugriff haben, zu Ihren Gruppen und Untergruppen hinzu. Oder fügen Sie Benutzer zu Gruppen und Untergruppen hinzu, indem Sie deren Profile bearbeiten.

  Sie können die Felder im Profil eines Gruppenmitglieds auch aktualisieren, wenn in Ihrer Zugriffsebene die Berechtigung Benutzeradmin (Gruppenbenutzer) aktiviert ist.

  Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Workfront-Administratoren können Änderungen an Gruppenmitgliedschaften überschreiben, die von einem Gruppenadministrator vorgenommen wurden.

* Setzen Sie Kennwörter für Benutzer zurück, die Mitglieder der von Ihnen verwalteten Gruppen sind. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Melden Sie sich als Benutzer an, die Mitglieder der von Ihnen verwalteten Gruppen sind. Weitere Informationen finden Sie unter [Als anderer Benutzer anmelden](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Anzeigen der Anzahl der für Ihre Gruppe verfügbaren Lizenzen und der darunter liegenden Untergruppen Weitere Informationen finden Sie unter [Verfügbare Lizenzen in Ihrem System verwalten](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Gruppenobjekte verwalten {#manage-group-objects}

* Erstellen Sie Layoutvorlagen auf Gruppenebene und verknüpfen Sie sie mit den von Ihnen verwalteten Gruppen und Untergruppen. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Erstellen Sie Arbeitszeittabellen-Profile auf Gruppenebene, verknüpfen Sie sie mit von Ihnen verwalteten Benutzern und Gruppen und generieren Sie Arbeitszeittabellen manuell. Weitere Informationen finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Erstellen und bearbeiten Sie Genehmigungsprozesse für die von Ihnen verwalteten Gruppen und Untergruppen ohne administrativen Zugriff auf Genehmigungsprozesse. Weitere Informationen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Informationen zum administrativen Zugriff auf Genehmigungsprozesse finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Erstellen Sie Zeitpläne und verknüpfen Sie sie mit einer von Ihnen verwalteten Gruppe. Weitere Informationen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Verwalten Sie ein Team, das einer von Ihnen verwalteten Gruppe zugewiesen ist, ohne Mitglied des Teams zu sein. Erstellen Sie außerdem einen auf dem Feld Gruppe basierenden Team-Bericht, um zu bestimmen, welcher Gruppe ein bestimmtes Team zugewiesen ist. Weitere Informationen finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Stellen Sie ein Projekt wieder her, das einer von Ihnen verwalteten Gruppe zugeordnet ist, sowie alle Aufgaben, Probleme oder Dokumente, die mit dem Projekt verknüpft sind. Weitere Informationen finden Sie unter [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Gruppenvoreinstellungen und Tools verwalten {#manage-group-preferences-and-tools}

* Wenn die Voreinstellung für ein Projekt, eine Aufgabe oder ein Problem oder die Voreinstellung für Arbeitszeittabellen und Stunden für Gruppen im gesamten System entsperrt ist, bearbeiten Sie diese Voreinstellung für von Ihnen verwaltete Gruppen. Diese Voreinstellungen wirken sich auf das Verhalten von Projekten, Aufgaben und Problemen aus. Weitere Informationen finden Sie hier:

   * [Projektvoreinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Konfigurieren der Voreinstellungen für Aufgaben und Probleme für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Gruppenstatus für von Ihnen verwaltete Gruppen erstellen und bearbeiten. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Konfigurieren Sie eine Ereignisbenachrichtigung für von Ihnen verwaltete Gruppen. Dies ist nur möglich, wenn ein Workfront-Administrator die Möglichkeit zur systemweiten Konfiguration von Ereignisbenachrichtigungen für Gruppen freigeschaltet hat. Weitere Informationen finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
