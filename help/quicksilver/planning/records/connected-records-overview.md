---
title: Übersicht über verbundene Datensätze
description: Nachdem Sie Verbindungen zwischen Datensatztypen erstellt haben, können Sie einzelne Datensätze miteinander verbinden. In diesem Artikel werden Überlegungen beschrieben, die Sie beim Verbinden von Datensätzen in Adobe Workfront Planning berücksichtigen müssen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 98ef4a4f0a30dc90956132cb715393a29170d715
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Übersicht über verbundene Datensätze

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Sie können Adobe Workfront-Planungsdatensätze miteinander oder mit Objekten aus anderen Programmen verbinden.

In diesem Artikel werden Überlegungen beschrieben, die Sie beim Verbinden von Datensätzen in Adobe Workfront Planning berücksichtigen müssen.

Weitere Informationen zum Verbinden von Datensätzen miteinander oder mit einem anderen Objekt finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).


## Überlegungen zum Verbinden von Datensätzen

* Nachdem Sie Datensatztypen verbunden haben, werden die verbundenen Datensatztypen als verknüpfte Datensatzfelder in der Tabelle der Datensatztypen angezeigt, mit denen sie verknüpft sind, und auf den Seiten der Datensätze.
* Sie können Datensätze und Objekte der verknüpften Datensätze und Objekttypen aus den verknüpften Datensatzfeldern durchsuchen und hinzufügen.
* Sie können Felder (Lookup-Felder) der verknüpften Datensatztypen in der Tabelle des Datensatztyps hinzufügen, mit dem Sie eine Verknüpfung herstellen.

  Außerdem können Sie Felder (Suchfelder) der Datensatztypen, mit denen Sie eine Verknüpfung herstellen, in der Tabelle des Datensatztyps hinzufügen, mit dem Sie eine Verknüpfung herstellen.

  Wenn Sie beispielsweise den Datensatztyp Produkt mit dem Datensatztyp einer Kampagne verknüpfen, können Sie Produktfelder für Kampagnen sowie Kampagnenfelder für Produkte anzeigen.
* Die Werte der Suchfelder für die Datensätze, mit denen eine Verknüpfung hergestellt wird, können nicht manuell aktualisiert werden.

  Die Werte der Suchfelder werden in den Workfront-Planungsdatensatz eingegeben, aus dem Sie eine Verknüpfung herstellen, nachdem sie im ursprünglichen Datensatz oder Objekt aktualisiert wurden.

* Jeder, der Zugriff auf Workfront Planning and View oder höhere Berechtigungen für den Arbeitsbereich und einen Datensatztyp hat, kann die Verbindungen sehen, die Sie zwischen Datensätzen oder zwischen Datensätzen und Objekten anderer Anwendungen herstellen. Sie können verbundene Datensätze und Objekte unabhängig von ihren Berechtigungen in den Programmen anzeigen, mit denen Sie eine Verbindung herstellen.
* Sie können die Verbindungen aller anderen anzeigen und bearbeiten, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich und den Datensatztyp verfügen, in dem sich die verbundenen Datensätze befinden.
* Je nach Verbindungstyp, den Sie beim Verbinden der Datensatztypen ausgewählt haben, können Sie einen Datensatz mit einem oder mehreren Objekten aus einer anderen Anwendung verbinden. Weitere Informationen finden Sie im Abschnitt „Verbindungstypen“ im Artikel &quot;[&#x200B; Datensatztypen - Übersicht](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
* <span class="preview">Wenn verbundene Datensatztypen Teil von Hierarchien sind, können Sie von den Datensatzseiten aus auf jeden Objekttyp innerhalb der Hierarchie zugreifen. Weitere Informationen finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md). </span>
* <span class="preview">* Wenn verbundene Datensatztypen Teil von Hierarchien sind, können Sie einen Datensatz aus einem untergeordneten Datensatztyp mit bis zu 10 Datensätzen aus einem übergeordneten Datensatztyp verbinden. Weitere Informationen finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md). </span>

## Bereiche, in denen Datensätze verbunden werden können

In den folgenden Bereichen können Sie Datensätze mit anderen Datensätzen oder mit Objekten aus einer anderen Anwendung verbinden:

* Sie können Datensätze aus Workfront Planning in den folgenden Bereichen eines Planning-Datensatzes mit Workfront-Objekten, Experience Manager Assets-Objekten oder GenStudio Brands verbinden:

   * Die verbundenen Datensatzfelder in der Tabellenansicht eines Datensatztyps in Planning.
   * Die Vorschau oder Detailseite des Datensatzes in den verbundenen Datensatzfeldern auf der Registerkarte Details .
   * Die Vorschau- oder Detailseite des Datensatzes auf der Registerkarte Verbindungen .
   * Die Seite des Datensatzes auf der Registerkarte „Verbundene Datensatzseite“ eines verbundenen Datensatzes.

* Sie können Workfront-Objekte in den folgenden Bereichen von Workfront mit Workfront-Planungsdatensätzen verbinden:

   * Der Planungsabschnitt eines Workfront-Objekts.
   * Ein Planning-Verbindungsfeld im benutzerdefinierten Formular eines Workfront-Objekts.

  Weitere Informationen finden Sie unter [Verwalten von Datensatzverbindungen aus Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
