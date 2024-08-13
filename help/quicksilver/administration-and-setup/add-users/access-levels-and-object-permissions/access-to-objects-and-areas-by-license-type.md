---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Zugriff auf Objekte und Bereiche nach Lizenztyp
description: Die nachstehende Tabelle zeigt Ihnen die höchste Zugriffsstufe (Bearbeiten oder Anzeigen), die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 20%

---

# Zugriff auf Objekte und Bereiche nach Lizenztyp

Die nachstehende Tabelle zeigt Ihnen die höchste Zugriffsstufe (Bearbeiten oder Anzeigen), die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.

* **Ansicht**: Der Benutzer kann Elemente überprüfen und freigeben.
* **Bearbeiten**: Der Benutzer kann Elemente erstellen, bearbeiten, löschen und freigeben.

  >[!NOTE]
  >
  >Wenn ein anderer Benutzer ein Objekt teilt, kann der Freigebende Berechtigungen festlegen, die dessen Bearbeitung einschränken. Weitere Informationen finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | Plan | Arbeit | Überprüfung | Anfrage | Extern |
|---|---|---|---|---|---|
| Projekte | Bearbeiten | Bearbeiten (ohne Berechtigungen erstellen) | Anzeigen | Anzeigen (nur die Detailseite) | Kein Zugriff |
| Aufgaben | Bearbeiten | Bearbeiten | Anzeigen | Anzeigen | Anzeigen |
| Probleme | Bearbeiten | Bearbeiten | Bearbeiten | Bearbeiten | Kein Zugriff |
| Portfolios | Bearbeiten | Anzeigen | Anzeigen | Kein Zugriff | Kein Zugriff |
| Programme | Bearbeiten | Anzeigen | Anzeigen | Kein Zugriff | Kein Zugriff |
| Berichte, Dashboards und Kalender | Bearbeiten | Anzeigen | Anzeigen | Ansicht&#42; | Ansicht (nur für Kalender, keine Freigabeberechtigungen) |
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
>Benutzer mit einer Review-Lizenz oder einer Request-Lizenz verfügen über eingeschränkte Freigabemöglichkeiten. Weitere Informationen finden Sie unter [Übersicht über Adobe Workfront-Lizenzen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Externe Benutzer können in Workfront nicht nach Elementen suchen. Sie können Dokumente und Kalender anzeigen, die speziell für sie freigegeben wurden. Sie können auch die Benutzer sehen, die Elemente für sie freigeben.

Detaillierte Informationen dazu, was die Zugriffsebenen für jedes Objekt und jeden Bereich zulassen, finden Sie in den folgenden Artikeln:

* [Gewähren des Zugriffs auf Projekte](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Gewähren des Zugriffs auf Probleme](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Zugriff auf Dokumente gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Gewähren des Zugriffs auf Portfolios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Gewähren des Zugriffs auf Programme](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Gewähren des Zugriffs auf Filter, Ansichten und Gruppierungen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Gewähren des Zugriffs für Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Gewähren von Zugriff auf Teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Zugriff auf Vorlagen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Gewähren des Zugriffs auf die Ressourcenverwaltung](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Gewähren des Zugriffs auf den Szenario-Planer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Zugriff auf Adobe Workfront-Ziele gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
