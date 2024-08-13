---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Zugriff auf Objekte und Bereiche durch neue Lizenzen
description: Die nachstehende Tabelle zeigt Ihnen die höchste Zugriffsstufe (Bearbeiten oder Anzeigen), die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 18%

---

# Zugriff auf Objekte und Bereiche durch neue Lizenzen

<!-- Audited: 2/2024 -->

Die nachstehende Tabelle zeigt Ihnen die höchste Zugriffsstufe (Bearbeiten oder Anzeigen), die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.

* **Ansicht**: Der Benutzer kann Elemente überprüfen und freigeben.
* **Bearbeiten**: Der Benutzer kann Elemente erstellen, bearbeiten, löschen und freigeben.

  >[!NOTE]
  >
  >Wenn ein anderer Benutzer ein Objekt teilt, kann der Freigebende Berechtigungen festlegen, die dessen Bearbeitung einschränken. Weitere Informationen finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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
        <td>Anzeigen</td>
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
        <td>Anzeigen</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Programme</td>
        <td>Bearbeiten</td>
        <td>Anzeigen</td>
        <td>Anzeigen</td>
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

&#42; Benutzer mit einer Mitarbeiter-Lizenz können nur Berichte, Dashboards und Kalender anzeigen, die für sie freigegeben sind.

>[!NOTE]
>
>Benutzer mit einer Light-Lizenz oder einer Contributor-Lizenz verfügen über eingeschränkte Freigabemöglichkeiten. Weitere Informationen finden Sie unter [Überblick über Lizenzen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
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
