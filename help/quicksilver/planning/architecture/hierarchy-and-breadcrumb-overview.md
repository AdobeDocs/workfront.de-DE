---
title: Übersicht über Hierarchie und Breadcrumb
description: Sie können mehrere Workspace-Hierarchien zwischen den Datensatztypen in einem Workspace erstellen, nachdem Sie die Datensatztypen verbunden haben.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 98ef4a4f0a30dc90956132cb715393a29170d715
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---



# Übersicht über Hierarchie und Breadcrumb

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Als Workspace-Manager können Sie in Adobe Workfront Planning flexible, aber strukturierte Hierarchien zwischen verbundenen Datensatztypen und anderen Objekttypen definieren.

Hierarchien sind Verbindungen zwischen Datensatztypen oder zwischen Datensatztypen und einem Workfront-Projekt.

Weitere Informationen zum Erstellen von Hierarchien finden Sie unter [Erstellen von Workspace-Hierarchien](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).

Die Verwendung von Hierarchien in Ihren Arbeitsbereichen bietet folgende Vorteile:

* Um die Arbeit so zu organisieren, dass sie widergespiegelt wird, wie Ihre Teams tatsächlich planen, arbeiten und Ergebnisse liefern.
* Damit Benutzer verstehen können, wo sie sich befinden, wie Datensatztypen miteinander verbunden sind und wie die Strategie in die Ausführung einfließt, indem auf eine Reihe von Breadcrumbs verwiesen wird, die ihren Platz im System angeben.
* Für eine bessere Navigation und für mehr Klarheit und Kontinuität in allen Workflows.
* Um Flüsse zu definieren, die zur Funktionsweise Ihres Unternehmens passen, und so Flexibilität und Konsistenz über alle Arbeitsphasen hinweg zu unterstützen.

## Überlegungen beim Arbeiten mit Hierarchien

* Sie können bis zu 5 Hierarchien für einen Arbeitsbereich erstellen.
* Es können bis zu 4 Datensatz- und Objekttypen in einer Hierarchie verbunden sein.
* Sie können in einer Workspace-Hierarchie nur die folgenden Objekttypen verbinden:
   * Datensatztypen, die zu dem Arbeitsbereich gehören, in dem Sie die Hierarchien erstellen.
   * Workfront-Projekte. Workfront-Projekte können nicht als übergeordnete Elemente anderer Datensatztypen hinzugefügt werden. Sie sind immer der letzte Objekttyp in einer Hierarchie.
* Die folgenden Objekttypen können nicht in einer Hierarchie hinzugefügt werden:
   * Datensatztypen aus anderen Arbeitsbereichen, auch wenn sie als verbindbare oder globale Datensatztypen festgelegt sind. Sie können globale Datensatztypen nur dann zu Hierarchien hinzufügen, wenn sie zu dem Arbeitsbereich hinzugefügt wurden, aus dem Sie die Hierarchie erstellen.
   * Alle anderen Workfront-Objekte.
   * AEM Assets.
* Hierarchien können sowohl Planning-Datensatztypen als auch Workfront-Projekte gleichzeitig enthalten.

  Sie können beispielsweise einen Kampagnen-Datensatztyp mit Planungstaktiken und Workfront-Projekten als untergeordnete Elemente in derselben Workspace-Hierarchie verwenden.

