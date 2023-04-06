---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Veralteter Zugriff auf Objekte und Bereiche nach Lizenztyp
description: Die nachstehende Tabelle zeigt Ihnen die höchste Zugriffsstufe (Bearbeiten oder Anzeigen), die jede der älteren Adobe Workfront-Lizenzen für die Objekte und Bereiche in Workfront zulässt.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: e3211ac5801c1318978427bc0a48d9b3a3028984
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 19%

---

# Veralteter Zugriff auf Objekte und Bereiche nach Lizenztyp

In der folgenden Tabelle finden Sie Informationen zur höchsten Ebene des Legacy-Zugriffs (Bearbeiten oder Anzeigen), die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.

* **Ansicht**: Der Benutzer kann Elemente überprüfen und freigeben.
* **Bearbeiten**: Der Benutzer kann Elemente erstellen, bearbeiten, löschen und freigeben.

   >[!NOTE]
   >
   >Wenn ein anderer Benutzer ein Objekt teilt, kann der Freigebende Berechtigungen festlegen, die dessen Bearbeitung einschränken. Weitere Informationen finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | Plan | Arbeit | Überarbeitung | Anfrage | Extern |
|---|---|---|---|---|---|
| Projekte | Bearbeiten | Bearbeiten (ohne Berechtigungen erstellen) | Anzeigen | Anzeigen (nur die Detailseite) | Kein Zugriff |
| Aufgaben | Bearbeiten | Bearbeiten | Anzeigen | Anzeigen | Anzeigen |
| Probleme | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff |
| Portfolios | Bearbeiten | Anzeigen | Anzeigen | Kein Zugriff | Kein Zugriff |
| Programme | Bearbeiten | Anzeigen | Anzeigen | Kein Zugriff | Kein Zugriff |
| Berichte, Dashboards und Kalender | Bearbeiten | Anzeigen | Anzeigen | &#42; anzeigen | Ansicht (nur für Kalender, keine Freigabeberechtigungen) |
| Filter, Ansichten und Gruppierungen | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff |
| Dokumente | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Anzeigen (keine Freigabeberechtigungen) |
| Benutzende | Bearbeiten | Anzeigen | Anzeigen | Anzeigen | Anzeigen |
| Teams | Bearbeiten | Bearbeiten | Anzeigen | Anzeigen | Kein Zugriff |
| Vorlagen | Bearbeiten | Kein Zugriff | Kein Zugriff | Kein Zugriff | Kein Zugriff |
| Finanzdaten | Bearbeiten | Anzeigen (nur im Bereich &quot;Finanzen&quot;in Projektdetails) | Anzeigen | Kein Zugriff | Kein Zugriff |
| Ressourcenverwaltung | Bearbeiten | Anzeigen | Anzeigen | Kein Zugriff | Kein Zugriff |
| Szenarienplaner | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff | Kein Zugriff |
| Workfront-Ziele | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff |

&#42; Benutzer mit einer Anforderungslizenz können nur Berichte, Dashboards und Kalender anzeigen, die für sie freigegeben sind.

>[!NOTE]
>
>Benutzer mit einer Review-Lizenz oder einer Request-Lizenz verfügen über eingeschränkte Freigabemöglichkeiten. Weitere Informationen finden Sie unter [Übersicht über Adobe Workfront-Lizenzen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) oder [Übersicht über veraltete Adobe Workfront-Lizenzen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Externe Benutzer können in Workfront nicht nach Elementen suchen. Sie können Dokumente und Kalender anzeigen, die speziell für sie freigegeben wurden. Sie können auch die Benutzer sehen, die Elemente für sie freigeben.

Detaillierte Informationen dazu, was die alten Zugriffsebenen für jedes Objekt und jeden Bereich zulassen, finden Sie in den folgenden Artikeln:

* [Projektzugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Zugriff auf Probleme gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Zugriff auf Dokumente gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Zugriff auf Portfolios gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Zugriff auf Programme gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Zugriff auf Filter, Ansichten und Gruppierungen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Gewähren von Zugriff auf Teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Zugriff auf Vorlagen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Zugriff auf Resource Management gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Zugriff auf den Szenario-Planer gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Zugriff auf Adobe Workfront-Ziele gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
