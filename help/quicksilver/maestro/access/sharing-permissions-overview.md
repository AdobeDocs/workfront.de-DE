---
title: Übersicht über die Freigabe von Berechtigungen in den Planungsfunktionen von Adobe Workfront
description: Sie können Berechtigungen für einen Adobe Maestro-Arbeitsbereich oder eine Ansicht freigeben oder entfernen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 7%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Übersicht über die Freigabe von Berechtigungen in den Planungsfunktionen von Adobe Workfront

{{maestro-important-intro}}

Sie können Berechtigungen für einen Arbeitsbereich oder eine Ansicht freigeben oder entfernen, wenn Sie die Planungsfunktionen in Adobe Workfront verwenden.

In diesem Artikel werden die Berechtigungsebenen für Planungs-Funktionsobjekte beschrieben.

Informationen zum Freigeben von Arbeitsbereichen oder Ansichten finden Sie in den folgenden Artikeln:

* [Freigeben von Arbeitsbereichen](/help/quicksilver/maestro/access/share-workspaces.md)

* [Ansichten freigeben](/help/quicksilver/maestro/access/share-views.md)

## Objekte, die Sie in den Planungsfunktionen von Adobe Workfront freigeben können

Sie können die folgenden Objekte freigeben:

* Arbeitsbereiche

  Wenn Sie einen Arbeitsbereich freigeben, werden auch alle Datensatztypen, Datensätze und Felder freigegeben, die mit den Arbeitsbereichen verknüpft sind. Ansichten werden nicht freigegeben.

* Ansichten

## Überlegungen zum Freigeben von Objekten in den Planungsfunktionen von Adobe Workfront

* Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Berechtigungen zusammen, um Ihnen bei der Verwendung von Planungsfunktionen Zugriff auf die Ansicht, den Beitrag oder die Verwaltung von Objekten zu gewähren.

  Informationen darüber, wie sich Lizenztypen auf die Berechtigungsstufen für Planungs-Funktionsobjekte auswirken, finden Sie unter [Übersicht über den Lizenztyp bei Verwendung der Planungsfunktionen von Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).
* Systemadministratoren können von anderen Benutzern erstellte Arbeitsbereiche verwalten und freigeben.
* Wenn Sie kein Systemadministrator sind, können Sie zu Arbeitsbereichen beitragen, die von anderen erstellt wurden, wenn diese für Sie freigegeben sind.
* Arbeitsbereiche können nicht gemeinsam genutzt werden.
* Sie können einen Arbeitsbereich oder eine Ansicht für die folgenden Entitäten freigeben:
   * Benutzende
   * Gruppen
* Andere Benutzer, einschließlich Systemadministratoren, können nur auf Ansichten zugreifen, die sie erstellt haben oder die für sie freigegeben wurden. Systemadministratoren können nur Berechtigungen zum Verwalten einer Ansicht erhalten.
* Sie können einen Link zu einem Arbeitsbereich oder zu einer Ansicht von einer Seite vom Typ Datensatz für andere freigeben. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf den Arbeitsbereich oder die Seite vom Typ Datensatz zugreifen zu können, die in der ausgewählten Ansicht angezeigt wird.

## Freigeben von Berechtigungen für Adobe Workfront-Planungs-Funktionsobjekte

Die Tabellen in den folgenden Abschnitten veranschaulichen den Umfang der Berechtigungen, die Sie beim Freigeben eines Arbeitsbereichs oder einer Ansicht auswählen können, und welche Funktionen jede Ebene zulässt.

>[!IMPORTANT]
>
>Nicht alle Benutzer können über die unten beschriebenen Berechtigungsstufen verfügen. Die individuelle Lizenz eines Benutzers legt fest, welche Höhe von Berechtigungen er für Planungs-Funktionsobjekte erhalten kann.
>
>Weitere Informationen finden Sie unter [Übersicht über den Lizenztyp bei Verwendung der Planungsfunktionen von Adobe Workfront](/help/quicksilver/maestro/access/license-type-overview.md).


### Workspace-Berechtigungen

|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Bearbeiten | ✓ |            |       |
| Freigeben | ✓ |            |       |
| Löschen | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |

### Berechtigungen für Datentypen

Berechtigungen für Datensatztypen werden vererbt, wenn Sie Berechtigungen für den Arbeitsbereich erteilen.

|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ |            |       |
| Löschen | ✓ |            |       |
| Bearbeiten | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |

### Berechtigungen aufzeichnen

Datensatzberechtigungen werden vererbt, wenn Sie Berechtigungen für den Arbeitsbereich erteilen.

|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ |            |       |
| Löschen | ✓ | ✓ |       |
| Bearbeiten | ✓ | ✓ |       |
| Anzeigen | ✓ | ✓ | ✓ |

### Feldberechtigungen

Feldberechtigungen werden übernommen, wenn Sie Berechtigungen für den Arbeitsbereich erteilen.
Die folgenden Berechtigungen beziehen sich auf die Felder selbst und nicht auf die Werte, die den Feldern zugeordnet sind. Um Feldwerte zu bearbeiten, müssen Sie über die Berechtigung zum Bearbeiten von Datensätzen verfügen.

|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ |            |       |
| Löschen | ✓ |            |       |
| Bearbeiten | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |


### Berechtigungen anzeigen

Sie müssen separate Berechtigungen zum Aufzeichnen von Ansichten gewähren. Wenn Sie Berechtigungen für den Arbeitsbereich erteilen, erhalten Sie keine Berechtigungen für die Datensatzansichten im Arbeitsbereich.

|        | Verwalten | Anzeigen |
|--------|--------|-------|
| Bearbeiten | ✓ |       |
| Löschen | ✓ |       |
| Anzeigen | ✓ | ✓ |
| Anwenden | ✓ | ✓ |






