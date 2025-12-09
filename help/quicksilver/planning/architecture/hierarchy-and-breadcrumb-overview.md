---
title: Übersicht über Hierarchie und Breadcrumb
description: Sie können mehrere Workspace-Hierarchien zwischen den Datensatztypen in einem Workspace erstellen.
hide: true
hidefromtoc: true
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '612'
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

Hierarchien sind Verbindungen zwischen Datensatztypen. Es können bis zu 4 Datensatz- und Objekttypen in einer Hierarchie verbunden sein.

Weitere Informationen zum Erstellen von Hierarchien finden Sie unter [Erstellen von Workspace-Hierarchien](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Die Verwendung von Hierarchien in Ihren Arbeitsbereichen bietet folgende Vorteile:

* Um die Arbeit so zu organisieren, dass sie widergespiegelt wird, wie Ihre Teams tatsächlich planen, arbeiten und Ergebnisse liefern.
* Damit Benutzer verstehen können, wo sie sich befinden, wie Datensatztypen miteinander verbunden sind und wie die Strategie in die Ausführung einfließt, indem auf eine Reihe von Breadcrumbs verwiesen wird, die ihren Platz im System angeben.
* Für eine bessere Navigation und für mehr Klarheit und Kontinuität in allen Workflows.
* Um Flüsse zu definieren, die zur Funktionsweise Ihres Unternehmens passen, und so Flexibilität und Konsistenz über alle Arbeitsphasen hinweg zu unterstützen.

## Überlegungen beim Arbeiten mit Hierarchien

* Als Workspace-Manager können Sie mehrere Hierarchien für einen Workspace erstellen.
* Wenn bereits eine Verbindung zwischen den ausgewählten Datensatztypen besteht, verwendet das System die vorhandene Verbindung erneut.
* Wenn keine Verbindung vorhanden ist, erstellt Workfront automatisch eine Verbindung im Rahmen der Hierarchieeinrichtung.
* Im Folgenden finden Sie Regeln für die Einrichtung von Hierarchien:
   * Ein Datensatztyp kann in einem Arbeitsbereich nur einen übergeordneten Datensatztyp haben.

     Beispielsweise kann ein taktischer Datensatztyp nicht sowohl einen Campaign- als auch einen Target-Datensatztyp als übergeordnetes Element im selben Arbeitsbereich haben.
   * Ein Datensatz kann mit mehreren übergeordneten Datensätzen desselben Typs verbunden werden, wenn Sie einen mit vielen oder viele mit vielen Datensatztypen verbinden.
Beispielsweise kann Taktik A sowohl zu Campaign X als auch zu Campaign Y gehören.
   * Ein Datensatztyp kann eine Verbindung zu mehreren untergeordneten Datensatztypen herstellen.

     Ein Campaign-Datensatztyp kann beispielsweise mehreren anderen Datensatztypen übergeordnet sein, z. B. Taktiken, Tests und anderen Datensatztypen.
   * Hierarchien können sowohl Planning-Datensatztypen als auch Workfront-Objekttypen enthalten.

     Sie können beispielsweise einen Kampagnen-Datensatztyp mit Planungstaktiken und Workfront-Projekten als untergeordnete Elemente verwenden.

     <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
   * Globale Datensatztypen können in mehreren Arbeitsbereichen innerhalb mehrerer Hierarchien angezeigt werden. <!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
   * Workfront-Objekttypen können auch in mehreren Hierarchien und über verschiedene Arbeitsbereiche hinweg angezeigt werden.
   * Globale Datensatztypen können nicht Teil von Hierarchien in verschiedenen Arbeitsbereichen sein.

     Wenn eine Kampagne beispielsweise ein globaler Datensatztyp und Teil einer Hierarchie in Workspace 1 ist, kann sie als bestehender Datensatztyp zu Workspace 2 hinzugefügt werden, dort jedoch nicht Teil einer Hierarchie sein. <!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
   * Die Datensatztypen mit Verbindungen, die kein entsprechendes Feld in ihren verknüpften Datensatztypen erstellen, können auch Teil von Hierarchien sein. Bei neuen Verbindungen, die bei der Einrichtung der Hierarchie erstellt werden, wird standardmäßig immer ein entsprechendes Feld für die verknüpften Datensatztypen erstellt.

## Überlegungen beim Anzeigen von Breadcrumbs

Wenn Sie Hierarchien zwischen Datensatztypen erstellen, generieren diese Breadcrumbs für Datensätze, die zu diesen Datensatztypen gehören.

Wenn Sie beispielsweise eine Hierarchie erstellen und Kampagnen mit Taktiken mit Programmen und dann mit Projekten verbinden und zu einem Datensatz eines der in der Hierarchie verbundenen Typen navigieren, können Sie anzeigen, wo in der Hierarchie der Datensatz platziert wird.

Beachten Sie Folgendes:

* Wenn ein Datensatztyp Teil mehrerer Hierarchien in mehreren Arbeitsbereichen ist, können Sie über den Breadcrumb des Datensatzes auf der Datensatzseite zwischen Hierarchien wechseln.
* Breadcrumbs funktionieren in Workfront und Planning.

  Wenn Sie sich beispielsweise ein Projekt ansehen, das mit Planungskampagnen und -taktiken sowie mit Workfront-Portfolios und -Programmen verbunden ist, können Sie über den Breadcrumb zwischen der Planning- und der Workfront-Hierarchie wechseln.

  Weitere Informationen finden Sie unter [Erstellen von Workspace-Hierarchien](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


