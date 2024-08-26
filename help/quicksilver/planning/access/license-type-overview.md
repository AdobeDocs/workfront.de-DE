---
title: Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung
description: Ihr Zugriff auf die Adobe Workfront-Planung hängt von Ihrem Lizenztyp ab, zusätzlich zu Ihren Berechtigungen für Objekte. Nicht alle Benutzer in der Organisation haben denselben Zugriff und dieselben Berechtigungen für die Verwendung von Adobe Workfront Planning. In diesem Artikel werden die Zugriffsstufen beschrieben, die Benutzer für die Adobe Workfront-Planung haben können.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: f9abcd9ff4c80376bed229a1d65e0efcbfc332b0
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung

{{planning-important-intro}}

Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Adobe Workfront Planning-Berechtigungen zusammen, um folgenden Zugriff zu gewähren:

* Arbeitsbereiche anzeigen, einbringen oder verwalten
* Anzeigen oder Verwalten von Ansichten

Informationen zu Berechtigungen für Objekte in der Workfront-Planung finden Sie unter [Übersicht über die Freigabe von Berechtigungen in der Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Informationen zum Zugriff auf die Workfront-Planung finden Sie unter [Zugriffsübersicht](/help/quicksilver/planning/access/access-overview.md).

## Beziehung zwischen Workfront-Lizenztypen und Workfront-Planungsberechtigungen

In der folgenden Tabelle wird die Beziehung zwischen dem Lizenztyp eines Benutzers in Adobe Workfront und der Höhe der Berechtigungen beschrieben, die Sie ihm für Adobe Workfront Planning-Objekte auf der Grundlage dieser Lizenz gewähren können.

Wenn Sie einem Benutzer Berechtigungen für einen Arbeitsbereich erteilen, erhalten diese auch Berechtigungen zum Aufzeichnen von Typen, Datensätzen und Feldern.

Sie müssen Benutzern neben den Berechtigungen für Arbeitsbereiche separate Berechtigungen für Ansichten gewähren, damit sie auf Ansichten zugreifen und diese verwalten können.

| Adobe Workfront-Lizenztyp* | Höchste in der Adobe Workfront-Planung zulässige Berechtigungen |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Benutzer können Arbeitsbereiche und Ansichten verwalten. Sie können Arbeitsbereiche, Datensatztypen, Datensätze, Felder und Ansichten erstellen, bearbeiten oder löschen.</p> <br> <p>Systemadministratoren haben Verwaltungsberechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.</p> |
| Light oder Contributor | <p>Benutzer können die für sie freigegebenen Arbeitsbereiche sowie die Datensatztypen, Datensätze und Felder dieser Arbeitsbereiche anzeigen.</p> <br> <p>Benutzer können die für sie freigegebenen Ansichten anzeigen, jedoch keine eigenen erstellen. </p><br> <p>Benutzer können keine Arbeitsbereiche, Datensatztypen, Datensätze oder Felder erstellen, bearbeiten oder löschen.</p> |

*Die Workfront-Planung ist nicht für ältere Workfront-Lizenzen verfügbar.
Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### Lizenztypen und Workspace-Berechtigungen

Nur Benutzer mit einer Standardlizenz können über Contribute- oder Verwaltungsberechtigungen für Arbeitsbereiche verfügen. Benutzer mit allen anderen Lizenztypen können über Anzeigeberechtigungen für Arbeitsbereiche verfügen, die für sie freigegeben sind.

Systemadministratoren können alle Arbeitsbereiche im System anzeigen, selbst die Arbeitsbereiche, die sie nicht erstellt haben.

>[!INFO]
>
>**BEISPIEL:**
>
>Mitarbeiter oder Benutzer mit Light-Lizenz können nicht zu Arbeitsbereichen und deren Objekten beitragen oder diese verwalten.
>
>Es gibt einen Hinweis im Freigabefeld, dass Benutzern keine Berechtigungen zum Beitrag zu oder zur Verwaltung eines Arbeitsbereichs erteilt werden können, wenn sie über eine Lizenz der unteren Ebene verfügen, da diese Berechtigungsebenen abgeblendet sind.
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Lizenztypen und Anzeigeberechtigungen

Nur Benutzer mit einer Standardlizenz können über die Berechtigung zum Verwalten von Ansichten verfügen. Benutzer mit allen anderen Lizenztypen können über Anzeigeberechtigungen für Ansichten verfügen, die für sie freigegeben sind.

>[!INFO]
>
>**BEISPIEL:**
>
>Mitarbeiter oder Benutzer mit Light-Lizenz können keine Ansichten verwalten. Sie können temporäre Filter, Sorten oder Gruppierungen auf Ansichten anwenden, auf die sie zugreifen können.
>
>Es gibt einen Hinweis im Freigabefeld, dass Benutzern keine Berechtigungen zum Verwalten einer Ansicht erteilt werden können, wenn sie eine Lizenz der unteren Ebene besitzen, da diese Berechtigungsebenen abgeblendet sind.
>
>![](assets/permissions-grayed-out-for-light-user.png)
