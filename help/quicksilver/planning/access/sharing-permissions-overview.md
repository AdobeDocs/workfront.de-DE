---
title: Übersicht über Freigabeberechtigungen in Adobe Workfront Planning
description: Nicht alle Benutzenden in der Organisation haben dieselben Berechtigungen für die Verwendung von Adobe Workfront Planning. In diesem Artikel werden allgemeine Informationen zum Freigeben oder Entfernen von Berechtigungen für einen Adobe Workfront Planning-Arbeitsbereich oder eine Ansicht beschrieben.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 5%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Übersicht über Freigabeberechtigungen in Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

Sie können Berechtigungen für einen Adobe Workfront Planning-Arbeitsbereich, einen Datensatztyp oder eine Ansicht freigeben oder entfernen.

Sie können auch Planungsanfrageformulare freigeben. Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

In diesem Artikel werden die Berechtigungsebenen für Workfront Planning-Arbeitsbereiche, Datensatztypen, Datensätze, Felder und Ansichten beschrieben.

## Objekte, die Sie in Adobe Workfront Planning freigeben können

Einige Workfront Planning-Objekte können manuell freigegeben werden, während andere Objekte diese Berechtigungen von anderen Objekten erben.

Sie können die folgenden Objekte in Workfront Planning manuell freigeben:

* Arbeitsbereiche

   * Sie können Arbeitsbereiche für Personen innerhalb Ihrer Organisation freigeben.
   * Wenn Sie einen Arbeitsbereich freigeben, werden alle Datensatztypen, Datensätze und Felder, die mit den Arbeitsbereichen verknüpft sind, ebenfalls freigegeben.
   * Wenn Sie einen Arbeitsbereich freigeben, werden Ansichten nicht freigegeben. Ansichten werden separat freigegeben.

  Weitere Informationen finden Sie unter [Freigeben von Arbeitsbereichen](/help/quicksilver/planning/access/share-workspaces.md)

* Eintragstypen

   * Sie können Datensatztypen für Personen in Ihrer Organisation freigeben.
   * Die Ebene der für den Arbeitsbereich gewährten Berechtigungen wird als geerbte Berechtigungen für den Datensatztyp angezeigt.
   * Sie können keinen Datensatztyp mit einer höheren Berechtigungsstufe freigeben, als der Benutzer für den Arbeitsbereich hat.

  Weitere Informationen finden Sie unter [Freigeben von Datensatztypen](/help/quicksilver/planning/access/share-record-types.md).


* Ansichten 

   * Sie müssen Benutzenden, einschließlich Systemadministratoren, Berechtigungen für den Zugriff auf Ansichten erteilen, getrennt von ihren Berechtigungen für den Zugriff auf Arbeitsbereiche.
   * Wenn Sie eine Ansicht freigeben, werden alle Ansichtselemente freigegeben, einschließlich Filter, Gruppierung, Sortierung oder Einstellungen.
   * Wenn Sie eine Ansicht freigeben, werden die in der Ansicht sichtbaren Datensätze nicht freigegeben. Datensätze müssen durch die Freigabe von Arbeitsbereichen freigegeben werden.
   * Sie können eine Ansicht öffentlich für Personen außerhalb Ihres Unternehmens freigeben, wenn Sie einen öffentlichen Link für eine Ansicht generieren. Personen, die über einen öffentlichen Link auf die Datensatzseite zugreifen, können alle Datensätze und ihre Felder anzeigen, einschließlich der verbundenen Datensätze und Felder.

  Weitere Informationen finden Sie unter [Freigeben von Ansichten](/help/quicksilver/planning/access/share-views.md).

## Überlegungen zur Freigabe von Objekten in Adobe Workfront Planning

