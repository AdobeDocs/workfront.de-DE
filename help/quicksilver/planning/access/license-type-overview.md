---
title: Lizenztyp-Übersicht bei Verwendung von Adobe Workfront Planning
description: Ihr Zugriff auf Adobe Workfront Planning hängt von Ihrem Lizenztyp ab, zusätzlich zu Ihren Berechtigungen für Objekte. Nicht alle Benutzenden in der Organisation haben dieselben Berechtigungen für die Verwendung von Adobe Workfront Planning. In diesem Artikel werden die Zugriffsebenen beschrieben, die Benutzende für Adobe Workfront Planning haben können.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/2V2i9ZZOyQ6gShXK-QUKDeCZCxcrbYwb8-mn-9kQbc8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 650
ht-degree: 1%

---

# Überblick über die Lizenztypen bei Verwendung von Adobe Workfront-Planung

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Adobe Workfront Planning-Berechtigungen zusammen, um den folgenden Zugriff zu gewähren:

* Anzeigen, Bereitstellen oder Verwalten von Arbeitsbereichen oder Datensatztypen
* Ansichten anzeigen oder verwalten. <!--<span class="preview">and records</span>-->

Informationen zu Berechtigungen für Objekte in Workfront Planning finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Informationen zum Zugriff auf Workfront Planning finden Sie unter [Adobe Planning-Zugriffsübersicht](/help/quicksilver/planning/access/access-overview.md).

## Die Beziehung zwischen Workfront-Lizenztypen und Workfront Planning-Berechtigungen

In der folgenden Tabelle wird die Beziehung zwischen dem Lizenztyp eines Benutzers in Adobe Workfront und der Ebene der Berechtigungen beschrieben, die Sie ihm auf der Grundlage dieser Lizenz für Adobe Workfront Planning-Objekte gewähren können.

Durch das Gewähren von Benutzerberechtigungen für einen Arbeitsbereich werden auch Berechtigungen für Datensatztypen, Datensätze und Felder gewährt.

Sie müssen Benutzenden zusätzlich zu den für Arbeitsbereiche separate Berechtigungen für Ansichten gewähren, damit sie auf Ansichten zugreifen und diese verwalten können.

Beachten Sie beim Arbeiten mit Berechtigungen für Datensatztypen Folgendes:

* Benutzer erben automatisch Berechtigungen für Datensatztypen von Arbeitsbereichen.
* Wenn ein(e) Benutzende(r) Verwaltungsberechtigungen für einen Arbeitsbereich hat, kann er/sie keinen geringeren Zugriff auf einen Datensatztyp haben.
* Benutzende können nicht über größere Berechtigungen für einen Datensatztyp verfügen als für den Arbeitsbereich, zu dem der Datensatztyp gehört.
* Wenn Sie Benutzenden die Berechtigungen für einen Datensatztyp entziehen, wird nicht ihr Anzeigezugriff auf alle Datensatztypen im Arbeitsbereich entfernt, da dadurch nicht ihre Berechtigungen für den Arbeitsbereich entfernt werden.

| Adobe Workfront-Lizenztyp | Höchste in Adobe Workfront Planning zulässige Berechtigungen |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Benutzer können Arbeitsbereiche, Datensatztypen, <!--<span class="preview">records</span>--> und Ansichten verwalten. Sie können Workspaces, Datensatztypen, Datensätze, Felder und Ansichten erstellen, bearbeiten oder löschen.</p><br><p>Systemadministratoren haben Verwaltungsberechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.</p> |
| Licht oder Mitwirkender | <p>Benutzer können die für sie freigegebenen Arbeitsbereiche sowie die Datensatztypen, Datensätze und Felder dieser Arbeitsbereiche anzeigen.</p> <br> <p>Benutzer können die Ansichten anzeigen, die für sie freigegeben wurden, sie können jedoch keine eigenen erstellen. </p><br> <p>Benutzende können keine Arbeitsbereiche, Datensatztypen, Datensätze oder Felder erstellen, bearbeiten oder löschen.</p> |

<!--
Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->


### Lizenztypen und Berechtigungen für Arbeitsbereiche und Datensatztypen

Nur Benutzer mit einer Standardlizenz können Berechtigungen zum Beitragen oder Verwalten für Arbeitsbereiche und Datensatztypen haben. Die Berechtigungen Beitragen und Verwalten für Arbeitsbereiche und Datensatztypen werden standardmäßig auch auf Datensätze und Felder übertragen.

Systemadministratoren können alle Arbeitsbereiche im System anzeigen, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.

Benutzer mit allen anderen Lizenztypen haben Ansichtsberechtigungen für Arbeitsbereiche und Datensatztypen, die für sie freigegeben sind, sowie für ihre Datensätze und Felder.


>[!INFO]
>
>**BEISPIEL:**
>
>Mitwirkende oder Light-License-Benutzende können nicht zu Arbeitsbereichen und deren Objekten beitragen oder diese verwalten.
>
>Im Freigabefeld gibt es einen Hinweis darauf, dass Benutzenden keine Berechtigungen zum Bereitstellen oder Verwalten eines Arbeitsbereichs erteilt werden können, wenn sie über eine Lizenz auf niedrigerer Ebene verfügen, da diese Berechtigungsebenen abgeblendet sind.
>
>![Berechtigungen für Mitwirkende auf Arbeitsbereich ausgegraut](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Lizenztypen und Berechtigungen für Ansichten

Nur Benutzer mit einer Standardlizenz können über Verwaltungsberechtigungen für Ansichten verfügen.

Systemadministratoren können nicht auf Ansichten zugreifen, die sie nicht erstellt haben. Sie müssen mit ihnen geteilt werden.

Benutzer mit allen anderen Lizenztypen können über Anzeigeberechtigungen für Ansichten verfügen, die für sie freigegeben wurden.

>[!INFO]
>
>**BEISPIEL:**
>
>Mitwirkende oder Light-License-Benutzende können Ansichten nicht verwalten. Sie können temporäre Filter, Sortierungen oder Gruppierungen auf Ansichten anwenden, auf die sie zugreifen können.
>
>Im Freigabefeld wird angegeben, dass Benutzenden keine Berechtigungen zum Verwalten einer Ansicht erteilt werden können, wenn sie Inhaber einer Lizenz auf niedrigerer Ebene sind, da diese Berechtigungsebenen abgeblendet sind.
>
>![Berechtigungen sind für Light User on View Share ausgegraut](assets/permissions-grayed-out-for-light-user.png)
