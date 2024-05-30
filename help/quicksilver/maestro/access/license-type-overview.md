---
title: Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung
description: Ihr Zugriff auf die Adobe Workfront-Planung hängt von Ihrem Lizenztyp ab, zusätzlich zu Ihren Berechtigungen für Objekte.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung

{{planning-important-intro}}

Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Adobe Workfront Planning-Berechtigungen zusammen, um Ihnen Zugriff auf die Ansicht, den Beitrag und die Verwaltung von Arbeitsbereichen zu gewähren. <!--add more objects here when we can grant other object-specific permissions-->

Benutzer mit allen Lizenztypen können Workfront-Planungsansichten anzeigen, erstellen, bearbeiten oder verwalten.

In diesem Artikel werden die in Workfront erforderlichen Lizenztypen und die Berechtigungen beschrieben, die Arbeitsbereichen in der Workfront-Planung je nach Lizenztyp gewährt werden.

Ein Benutzer mit einem Lizenztyp der unteren Ebene hat bei der Verwendung von Workfront-Planungsfunktionen nur eingeschränkte Berechtigungen für Arbeitsbereiche.

>[!INFO]
>
>**BEISPIEL**
>
>Antragsteller (oder Mitwirkende, je nach dem neuen Lizenzmodell) können nicht zu Arbeitsbereichen und deren Objekten beitragen oder diese verwalten.
>
>Im Freigabefeld wird angegeben, dass Benutzern keine Berechtigungen zum Beitrag zu einem Arbeitsbereich oder zur Verwaltung von Arbeitsbereichen erteilt werden können, wenn sie über eine Lizenz der unteren Ebene verfügen.
>
>![](assets/permissions-grayed-out-for-requestor-user.png)


Informationen zu Berechtigungen für Objekte in der Workfront-Planung finden Sie unter [Übersicht über die Freigabe von Berechtigungen in der Adobe Workfront-Planung](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

## Beziehung zwischen Workfront-Lizenztypen und Workfront-Planungsberechtigungen

In der folgenden Tabelle wird die Beziehung zwischen dem Lizenztyp eines Benutzers in Adobe Workfront und der Höhe der Berechtigungen beschrieben, die Sie ihm für Adobe Workfront Planning-Objekte auf der Grundlage dieser Lizenz gewähren können.

Wenn Sie einem Benutzer Berechtigungen für einen Arbeitsbereich erteilen, erhalten diese auch Berechtigungen zum Aufzeichnen von Typen, Datensätzen und Feldern.


| Adobe Workfront-Lizenztyp* | In der Adobe Workfront-Planung zulässige Berechtigungen |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Neu: Standard <br> oder <br>Aktuell: Plan | Benutzer können Arbeitsbereiche, Datensatztypen und Datensätze erstellen und verwalten.<br> Systemadministratoren haben Verwaltungsberechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben. |
| Neu: hell <br> oder <br>Aktuell: Arbeit | Benutzer können einen für sie freigegebenen Arbeitsbereich sowie die Datensatztypen und -datensätze aus diesem Arbeitsbereich beitragen und anzeigen. <br> Benutzer können Datensätze in den Arbeitsbereichen erstellen, bearbeiten und löschen, für die sie über Beitragsberechtigungen verfügen. |
| Neu: Mitarbeiter <br> oder <br>Aktuell: Überprüfer oder Anforderer | Benutzer können die für sie freigegebenen Arbeitsbereiche sowie die Datensatztypen und -datensätze dieser Arbeitsbereiche anzeigen. <br> Benutzer können keine Datensatztypen oder Datensätze erstellen, bearbeiten oder löschen. |

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).