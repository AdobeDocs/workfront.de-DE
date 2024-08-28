---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Beispiele für Data Connect-Abfragen
description: Beispielabfragen, mit denen Sie sich mit der Syntax und Struktur bestimmter Abfragen vertraut machen können.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Workfront Data Connect-Abfragebeispiele

Damit Sie Ihre Workfront Data Connect-Daten besser nutzen können, enthält diese Seite grundlegende Beispielabfragen, mit denen Sie sich mit der Syntax und Struktur bestimmter Abfragen vertraut machen können.

## Benutzerdefinierte Datenabfrage

In diesem Beispiel wird gezeigt, wie Sie eine Abfrage erstellen können, um Ihre benutzerdefinierten Daten in Workfront zurückzugeben, z. B. benutzerdefinierte Formulare und benutzerdefinierte Felder.

### Szenario:

Ihr Unternehmen, PeopleSoft, verwendet ein benutzerdefiniertes Formular namens Finance Integration. Das Formular wird an jedes Projekt angehängt und enthält die folgenden Felder:

* **PeopleSoft Business Unit** - Ein benutzerdefiniertes Feld, das eine Zeichenfolge enthält.
* **PeopleSoft ProjectID** - Ein benutzerdefiniertes Feld, das eine numerische Zeichenfolge enthält.
* **Erweiterter Projektname** - Ein berechnetes benutzerdefiniertes Datenfeld, das die Werte von PeopleSoft Business Unit, PeopleSoft ProjectID und dem nativen Workfront-Projektnamen in einer einzigen Zeichenfolge verkettet.

Sie müssen diese Informationen in die Antwort für eine Abfrage gegen Data Connect aufnehmen. Benutzerdefinierte Datenwerte für einen Datensatz im Data Lake sind in einer Spalte mit dem Titel `parameterValues` enthalten. Diese Spalte wird als JSON-Objekt gespeichert.

### Abfrage:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:PeopleSoft Business Unit" :: int as PeopleSoftBusinessUnit,
    parametervalues:"DE:PeopleSoft Project ID" :: int as PeopleSoftProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Reaktion

Die obige Abfrage gibt die folgenden Daten zurück:

* `projectid` - die native Workfront-Projekt-ID
* `parametervalues` - eine Spalte, die ein JSON-Objekt speichert
* `name` - der native Workfront-Projektname
* `PeopleSoft Business Unit` - ein benutzerdefinierter Datenwert, der im `parametervalues` -Objekt enthalten ist
* `PeopleSoft Project ID` - ein benutzerdefinierter Datenwert, der im `parametervalues` -Objekt enthalten ist
* `Expanded Project Name` - ein benutzerdefinierter Datenwert, der im `parametervalues` -Objekt enthalten ist

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
