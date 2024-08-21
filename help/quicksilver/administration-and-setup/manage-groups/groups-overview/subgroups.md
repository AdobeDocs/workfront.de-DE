---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Untergruppen - Übersicht
description: Sie können bis zu 14 Ebenen von Untergruppen unter einer Gruppe erstellen. Auf jeder dieser Ebenen können Sie eine unbegrenzte Anzahl paralleler Untergruppen erstellen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Übersicht über Untergruppen

Sie können bis zu 14 Ebenen von Untergruppen unter einer Gruppe erstellen. Auf jeder dieser Ebenen können Sie eine unbegrenzte Anzahl paralleler Untergruppen erstellen. Anweisungen finden Sie unter [Erstellen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Weitere Informationen zu Gruppen finden Sie unter [Gruppenübersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Was erben Untergruppen?

Untergruppen erben die Mitgliedschaft ihrer übergeordneten Gruppe. Benutzer und Gruppen in einer Untergruppe haben also die gleiche Sichtbarkeit, Berechtigungen und Zugriff auf alle Objekte wie Benutzer und Gruppen, die zur übergeordneten Gruppe gehören, die sie gemeinsam nutzen.

Außerdem erbt eine Untergruppe automatisch die Gruppenadministratoren ihrer Gruppe auf oberster Ebene. Sie können jedoch auch Mitgliedern einer Untergruppe zuweisen, die als Gruppenadministratoren fungieren.

>[!TIP]
>
>Manchmal können Sie Untergruppen verwenden, um einer vorhandenen Gruppe mehrere Benutzer hinzuzufügen, um ihnen Zugriff auf ein benötigtes Objekt zu gewähren.
>
>Angenommen, Sie haben eine Gruppe von Helpdesk-Technikern und eine separate Gruppe von IT-Direktoren. Die Helpdesk-Gruppe hat Berechtigungen für eine bestimmte Anforderungswarteschlange. Sie möchten die IT-Direktoren zur Helpdesk-Gruppe hinzufügen, damit sie auch über Berechtigungen für die Anforderungswarteschlange verfügen. Ohne die Untergruppenfunktion müssten Sie die IT-Direktoren manuell zur Helpdesk-Gruppe hinzufügen, was ineffizient und schwer zu verwalten sein könnte. Wenn Sie die Gruppe IT-Direktoren zur Helpdesk-Gruppe als Untergruppe hinzufügen, können Sie diese Aufgabe mit nur einer Änderung schneller erledigen.

>[!NOTE]
>
>Wenn ein Benutzer sowohl zu einer Untergruppe als auch zu ihrer übergeordneten Gruppe getrennt hinzugefügt wurde, wird der Benutzer beim Entfernen des Benutzers von einer Untergruppe nicht von der anderen entfernt. Wenn Sie nicht möchten, dass der Benutzer Zugriff für die übergeordnete Gruppe erhält, müssen Sie den Benutzer sowohl aus der Untergruppe als auch aus der übergeordneten Gruppe entfernen.

## Öffentliche und private Untergruppen

Für eine öffentliche Gruppe kann jeder Benutzer (in oder außerhalb der Gruppe), der über Bearbeitungs-Benutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können dies nicht für eine private Gruppe tun.

Sie können diese Option nur auf der obersten übergeordneten Gruppe in einer Hierarchie von Gruppen mit mehr als einer Ebene bearbeiten. Alle Untergruppen der übergeordneten Gruppe übernehmen ihre Einstellung.

Wenn Sie eine Untergruppe unter einer öffentlichen Gruppe erstellen, ist die Untergruppe standardmäßig ebenfalls öffentlich. Weitere Informationen zum Erstellen einer Gruppe und zum Veröffentlichen finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Weitere Informationen zum Zugriff, der zum Bearbeiten von Benutzern erforderlich ist, finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Jede Gruppe, die Sie einer vorhandenen Gruppe hinzufügen, wird automatisch zu einer Untergruppe und ist nicht mehr eine Hauptgruppe. Die Untergruppe behält jedoch zusätzlich zu allen Projekt-, Aufgaben- und Problemstatus-Status, die zur neuen übergeordneten Gruppe gehören, ihre vorhandenen Benutzer sowie alle Verbindungen mit Projekten, Problemen und Aufgaben bei.

## Gruppenadministratoren für Untergruppen

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

Sie können der Untergruppe Mitglieder der Untergruppe als Gruppenadministratoren zuweisen, wenn Sie sie erstellen oder bearbeiten. Anweisungen finden Sie unter [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) im Artikel [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Alternativ können Sie die Verwaltung der Untergruppe den Gruppenadministratoren überlassen, die den oben genannten Gruppen zugewiesen sind. Wenn Sie eine Untergruppe erstellen, gruppieren Sie Administratoren über die oben stehenden Gruppen und haben automatisch Zugriff auf die Verwaltung der Untergruppe.

>[!NOTE]
>
>Wenn Sie einen Benutzer zu einer Untergruppe hinzufügen und dieser Benutzer ein Gruppenadministrator für eine Gruppe ist, die sich irgendwo oberhalb der Untergruppe befindet, hat dieser Benutzer Administratorrechte zur Verwaltung der Untergruppe, selbst wenn er nicht als Gruppenadministrator für diese Gruppe zugewiesen wurde.

Informationen dazu, welche Aktionen einem Adobe Workfront-Administrator, der das Workfront-System verwaltet, einem Gruppenadministrator, der eine Gruppe der obersten Ebene verwaltet, und einem Gruppenadministrator, der eine Untergruppe verwaltet, zur Verfügung stehen, finden Sie unter [Für unterschiedliche Administratortypen zulässige Aktionen](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
