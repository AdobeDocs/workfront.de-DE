---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Zugriff auf Objekte und Bereiche nach Lizenztyp
description: Die nachstehende Tabelle zeigt Ihnen die höchste Zugriffsstufe (Bearbeiten oder Anzeigen), die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 0e690cf9cd6351ee89e32b8f1625e8493aa0ad4b
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 17%

---

# Zugriff auf Objekte und Bereiche nach Lizenztyp

Die nachstehende Tabelle zeigt Ihnen die höchste Zugriffsstufe (Bearbeiten oder Anzeigen), die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.

* **Ansicht**: Der Benutzer kann Elemente überprüfen und freigeben.
* **Bearbeiten**: Der Benutzer kann Elemente erstellen, bearbeiten, löschen und freigeben.

   >[!NOTE]
   >
   >Wenn ein anderer Benutzer ein Objekt teilt, kann der Freigebende Berechtigungen festlegen, die dessen Bearbeitung einschränken. Weitere Informationen finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Standard</td>
        <td>Leicht</td>
        <td>Mitwirkender oder Mitwirkende</td>
        <td>Extern</td>
    </tr>
    <tr>
        <td>Projekte</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Anzeigen (nur die Detailseite)</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Aufgaben</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Anzeigen</td>
        <td>Anzeigen</td>
    </tr>
    <tr>
        <td>Probleme</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Portfolios</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Programme</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Berichte, Dashboards und Kalender</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Anzeigen*</td>
        <td>Ansicht (nur für Kalender, keine Freigabeberechtigungen)</td>
    </tr>
    <tr>
        <td>Filter, Ansichten und Gruppierungen</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Dokumente</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten</td>
        <td>Anzeigen (keine Freigabeberechtigungen)</td>
    </tr>
    <tr>
        <td>Benutzende</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Anzeigen</td>
        <td>Anzeigen</td>
    </tr>
    <tr>
        <td>Teams</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Anzeigen</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Vorlagen</td>
        <td>Bearbeiten</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Finanzdaten</td>
        <td>Bearbeiten</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Ressourcenverwaltung</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Szenarienplaner</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Workfront-Ziele</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten</td>
        <td>Kein Zugriff</td>
    </tr>
</table>

&#42; Benutzer mit einer Contributor-Lizenz können nur Berichte, Dashboards und Kalender anzeigen, die für sie freigegeben sind.

>[!NOTE]
>
>Benutzer mit einer Light-Lizenz oder einer Contributor-Lizenz verfügen über eingeschränkte Freigabemöglichkeiten. Weitere Informationen finden Sie unter [Überblick über Lizenzen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>Externe Benutzer können in Workfront nicht nach Elementen suchen. Sie können Dokumente und Kalender anzeigen, die speziell für sie freigegeben wurden. Sie können auch die Benutzer sehen, die Elemente für sie freigeben.

Detaillierte Informationen dazu, was die Zugriffsebenen für jedes Objekt und jeden Bereich zulassen, finden Sie in den folgenden Artikeln:

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
