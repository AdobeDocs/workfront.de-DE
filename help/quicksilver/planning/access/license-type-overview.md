---
title: Lizenztyp-Übersicht bei Verwendung von Adobe Workfront Planning
description: Ihr Zugriff auf Adobe Workfront Planning hängt von Ihrem Lizenztyp ab, zusätzlich zu Ihren Berechtigungen für Objekte. Nicht alle Benutzenden in der Organisation haben dieselben Berechtigungen für die Verwendung von Adobe Workfront Planning. In diesem Artikel werden die Zugriffsebenen beschrieben, die Benutzende für Adobe Workfront Planning haben können.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: ddcefb0baf10df9ae9ac3b29d7da1e2a070101c8
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Lizenztyp-Übersicht bei Verwendung von Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Adobe Workfront Planning-Berechtigungen zusammen, um den folgenden Zugriff zu gewähren:

* Arbeitsbereiche anzeigen, beitragen oder verwalten
* Ansichten anzeigen oder verwalten.

Informationen zu Berechtigungen für Objekte in Workfront Planning finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Informationen zum Zugriff auf Workfront Planning finden Sie unter [Adobe Planning-Zugriffsübersicht](/help/quicksilver/planning/access/access-overview.md).

## Die Beziehung zwischen Workfront-Lizenztypen und Workfront Planning-Berechtigungen

In der folgenden Tabelle wird die Beziehung zwischen dem Lizenztyp eines Benutzers in Adobe Workfront und der Ebene der Berechtigungen beschrieben, die Sie ihm auf der Grundlage dieser Lizenz für Adobe Workfront Planning-Objekte gewähren können.

Durch das Gewähren von Benutzerberechtigungen für einen Arbeitsbereich werden auch Berechtigungen für Datensatztypen, Datensätze und Felder gewährt.

Sie müssen Benutzenden zusätzlich zu den für Arbeitsbereiche separate Berechtigungen für Ansichten gewähren, damit sie auf Ansichten zugreifen und diese verwalten können.

| Adobe Workfront Lizenztyp* | Höchste in Adobe Workfront Planning zulässige Berechtigungen |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Benutzer können Arbeitsbereiche und Ansichten verwalten. Sie können Workspaces, Datensatztypen, Datensätze, Felder und Ansichten erstellen, bearbeiten oder löschen.</p> <br> <p>Systemadministratoren haben Verwaltungsberechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.</p> |
| Licht oder Mitwirkender | <p>Benutzer können die für sie freigegebenen Arbeitsbereiche sowie die Datensatztypen, Datensätze und Felder dieser Arbeitsbereiche anzeigen.</p> <br> <p>Benutzer können die Ansichten anzeigen, die für sie freigegeben wurden, sie können jedoch keine eigenen erstellen. </p><br> <p>Benutzende können keine Arbeitsbereiche, Datensatztypen, Datensätze oder Felder erstellen, bearbeiten oder löschen.</p> |

*Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar.
Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### Lizenztypen und Workspace-Berechtigungen

Nur Benutzer mit einer Standardlizenz können Berechtigungen zum Beitragen oder Verwalten für Arbeitsbereiche haben. Benutzer aller anderen Lizenztypen können Ansichtsberechtigungen für Arbeitsbereiche haben, die für sie freigegeben wurden.

Systemadministratoren können alle Arbeitsbereiche im System anzeigen, auch die, die sie nicht erstellt haben.

>[!INFO]
>
>**BEISPIEL:**
>
>Mitwirkende oder Light-License-Benutzende können nicht zu Arbeitsbereichen und deren Objekten beitragen oder diese verwalten.
>
>Im Freigabefeld gibt es einen Hinweis darauf, dass Benutzenden keine Berechtigungen zum Bereitstellen oder Verwalten eines Arbeitsbereichs erteilt werden können, wenn sie über eine Lizenz auf niedrigerer Ebene verfügen, da diese Berechtigungsebenen abgeblendet sind.
>
>![Berechtigungen für Mitwirkende auf Arbeitsbereich ausgegraut](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Lizenztypen und Anzeigeberechtigungen

Nur Benutzer mit einer Standardlizenz können über Verwaltungsberechtigungen für Ansichten verfügen. Benutzer mit allen anderen Lizenztypen können über Anzeigeberechtigungen für Ansichten verfügen, die für sie freigegeben wurden.

>[!INFO]
>
>**BEISPIEL:**
>
>Mitwirkende oder Light-License-Benutzende können Ansichten nicht verwalten. Sie können temporäre Filter, Sortierungen oder Gruppierungen auf Ansichten anwenden, auf die sie zugreifen können.
>
>Im Freigabefeld wird angegeben, dass Benutzenden keine Berechtigungen zum Verwalten einer Ansicht erteilt werden können, wenn sie Inhaber einer Lizenz auf niedrigerer Ebene sind, da diese Berechtigungsebenen abgeblendet sind.
>
>![Berechtigungen sind für Light User on View Share ausgegraut](assets/permissions-grayed-out-for-light-user.png)
