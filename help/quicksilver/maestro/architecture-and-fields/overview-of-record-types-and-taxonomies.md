---
title: Übersicht über Datensatztypen und Taxonomien
description: Datensatztypen sind die Bausteine eines Maestro-Arbeitsbereichs.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Übersicht über Datensatztypen und Taxonomien

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Im Gegensatz zu Workfront, wo die Objekttypen vordefiniert sind, können Sie in Adobe Maestro eigene Objekttypen erstellen. Beispielsweise sind in Workfront die Objektarten &quot;Programm&quot;, &quot;Portfolio&quot;, &quot;Projekt&quot;, &quot;Aufgabe&quot;oder &quot;Problem&quot;bereits erstellt.

Maestro-Objekttypen werden als &quot;Datensatztypen&quot;bezeichnet. Datensatztypen sind die Bausteine eines Maestro-Arbeitsbereichs. Weitere Informationen zu Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture-and-fields/create-workspaces.md).

## Übersicht über Datentypen

In Maestro können Sie benutzerdefinierte Datensatztypen erstellen, die den Anforderungen Ihres Unternehmens entsprechen.

* Die folgenden Maestro-Datensatztypen sind verfügbar:

   * [Betriebsdatentyp](#operational-record-type): Ein Datensatztyp, der strategische Pläne, Initiativen oder geplante Arbeiten darstellt. Beispielsweise können Campaign, Activity, Tactic und Opportunity betriebliche Datensatztypen sein.
   * [Taxonomie](#taxonomy): Record types, die Attribute zu einem betrieblichen Datensatztyp erfassen. So können beispielsweise Region, Adresse und Zielgruppe Taxonomien sein.

* Wenn Sie einen Datensatztyp erstellen, kann jeder in Ihrer Organisation ihn anzeigen, bearbeiten oder löschen. <!--this will change with access levels and permissions-->
* Sie müssen einen Arbeitsbereich erstellen, bevor Sie Datensatztypen für den Arbeitsbereich erstellen können.
* Sie können in einem Arbeitsbereich insgesamt 1.000 betriebliche Datensatztypen und Taxonomien zusammenführen. Dies umfasst Datensatztypen oder Taxonomien, die Sie von Grund auf neu erstellen oder die Sie aus anderen Systemen importieren.

### Betriebsdatentyp{#operational-record-type}

Ein operationeller Datensatztyp ist ein Maestro-Record-Typ, der arbeitsbezogene Objekte darstellt.

![](assets/operational-record-type-blank.png)

Weitere Informationen zu operativen Datensatztypen, einschließlich ihrer Erstellung, finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

### Taxonomie{#taxonomy}

Eine Taxonomie ist ein Datensatztyp, der Attribute über einen operationellen Datensatztyp erfasst.

![](assets/taxonomy-record-type-blank.png)

Weitere Informationen zu Taxonomie-Datensatztypen finden Sie unter [Erstellen einer Taxonomie](../architecture-and-fields/create-a-taxonomy.md).

Obwohl das Erstellen von Taxonomien mit dem Erstellen von operationellen Datensatztypen identisch ist, unterscheidet Maestro konzeptionell zwischen einem operationellen Datensatztyp und einem Taxonomiedatensatstyp. Ziel von Taxonomien ist es, die operationellen Datensatztypen zu verbessern. Taxonomien sollten keine Arbeitsobjekte direkt darstellen.  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

Beispielsweise können Datensatztypen vom Typ Zielgruppe, Region oder Adresse vom Typ Taxonomie sein.

Weitere Informationen finden Sie unter [Erstellen einer Taxonomie](../architecture-and-fields/create-a-taxonomy.md).

## Ähnlichkeiten und Unterschiede zwischen operationellen Datensatztypen und Taxonomien

Die folgende Tabelle zeigt einige der Ähnlichkeiten und Unterschiede zwischen operationellen Datensatztypen und Taxonomien:

| Art der Aufzeichnung und Kennzeichen | Betriebsdatentyp | Taxonomie-Record-Typ |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| Sie sind Teil eines Arbeitsbereichs | ✓ | ✓ |
| Sie können sie automatisch über eine Workspace-Vorlage erstellen | ✓ | ✓ |
| Sie können sie manuell neu erstellen | ✓ | ✓ |
| Sie können sie erstellen, indem Sie Informationen aus einer externen Datei oder Liste kopieren und einfügen | ✓ | ✓ |
| Sie können eine Excel- oder CSV-Datei erstellen | ✓ |                     |
| Sie können schreibgeschützte Datensatztypen erstellen, indem Sie von anderen Anwendungen aus eine Verbindung zu Objektarten herstellen | ✓ |                     |
| Sie stellen arbeitsbezogene Objekte dar | ✓ |                      |
| Sie stellen Attribute zu arbeitsbezogenen Objekten dar |                         | ✓ |
| Sie können von Grund auf neu erstellen | ✓ | ✓ |
| Sie können eine Excel- oder CSV-Datei erstellen | ✓ |                      |
| Sie können den Datensatztyp von einer Drittanbieteranwendung mit einem Objekt verbinden | ✓ |                      |
| Sie können eine Verbindung zu anderen Maestro-Datensatztypen herstellen | ✓ |                    |
| Die zugehörigen Datensätze können in einer Tabellenansicht angezeigt werden. | ✓ | ✓ |
| Sie können die zugehörigen Datensätze in einer Timeline-Ansicht anzeigen. | ✓ | ✓ |