* Ihr Adobe Workfront-Lizenztyp arbeitet mit Ihren Workfront Planning-Berechtigungen zusammen, um Ihnen Zugriff zum Anzeigen, Bereitstellen oder Verwalten von Arbeitsbereichen und deren Objekten zu gewähren.

  Informationen dazu, wie sich Lizenztypen auf Berechtigungsebenen für Workfront Planning auswirken, finden Sie [Lizenztypübersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Systemadministratoren können alle Arbeitsbereiche im System verwalten, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben.
* Andere Benutzende, einschließlich Systemadministratoren, können nur auf Ansichten zugreifen, die sie erstellt haben oder die für sie freigegeben wurden. Systemadministratoren können nur Berechtigungen zum Verwalten einer Ansicht erteilen.

* Wenn Sie Arbeitsbereiche und Datensatztypen für andere freigeben, wird die Berechtigungsstufe des Datensatztyps automatisch auf die Datensätze und die mit ihnen verknüpften Felder übernommen.

  >[!IMPORTANT]
  >
  >Wenn die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert wurde, müssen die Benutzenden, für die Sie Planning-Objekte freigeben möchten, zum Adobe Admin Console hinzugefügt werden. Sie können Planning-Objekte nicht für Benutzende von Workfront freigeben, die nicht zum Adobe Admin Console hinzugefügt wurden.

* Sie können Planning-Objekte wie folgt freigeben:

   * Intern können Sie einen Arbeitsbereich, eine Ansicht oder einen Datensatztyp für die folgenden Workfront-Entitäten freigeben:

      * Benutzende
      * Gruppen
      * Teams
      * Firmen
      * Aufgabengebiete

     Sie können ein Planning-Objekt für bis zu 100 Entitäten pro Objekt freigeben.

   * Intern durch die Freigabe eines Links zu einem Arbeitsbereich oder einer Ansicht mit anderen Planning-Benutzern. Die folgenden Szenarien sind vorhanden:

      * Benutzer, die den Link zu einem Arbeitsbereich erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf den Arbeitsbereich zuzugreifen.
      * Benutzende, die einen internen Freigabelink für eine Ansicht erhalten, müssen aktive Benutzende sein und sich bei Workfront anmelden, um auf die Ansicht zuzugreifen.
   * Extern durch Freigeben eines öffentlichen Freigabe-Links zu einer Ansicht für externe Benutzer, die kein Workfront-Konto haben.

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


### Berechtigungen für Arbeitsbereiche

Sie müssen Benutzern Berechtigungen für Arbeitsbereiche erteilen, damit sie Zugriff auf die folgenden Entitäten erhalten:

* Arbeitsbereiche
* Eintragstypen
* Einträge
* Felder

Im Folgenden finden Sie die Berechtigungsebenen für Arbeitsbereiche:

|        | Verwalten | Mitwirken | Ansicht |
|--------|--------|------------|-------|
| Bearbeiten | ✓ |            |       |
| Freigeben | ✓ |            |       |
| Löschen | ✓ |            |       |
| Ansicht | ✓ | ✓ | ✓ |

### Berechtigungen für Datensatztypen

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

Berechtigungen vom Typ „Datensatz“ werden immer vererbt, wenn Sie Berechtigungen für den Arbeitsbereich erteilen.

Sie können die geerbten Berechtigungen des Datensatztyps, die Sie vom Arbeitsbereich erhalten haben, entfernen.

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
| Ansicht | Ansicht | Anzeigen, Entfernen von Berechtigungen* |

>[!NOTE]
>
>Wenn Sie Berechtigungen von einem Datensatztyp entfernen, behalten Benutzer weiterhin Anzeigeberechtigungen für den Arbeitsbereich und alle Datensatztypen bei, es sei denn, Sie entfernen deren Berechtigungen vom Arbeitsbereich.

### Berechtigungen für Datensätze

Datensatzberechtigungen werden vom Datensatztyp übernommen, wenn Sie Berechtigungen für den Arbeitsbereich und den Datensatztyp gewähren.

Im Folgenden finden Sie die Berechtigungsebenen für Datensätze:


|        | Verwalten | Mitwirken | Ansicht |
|--------|--------|------------|-------|
| Erstellen | ✓ | ✓ |       |
| Löschen | ✓ | ✓ |       |
| Bearbeiten | ✓ | ✓ |       |
| Ansicht | ✓ | ✓ | ✓ |

### Berechtigungen zum Aufzeichnen von Feldern

Feldberechtigungen werden vom Datensatztyp übernommen, wenn Sie Berechtigungen für den Arbeitsbereich und den Datensatztyp gewähren.

Die folgenden Berechtigungen beziehen sich auf die Felder selbst und nicht auf die mit den einzelnen Feldern verknüpften Werte. Zum Bearbeiten von Feldwerten benötigen Sie Berechtigungen zum Bearbeiten von Datensätzen.

|        | Verwalten | Mitwirken | Ansicht |
|--------|--------|------------|-------|
| Erstellen | ✓ |            |       |
| Löschen | ✓ |            |       |
| Bearbeiten | ✓ |            |       |
| Ansicht | ✓ | ✓ | ✓ |


### Berechtigungen für Ansichten

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
| Ansicht | ✓ | ✓ | ✓ |
| Anwenden | ✓ | ✓ | ✓ |

| Öffentliche Freigabe | Ansicht |
|--------|-------|
| Ansicht | ✓ |
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