* Wenn bereits eine Verbindung zwischen den ausgewählten Datensatztypen besteht, verwendet das System die vorhandene Verbindung erneut.
* Wenn keine Verbindung vorhanden ist, erstellt Workfront im Rahmen der Hierarchieeinrichtung eine.
* Die Einstellung **Entsprechendes Feld für verknüpften Datensatztyp erstellen** muss für das verbundene Feld für Datensätze und Objekttypen aktiviert sein, die Sie in eine Hierarchie einbeziehen möchten.
* Sie können einen Datensatztyp nicht löschen, wenn er Teil einer Hierarchie ist.
* Sie können ein Verbindungsfeld nicht löschen, wenn der in dem Feld referenzierte Datensatztyp Teil einer Hierarchie ist. Sie müssen zunächst den Datensatztyp aus der Hierarchie entfernen oder die Hierarchie löschen, bevor Sie den Datensatztyp löschen können.
* Sie können ein Suchfeld aus einem verbundenen Datensatztyp löschen. Die Informationen im Feld können nicht wiederhergestellt werden.
* Im Folgenden finden Sie Regeln für die Einrichtung von Hierarchien:
   * Ein Datensatztyp kann in einem Arbeitsbereich nur einen übergeordneten Datensatztyp haben.

     Beispielsweise kann ein taktischer Datensatztyp nicht sowohl einen Campaign- als auch einen Target-Datensatztyp als übergeordnetes Element im selben Arbeitsbereich haben.
   * Ein Datensatztyp kann in mehreren Hierarchien das übergeordnete Element sein.

     Sie können beispielsweise drei verschiedene Hierarchien in einem Arbeitsbereich haben, und jede davon kann Kampagnen als übergeordneten Datensatztyp haben.
   * Ein Datensatz kann mit mehreren übergeordneten Datensätzen desselben Typs verbunden werden, wenn Sie einen mit vielen oder viele mit vielen Datensatztypen verbinden.

     Beispielsweise kann Taktik A sowohl zu Campaign X als auch zu Campaign Y gehören.
   * Ein Datensatztyp kann jeweils nur mit einem untergeordneten Datensatztyp verbunden werden. Ein untergeordneter Datensatztyp kann auch ein übergeordneter Datensatz für einen anderen Datensatztyp sein.

     Ein Campaign-Datensatztyp kann beispielsweise nur einem anderen Datensatztyp in derselben Hierarchie (Taktik) übergeordnet sein. Taktiken können wiederum den Programmen übergeordnet sein, die den Projekten übergeordnet sein können.
   * Ein Datensatztyp kann nicht das übergeordnete Element in einer Hierarchie und das untergeordnete Element in einer anderen Hierarchie im selben Arbeitsbereich sein.
   * Globale Datensatztypen können in mehreren Arbeitsbereichen innerhalb mehrerer Hierarchien angezeigt werden, nachdem sie diesen Arbeitsbereichen hinzugefügt wurden.

     Wenn eine Kampagne beispielsweise ein globaler Datensatztyp und Teil einer Hierarchie in Workspace 1 ist, kann sie als bestehender Datensatztyp zu Workspace 2 hinzugefügt und dort Teil einer Hierarchie sein. Sie kann jedoch nur dann Teil einer Hierarchie in Workspace 2 sein, wenn sie in Workspace 1 als globaler Datensatztyp angegeben, aber nicht zu Workspace 2 hinzugefügt wird.
   * Wenn verbundene Datensatztypen Teil von Hierarchien sind, können Sie einen Datensatz aus einem untergeordneten Datensatztyp mit bis zu 10 Datensätzen aus einem übergeordneten Datensatztyp verbinden.

     Wenn Sie beispielsweise eine Hierarchie zwischen Kampagnen als übergeordnetem Element und Persona als untergeordnetem Datensatz erstellen, können Sie dieselbe Persona mit bis zu 10 Kampagnen verbinden.

## Überlegungen beim Anzeigen von Breadcrumbs

Wenn Sie Hierarchien zwischen Datensatztypen erstellen, generieren diese Breadcrumbs für Datensätze, die zu diesen Datensatztypen gehören.

Wenn Sie beispielsweise eine Hierarchie erstellen und Kampagnen mit Taktiken, dann mit Aktivitäten und schließlich mit Projekten verbinden und zu einem Datensatz eines der in der Hierarchie verbundenen Typen navigieren, können Sie sehen, wo in der Hierarchie der Datensatz platziert wird.

![Breadcrumb](assets/breadcrumbs-on-project.png)

Beachten Sie Folgendes:

* Wenn ein Datensatztyp Teil mehrerer Hierarchien ist, können Sie über den Breadcrumb des Datensatzes auf der Datensatzseite zwischen Hierarchien wechseln.
* Wenn der Datensatztyp in einer Hierarchie über mehrere Datensätze verfügt, können Sie Datensätze aus dem Breadcrumb auswählen.
* Breadcrumbs funktionieren in Workfront und Planning.

  Wenn Sie sich beispielsweise ein Projekt ansehen, das mit Planungskampagnen und -taktiken sowie mit Workfront-Portfolios und -Programmen verbunden ist, können Sie aus dem Breadcrumb zwischen den Objekttypen Planning und Workfront wechseln.

  Weitere Informationen finden Sie unter [Erstellen von Workspace-Hierarchien](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* Wenn Sie einen Datensatz bearbeiten, sind die Änderungen in allen Arbeitsbereichen und Hierarchien sichtbar, zu denen der Datensatz gehört.


