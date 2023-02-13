---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das vorgeschlagene Projektstartdatum
description: Das geplante Startdatum ist ein Echtzeit-Datum, an dem das Projekt basierend auf dem geplanten Startdatum der ersten Aufgabe des Projekts beginnen wird.
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Übersicht über das vorgeschlagene Projektstartdatum

## Übersicht über das geplante Startdatum für Projekte und Aufgaben

Das geplante Startdatum ist ein Echtzeit-Datum, an dem das Projekt basierend auf dem geplanten Startdatum der ersten Aufgabe des Projekts beginnen wird. 

Wenn Sie ein Projekt zum ersten Mal planen, sind das geplante Startdatum und das geplante Startdatum der Aufgaben und des Projekts identisch. Da Verzögerungen auftreten können oder Aufgaben früher abgeschlossen werden können, kann sich das geplante Startdatum vom geplanten Startdatum unterscheiden. 

Änderungen am geplanten Startdatum der ersten Aufgabe auf dem Projekt-Trigger ändern sich im geplanten Projektstartdatum. 

## Ändern des geplanten Startdatums einer Aufgabe

Das geplante Startdatum für ein Projekt oder eine Aufgabe ist eine von Adobe Workfront vorgenommene Berechnung und kann nicht manuell geändert werden. 

Mit den folgenden Ereignissen kann eine Änderung am geplanten Startdatum einer Aufgabe Trigger werden:

* Wenn Sie mit der Arbeit an einer Aufgabe beginnen, wird das tatsächliche Startdatum der Aufgabe zum geplanten Startdatum.
* Wenn das geplante Startdatum einer Aufgabe überschritten wird, wird das geplante Startdatum in die Zukunft verschoben und gibt das nächstverfügbare Startdatum an, an dem die Aufgabe beginnen soll.\
   Workfront berücksichtigt bei der Berechnung des frühestmöglichen Aufgabenbeginns die geplante Zeitdauer sowie den Zeitplan des Projekts oder des der Aufgabe zugewiesenen Benutzers. 
* Vorläufige Aufgaben, die im Verzug sind, wirken sich auf das geplante Startdatum der abhängigen Aufgaben aus. Das geplante Startdatum der abhängigen Aufgaben wird entsprechend dem Abhängigkeitstyp der Vorgängerbeziehung und den voraussichtlichen Datumsangaben der Vorgänger-Beziehung verschoben. 

Wenn eine dieser Aufgaben die erste Aufgabe in einem Projekt ist, wird das geplante Startdatum des Projekts an das geplante Startdatum dieser Aufgabe angepasst. 

## Suchen Sie nach dem geplanten Startdatum eines Projekts oder einer Aufgabe.

Sie können das geplante Startdatum eines Projekts oder einer Aufgabe in den folgenden Bereichen von Workfront ermitteln:

* Sie können sie zu einem Projekt oder einem Aufgabenbericht oder einer Ansicht hinzufügen.

   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Im Abschnitt &quot;Projektdetails&quot;eines Projekts oder im Abschnitt &quot;Aufgabendetails&quot;einer Aufgabe.
