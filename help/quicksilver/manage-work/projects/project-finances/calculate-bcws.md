---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Geplante Arbeitskosten berechnen (BCWS)
description: Die geplante Arbeitsaufgabe (BCWS), auch als geplanter Wert bezeichnet, ist eine Metrik zur Projektleistung, die den Umfang der Aufgabe darstellt, die zum Zeitpunkt der Berechnung dieser Metrik abgeschlossen sein sollte.
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 2%

---

# Geplante Arbeitskosten berechnen (BCWS)

## Übersicht über die geplanten Arbeitskosten (BCWS)

Die geplante Arbeitsaufgabe (BCWS), auch als geplanter Wert bezeichnet, ist eine Metrik zur Projektleistung, die den Umfang der Aufgabe darstellt, die zum Zeitpunkt der Berechnung dieser Metrik abgeschlossen sein sollte.

Adobe Workfront berechnet die geplanten Arbeitskosten (BCWS) für Projekte und Aufgaben.

Beachten Sie bei der Überprüfung der Werte für die BCWS für eine Aufgabe oder ein Projekt Folgendes:

* Workfront berechnet die BCWS für eine Aufgabe basierend auf Ihrer Konfiguration für die Leistungsindex-Methode (PIM) des Projekts.

  Sie können Ihr Projekt so konfigurieren, dass die PIM anhand von Stunden oder Kosten berechnet wird und die BCWS auch anhand derselben Werte berechnet werden.

  Informationen zum Konfigurieren der Berechnung der BCWS finden Sie im Abschnitt [Konfigurieren der Berechnung der BCWS](#configure-how-bcws-is-calculated) in diesem Artikel.

* Workfront berechnet die BCWS für ein Projekt, indem alle BCWS-Werte aus allen übergeordneten Aufgaben und Aufgaben des Projekts hinzugefügt werden.

  Die Werte von untergeordneten Aufgaben werden nicht zum BCWS des Projekts hinzugefügt.

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

## Konfiguration der BCWS-Berechnung {#configure-how-bcws-is-calculated}

Sie können konfigurieren, ob die BCWS in Stunden oder Kosten berechnet wird, indem Sie konfigurieren, wie die Performance Index Method (PIM) des Projekts berechnet wird.

1. Wechseln Sie zu einem Projekt und klicken Sie im linken Bereich auf **Projektdetails** .
1. Suchen Sie im Bereich **Finance** das Feld **Performance Index Method** und doppelklicken Sie darauf, um es zu bearbeiten.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Wählen Sie aus den folgenden Optionen aus:

   | Option | Durchführung der Berechnung |
   |---|---|
   | Stundenbasiert | Workfront berechnet die BCWS mithilfe der geplanten Stunden der Aufgaben. |
   | Kostenbasiert | Workfront berechnet die BCWS mithilfe der Plankosten der Aufgaben. |


1. Klicken Sie auf **Änderungen speichern**.

   Die BCWS der Aufgaben im Projekt werden anhand von Stunden oder Kosten berechnet.

## BCWS berechnen

Workfront berechnet die geplanten Arbeitskosten (BCWS) für Aufgaben oder Projekte anhand der folgenden Formeln:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

In dieser Berechnung werden die folgenden Werte verwendet:

| Verwendeter Wert | Beschreibung des verwendeten Werts |
|---|---|
| Geplanter Prozentsatz abgeschlossen | Dies ist der prozentuale Abschluss der Aufgabe, indem man sich die Zeit ansieht, die zwischen dem Beginn der Aufgabe und dem heutigen Tag verstrichen ist. |
| Aufgabenbudget | Dies ist der Wert für die geplanten Stunden oder geplanten Kosten der Aufgabe. |

Wenn es beispielsweise heute den 12. Februar ist und eine Aufgabe vom 10. Februar bis zum 20. Februar dauern soll, sollte die Aufgabe heute zu 20 % abgeschlossen sein. Wenn das Aufgabenbudget (Geplante Kosten) 10.000 USD beträgt, lautet das BCWS für die Aufgabe:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Suchen Sie die BCWS für ein Projekt oder eine Aufgabe

Sie können den Wert der in einem Bericht oder in einer Liste geplanten budgetierten Arbeitskosten anzeigen, indem Sie die Spalte BCWS zu Ihrer Ansicht hinzufügen.

1. Gehen Sie zu einer Liste von Aufgaben oder Projekten.
1. Erweitern Sie das Menü **Ansicht** und wählen Sie **Neue Ansicht** oder **Ansicht anpassen** aus.

1. Klicken Sie auf **Spalte hinzufügen**.
1. Geben Sie in der Spalte **In dieser Spalte anzeigen:** das Feld **BCWS** ein und klicken Sie auf , um es auszuwählen, wenn es in der Liste angezeigt wird.

   ![](assets/bcws-in-project-view.png)

1. Klicken Sie auf **Ansicht speichern**.
1. Das Feld **BCWS** wird in der Ansicht angezeigt.
