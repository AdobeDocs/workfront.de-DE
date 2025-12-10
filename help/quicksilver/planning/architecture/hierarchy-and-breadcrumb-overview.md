---
title: Übersicht über Hierarchie und Breadcrumb
description: Sie können mehrere Workspace-Hierarchien zwischen den Datensatztypen in einem Workspace erstellen.
hide: true
hidefromtoc: true
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Übersicht über Hierarchie und Breadcrumb

Als Workspace-Manager können Sie in Adobe Workfront Planning flexible, aber strukturierte Hierarchien zwischen Datensatztypen und anderen Objekttypen definieren.

Hierarchien sind Verbindungen zwischen Datensatztypen oder zwischen Datensatztypen und einem Workfront-Projekt.

Weitere Informationen zum Erstellen von Hierarchien finden Sie unter [Erstellen von Workspace-Hierarchien](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Die Verwendung von Hierarchien in Ihren Arbeitsbereichen bietet folgende Vorteile:

* Um die Arbeit so zu organisieren, dass sie widergespiegelt wird, wie Ihre Teams tatsächlich planen, arbeiten und Ergebnisse liefern.
* Damit Benutzer verstehen können, wo sie sich befinden, wie Datensatztypen miteinander verbunden sind und wie die Strategie in die Ausführung einfließt, indem auf eine Reihe von Breadcrumbs verwiesen wird, die ihren Platz im System angeben.
* Für eine bessere Navigation und für mehr Klarheit und Kontinuität in allen Workflows.
* Um Flüsse zu definieren, die zur Funktionsweise Ihres Unternehmens passen, und so Flexibilität und Konsistenz über alle Arbeitsphasen hinweg zu unterstützen.

## Überlegungen beim Arbeiten mit Hierarchien

* Sie können mehrere Hierarchien für einen Arbeitsbereich erstellen.
* Es können bis zu 4 Datensatz- und Objekttypen in einer Hierarchie verbunden sein.
* Sie können in einer Workspace-Hierarchie nur die folgenden Objekttypen verbinden:
   * Datensatztypen, die zu dem Arbeitsbereich gehören, in dem Sie die Hierarchien erstellen.
   * Workfront-Projekte.
* Die folgenden Objekttypen können nicht in einer Hierarchie hinzugefügt werden:
   * Datensatztypen aus anderen Arbeitsbereichen, auch wenn sie als verbindbare oder globale Datensatztypen festgelegt sind.
   * Alle anderen Workfront-Objekte.
   * AEM Assets
* Hierarchien können sowohl Planning-Datensatztypen als auch Workfront-Objekttypen gleichzeitig enthalten.

      Sie können beispielsweise einen Campaign-Datensatztyp mit Planungstaktiken und Workfront-Projekten als untergeordnete Elemente in derselben Workspace-Hierarchie verwenden.
  * Wenn bereits eine Verbindung zwischen den ausgewählten Datensatztypen besteht, verwendet das System die vorhandene Verbindung erneut.
* Wenn keine Verbindung vorhanden ist, erstellt Workfront im Rahmen der Hierarchieeinrichtung eine.
* Die Einstellung **Entsprechendes Feld für verknüpften Datensatztyp erstellen** muss für das verbundene Feld aktiviert sein.

  Die Datensatztypen mit Verbindungen, die kein entsprechendes Feld für die verknüpften Datensatztypen erstellen, können ebenfalls Teil von Hierarchien sein. Wenn Sie jedoch während der Einrichtung der Hierarchie eine neue Verbindung erstellen, müssen Sie immer ein entsprechendes Feld für den verknüpften Datensatztyp erstellen.
* Im Folgenden finden Sie Regeln für die Einrichtung von Hierarchien:
   * Ein Datensatztyp kann in einem Arbeitsbereich nur einen übergeordneten Datensatztyp haben.

     Beispielsweise kann ein taktischer Datensatztyp nicht sowohl einen Campaign- als auch einen Target-Datensatztyp als übergeordnetes Element im selben Arbeitsbereich haben.
   * Ein Datensatztyp kann in mehreren Hierarchien das übergeordnete Element sein.

     Sie können beispielsweise drei verschiedene Hierarchien in einem Arbeitsbereich haben, und jede davon kann Kampagnen als übergeordneten Datensatztyp haben.
   * Ein Datensatz kann mit mehreren übergeordneten Datensätzen desselben Typs verbunden werden, wenn Sie einen mit vielen oder viele mit vielen Datensatztypen verbinden.
Beispielsweise kann Taktik A sowohl zu Campaign X als auch zu Campaign Y gehören.
   * Ein Datensatztyp kann eine Verbindung zu mehreren untergeordneten Datensatztypen herstellen.

     Ein Campaign-Datensatztyp kann beispielsweise mehreren anderen Datensatztypen übergeordnet sein, z. B. Taktiken, Tests und anderen Datensatztypen.
   * Globale Datensatztypen können in mehreren Arbeitsbereichen innerhalb mehrerer Hierarchien angezeigt werden, nachdem sie diesen Arbeitsbereichen hinzugefügt wurden.

     Wenn eine Kampagne beispielsweise ein globaler Datensatztyp und Teil einer Hierarchie in Workspace 1 ist, kann sie als bestehender Datensatztyp zu Workspace 2 hinzugefügt und dort Teil einer Hierarchie sein. Sie kann jedoch nur dann Teil einer Hierarchie in Workspace 2 sein, wenn sie in Workspace 1 als globaler Datensatztyp angegeben, aber nicht zu Workspace 2 hinzugefügt wird.


## Überlegungen beim Anzeigen von Breadcrumbs

Wenn Sie Hierarchien zwischen Datensatztypen erstellen, generieren diese Breadcrumbs für Datensätze, die zu diesen Datensatztypen gehören.

Wenn Sie beispielsweise eine Hierarchie erstellen und Kampagnen mit Taktiken, dann mit Programmen und schließlich mit Projekten verbinden und zu einem Datensatz eines der in der Hierarchie verbundenen Typen navigieren, können Sie anzeigen, wo in der Hierarchie der Datensatz platziert wird.

Beachten Sie Folgendes:

* Wenn ein Datensatztyp Teil mehrerer Hierarchien ist, können Sie über den Breadcrumb des Datensatzes auf der Datensatzseite zwischen Hierarchien wechseln.
* Breadcrumbs funktionieren in Workfront und Planning.

  Wenn Sie sich beispielsweise ein Projekt ansehen, das mit Planungskampagnen und -taktiken sowie mit Workfront-Portfolios und -Programmen verbunden ist, können Sie aus dem Breadcrumb zwischen den Objekttypen Planning und Workfront wechseln.

  Weitere Informationen finden Sie unter [Erstellen von Workspace-Hierarchien](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


