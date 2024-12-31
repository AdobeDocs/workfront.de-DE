---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Schätzung bei Abschluss berechnen (EAC)
description: Als Leistungskennzahl gibt die Kalkulation bei Abschluss (BK) die erwarteten Gesamtkosten Ihres Projekts oder Ihrer Aufgabe zum Zeitpunkt der Fertigstellung an.
author: Lisa
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# Schätzung bei Abschluss berechnen (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Als Leistungskennzahl gibt die Kalkulation bei Abschluss (BK) die erwarteten Gesamtkosten Ihres Projekts oder Ihrer Aufgabe zum Zeitpunkt der Fertigstellung an.

Als Einstellung können Sie festlegen, wie der EAC-Wert berechnet werden soll. 

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Licht oder höher</p>
   <p>oder</p>
   <p>Aktuell: Überprüfung oder höher</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Anzeigen des Zugriffs auf Projekte und Finanzdaten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Anzeigen von oder höheren Berechtigungen für das Projekt mit Berechtigungen zum Anzeigen von Finanzdaten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definieren, wie EAC berechnet wird

Im Rahmen der Voreinstellungen für das Projektsystem kann der Adobe Workfront-Administrator festlegen, wie die EAC berechnet wird. EAC kann auf eine der beiden folgenden Arten berechnet werden:

* [Berechnung auf Projektebene](#calculate-at-the-project-level)
* [Rollup aus Aufgaben und Teilaufgaben](#roll-up-from-tasks-and-subtasks)

Weitere Informationen zum Einrichten von Projektvoreinstellungen in Workfront, einschließlich der Berechnung der Kalkulation bei Abschluss, finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Als Projekt-Manager können Sie diese Einstellung auch auf Projektebene auf der Unterregisterkarte Finanzen des Projekts ändern. Weitere Informationen zum Bearbeiten der Unterregisterkarte „Finanzen“ eines Projekts finden Sie unter [Informationen im Projektfinanzierungsbereich verwalten](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Auf Projektebene berechnen {#calculate-at-the-project-level}

Die BK für die übergeordnete Aufgabe und das übergeordnete Projekt werden durch Eingabe der tatsächlichen Stunden/tatsächlichen Arbeitskosten in die BK-Formeln bestimmt. Diese Berechnung beinhaltet die tatsächlichen Stunden/Kosten und Ausgaben, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.

### Rollup aus Aufgaben und Teilaufgaben {#roll-up-from-tasks-and-subtasks}

Die BK für die übergeordnete Aufgabe und das übergeordnete Projekt werden bestimmt, indem die BK für jede untergeordnete Aufgabe zusammengefasst werden. Diese Berechnung schließt die tatsächlichen Stunden/Kosten und Ausgaben aus, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.

## So berechnen Sie die EAC anhand der Performance-Index-Methode (PIM)

In Workfront hängt die Berechnung für EAC von der ausgewählten Leistungsindexmethode (PIM) des Projekts ab. Weitere Informationen zum Festlegen des PIM für Ihr System oder Projekt finden Sie unter [Festlegen der Leistungsindexmethode (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [EAC mit stundenbasiertem PIM berechnen](#calculate-eac-using-hour-based-pim)
* [EAC mit kostenbasiertem PIM berechnen](#calculate-eac-using-cost-based-pim)

### EAC mit stundenbasiertem PIM berechnen {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;If Cost Performance Index [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Gesamte geplante Stunden + Tatsächliche Stunden. Dies tritt auf, wenn Stunden erfasst wurden, das Projekt/die Aufgabe jedoch zu 0 % abgeschlossen ist.

Weitere Informationen zur Berechnung des CPI finden Sie [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### EAC mit kostenbasiertem PIM berechnen {#calculate-eac-using-cost-based-pim}

Die EAC eines Projekts wird anhand der folgenden Formel berechnet:

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC-Arbeitszeit =  <em>IF</em> CPI Arbeit &lt;&gt; 0 DANN EAC Arbeit = Geplante Lohnkosten / CPI Arbeit</pre><pre><em>ELSE</em> EAC  Arbeit = Geplante Arbeitskosten + Ist-Arbeitskosten</pre><pre>CPI Arbeit = WENN Ist-Lohnkosten &lt;&gt; 0 DANN CPI Arbeit = TotalBudgetedCostWorkPerformed / Ist-Lohnkosten</pre><pre>SONST CPI Arbeit = 1 </pre>Die folgenden Felder werden bei der Berechnung der EAC berücksichtigt:

* Gesamte budgetierte Kosten Abgeschlossene Arbeit (SKAA) = Ergebnis der Multiplikation der budgetierten Kosten der geplanten Arbeit (budgetierte Kosten) mit dem Prozentsatz der Aufgabe, der bisher abgeschlossen wurde.

  Informationen über die insgesamt budgetierten Kosten der durchgeführten Arbeit (SKAA) finden Sie unter [Budgetierte Kosten der durchgeführten Arbeit (SKAA) berechnen](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Für eine nicht übergeordnete Aufgabe:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **Für eine übergeordnete Aufgabe:**
Gesamte budgetierte Kosten Ausgeführte Arbeit = Summe der insgesamt budgetierten Kosten Ausgeführte Arbeit für alle direkt untergeordneten Aufgaben.

   * **Für ein Projekt:**
Gesamte budgetierte Kosten Ausgeführte Arbeit = Summe der insgesamt budgetierten Kosten Ausgeführte Arbeit für alle Aufgaben der obersten Ebene (übergeordnete und eigenständige Aufgaben). 

* EAC-Kosten = das Ergebnis der Hinzufügung der angefallenen Ist-Kosten zu den nicht angefallenen geplanten Kosten. Sie wird nach folgender Formel berechnet:

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Angefallene Istkosten = Summe des Felds „Geplanter Betrag“ für alle Ausgaben, bei denen das Feld „Tatsächlicher Betrag“ > 0 ist. Beispiel: Wenn Sie eine Ausgabe für Aufgabe 1 erstellen und im Feld Geplanter Betrag 500,00 $ und im Feld Tatsächlicher Betrag einen Betrag > 0 (d. h. 600,00 $) eingeben, betragen die Kosten für geplante Ausgaben für diese Aufgabe 500,00 $.
   * Nicht angefallene geplante Ausgaben = Summe des Felds Geplanter Betrag für alle Ausgaben, bei denen das Feld Tatsächlicher Betrag = 0 ist. Beispiel: Wenn Sie zwei Ausgaben für Aufgabe 1 erstellen, bei denen für die erste Ausgabe der Wert im Feld Geplanter Betrag $500.00 und der Wert im Istbetrag $600.00 ist und für die zweite Ausgabe der Wert im Feld Geplanter Betrag $300.00 ist und der Wert im Feld Tatsächlicher Betrag $0.00 ist, lautet der Wert der nicht angefallenen geplanten Ausgabe für diese Aufgabe $300.00. 

## Suchen der EAC in einem Projekt oder einer Aufgabe

1. Wechseln Sie zu dem Projekt oder der Aufgabe, in dem bzw. der Sie die EAC anzeigen möchten.
1. Erweitern Sie **Projektdetails** oder **Aufgabendetails** im linken Bereich des Projekts oder der Aufgabe, je nachdem, wo Sie die EAC anzeigen.

1. Klicken Sie auf **Finanzen**. 

   Der EAC-Wert wird im Feld **Schätzung bei Abschluss** angezeigt.

   ![](assets/eac-highlighted-on-project-350x112.png)
