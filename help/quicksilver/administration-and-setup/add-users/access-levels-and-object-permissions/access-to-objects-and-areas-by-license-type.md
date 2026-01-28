---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Zugriff auf Objekte und Bereiche nach Lizenztyp (veraltet)
description: In der folgenden Tabelle wird die höchste Zugriffsebene (Bearbeiten oder Anzeigen) angegeben, die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 23%

---

# Zugriff auf Objekte und Bereiche nach Lizenztyp (veraltet)

<!-- Audited: 11/2025 -->

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die alten Zugriffsebenen. Informationen zu den aktuellen Zugriffsebenen finden Sie unter [Übersicht über neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

In der folgenden Tabelle wird die höchste Zugriffsebene (Bearbeiten oder Anzeigen) angegeben, die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.

* Anzeigen : Der/die Benutzende kann Elemente überprüfen und freigeben.
* Bearbeiten: Benutzende können Elemente erstellen, bearbeiten, löschen und freigeben.

  >[!NOTE]
  >
  >Wenn ein anderer Benutzer ein Objekt freigibt, kann der freigebende Benutzer Berechtigungen festlegen, die seine Möglichkeit zur Bearbeitung einschränken. Weitere Informationen zu den neuen Lizenztypen finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

  >[!NOTE]
  >
  >Dieser Artikel enthält Informationen zum Objektzugriff für ältere Lizenztypen. Informationen zu den neuen Lizenztypen finden Sie unter [Übersicht über neue ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) und [Übersicht über neue Lizenzen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

|   | Plan | Arbeit | Überprüfung | Anfrage | Extern |
|---|---|---|---|---|---|
| Projekte | Bearbeiten | Bearbeiten (ohne Erstellungsberechtigungen) | Ansicht | Anzeigen (nur die Detailseite) | Kein Zugriff |
| Aufgaben | Bearbeiten | Bearbeiten | Ansicht | Ansicht | Kein Zugriff |
| Probleme | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff |
| Portfolios | Bearbeiten | Ansicht | Ansicht | Kein Zugriff | Kein Zugriff |
| Programme | Bearbeiten | Ansicht | Ansicht | Kein Zugriff | Kein Zugriff |
| Berichte, Dashboards und Kalender | Bearbeiten | Ansicht | Ansicht | Anzeigen&#42; | Anzeigen (nur für Kalender, keine Freigabeberechtigungen) |
| Filter, Ansichten und Gruppierungen | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff |
| Dokumente | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Ansicht (keine Freigabeberechtigungen) |
| Benutzende | Bearbeiten | Ansicht | Ansicht | Ansicht | Ansicht |
| Teams | Bearbeiten | Bearbeiten | Ansicht | Ansicht | Kein Zugriff |
| Vorlagen | Bearbeiten | Kein Zugriff | Kein Zugriff | Kein Zugriff | Kein Zugriff |
| Finanzdaten | Bearbeiten | Anzeigen (nur den Bereich „Finanzen“ in den Projektdetails) | Ansicht | Kein Zugriff | Kein Zugriff |
| Ressourcenverwaltung | Bearbeiten | Ansicht | Ansicht | Kein Zugriff | Kein Zugriff |
| Szenarienplaner | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff | Kein Zugriff |
| Workfront-Ziele | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff |

&#42; Benutzer mit einer Anfragelizenz können nur Berichte, Dashboards und Kalender anzeigen, die für sie freigegeben sind.

>[!NOTE]
>
>Benutzende mit einer Überprüfungs- oder Anforderungslizenz verfügen über eingeschränkte Freigabefunktionen. Weitere Informationen finden Sie unter [Lizenzen - Übersicht](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Externe Benutzende können in Workfront nicht nach Elementen suchen. Sie können Dokumente und Kalender anzeigen, die speziell für sie freigegeben wurden. Sie können auch die Benutzenden sehen, die Elemente für sie freigeben.

Detaillierte Informationen zu den Zugriffsebenen für die einzelnen Objekte und Bereiche finden Sie in den folgenden Artikeln:

* [Zugriff auf Projekte gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Zugriff auf Anfragen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Zugriff auf Dokumente gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Zugriff auf Portfolios gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Zugriff auf Programme gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Benutzern Zugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Zugriff auf Teams gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Zugriff auf Vorlagen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Zugriff auf Ressourcenverwaltung gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Zugriff auf den Szenario-Planer gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Zugriff auf Adobe Workfront-Ziele gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
