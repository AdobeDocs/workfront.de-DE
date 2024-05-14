---
title: Übersicht über Datensatztypen
description: Datensatztypen sind die Bausteine eines Arbeitsbereichs für die Adobe Workfront-Planung.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: b2ec979cf9aa2431c8c908440c227758d9dab521
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Übersicht über Datensatztypen

{{maestro-important-intro}}

Im Gegensatz zu Workfront, wo die Objekttypen vordefiniert sind, können Sie in der Adobe Workfront-Planung eigene Objekttypen erstellen. Beispielsweise sind in Workfront die Objektarten &quot;Programm&quot;, &quot;Portfolio&quot;, &quot;Projekt&quot;, &quot;Aufgabe&quot;oder &quot;Problem&quot;bereits erstellt.

Workfront-Planungs-Objekttypen werden als &quot;Datensatztypen&quot;bezeichnet und können alle Objektarten erstellen und anpassen. Datensatztypen sind die Bausteine eines Arbeitsbereichs für die Workfront-Planung. Weitere Informationen zu Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).

## Übersicht über Datentypen

In der Workfront-Planung können Sie benutzerdefinierte Datensatztypen erstellen, die den Anforderungen Ihres Unternehmens entsprechen.

* Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen, werden Datensatztypen in den folgenden Arbeitsbereich-Abschnitten erstellt:

   * [Operative Datensatztypen](#operational-record-type): Ein Datensatztyp, der strategische Pläne, Initiativen oder geplante Arbeiten darstellt. Beispielsweise können Campaign, Activity, Tactic und Opportunity betriebliche Datensatztypen sein.
   * [Taxonomien](#taxonomy): Record types, die Attribute zu einem betrieblichen Datensatztyp erfassen. So können beispielsweise Region, Adresse und Zielgruppe Taxonomien sein.

* Wenn Sie einen Datensatztyp in einem von Ihnen erstellten Arbeitsbereich erstellen, können Sie den Datensatztyp in einem beliebigen Abschnitt platzieren, den Sie im Arbeitsbereich erstellen.
* Wenn Sie einen Datensatztyp erstellen, können nur Sie und diejenigen, die Sie für den Zugriff auf den Arbeitsbereich berechtigen, den Datensatztyp anzeigen.
* Sie müssen einen Arbeitsbereich erstellen, bevor Sie Datensatztypen für den Arbeitsbereich erstellen können.
* Sie können in einem Arbeitsbereich insgesamt 1.000 Datensatztypen verwenden, unabhängig davon, wie viele Abschnitte der Arbeitsbereich umfasst. Dies umfasst Datensatztypen, die Sie von Grund auf neu erstellen oder die bei Verwendung einer Vorlage erstellt werden.


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](../architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

For more information about taxonomy record types, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->