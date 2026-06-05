---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Zugriff auf Objekte und Bereiche durch Lizenzen
description: In der folgenden Tabelle wird die höchste Zugriffsebene (Bearbeiten oder Anzeigen) angegeben, die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
TQID: https://experienceleague.adobe.com/R6F5ULNqGlQBbYQMh4Huh6Vcu7ZgXG6EgzQf42iZmdA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d3382524-5489-431b-bde9-271ab257bc37
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 489
ht-degree: 31%

---

# Zugriff auf Objekte und Bereiche durch Lizenzen

<!-- Audited: 2/2024 -->

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die aktuellen Zugriffsebenen. Informationen zu den alten Zugriffsebenen finden Sie unter [Überblick über Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

In der folgenden Tabelle wird die höchste Zugriffsebene (Bearbeiten oder Anzeigen) angegeben, die jede Adobe Workfront-Lizenz für die Objekte und Bereiche in Workfront zulässt.

* **Anzeigen**: Der Benutzer kann Elemente überprüfen und freigeben.
* **Bearbeiten**: Der Benutzer kann Elemente erstellen, bearbeiten, löschen und freigeben.

  >[!NOTE]
  >
  >Wenn ein anderer Benutzer ein Objekt freigibt, kann der freigebende Benutzer Berechtigungen festlegen, die seine Möglichkeit zur Bearbeitung einschränken. Weitere Informationen finden Sie unter [Überblick über Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Standard</td>
        <td>Light</td>
        <td>Mitwirkende</td>
        <td>Extern</td>
    </tr>
    <tr>
        <td>Projekte</td>
        <td>Bearbeiten</td>
        <td>Bearbeiten**</td>
        <td>Ansicht</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Aufgaben</td>
        <td>Bearbeiten</td>
        <td>Ansicht</td>
        <td>Ansicht</td>
        <td>Kein Zugriff</td>
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
        <td>Ansicht</td>
        <td>Ansicht</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Programme</td>
        <td>Bearbeiten</td>
        <td>Ansicht</td>
        <td>Ansicht</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Berichte, Dashboards und Kalender</td>
        <td>Bearbeiten</td>
        <td>Ansicht</td>
        <td>Anzeigen*</td>
        <td>Anzeigen (nur für Kalender, keine Freigabeberechtigungen)</td>
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
        <td>Ansicht (keine Freigabeberechtigungen)</td>
    </tr>
    <tr>
        <td>Benutzende</td>
        <td>Bearbeiten</td>
        <td>Ansicht</td>
        <td>Ansicht</td>
        <td>Ansicht</td>
    </tr>
    <tr>
        <td>Aufgabengebiete</td>
        <td>Bearbeiten</td>
        <td>Ansicht</td>
        <td>Ansicht</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Teams</td>
        <td>Bearbeiten</td>
        <td>Ansicht</td>
        <td>Ansicht</td>
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
        <td>Ansicht</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Szenarienplaner</td>
        <td>Bearbeiten</td>
        <td>Ansicht</td>
        <td>Kein Zugriff</td>
        <td>Kein Zugriff</td>
    </tr>
    <tr>
        <td>Tarifkarten</td>
        <td>Bearbeiten</td>
        <td>Ansicht</td>
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

&#42; Benutzer mit der Lizenz Mitwirkende können nur Berichte, Dashboards und Kalender anzeigen, die für sie freigegeben sind.

&#42;&#42; Benutzer mit einer Light-Lizenz können die Zeit nur auf Projektebene protokollieren, wenn der Bearbeitungszugriff aktiviert ist. Sie können keine Projekte erstellen, bearbeiten, löschen oder freigeben. Die standardmäßige Zugriffsebene für Projekte für Light-Benutzer ist Ansicht.

>[!NOTE]
>
>* Benutzende mit einer Light-Lizenz oder einer Contributor-Lizenz verfügen über eingeschränkte Freigabefunktionen. Weitere Informationen finden Sie unter [Überblick über Lizenzen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>* Externe Benutzende können in Workfront nicht nach Elementen suchen. Sie können Dokumente und Kalender anzeigen, die speziell für sie freigegeben wurden. Sie können auch die Benutzenden sehen, die Elemente für sie freigeben.
>
>* Mitwirkende und externe Benutzer können keine Inhalte sehen, die systemweit freigegeben sind.  Es muss ausdrücklich für sie freigegeben werden.

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
* [Gewähren von Zugriff auf Teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Zugriff auf Vorlagen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Zugriff auf Ressourcenverwaltung gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Zugriff auf den Szenario-Planer gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Zugriff auf Tarifkarten gewähren](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-rate-cards.md)
* [Zugriff auf Adobe Workfront-Ziele gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
