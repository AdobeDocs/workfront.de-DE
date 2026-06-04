---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Überblick über das voraussichtliche Startdatum des Projekts
description: Das voraussichtliche Startdatum ist ein Echtzeit-Datum, an dem das Projekt beginnen wird, basierend auf dem voraussichtlichen Startdatum der ersten Aufgabe im Projekt.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
TQID: https://experienceleague.adobe.com/2rcx201EGt4cqRpqfXws6P-NbRnXyVlFoTbJrQJBipg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 430
ht-degree: 6%

---

# Überblick über das voraussichtliche Startdatum des Projekts

## Übersicht über das voraussichtliche Startdatum für Projekte und Aufgaben

Das voraussichtliche Startdatum ist ein Echtzeit-Datum, an dem das Projekt beginnen wird, basierend auf dem voraussichtlichen Startdatum der ersten Aufgabe im Projekt.

Beim ersten Planen eines Projekts sind das geplante Startdatum und das voraussichtliche Startdatum der Aufgaben und des Projekts identisch. Da es zu Verzögerungen kommen kann oder Aufgaben unter Umständen früher abgeschlossen werden, kann das voraussichtliche Startdatum von dem geplanten Startdatum abweichen.

Änderungen am voraussichtlichen Startdatum des ersten Vorgangs im Projekt-Trigger ändern sich am voraussichtlichen Startdatum des Projekts.

## Ändern des geplanten Startdatums einer Aufgabe

Das voraussichtliche Startdatum für ein Projekt oder eine Aufgabe wird von Adobe Workfront berechnet und kann nicht manuell geändert werden.

Die folgenden Ereignisse können eine Änderung am voraussichtlichen Startdatum einer Aufgabe in Trigger setzen:

* Wenn Sie mit der Arbeit an einer Aufgabe beginnen, wird das tatsächliche Startdatum der Aufgabe zum geplanten Startdatum.
* Wenn das geplante Startdatum einer Aufgabe überschritten wird, wird das voraussichtliche Startdatum in die Zukunft verschoben, was das früheste verfügbare Datum für den Start der Aufgabe angibt.\
  Workfront berücksichtigt bei der Berechnung des frühesten verfügbaren Datums für den Start der Aufgabe die Anzahl der für die Aufgabe geplanten Stunden sowie den Zeitplan des Projekts oder des Benutzers, der der Aufgabe zugewiesen wurde.
* Vorgängeraufgaben, die in Verzug sind, haben Auswirkungen auf das voraussichtliche Startdatum ihrer abhängigen Aufgaben. Das voraussichtliche Startdatum der abhängigen Aufgaben wechselt entsprechend dem Abhängigkeitstyp der Vorgängerbeziehung und entsprechend den voraussichtlichen Terminen der Vorgänger.

Wenn eine dieser Aufgaben die erste Aufgabe in einem Projekt ist, ändert sich das voraussichtliche Startdatum des Projekts entsprechend dem voraussichtlichen Startdatum dieser Aufgabe.

## Suchen Sie das voraussichtliche Startdatum eines Projekts oder einer Aufgabe

Sie können das voraussichtliche Startdatum eines Projekts oder einer Aufgabe in den folgenden Bereichen von Workfront suchen:

* Sie können sie zu einem Projekt oder einer Aufgabe hinzufügen oder einen Bericht oder eine Ansicht anzeigen.

  Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Im Projektdetailabschnitt eines Projekts oder im Aufgabendetailabschnitt einer Aufgabe.
