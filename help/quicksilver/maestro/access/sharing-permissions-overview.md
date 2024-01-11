---
title: Übersicht über die Freigabe von Berechtigungen in Adobe Maestro
description: Sie können Berechtigungen für einen Adobe Maestro-Arbeitsbereich oder eine Ansicht freigeben oder entfernen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 1ae60512c337d778939ef6c48fd2eda8b279dcce
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Übersicht über die Freigabe von Berechtigungen in Adobe Maestro

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Zugriff auf Maestro zu erhalten.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Berechtigungen für einen Adobe Maestro-Arbeitsbereich oder eine Ansicht freigeben oder entfernen.

In diesem Artikel werden die Berechtigungsebenen für Maestro-Objekte beschrieben.

Informationen zum Freigeben von Arbeitsbereichen oder Ansichten finden Sie in den folgenden Artikeln:

* [Freigeben eines Arbeitsbereichs](/help/quicksilver/maestro/access/share-workspaces.md)

* [Anzeigen freigeben](/help/quicksilver/maestro/access/share-views.md)

## Objekte, die Sie in Adobe Maestro freigeben können

Sie können die folgenden Objekte in Maestro freigeben:

* Arbeitsbereiche

  Wenn Sie einen Arbeitsbereich freigeben, werden auch alle Datensatztypen, Datensätze und Felder freigegeben, die mit den Arbeitsbereichen verknüpft sind. Ansichten werden nicht freigegeben.

* Ansichten

## Überlegungen zum Freigeben von Objekten in Maestro

* Sie müssen über die folgende Lizenz verfügen, um Arbeitsbereiche in Maestro zu erstellen:

   * Neues Preismodell: Standardlizenz
   * Aktuelles Preismodell: Arbeite oder höhere Lizenz

  Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* Systemadministratoren können von anderen Benutzern erstellte Arbeitsbereiche verwalten und freigeben.
* Wenn Sie kein Systemadministrator sind, können Sie zu Arbeitsbereichen beitragen, die von anderen erstellt wurden, wenn diese für Sie freigegeben sind.
* Arbeitsbereiche können nicht gemeinsam genutzt werden.
* Sie können einen Arbeitsbereich für die folgenden Entitäten freigeben:
   * Benutzende
   * Gruppen
* Andere Benutzer, einschließlich Systemadministratoren, können nur auf Ansichten zugreifen, die sie erstellt haben oder die für sie freigegeben wurden.

## Berechtigungen für Maestro-Objekte freigeben

Die Tabellen in den folgenden Abschnitten veranschaulichen den Umfang der Berechtigungen, die Sie beim Freigeben eines Maestro-Arbeitsbereichs oder einer Ansicht auswählen können, und welche Funktionen jede Ebene zulässt.

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






