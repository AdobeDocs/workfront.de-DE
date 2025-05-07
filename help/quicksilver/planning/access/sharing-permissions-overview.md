---
title: Übersicht über Freigabeberechtigungen in Adobe Workfront Planning
description: Nicht alle Benutzenden in der Organisation haben dieselben Berechtigungen für die Verwendung von Adobe Workfront Planning. In diesem Artikel werden allgemeine Informationen zum Freigeben oder Entfernen von Berechtigungen für einen Adobe Workfront Planning-Arbeitsbereich oder eine Ansicht beschrieben.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 3550d7addcc0bb790f15d141d9470e0b75f940a6
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 5%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

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

<div class="preview">

* Datensatztypen

   * Sie können Datensatztypen für Personen in Ihrer Organisation freigeben.
   * Die Ebene der für den Arbeitsbereich gewährten Berechtigungen wird als geerbte Berechtigungen für den Datensatztyp angezeigt.
   * Sie können keinen Datensatztyp mit einer höheren Berechtigungsstufe freigeben, als der Benutzer für den Arbeitsbereich hat.

  Weitere Informationen finden Sie unter [Freigeben von Datensatztypen](/help/quicksilver/planning/access/share-record-types.md).

</div>


* Ansichten

   * Sie müssen Benutzenden, einschließlich Systemadministratoren, Berechtigungen für den Zugriff auf Ansichten erteilen, getrennt von ihren Berechtigungen für den Zugriff auf Arbeitsbereiche.
   * Wenn Sie eine Ansicht freigeben, werden alle Ansichtselemente freigegeben, einschließlich Filter, Gruppierung, Sortierung oder Einstellungen.
   * Wenn Sie eine Ansicht freigeben, werden die in der Ansicht sichtbaren Datensätze nicht freigegeben. Datensätze müssen durch die Freigabe von Arbeitsbereichen freigegeben werden.
   * Sie können eine Ansicht öffentlich für Personen außerhalb Ihres Unternehmens freigeben, wenn Sie einen öffentlichen Link für eine Ansicht generieren. Personen, die über einen öffentlichen Link auf die Datensatzseite zugreifen, können alle Datensätze und ihre Felder anzeigen, einschließlich der verbundenen Datensätze und Felder.

  Weitere Informationen finden Sie unter [Freigeben von Ansichten](/help/quicksilver/planning/access/share-views.md).

Intern können Sie einen Arbeitsbereich, eine Ansicht oder <span class="preview"> Datensatztyp-</span> für die folgenden Workfront-Entitäten freigeben:

* Benutzende
* Gruppen
* Teams
* Firmen
* Aufgabengebiete

<span class="preview"> Wenn Sie Arbeitsbereiche und Datensatztypen für andere freigeben, wird die Berechtigungsstufe des Datensatztyps automatisch auf die Datensätze und die mit ihnen verknüpften Felder übernommen. </span>

>[!IMPORTANT]
>
>Wenn die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert wurde, müssen die Benutzenden, für die Sie Planning-Objekte freigeben möchten, zum Adobe Admin Console hinzugefügt werden. Sie können Planning-Objekte nicht für Benutzende von Workfront freigeben, die nicht zum Adobe Admin Console hinzugefügt wurden.


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

In der Produktionsumgebung werden Berechtigungen vom Typ Datensatz immer vererbt, wenn Sie Berechtigungen für den Arbeitsbereich erteilen.

Im Folgenden finden Sie die Berechtigungsebenen für Datensatztypen:


|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ |            |       |
| Löschen | ✓ |            |       |
| Bearbeiten | ✓ |            |       |
| Anzeigen | ✓ | ✓ | ✓ |

<div class="preview">

In der Vorschau-Umgebung können Sie die geerbten Berechtigungen des Datensatztyps, die Sie vom Arbeitsbereich erhalten haben, entfernen.

Sie können Benutzenden für den Datensatztyp niedrigere Berechtigungen erteilen als für den Arbeitsbereich.

Folgendes können Sie jedoch nicht tun:

* Gewähren Sie höhere Berechtigungen für den Datensatztyp als Benutzer für den Arbeitsbereich.
* Erteilen Sie Workspace-Managern niedrigere Berechtigungen für einen Datensatztyp.
* Entfernen Sie Anzeigeberechtigungen für den Datensatztyp oder den Arbeitsbereich, indem Sie Benutzer aus den Berechtigungen für den Datensatztyp entfernen.

Die folgenden Szenarien sind vorhanden:

| Workspace-Berechtigungen | Automatische geerbte Berechtigungen für einen Datensatztyp | Mögliche Datensatztyp-Berechtigungen, wenn übernommene Berechtigungen deaktiviert (manuell gewährt) werden |
|--------|--------|-------------|
| Verwalten | Verwalten | Verwalten, Entfernen von Berechtigungen* |
| Mitwirken | Mitwirken | Beitragen, Anzeigen, Entfernen von Berechtigungen* |
| Anzeigen | Anzeigen | Anzeigen, Entfernen von Berechtigungen* |

>[!NOTE]
>
>*Wenn Sie Berechtigungen von einem Datensatztyp entfernen, behalten Benutzer weiterhin Anzeigeberechtigungen für den Arbeitsbereich und alle Datensatztypen bei, es sei denn, Sie entfernen deren Berechtigungen vom Arbeitsbereich.

</div>

### Datensatzberechtigungen

Datensatzberechtigungen werden vom <span class="preview">Datensatztyp) übernommen</span> wenn Sie Berechtigungen für den Arbeitsbereich und <span class="preview">den Datensatztyp) </span>.

Im Folgenden finden Sie die Berechtigungsebenen für Datensätze:


|        | Verwalten | Mitwirken | Anzeigen |
|--------|--------|------------|-------|
| Erstellen | ✓ | ✓ |       |
| Löschen | ✓ | ✓ |       |
| Bearbeiten | ✓ | ✓ |       |
| Anzeigen | ✓ | ✓ | ✓ |

### Feldberechtigungen

Feldberechtigungen werden vom <span class="preview">Datensatztyp) übernommen</span> wenn Sie Berechtigungen für den Arbeitsbereich und <span class="preview">den Datensatztyp</span> erteilen.

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
