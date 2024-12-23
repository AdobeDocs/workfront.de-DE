---
title: Übersicht über die Objektbeschränkungen für die Adobe Workfront-Planung
description: Die Adobe Workfront-Planung hat Einschränkungen dafür, wie viele Objekte Sie in Ihrer Instanz erstellen können. Es gibt Objektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit der Workfront-Planung zu verbessern.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: d962d60294295dd1f3771d1f0b737c9d1f03dfef
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 1%

---

<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Übersicht über die Objektbeschränkungen für Adobe Workfront Planung

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}


Die Adobe Workfront-Planung hat Einschränkungen dafür, wie viele Objekte Sie in Ihrer Instanz erstellen können. Es gibt Objektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit der Workfront-Planung zu verbessern.

Die folgende Tabelle zeigt die Einschränkungen für die Anzahl der Objekte, die Sie in der Workfront-Planung erstellen können. Die Einschränkungen können sich ändern, wenn wir in die nächsten Entwicklungsphasen eintreten.

| Adobe Workfront Planning-Objekt | Limit |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Anzahl der Arbeitsbereiche für eine Workfront-Instanz | unlimited* |
| Anzahl der Abschnitte für einen Arbeitsbereich | 50 |
| Anzahl der Datensatztypen für einen Arbeitsbereich | 1.000 (dies umfasst Datensatztypen aus allen Abschnitten und solche, die bei Verwendung einer Workspace-Vorlage erstellt werden) |
| Datensatzanzahl für einen Datensatztyp | 25.000 |
| Datensatzanzahl für einen Arbeitsbereich | 25.000 für Kunden mit Planung <br> 500.000 für Kunden mit Planung Plus |
| Anzahl der Datensätze für eine Instanz der Workfront-Planung | 500.000 für Kunden mit Planungsplan <br>2 Mio. für Kunden mit Planning Plus |
| Anzahl der Felder für einen Datensatztyp oder eine Taxonomie | 500 |
| Anzahl der Zeichen für ein einzeiliges Textfeld | 1.000 Zeichen |
| Anzahl der Zeichen für ein Absatzfeld | 10.000 Zeichen |
| Anzahl der Absatzfelder für einen Datensatztyp | 20 Absatzfelder |
| Dateigröße, die Sie in eine Datensatztyp-Tabelle einfügen können | 1 MB |
| Dateigröße, die Sie über die API für eine Datentyptabelle importieren können | 1,5 MB |
| Die Rate, mit der API-Anfragen gestellt werden können | 200 Anfragen pro Minute |
| Anzahl der Ansichten, die ein Benutzer für einen Datensatztyp erstellen kann | 100 |
| Größe der CSV-Datei von Excel, die Sie importieren können, um Datensatztypen zu erstellen | 5 MB |
| <span class="preview">Anzahl der Zeilen, die Sie in eine CSV- oder Excel-Datei importieren können, um Datensatztypen zu erstellen</span> | 10.000 |
| <span class="preview">Anzahl der Spalten, die Sie in eine CSV- oder Excel-Datei importieren können, um Datensatztypen zu erstellen</span> | 500 |

*Es wird empfohlen, nicht zu viele Arbeitsbereiche zu verwenden, da diese sich als schwierig erweisen könnten und Ihre Arbeitsabläufe zu fragmentiert sein könnten.

Informationen zu Preisen und Verpackungen für die Workfront-Planung finden Sie unter [Preise und Verpackung für Adobe Workfront](https://business.adobe.com/products/workfront/pricing.html).

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

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

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->
