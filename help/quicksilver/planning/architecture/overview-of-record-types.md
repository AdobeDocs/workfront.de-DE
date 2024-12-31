---
title: Übersicht über Datensatztypen
description: Datensatztypen sind die Bausteine eines Adobe Workfront Planning Workspace.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 425c3d3afb892ac83a10bbd36efb4c7d9712c4dc
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---


# Übersicht über Datensatztypen

{{planning-important-intro}}

Im Gegensatz zu Workfront, wo die Objekttypen vordefiniert sind, können Sie in Adobe Workfront Planning Ihre eigenen Objekttypen erstellen. In Workfront werden beispielsweise die Objekttypen „Programm“, &quot;Portfolio&quot;, „Projekt“, „Aufgabe“ oder „Problem“ bereits erstellt.

Workfront Planning-Objekttypen werden als „Datensatztypen“ bezeichnet und existieren nur, wenn sie von Benutzenden erstellt werden. Datensatztypen sind die Bausteine eines Workfront Planning Workspace. Weitere Informationen zu Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

## Übersicht über den Datensatztyp

In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die den Anforderungen Ihres Unternehmens entsprechen.

Weitere Informationen zum Erstellen von Datensatztypen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

* Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen, werden Datensatztypen in den folgenden Abschnitten des Arbeitsbereichs erstellt:

   * **Operative Datensatztypen**: Datensatztypen, die strategische Pläne, Initiativen oder geplante Arbeiten darstellen. Beispielsweise sind Kampagne, Aktivität, Taktik und Opportunity operative Datensatztypen.
   * **Taxonomien**: Datensatztypen, die Attribute über einen betrieblichen Datensatztyp erfassen. Beispielsweise sind Region, Adresse und Zielgruppe Taxonomien.

* Wenn Sie einen Datensatztyp in einem Arbeitsbereich erstellen, den Sie von Grund auf neu erstellt haben, können Sie den Datensatztyp in jedem Abschnitt platzieren, den Sie im Arbeitsbereich erstellen.
* Wenn Sie einen Datensatztyp erstellen, können nur Sie und diejenigen, denen Sie Zugriff auf den Arbeitsbereich gewähren, den Datensatztyp anzeigen.
* Sie müssen einen Arbeitsbereich erstellen, bevor Sie Datensatztypen für den Arbeitsbereich erstellen können.
* Einschränkungen dazu, wie viele Datensatztypen Sie in einer Workspace- oder Workfront-Instanz haben können, finden Sie unter [Übersicht über Adobe Workfront Planning-Objektbeschränkungen](/help/quicksilver/planning/general/limitations-overview.md).


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

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
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->