---
title: Übersicht über Hierarchie und Breadcrumb
description: Sie können mehrere Workspace-Hierarchien zwischen den Datensatztypen in einem Workspace erstellen.
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
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

Die Verwendung von Hierarchien in Ihren Arbeitsbereichen bietet folgende Vorteile:

* Um die Arbeit so zu organisieren, dass sie widergespiegelt wird, wie Ihre Teams tatsächlich planen, arbeiten und Ergebnisse liefern.
* Benutzer verstehen, wo sie sich befinden, wie Datensatztypen miteinander verbunden sind und wie die Strategie in die Ausführung einfließt, indem sie auf eine Reihe von Breadcrumbs verweisen, die ihren Platz im System angeben.
* Bieten Sie eine bessere Navigation und schaffen Sie Klarheit und Kontinuität in allen Workflows.
* Hierarchien erzwingen keine starre, systemdefinierte Struktur und ermöglichen es Ihnen stattdessen, Flüsse zu definieren, die der Funktionsweise Ihres Unternehmens entsprechen und sowohl Flexibilität als auch Konsistenz über alle Arbeitsschritte hinweg unterstützen.

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
   * Globale Datensatztypen können in mehreren Arbeitsbereichen innerhalb mehrerer Hierarchien angezeigt werden.
   * Workfront-Objekttypen können auch in mehreren Hierarchien und über verschiedene Arbeitsbereiche hinweg angezeigt werden.
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * Die Datensatztypen mit Verbindungen, die kein entsprechendes Feld in ihren verknüpften Datensatztypen erstellen, können auch Teil von Hierarchien sein. Bei neuen Verbindungen, die bei der Einrichtung der Hierarchie erstellt werden, wird standardmäßig immer ein entsprechendes Feld für die verknüpften Datensatztypen erstellt.

## Überlegungen beim Anzeigen von Breadcrumbs


