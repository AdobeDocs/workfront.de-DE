---
title: Übersicht über Connected Records
description: Nachdem Sie Verbindungen zwischen Datensatztypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden. In diesem Artikel werden Überlegungen beschrieben, die Sie beim Verbinden von Datensätzen in der Adobe Workfront-Planung berücksichtigen müssen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Übersicht über verbundene Datensätze

<!--for the Planning connection field, see commented out below; also add preview tags-->

{{planning-important-intro}}

Sie können Adobe Workfront Planning-Datensätze miteinander oder mit Objekten aus anderen Anwendungen verbinden.

In diesem Artikel werden Überlegungen beschrieben, die Sie beim Verbinden von Datensätzen in der Adobe Workfront-Planung berücksichtigen müssen.

Informationen dazu, wie Sie Datensätze miteinander oder mit einem anderen Objekt verbinden können, finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).


## Überlegungen zum Verbinden von Datensätzen

* Nachdem Sie die Datensatztypen miteinander verbunden haben, werden die verbundenen Datensatztypen in der Tabelle der Datensatztypen, von denen sie verknüpft sind, und auf den Datensatzseiten als verknüpfte Datensatzfelder angezeigt.
* Sie können Datensätze und Objekte der verknüpften Datensätze und Objekttypen aus den verknüpften Datensatzfeldern durchsuchen und hinzufügen.
* Sie können in der Tabelle des Datensatztyps, von dem Sie die Relation herstellen, Felder (Suchfelder) der verknüpften Datensatztypen hinzufügen.

  Außerdem können Sie in der Tabelle des Datensatztyps, zu dem Sie eine Verknüpfung herstellen, Felder (Suchfelder) der Datensatztypen hinzufügen.

  Wenn Sie beispielsweise den Datensatztyp Produkt aus dem Datensatztyp von Campaign verknüpfen, können Sie Produktfelder für Kampagnen sowie Kampagnenfelder für Produkte anzeigen.
* Sie können die Werte der Suchfelder in den Datensätzen, von denen Sie eine Verknüpfung herstellen, nicht manuell aktualisieren.

  Die Werte der Suchfelder füllen den Workfront Planning-Datensatz aus, den Sie verknüpfen, nachdem sie für den ursprünglichen Datensatz oder das ursprüngliche Objekt aktualisiert wurden.

* Jeder, der Zugriff auf die Workfront-Planung und -Ansicht oder höhere Berechtigungen für den Arbeitsbereich hat, kann die Verbindungen sehen, die Sie zwischen Datensätzen oder zwischen Datensätzen und Objekten anderer Anwendungen herstellen. Sie können verbundene Datensätze und Objekte unabhängig von ihren Berechtigungen in den Anwendungen anzeigen, mit denen Sie eine Verbindung herstellen.
* Sie können die Verbindungen aller anderen Benutzer anzeigen und bearbeiten, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, in dem die verbundenen Datensätze gespeichert sind.
* Sie können einen Datensatz mit einem oder mehreren Objekten aus einer anderen Anwendung verbinden. Weitere Informationen finden Sie im Abschnitt &quot;Verbindungstypen&quot;im Artikel [Übersicht über Connected record types](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Bereiche, in denen Sie Datensätze verbinden können

In den folgenden Bereichen können Sie Datensätze mit anderen Datensätzen oder Objekten aus einer anderen Anwendung verbinden:

* Sie können Datensätze aus der Workfront-Planung mit Workfront-Objekten oder Experience Manager Assets-Objekten in den folgenden Bereichen eines Planungsdatensatzes verbinden:

   * Die verbundenen Datensatzfelder in der Tabellenansicht eines Datensatztyps in der Planung.
   * Vorschau oder Seite des Datensatzes in den verbundenen Datensatzfeldern auf der Registerkarte Details .
   * Vorschau oder Seite des Datensatzes auf der Registerkarte Verbindungen .

* In den folgenden Bereichen können Sie Workfront-Objekte mit Datensätzen in der Workfront-Planung verbinden:

   * Im Planungsabschnitt eines Workfront-Objekts.
  <!--* From a Planning connection field on a Workfront object's custom form. -->

  Weitere Informationen finden Sie unter [Verwalten von Datensatzverbindungen von Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md)