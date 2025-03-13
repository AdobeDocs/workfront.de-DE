---
title: Übersicht über Freigabeberechtigungen in Adobe Workfront Planning
description: Nicht alle Benutzenden in der Organisation haben dieselben Berechtigungen für die Verwendung von Adobe Workfront Planning. In diesem Artikel werden allgemeine Informationen zum Freigeben oder Entfernen von Berechtigungen für einen Adobe Workfront Planning-Arbeitsbereich oder eine Ansicht beschrieben.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 6%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Übersicht über Freigabeberechtigungen in Adobe Workfront Planning

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>



{{planning-important-intro}}

Sie können Berechtigungen für einen Adobe Workfront Planning-Arbeitsbereich oder eine Ansicht freigeben oder entfernen.

In diesem Artikel werden die Berechtigungsebenen für Workfront Planning-Objekte beschrieben.

## Objekte, die Sie in Adobe Workfront Planning freigeben können

Sie können die folgenden Objekte in Workfront Planning manuell freigeben:

* Arbeitsbereiche

   * Sie können Arbeitsbereiche für Personen innerhalb Ihrer Organisation freigeben.
   * Wenn Sie einen Arbeitsbereich freigeben, werden alle Datensatztypen, Datensätze und Felder, die mit den Arbeitsbereichen verknüpft sind, ebenfalls freigegeben.
   * Wenn Sie einen Arbeitsbereich freigeben, werden Ansichten nicht freigegeben. Ansichten werden separat freigegeben.

  Weitere Informationen finden Sie unter [Freigeben von Arbeitsbereichen](/help/quicksilver/planning/access/share-workspaces.md)

<!--
<div class="preview">

* Record types

    * You can share record types with people inside your organization.
    * The level of permissions granted for the workspace displays as Inherited permissions for the record type. 
    * You cannot share a record type with a higher permission level than the user has on the workspace. 

    For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>
-->

* Ansichten

   * Sie müssen Benutzenden, einschließlich Systemadministratoren, Berechtigungen für den Zugriff auf Ansichten erteilen, getrennt von ihren Berechtigungen für den Zugriff auf Arbeitsbereiche.
   * Wenn Sie eine Ansicht freigeben, werden alle Ansichtselemente freigegeben, einschließlich Filter, Gruppierung, Sortierung oder Einstellungen.
   * Wenn Sie eine Ansicht freigeben, werden die in der Ansicht sichtbaren Datensätze nicht freigegeben. Datensätze müssen durch die Freigabe von Arbeitsbereichen freigegeben werden.
   * Sie können eine Ansicht öffentlich für Personen außerhalb Ihres Unternehmens freigeben, wenn Sie einen öffentlichen Link für eine Ansicht generieren. Personen, die über einen öffentlichen Link auf die Datensatzseite zugreifen, können alle Datensätze und ihre Felder anzeigen, einschließlich der verbundenen Datensätze und Felder.

  Weitere Informationen finden Sie unter [Freigeben von Ansichten](/help/quicksilver/planning/access/share-views.md).

Intern können Sie einen Arbeitsbereich oder eine Ansicht für die folgenden Workfront-Entitäten freigeben:

* Benutzende
* Gruppen

<div class="preview">

* Teams
* Firmen
* Aufgabengebiete

</div>

<span class="preview"> Wenn Sie Arbeitsbereiche und Datensatztypen für andere freigeben, wird die Berechtigungsstufe des Datensatztyps automatisch auf die Datensätze und die mit ihnen verknüpften Felder übernommen. </span>

## Überlegungen zur Freigabe von Objekten in Adobe Workfront Planning

* Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Workfront Planning-Berechtigungen zusammen, um Ihnen Zugriff zum Anzeigen, Bereitstellen oder Verwalten von Arbeitsbereichen und deren Objekten zu gewähren.

  Informationen dazu, wie sich Lizenztypen auf Berechtigungsebenen für Workfront Planning auswirken, finden Sie [Lizenztypübersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Systemadministratoren können alle Arbeitsbereiche im System verwalten, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.
* Andere Benutzende, einschließlich Systemadministratoren, können nur auf Ansichten zugreifen, die sie erstellt haben oder die für sie freigegeben wurden. Systemadministratoren können nur Berechtigungen zum Verwalten einer Ansicht erteilen.
* Sie können einen Link zu einem Arbeitsbereich oder zu einer Ansicht für andere freigeben.

  Die folgenden Szenarien sind vorhanden:
   * Benutzer, die den Link zu einem Arbeitsbereich erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf den Arbeitsbereich zugreifen zu können.
   * Benutzende, die den Link zu einer Ansicht erhalten, können auf folgende Weise auf die Ansicht zugreifen:

      * Muss aktive Benutzende sein und sich bei Workfront anmelden, wenn der Link zur Ansicht intern freigegeben wurde.
      * Kann externe Benutzer von Workfront sein und über einen öffentlich freigegebenen Link auf die Ansicht zugreifen, ohne sich bei Workfront anzumelden.

## Freigeben von Berechtigungen für Adobe Workfront Planning-Objekte

Die Tabellen in den folgenden Abschnitten veranschaulichen die Berechtigungsebenen, die Sie beim Freigeben eines Arbeitsbereichs oder einer Ansicht auswählen können, und geben an, welche Funktionen jede Ebene zulässt.

>[!IMPORTANT]
>
>Nicht alle Benutzer können über die unten beschriebenen Berechtigungsebenen verfügen. Die individuelle Lizenz eines Benutzers bestimmt, welche Berechtigungsstufe er für Workfront Planning-Objekte erhalten kann.
>
>Nur Benutzer von Standard- (oder Plan-) Lizenzen können über die Berechtigungen Beitragen oder Verwalten für Arbeitsbereiche und Verwalten von Berechtigungen für Ansichten verfügen.
> 
>Benutzer mit allen anderen Lizenztypen können Ansichtsberechtigungen für Arbeitsbereiche und Ansichten haben.
>
>Weitere Informationen finden Sie unter [Lizenztyp - Übersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Workspace-Berechtigungen

Sie müssen Benutzern Berechtigungen für Arbeitsbereiche erteilen, damit sie Zugriff auf die folgenden Entitäten erhalten:

* Arbeitsbereiche
* Datensatztypen
* Einträge
* Felder

Im Folgenden finden Sie die Berechtigungsebenen für Arbeitsbereiche:

|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Bearbeiten | ✓ |            |       |
| Freigeben | ✓ |            |       |
| Löschen | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |

### Berechtigungen für Datensatztyp

<!--In the Production environment,--> Berechtigungen vom Typ Datensatz werden <!--always--> vererbt, wenn Sie Berechtigungen für den Arbeitsbereich erteilen.

Im Folgenden finden Sie die Berechtigungsebenen für Datensatztypen:


|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ |            |       |
| Löschen | ✓ |            |       |
| Bearbeiten | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |

<!--

<div class="preview">

In the Preview environment, you can remove the record type's inherited permissions received from the workspace. 

You can give users different permissions on the record type than they have on the workspace. However, you can never grant higher permissions for the record type than users have on the workspace. 

The following scenarios exist: 

|   Workspace permissions     | Automatic inherited permissions for a Record Type |Possible Record Type permissions when Inherited permissions are turned off (granted manually)| 
|--------|--------|-------------|
| Manage |   Manage    |   Manage, Remove permissions           | 
| Contribute |     Contribute |  Contribute, View, Remove permissions        |
| View   |  View     |      View, Remove permissions        |     

</div>

-->

### Datensatzberechtigungen

Datensatzberechtigungen werden vom (<!--<span class="preview">the record type</span>, when you grant permissions to -->) <!-- and <span class="preview">the record type</span>-->.

Im Folgenden finden Sie die Berechtigungsebenen für Datensätze:


|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ | ✓ |       |
| Löschen | ✓ | ✓ |       |
| Bearbeiten | ✓ | ✓ |       |
| Anzeigen | ✓ | ✓ | ✓ |

### Feldberechtigungen

Feldberechtigungen werden von (<!--<span class="preview">the record type</span>, when you grant permissions to --> Workspace-<!--and <span class="preview">the record type</span>--> übernommen.

Die folgenden Berechtigungen beziehen sich auf die Felder selbst und nicht auf die mit den einzelnen Feldern verknüpften Werte. Zum Bearbeiten von Feldwerten benötigen Sie Berechtigungen zum Bearbeiten von Datensätzen.

|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ |            |       |
| Löschen | ✓ |            |       |
| Bearbeiten | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |


### Berechtigungen anzeigen

Für Datensatzansichten müssen Sie separate Berechtigungen erteilen. Bei der Erteilung von Berechtigungen für den Arbeitsbereich werden keine Berechtigungen für die Datensatzansichten im Arbeitsbereich gewährt.

Sie müssen Benutzern die Berechtigung für Ansichten erteilen, damit sie Zugriff auf die folgenden Ansichtselemente haben:

* Filter
* Sichtbarkeit der Felder
* Sortieren
* Gruppierung
* Zeilenhöhe
* Einstellungen

Sie können Ansichten intern oder öffentlich austauschen.

Im Folgenden finden Sie die Berechtigungsebenen für Ansichten und Ansichtselemente:

| Interne Freigabe | Verwalten (nur eingeladene Personen können darauf zugreifen) | Anzeigen (nur eingeladene Personen können darauf zugreifen) | Alle Personen im Arbeitsbereich können* |
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

*Benutzer müssen über Ansichtsberechtigungen oder höhere Berechtigungen für einen Arbeitsbereich verfügen, um Zugriff auf diese Ansicht zu erhalten.

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