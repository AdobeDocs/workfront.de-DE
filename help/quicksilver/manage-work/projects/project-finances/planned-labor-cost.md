---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Planete Arbeitskosten berechnen
description: Während Sie die Arbeit an Ihren Projekten planen, berechnet Adobe Workfront die geplanten Arbeitskosten für die dieser Arbeit zugewiesenen Rollen und Benutzer anhand ihrer Kosten pro Stunde .
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Planete Arbeitskosten berechnen

Während Sie die Arbeit an Ihren Projekten planen, berechnet Adobe Workfront die geplanten Arbeitskosten für die dieser Arbeit zugewiesenen Rollen und Benutzer anhand ihrer Kosten pro Stunde .

Die geplanten Arbeitskosten eines Projekts sind eine Berechnung zwischen den Kosten im Zusammenhang mit den Stellenrollen oder den Benutzern, die zum Abschließen der Arbeit an dem Projekt zugewiesen sind, und der geplanten Stundenzahl (geplante Stunden), die die einzelnen Rollen oder Benutzer benötigen können, um die Arbeit abzuschließen.

## Übersicht über die geplanten Arbeitskosten

Die **geplanten Arbeitskosten** eines Projekts werden berechnet, indem alle geplanten Arbeitskosten aller Aufgaben des Projekts hinzugefügt werden.

>[!TIP]
>
>Mit Problemen oder mit dem Projekt selbst sind keine geplanten Arbeitskosten verbunden.

Workfront berechnet die geplanten Arbeitskosten eines Projekts nach folgender Formel:

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

Die Berechnung der geplanten Arbeitskosten für die Aufgabe basiert auf Folgendem:

* Die Anzahl der Ressourcen für die Aufgabe und ihre individuelle Zuweisung zur Aufgabe
* Der Kostentyp der Aufgabe.

Die geplanten Arbeitskosten werden anhand der folgenden Formel berechnet:

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Weitere Informationen dazu, wie Workfront geplante Arbeitskosten für Aufgaben entsprechend Aufgabenzuweisungen und Kostentyp berechnet, finden Sie im Abschnitt &quot;Ändern von Kostentypen für einzelne Aufgaben&quot;im Artikel [Kosten-Tracking](../../../manage-work/projects/project-finances/track-costs.md).

## Geplante Arbeitskosten ermitteln

Die geplanten Arbeitskosten eines Projekts finden Sie in den folgenden Bereichen von Workfront:

* Ein Projektbericht
* Liste der Projekte
* Ein Baseline-Bericht, in dem Sie ihn über einen bestimmten Zeitraum verfolgen können
* Über die API

Informationen zum Erstellen von Berichten und zur Verwendung der Workfront-API finden Sie in den folgenden Artikeln:

* [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API-Grundlagen](../../../wf-api/general/api-basics.md)
