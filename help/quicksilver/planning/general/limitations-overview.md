---
title: Übersicht über Adobe Workfront Planning-Objektbeschränkungen
description: In Adobe Workfront Planning gibt es Beschränkungen für die Anzahl der Objekte, die Sie in Ihrer Instanz erstellen können. Es gibt Objektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit Workfront Planning zu verbessern.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/WmG-52JaTKD-0-bH2qKniwUBrpGyOKz5jJ3s9nwd12A
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: f8667931-f646-4dd3-af2a-b9d0cb8098ad
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 537
ht-degree: 5%

---

<!--keep the 30 connection limit in yellow till Jan 2026-->

# Überblick über Objektbeschränkungen bei Adobe Workfront-Planung


<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}


In Adobe Workfront Planning gibt es Beschränkungen für die Anzahl der Objekte, die Sie in Ihrer Instanz erstellen können. Es gibt Objektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit Workfront Planning zu verbessern.

In der folgenden Tabelle sind die Beschränkungen für die Anzahl der Objekte aufgeführt, die Sie in Workfront Planning erstellen können. Die Einschränkungen können sich ändern.

| Adobe Workfront Planning-Objekt | Beschränkungen |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Anzahl der Arbeitsbereiche für eine Workfront-Instanz | Unbegrenzt* |
| Anzahl der Abschnitte für einen Arbeitsbereich | 50 |
| Anzahl der Datensatztypen für einen Arbeitsbereich | 100 (dies umfasst Datensatztypen aus allen Bereichen sowie aus denjenigen, die bei Verwendung einer Workspace-Vorlage erstellt werden) |
| Anzahl von Datensätzen für einen Datensatztyp | 25.000 |
| Anzahl von Datensätzen für einen Arbeitsbereich | Planung auswählen: 25.000 <br> Prime: 500.000 <br> Ultimate: 1.000.000 |
| Gesamtzahl der Datensätze für eine Instanz von Workfront Planning | Planung auswählen: 500.000 <br> Planen Prime: 2.000.000 <br> Planen Ultimate: Unbegrenzt |
| Anzahl der Felder für einen Datensatztyp oder eine Taxonomie | 500 |
| Anzahl der Zeichen für ein einzeiliges Textfeld | 1.000 Zeichen |
| Anzahl der Zeichen für ein Absatzfeld | 10.000 Zeichen |
| Anzahl der Absatzfelder für einen Datensatztyp | 20 Absatzfelder |
| Größe der Datei, die Sie zum Importieren von Informationen in eine Datensatztyptabelle verwenden können | 1MB |
| Dateigröße, mit der Sie Informationen in eine Datensatztyptabelle über die API importieren können | 1,5MB |
| Die Rate, mit der API-Anfragen gestellt werden können | 200 Anfragen pro Minute |
| Anzahl der Ansichten, die ein Benutzer für einen Datensatztyp erstellen kann | 100 |
| CSV-Größe der Excel-Datei, die Sie importieren können, um Datensatztypen zu erstellen | 5MB |
| Anzahl der Zeilen, die Sie in eine CSV- oder Excel-Datei importieren können, um Datensatztypen zu erstellen | 25.000 |
| Anzahl der Spalten, die Sie in eine CSV- oder Excel-Datei importieren können, um Datensatztypen zu erstellen | 500 |
| Anzahl der Formelfelder für einen Datensatztyp | 20 |
| Anzahl der Verbindungsfelder für einen Datensatztyp | 30 |
| Anzahl der Zeichen in einem Formelfeldausdruck | 50.000 |
| Anzahl der Entitäten (Benutzer, Rollen, Teams, Unternehmen, Gruppen), für die Sie ein Planning-Objekt freigeben können | 100 |
| <span class="preview">Anzahl der Datensätze, die gleichzeitig stapelweise freigegeben werden können</span> | 100 |
| Anzahl der Datensatztypen in einer Hierarchie | 4 |
| Anzahl der Hierarchien in einem Arbeitsbereich | 5 |
| Anzahl der Datensätze eines übergeordneten Datensatztyps, die mit einem Datensatz eines untergeordneten Datensatztyps verbunden sind, innerhalb einer Hierarchie | 10 |
| Anzahl der mit einem Datensatz verbundenen Datensätze bei einem Mehrfachauswahl-Verbindungstyp, ohne dass eine Hierarchie zwischen den Datensätzen konfiguriert ist | 500 |

*Es wird empfohlen, nicht zu viele Arbeitsbereiche zu verwenden, da diese möglicherweise schwer zu verwalten sind und Ihre Workflows zu fragmentiert sind.

Wenden Sie sich an Ihren Kundenbetreuer, wenn Sie Informationen zur Preisgestaltung und zur Verpackung von Workfront Planning benötigen.

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--
OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--
[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.
-->
