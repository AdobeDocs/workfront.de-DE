---
title: Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung
description: Ihr Zugriff auf die Adobe Workfront-Planung hängt von Ihrem Lizenztyp ab, zusätzlich zu Ihren Berechtigungen für Objekte.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: f3641e2207563f3fc9d9ed059d889ab6c22f05b1
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung

{{planning-important-intro}}

Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Adobe Workfront Planning-Berechtigungen zusammen, um folgenden Zugriff zu gewähren:

* Arbeitsbereiche anzeigen, einbringen oder verwalten
* Anzeigen oder Verwalten von Ansichten

Informationen zu Berechtigungen für Objekte in der Workfront-Planung finden Sie unter [Übersicht über die Freigabe von Berechtigungen in der Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Beziehung zwischen Workfront-Lizenztypen und Workfront-Planungsberechtigungen

In der folgenden Tabelle wird die Beziehung zwischen dem Lizenztyp eines Benutzers in Adobe Workfront und der Höhe der Berechtigungen beschrieben, die Sie ihm für Adobe Workfront Planning-Objekte auf der Grundlage dieser Lizenz gewähren können.

Wenn Sie einem Benutzer Berechtigungen für einen Arbeitsbereich erteilen, erhalten diese auch Berechtigungen zum Aufzeichnen von Typen, Datensätzen und Feldern.


| Adobe Workfront-Lizenztyp* | Höchste in der Adobe Workfront-Planung zulässige Berechtigungen |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Neu: Standard <br> oder <br>Aktuell: Plan | Benutzer können Arbeitsbereiche verwalten. Sie können Arbeitsbereiche, Datensatztypen, Datensätze und Felder erstellen, bearbeiten oder löschen. <br> Systemadministratoren haben Verwaltungsberechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben. |
| Neu: Leicht, Mitarbeiter <br> oder <br>Aktuell: Arbeit, Anforderer, Überprüfer | Benutzer können die für sie freigegebenen Arbeitsbereiche sowie die Datensatztypen, Datensätze und Felder dieser Arbeitsbereiche anzeigen. <br> Benutzer können keine Arbeitsbereiche, Datensatztypen, Datensätze oder Felder erstellen, bearbeiten oder löschen. |

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Replace the table above with the following at GA:


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Standard                     | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| Light or Contributor  | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

### Lizenztypen und Workspace-Berechtigungen

Nur Benutzer mit einer Standard-(oder Plan-)Lizenz können über Contribute- oder Verwaltungsberechtigungen für Arbeitsbereiche verfügen. Benutzer mit allen anderen Lizenztypen können über Anzeigeberechtigungen für Arbeitsbereiche verfügen, die für sie freigegeben sind.

Systemadministratoren können alle Arbeitsbereiche im System anzeigen, selbst die Arbeitsbereiche, die sie nicht erstellt haben.

>[!INFO]
>
>**BEISPIEL:**
>
>Antragsteller (oder Mitwirkende, je nach dem neuen Lizenzmodell) können nicht zu Arbeitsbereichen und deren Objekten beitragen oder diese verwalten.
>
>Es gibt einen Hinweis im Freigabefeld, dass Benutzern keine Berechtigungen zum Beitrag zu oder zur Verwaltung eines Arbeitsbereichs erteilt werden können, wenn sie über eine Lizenz der unteren Ebene verfügen, da diese Berechtigungsebenen abgeblendet sind.
>
>![](assets/permissions-grayed-out-for-requestor-user.png)


<!--Replace all the content in the section above with the following at Planning GA


Only users with a Standard license can have Contribute or Manage permissions to workspaces. Users with all other license types can have View permissions to workspaces shared with them. 

System administrators can view all workspaces in the system, even the ones they did not create. 

>[!INFO]
>
>**EXAMPLE:** 
>
>Contributors or Light-license users cannot contribute to or manage workspaces and their objects. 
>
>There is an indication in the sharing box that users cannot be granted permissions to contribute to or manage a workspace when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)
-->


### Lizenztypen und Anzeigeberechtigungen

Nur Benutzer mit einer Standard-(oder Plan-)Lizenz können über die Berechtigung &quot;Ansichten verwalten&quot;verfügen. Benutzer mit allen anderen Lizenztypen können über Anzeigeberechtigungen für Ansichten verfügen, die für sie freigegeben sind.

>[!INFO]
>
>**BEISPIEL:**
>
>Mitarbeiter (oder Anforderer und Überprüfer) können keine Ansichten verwalten. Sie können temporäre Filter, Sorten oder Gruppierungen auf Ansichten anwenden, auf die sie zugreifen können.
>
>Es gibt einen Hinweis im Freigabefeld, dass Benutzern keine Berechtigungen zum Verwalten einer Ansicht erteilt werden können, wenn sie eine Lizenz der unteren Ebene besitzen, da diese Berechtigungsebenen abgeblendet sind.
>
>![](assets/permissions-grayed-out-for-reviewer-user-on-a-view.png)


<!--Replace all of the above in this section with the following at GA:

Only users with a Standard license can have Manage permissions to views. Users with all other license types can have View permissions to views shared with them. 

>[!INFO]
>
>**EXAMPLE:** 
>
>Contributors or Light-license users cannot manage views. They can apply temporary filters, sorts, or groupings to views they can access. 
>
>There is an indication in the sharing box that users cannot be granted permissions to manage a view when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![](assets/permissions-grayed-out-for-light-user.png)-->
















<!--Replace all of the above with this:

The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant view permissions separately from workspace permissions. 


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | <ul><li>Users can contribute to or manage workspaces and they can manage views. They can create, edit, or delete workspaces, record types, records, fields, and views.</li> <li> System administrators have Manage permissions to all workspaces, including the ones they did not create.</li> <li> System administrators can only access views they created.</li></ul>                                                                                                                     |
|New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | <ul><li>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</li> <li>Users can access views shared with them and apply temporary filters, sorts, or groupings, but they cannot modify the views. </li><li> Users cannot create, edit, or delete workspaces, record types, records, fields, or views.</li></ul>|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->