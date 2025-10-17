---
title: Hauptgruppen - Übersicht
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Im Profil des Benutzers wird eine Hauptgruppe zugewiesen. Alle Benutzer müssen über eine Hauptgruppe verfügen.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Hauptgruppen - Übersicht

Im Profil des Benutzers wird eine Hauptgruppe zugewiesen. Alle Benutzer müssen über eine Hauptgruppe verfügen. Ein Benutzer kann zu mehr als einer Gruppe gehören, darf aber nur eine Hauptgruppe haben. Weitere Informationen zu Gruppen finden Sie unter [Gruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Obwohl jede im System vorhandene Gruppe als Hauptgruppe eines Benutzers zugewiesen werden kann, empfehlen wir, neue Gruppen zu erstellen und zuzuweisen, die größere Organisationseinheiten darstellen.

Berücksichtigen Sie beim Einrichten von Hauptgruppen, wie Ihr Unternehmen Ihre Adobe Workfront-Benutzenden aufteilt. Im Folgenden finden Sie einige Vorschläge, wie Sie festlegen können, welcher Gruppentyp als Hauptgruppe verwendet werden soll:

* Gruppen, die Abteilungen wie IT oder Marketing repräsentieren
* Gruppen mit unterschiedlichen Budgets
* Gruppen in verschiedenen Gebieten oder Regionen
* Gruppen bestehend aus mehreren Teams, die derselben Kostenstelle angehören

>[!NOTE]
>
>Wenn Sie Ihre Hauptgruppen in Organisationseinheiten neu organisieren müssen, müssen Sie Folgendes tun:>
>1. Erstellen Sie die neue Gruppe, wie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) beschrieben.
>1. Weisen Sie die neue Gruppe als Hauptgruppe des Benutzers zu, wie in [Bearbeiten des Profils eines Benutzers](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) beschrieben.
>

## Layout-Vorlagenverwaltung

Wenn Sie eine Layout-Vorlage einer Gruppe zuweisen, können alle Benutzenden, denen die Gruppe als Hauptgruppe zugewiesen ist, die in der Layout-Vorlage angegebenen Einstellungen sehen.

Wenn eine Layout-Vorlage einer Hauptgruppe zugewiesen ist, ist sie nur für Benutzer sichtbar, die dieser Hauptgruppe zugewiesen sind.

Weitere Informationen finden Sie unter [Erstellen und Verwalten von Layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)Vorlagen“ in [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Lizenzverwaltung

Jeder Benutzer kann nur einer Hauptgruppe zugewiesen werden, wodurch die Verwaltung der Lizenzanzahl vereinfacht wird.

Workfront-Administratoren haben die Möglichkeit, die maximale Lizenzanzahl für die Hauptgruppen festzulegen.

Wenn Sie eine maximale Lizenzanzahl festlegen, können Workfront-Admins verhindern, dass eine Geschäftseinheit Workfront-Lizenzen verwendet, die für andere Geschäftseinheiten erworben wurden.

Weitere Informationen finden Sie unter [Verfügbare Lizenzen in Ihrem System verwalten](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
