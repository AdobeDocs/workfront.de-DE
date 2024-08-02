---
title: Übersicht über die Freigabe von Berechtigungen in der Adobe Workfront-Planung
description: Sie können Berechtigungen für einen Adobe Workfront Planning-Arbeitsbereich oder eine Ansicht freigeben oder daraus entfernen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 1ffd8a3dbb31154186dc37132c7e77c35de42ac3
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 6%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Übersicht über die Freigabe von Berechtigungen in der Adobe Workfront-Planung

{{planning-important-intro}}

Sie können Berechtigungen für einen Arbeitsbereich oder eine Ansicht in der Adobe Workfront-Planung freigeben oder daraus entfernen.

In diesem Artikel werden die Berechtigungsebenen für Workfront Planning-Objekte beschrieben.

Informationen zum Freigeben von Arbeitsbereichen oder Ansichten finden Sie in den folgenden Artikeln:

* [Freigeben von Arbeitsbereichen](/help/quicksilver/planning/access/share-workspaces.md)

* [Ansichten freigeben](/help/quicksilver/planning/access/share-views.md)

## Objekte, die Sie in der Adobe Workfront-Planung freigeben können

Sie können die folgenden Objekte freigeben:

* Arbeitsbereiche

   * Sie können Arbeitsbereiche für Personen in Ihrem Unternehmen freigeben.
   * Wenn Sie einen Arbeitsbereich freigeben, werden auch alle Datensatztypen, Datensätze und Felder freigegeben, die mit den Arbeitsbereichen verknüpft sind. Ansichten werden nicht freigegeben.

* Ansichten

   * Sie müssen Benutzern, einschließlich Systemadministratoren, Berechtigungen erteilen, unabhängig von ihren Berechtigungen für den Zugriff auf Arbeitsbereiche auf Ansichten zuzugreifen.
   * Sie können eine Ansicht öffentlich für Personen außerhalb Ihres Unternehmens freigeben, wenn Sie einen öffentlichen Link für eine Ansicht generieren. Personen, die über einen öffentlichen Link auf die Datensatzseite zugreifen, können alle Datensätze und deren Felder, einschließlich verbundener Datensätze und Felder, anzeigen.

  Weitere Informationen finden Sie unter [Ansichten freigeben](/help/quicksilver/planning/access/share-views.md).

Intern können Sie einen Arbeitsbereich oder eine Ansicht für die folgenden Workfront-Entitäten freigeben:

* Benutzende
* Gruppen

## Überlegungen zum Freigeben von Objekten in der Adobe Workfront-Planung

* Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Workfront Planning-Berechtigungen zusammen, um Ihnen Zugriff auf die Ansicht, den Beitrag und die Verwaltung von Arbeitsbereichen und deren Objekten zu gewähren.

  Informationen dazu, wie sich Lizenztypen auf die Berechtigungsstufen für die Workfront-Planung auswirken, finden Sie unter [Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung](/help/quicksilver/planning/access/license-type-overview.md).
* Systemadministratoren können alle Arbeitsbereiche im System verwalten, einschließlich derjenigen, die sie nicht erstellt haben.
* Andere Benutzer, einschließlich Systemadministratoren, können nur auf Ansichten zugreifen, die sie erstellt haben oder die für sie freigegeben wurden. Systemadministratoren können nur Berechtigungen zum Verwalten einer Ansicht erhalten.
* Sie können einen Link zu einem Arbeitsbereich oder einer Ansicht für andere freigeben.

  Die folgenden Szenarien existieren:
   * Benutzer, die den Link zu einem Arbeitsbereich erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf den Arbeitsbereich zugreifen zu können.
   * Benutzer, die den Link zu einer Ansicht erhalten, können wie folgt auf die Ansicht zugreifen:

      * Muss aktive Benutzer sein und sich bei Workfront anmelden, wenn der Link zur Ansicht intern freigegeben wurde.
      * Kann externe Benutzer in Workfront sein und über einen öffentlich freigegebenen Link auf die Ansicht zugreifen, ohne sich bei Workfront anzumelden.

## Berechtigungen für Adobe Workfront Planning-Objekte freigeben

Die Tabellen in den folgenden Abschnitten veranschaulichen den Umfang der Berechtigungen, die Sie beim Freigeben eines Arbeitsbereichs oder einer Ansicht auswählen können, und welche Funktionen jede Ebene zulässt.

>[!IMPORTANT]
>
>Nicht alle Benutzer können über die unten beschriebenen Berechtigungsstufen verfügen. Die individuelle Lizenz eines Benutzers legt fest, welche Berechtigungen er für Workfront Planning-Objekte erhalten kann.
>
>Nur Standardlizenzbenutzer (oder -planbenutzer) können über Contribute- oder Verwaltungsberechtigungen für Arbeitsbereiche verfügen und Berechtigungen für Ansichten verwalten.
> 
>Benutzer mit allen anderen Lizenztypen können über Anzeigeberechtigungen für Arbeitsbereiche und Ansichten verfügen.
>
>Weitere Informationen finden Sie unter [Übersicht über den Lizenztyp bei Verwendung der Adobe Workfront-Planung](/help/quicksilver/planning/access/license-type-overview.md).


### Workspace-Berechtigungen

Sie müssen Benutzern Berechtigungen für Arbeitsbereiche erteilen, damit sie Zugriff auf die folgenden Entitäten haben können:

* Arbeitsbereiche
* Datensatztypen
* Datensätze
* Felder

Im Folgenden finden Sie die Berechtigungsstufen für Arbeitsbereiche:

|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Bearbeiten | ✓ |            |       |
| Freigeben | ✓ |            |       |
| Löschen | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |

### Berechtigungen für Datentypen

Berechtigungen für Datensatztypen werden vererbt, wenn Sie Berechtigungen für den Arbeitsbereich erteilen.

Im Folgenden finden Sie die Berechtigungsebenen für Datensatztypen:


|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ |            |       |
| Löschen | ✓ |            |       |
| Bearbeiten | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |

### Berechtigungen aufzeichnen

Datensatzberechtigungen werden vererbt, wenn Sie Berechtigungen für den Arbeitsbereich erteilen.

Im Folgenden finden Sie die Berechtigungsstufen für Datensätze:


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

Sie müssen Benutzern Berechtigungen für Ansichten erteilen, damit sie Zugriff auf die folgenden Ansichtselemente haben können:

* Filter
* Feldsichtbarkeit
* Sortieren
* Gruppierung
* Zeilenhöhe
* Einstellungen

Sie können Ansichten intern oder öffentlich freigeben.

Im Folgenden finden Sie die Berechtigungsebenen für Ansichten und Ansichtselemente:

| Interne Freigabe | Verwalten (nur eingeladene Personen können darauf zugreifen) | Anzeigen (nur eingeladene Personen können darauf zugreifen) | Jeder im Arbeitsbereich kann anzeigen* |
|--------|--------|-------|------------------------------|
| Bearbeiten | ✓ |       |                            |
| Löschen | ✓ |       |                            |
| Freigeben | ✓ |       |                           |
| Anzeigen | ✓ | ✓ | ✓ |
| Anwenden | ✓ | ✓ | ✓ |

| Öffentliche Freigabe | Anzeigen |
|--------|-------|
| Anzeigen | ✓ |
| Anwenden | ✓ |

*Benutzer müssen über Ansicht oder höhere Berechtigungen für einen Arbeitsbereich verfügen, um Zugriff auf diese Ansicht zu erhalten.



<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->