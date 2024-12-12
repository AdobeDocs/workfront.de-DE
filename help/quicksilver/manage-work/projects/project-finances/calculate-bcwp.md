---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Berechnung der veranschlagten Arbeitskosten (BCWP)
description: Die als Earned Value (Earned Value, Earned Value, Budgeted Cost of Work Performed, BCWP) bezeichnete Metrik zur Projektleistung, die den Betrag der Aufgabe darstellt, die zum Zeitpunkt der Berechnung dieser Metrik tatsächlich abgeschlossen wurde.
author: Lisa
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 2%

---

# Berechnung der veranschlagten Arbeitskosten (BCWP)

## Übersicht über die veranschlagten Arbeitskosten (BCWP)

Die als Earned Value (Earned Value, Earned Value, Budgeted Cost of Work Performed, BCWP) bezeichnete Metrik zur Projektleistung, die den Betrag der Aufgabe darstellt, die zum Zeitpunkt der Berechnung dieser Metrik tatsächlich abgeschlossen wurde.

Adobe Workfront berechnet die budgetierten Kosten der durchgeführten Arbeit (BCWP) für Projekte und Aufgaben.

Beachten Sie bei der Überprüfung der Werte für das BCWP für eine Aufgabe oder ein Projekt Folgendes:

* Workfront berechnet das BCWP für eine Aufgabe basierend auf Ihrer Konfiguration für die Leistungsindex-Methode (PMI) des Projekts.

  Sie können Ihr Projekt so konfigurieren, dass die PMI anhand von Stunden oder Kosten berechnet wird und der BCWP auch anhand der gleichen Werte berechnet wird.

  Informationen zum Konfigurieren der Berechnung des BCWP finden Sie im Abschnitt [Konfigurieren der Berechnung des BCWP](#configure-how-bcwp-is-calculated) in diesem Artikel.

* Workfront berechnet das BCWP für ein Projekt, indem es alle BCWP-Werte aus allen übergeordneten Aufgaben und Aufgaben des Projekts hinzufügt.

  Die Werte aus untergeordneten Aufgaben werden nicht zum BCWP des Projekts hinzugefügt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Zugriff auf Projekte bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Berechtigungen für das Projekt verwalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfiguration der BCWP-Berechnung {#configure-how-bcwp-is-calculated}

Sie können konfigurieren, ob das BCWP in Stunden oder Kosten berechnet wird, indem Sie konfigurieren, wie die Performance Index Method (PIM) des Projekts berechnet wird.

1. Wechseln Sie zu einem Projekt und erweitern Sie im linken Bereich **Projektdetails** .
1. Suchen Sie im Bereich **Finanzen** das Feld **Leistungsindex-Methode** und doppelklicken Sie auf , um es zu bearbeiten.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Wählen Sie aus den folgenden Optionen aus:

   | Option | Durchführung der Berechnung |
   |---|---|
   | Stundenbasiert | Workfront berechnet das BCWP mithilfe der geplanten Stunden der Aufgaben. |
   | Kostenbasiert | Workfront berechnet das BCWP mithilfe der Plankosten der Aufgaben. |

1. Klicken Sie auf **Änderungen speichern**.

Der BCWP der Aufgaben im Projekt wird anhand von Stunden oder Kosten berechnet.

## BCWP berechnen

Workfront berechnet die budgetierten Kosten der durchgeführten Arbeit (BCWP) für eine Aufgabe oder ein Projekt anhand der folgenden Formeln:

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

In dieser Berechnung werden die folgenden Werte verwendet:

| Verwendeter Wert | Beschreibung des verwendeten Werts |
|---|---|
| Tatsächlicher Prozentsatz abgeschlossen | Dies ist der tatsächliche Prozentsatz des Abschlusses der Aufgabe, wie er in Workfront angezeigt wird. |
| Aufgabenbudget | Dies ist der Wert für die geplanten Stunden oder geplanten Kosten der Aufgabe. |

Wenn der tatsächliche Prozentsatz des Abschlusses der Aufgabe beispielsweise 25 % beträgt und das Aufgabenbudget oder die geplanten Kosten 10.000 $ beträgt, lautet der BCWP für die Aufgabe:

```
BCWP = 25% x $10,000 = $2,500
```

## Suchen Sie den BCWP für ein Projekt oder eine Aufgabe.

Sie können den Wert der in einem Bericht oder in einer Liste ausgeführten budgetierten Arbeitskosten anzeigen, indem Sie die Spalte BCWP zu Ihrer Ansicht hinzufügen.

1. Gehen Sie zu einer Liste von Aufgaben oder Projekten.
1. Erweitern Sie das Menü **Ansicht** und wählen Sie **Neue Ansicht** oder **Ansicht anpassen** aus.

1. Klicken Sie auf **Spalte hinzufügen**.
1. Geben Sie in der Spalte **In dieser Spalte anzeigen:** das Feld **BCWP** ein und klicken Sie auf , um es auszuwählen, wenn es in der Liste angezeigt wird.

   ![](assets/bcwp-project-view.png)

1. Klicken Sie auf **Ansicht speichern**.
1. Das BCWP-Feld wird in der Ansicht angezeigt.
