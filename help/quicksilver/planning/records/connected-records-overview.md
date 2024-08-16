---
title: Übersicht über Connected Records
description: Nachdem Sie Verbindungen zwischen Datensatztypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden. In diesem Artikel werden Überlegungen beschrieben, die Sie beim Verbinden von Datensätzen in der Adobe Workfront-Planung berücksichtigen müssen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d56a4721353f8b7db856eab5a3ae3b53396bd079
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


<!--update metadata at GA-->

# Übersicht über verbundene Datensätze

{{planning-important-intro}}

Sie können Adobe Workfront Planning-Datensätze miteinander oder mit Objekten aus anderen Anwendungen verbinden.

In diesem Artikel werden Überlegungen beschrieben, die Sie beim Verbinden von Datensätzen in der Adobe Workfront-Planung berücksichtigen müssen.

Informationen dazu, wie Sie Datensätze miteinander oder mit einem anderen Objekt verbinden können, finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).


## Überlegungen zum Verbinden von Datensätzen

* Nachdem Sie die Datensatztypen miteinander verbunden haben, werden die verbundenen Datensatztypen in der Tabelle der Datensatztypen, von denen sie verknüpft sind, und auf den Datensatzseiten als verknüpfte Datensatzfelder angezeigt.
* Sie können Datensätze und Objekte der verknüpften Datensätze und Objekttypen aus den verknüpften Datensatzfeldern durchsuchen und hinzufügen.
* Sie können in der Tabelle des Datensatztyps, von dem Sie die Relation herstellen, Felder (Suchfelder) der verknüpften Datensatztypen hinzufügen.

  Sie können in der Tabelle des Datensatztyps, zu dem Sie die Relation herstellen, Felder (Suchfelder) der Datensatztypen hinzufügen.

  Wenn Sie beispielsweise den Datensatztyp Produkt aus dem Datensatztyp von Campaign verknüpfen, können Sie Produktfelder für Kampagnen sowie Kampagnenfelder für Produkte anzeigen.
* Sie können die Werte der Suchfelder in den Datensätzen, von denen Sie eine Verknüpfung herstellen, nicht manuell aktualisieren.

  Die Werte der Suchfelder füllen den Workfront Planning-Datensatz aus, den Sie verknüpfen, nachdem sie für den ursprünglichen Datensatz oder das ursprüngliche Objekt aktualisiert wurden.

* Jeder, der Zugriff auf die Workfront-Planung und -Ansicht oder höhere Berechtigungen für den Arbeitsbereich hat, kann die Verbindungen sehen, die Sie zwischen Datensätzen oder zwischen Datensätzen und Objekten anderer Anwendungen herstellen. Sie können verbundene Datensätze und Objekte unabhängig von ihren Berechtigungen in den Anwendungen anzeigen, mit denen Sie eine Verbindung herstellen.
* Sie können die Verbindungen aller anderen Benutzer anzeigen und bearbeiten, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, in dem die verbundenen Datensätze gespeichert sind.
* Sie können einen Datensatz mit einem oder mehreren Objekten aus einer anderen Anwendung verbinden. <!--For more information, see the "Connections types" section in the article [Connected record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md). -->

## Bereiche, in denen Sie Datensätze verbinden können

In den folgenden Bereichen können Sie Datensätze mit anderen Datensätzen oder Objekten aus einer anderen Anwendung verbinden:

* Sie können Datensätze aus der Workfront-Planung mit Workfront-Objekten in den folgenden Bereichen verbinden:
   * Aus einem Planungsdatensatz in der Workfront-Planung in den verbundenen Feldern in der Tabellenansicht.
   * Aus einem Planungsdatensatz in der Workfront-Planung in der Datensatzvorschau oder auf der Seite in den verbundenen Datensatzfeldern.
  <!--
  * From a Planning record in Workfront Planning in the record preview or page in the connected record fields on the Details tab.
  * From a Planning record in the record's preview or page on the Connections tab.  -->

* In den folgenden Bereichen können Sie Workfront-Planungsdatensätze mit Experience Manager Assets verbinden:

   * Aus einem Planungsdatensatz in der Workfront-Planung in der Tabellenansicht.
  <!--* From a Planning record in the Connections tab on the record's preview or page.  -->

* In den folgenden Bereichen können Sie Workfront-Objekte mit Datensätzen in der Workfront-Planung verbinden:

   * Im Planungsabschnitt eines Workfront-Objekts.

