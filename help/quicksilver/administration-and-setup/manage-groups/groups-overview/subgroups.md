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

# Untergruppen - Übersicht

Sie können bis zu 14 Ebenen von Untergruppen unter einer Gruppe erstellen. Auf jeder dieser Ebenen können Sie eine unbegrenzte Anzahl paralleler Untergruppen erstellen. Anweisungen finden Sie unter [Erstellen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

Informationen zu Gruppen finden Sie unter [Gruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Was erben Untergruppen?

Untergruppen übernehmen die Mitgliedschaft ihrer übergeordneten Gruppe. Benutzer und Gruppen in einer Untergruppe haben also dieselbe Sichtbarkeit, dieselben Berechtigungen und denselben Zugriff auf alle Objekte wie Benutzer und Gruppen, die der übergeordneten Gruppe angehören, die sie gemeinsam nutzen.

Außerdem erbt eine Untergruppe automatisch die Gruppenadministratoren ihrer Gruppe auf oberster Ebene. Sie können einer Untergruppe jedoch auch Mitglieder zuweisen, die als Gruppenadministratoren agieren.

>[!TIP]
>
>Manchmal empfiehlt es sich, mithilfe von Untergruppen mehrere Benutzer zu einer vorhandenen Gruppe hinzuzufügen, um ihnen Zugriff auf ein benötigtes Objekt zu gewähren.
>
>Angenommen, Sie verfügen über eine Gruppe von Helpdesk-Technikern und eine separate Gruppe von IT-Leitern. Die Helpdesk-Gruppe hat Berechtigungen für eine bestimmte Anfrage-Warteschlange. Sie möchten die IT-Direktoren der Helpdesk-Gruppe hinzufügen, damit sie auch über Berechtigungen für die Anfrage-Warteschlange verfügen. Ohne die Untergruppenfunktion müssten Sie die IT-Direktoren der Helpdesk-Gruppe manuell hinzufügen, was ineffizient und schwer zu verwalten sein könnte. Wenn Sie die Gruppe der IT-Direktoren der Helpdesk-Gruppe als Untergruppe hinzufügen, erreichen Sie diese Aufgabe mit nur einer Änderung schneller.

>[!NOTE]
>
>Wenn ein(e) Benutzende(r) sowohl einer Untergruppe als auch der übergeordneten Gruppe separat hinzugefügt wurde, wird beim Entfernen des/r Benutzenden aus einer Gruppe der/die Benutzende nicht aus der anderen entfernt. Wenn Sie nicht möchten, dass der Benutzer Zugriff auf die übergeordnete Gruppe hat, müssen Sie den Benutzer sowohl aus der Untergruppe als auch aus der übergeordneten Gruppe entfernen.

## Öffentliche und private Untergruppen

Für eine öffentliche Gruppe kann jeder Benutzer (innerhalb oder außerhalb der Gruppe), der über Bearbeitungsbenutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können das nicht für eine private Gruppe tun.

Sie können diese Option nur für die oberste übergeordnete Gruppe in einer Gruppenhierarchie bearbeiten, die mehr als eine Ebene hat. Alle Untergruppen der übergeordneten Gruppe übernehmen diese Einstellung.

Wenn Sie eine Untergruppe unter einer Gruppe erstellen, die öffentlich ist, ist die Untergruppe standardmäßig auch öffentlich. Weitere Informationen zum Erstellen und Veröffentlichen einer Gruppe finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). Weitere Informationen zum Zugriff, der zum Bearbeiten von Benutzern benötigt wird, finden Sie unter [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Jede Gruppe, die Sie einer vorhandenen Gruppe hinzufügen, wird automatisch zu einer Untergruppe und ist keine Hauptgruppe mehr. Die Untergruppe behält jedoch zusätzlich zu allen Projekt-, Aufgaben- und Problemstatus, die der neuen übergeordneten Gruppe angehören, ihre vorhandenen Benutzer sowie alle Verknüpfungen mit Projekten, Problemen und Aufgaben bei.

## Gruppenadministratoren für Untergruppen

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

Sie können der Untergruppe beim Erstellen oder Bearbeiten als Gruppenadministratoren Untergruppenmitglieder zuweisen. Anweisungen finden Sie unter [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) im Artikel [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Alternativ können Sie die Verwaltung der Untergruppe den Gruppenadministratoren überlassen, die den darüber liegenden Gruppen zugewiesen sind. Wenn Sie eine Untergruppe erstellen, haben Gruppenadministratoren über die darüber liegenden Gruppen automatischen Zugriff, um die Untergruppe zu verwalten.

>[!NOTE]
>
>Wenn Sie einen Benutzer zu einer Untergruppe hinzufügen und dieser Benutzer ein Gruppenadministrator für eine Gruppe ist, die sich an einer beliebigen Stelle über der Untergruppe befindet, verfügt dieser Benutzer über Administratorrechte zum Verwalten der Untergruppe, selbst wenn er nicht als Gruppenadministrator zugewiesen wurde.

Informationen dazu, welche Aktionen für einen Adobe Workfront-Administrator, der das Workfront-System verwaltet, einen Gruppenadministrator, der eine Gruppe auf oberster Ebene verwaltet, und einen Gruppenadministrator, der eine Untergruppe verwaltet, verfügbar sind, finden Sie unter [Aktionen für verschiedene Arten von Administratoren zulässig](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
