---
title: Übersicht über die Objektbeschränkungen für die Adobe Workfront-Planung
description: Die Adobe Workfront-Planung hat Einschränkungen dafür, wie viele Objekte Sie in Ihrer Instanz erstellen können. Es gibt Objektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit der Workfront-Planung zu verbessern.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Übersicht über die Objektbeschränkungen für Adobe Workfront Planung

Die Adobe Workfront-Planung hat Einschränkungen dafür, wie viele Objekte Sie in Ihrer Instanz erstellen können. Es gibt Objektbeschränkungen, um die Produktleistung zu verbessern und Ihr Erlebnis mit der Workfront-Planung zu verbessern.

Die folgende Tabelle zeigt die Einschränkungen für die Anzahl der Objekte, die Sie in der Workfront-Planung erstellen können. Die Einschränkungen können sich ändern, wenn wir in die nächsten Entwicklungsphasen eintreten.

| Adobe Workfront Planning-Objekt | Limit |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Anzahl der Arbeitsbereiche für eine Workfront-Instanz | 1.000 |
| Anzahl der Abschnitte für einen Arbeitsbereich | 50 |
| Anzahl der Datensatztypen für einen Arbeitsbereich | 1.000 (dies umfasst Datensatztypen aus allen Abschnitten und solche, die bei Verwendung einer Workspace-Vorlage erstellt werden) |
| Datensatzanzahl für einen Datensatztyp | 50.000 |
| Anzahl der Felder für einen Datensatztyp oder eine Taxonomie | 500 |
| Anzahl der Zeichen für ein Textfeld | 1.000 Zeichen |
| Dateigröße, die Sie in eine Datensatztyp-Tabelle einfügen können | 1 MB |
| Dateigröße, die Sie über die API für eine Datentyptabelle importieren können | 1,5 MB |
| Die Rate, mit der API-Anfragen gestellt werden können | 200 Anfragen pro Minute |
| Größe der CSV-Datei, die Sie importieren können* | 5 MB |
| Anzahl der Ansichten, die ein Benutzer für einen Datensatztyp erstellen kann | 100 |

<!--add to the table above: Maximum number of views created by one use 100 -->

>[!IMPORTANT]
>
>*Diese Funktion wurde vorübergehend deaktiviert und steht zu einem späteren Zeitpunkt zur Verfügung.

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import** | 5MB |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.
**This functionality has been temporarily disabled and it will be available at a later date.
-->