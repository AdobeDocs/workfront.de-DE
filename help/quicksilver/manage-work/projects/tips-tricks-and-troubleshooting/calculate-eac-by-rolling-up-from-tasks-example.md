---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Berechnungsbeispiel - Berechnung der EAC als Datenaggregation aus Aufgaben
description: PIM = Stunde-basiert
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 8%

---

# Berechnungsbeispiel - Berechnung der EAC als Datenaggregation aus Aufgaben

## EAC-Methode: Datenaggregation aus Aufgaben oder Unteraufgaben

* [PIM = Stunde-basiert](#pim-hour-based)
* [PIM = Kostenbasiert](#pim-cost-based)

### PIM = Stunde-basiert {#pim-hour-based}

* [Einfaches Beispiel: Projekt ohne untergeordnete Aufgaben](#simple-example-project-has-no-children-tasks)
* [Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben](#complicated-example-project-has-children-tasks)

#### Einfaches Beispiel: Projekt ohne untergeordnete Aufgaben {#simple-example-project-has-no-children-tasks}

PIM = Stunde-basiert

EAC-Methode = Datenaggregation aus Aufgaben/Unteraufgaben

1. Erstellen Sie Projekt A mit drei Aufgaben (keine untergeordneten Aufgaben), die Benutzer 1 zugewiesen sind und deren Kosten/Stunde 100,00 USD beträgt.
1. Fügen Sie geplante/tatsächliche Stunden zu jeder Aufgabe hinzu und % Fertig stellen gemäß der unten stehenden Tabelle:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <br> <p><strong>Gpl. Std.</strong> </p> </th> 
   <th> <br> <p><strong>Tatsächliche Stunden</strong> </p> </th> 
   <th> <p><strong>% Abgeschlossen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>5 Stunden</p> </td> 
   <td> <p>25 Std.</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>25 Std.</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>15 Stunden</p> </td> 
   <td> <p>25 Std.</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Finanzdaten neu berechnen
1. **CPI für Aufgabe 1** = 0,04 berechnet wie folgt:\
   **CPI für Aufgabe 1** = *IF* Tatsächliche Stunden > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Aufgabe 1** = 1 / 25\
   **CPI für Aufgabe 1** = 0,04

1. **EAC für Aufgabe 1** = 125 Std. berechnet wie folgt:\
   **EAC für Aufgabe 1** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC für Aufgabe 1** = 5 / 0,04\
   **EAC für Aufgabe 1** = 125 Std.

1. CPI/EAC für die Aufgaben 2 und 3 sind:\
   Aufgabe 2 = 0,12 / 83,33 Std.\
   Aufgabe 3 = 0,24 / 62,5 Std.

1. **CPI für Projekt** = 0,13 berechnet wie folgt:\
   **CPI für Projekt** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI für Projekt** = 10 / 75\
   **CPI für Projekt** = 0,13

1. **EAC für Projekt** = 270,83 Std. berechnet wie folgt\
   **EAC für Projekt** = EAC Aufgabe 1 + EAC Aufgabe 2 + EAC Aufgabe 3\
   **EAC für Projekt** = 125 + 83,33 + 62,5\
   **EAC für Projekt** = 270.83 Std.

#### Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben {#complicated-example-project-has-children-tasks}

PIM = Stunde-basiert

EAC-Methode = Datenaggregation aus Aufgaben/Unteraufgaben

1. Erstellen Sie Projekt A mit sechs Aufgaben, bei denen Aufgabe 3 die übergeordneten Aufgaben 4 und 5 und Aufgabe 1 die übergeordneten Aufgaben 2 und 3 ist, wie unten dargestellt:\
   Aufgabe 1\
      Aufgabe 2\
      Aufgabe 3\
         Aufgabe 4\
         Aufgabe 5\
   Aufgabe 6

1. Weisen Sie Benutzer 1 die Aufgaben 2, 4, 5 und 6 zu, deren Kosten/Std-Rate 100,00 USD beträgt.
1. Fügen Sie geplante/tatsächliche Stunden für jede Aufgabe hinzu und % Fertig stellen gemäß der unten stehenden Tabelle.

   >[!NOTE]
   >
   >Für die Aufgaben 1 und 3 fügen Sie nur die tatsächlichen Stunden hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <br> <p><strong>Gpl. Std.</strong> </p> </th> 
   <th> <br> <p><strong>Tatsächliche Stunden</strong> </p> </th> 
   <th> <p><strong>% Abgeschlossen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>5 Stunden</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>15 Stunden</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>20 Stunden</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie dem Projekt 50 Stunden direkt hinzu (Mehr > Stunden > Protokollzeiten), sodass 5.000,00 USD der tatsächlichen Arbeitskosten direkt im Projekt erfasst werden.
1. Führen Sie die Neuberechnung der Finanzierungen durch.
1. **CPI für Aufgabe 2** = .1 berechnet wie folgt:\
   **CPI für Aufgabe 2** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI für Aufgabe 2** = 1 / 10\
   **CPI für Aufgabe 2** = .1

1. **EAC für Aufgabe 2** = 50 Stunden, berechnet wie folgt:\
   **EAC für Aufgabe 2** = *IF* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = Geplante Stunden + tatsächliche Stunden\
   **EAC für Aufgabe 2** = 5 / .1\
   **EAC für Aufgabe 2** = 50 Std.

1. CPI/EAC für Aufgabe 4, Aufgabe 5 und Aufgabe 6:\
   Aufgabe 4 = 0,4 / 25 Std.\
   Aufgabe 5 = 0,75 / 20 Stunden\
   Aufgabe 6 = 1.2 / 16.67 Std.

1. **CPI für Aufgabe 3** = 0,38\
   **CPI für Aufgabe 3** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI für Aufgabe 3** = 11,5 / 30\
   **CPI für Aufgabe 3** = 0,38

1. **EAC für Aufgabe 3** = EAC Aufgabe 4 + EAC Aufgabe 5\
   **EAC für Aufgabe 3** = 25 + 20\
   **EAC für Aufgabe 3** = 45 Std.

1. **CPI für Aufgabe 1** = 0,25 berechnet wie folgt:\
   **CPI für Aufgabe 1** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI für Aufgabe 1** = 12,5 / 50\
   **CPI für Aufgabe 1** = 0,25

1. **EAC für Aufgabe 1** = EAC Aufgabe 2 + EAC Aufgabe 3\
   **EAC für Aufgabe 1** = 50 + 45\
   **EAC für Aufgabe 1** = 95 Std.

1. CPI für Projekt = 0,22 berechnet wie folgt:\
   **CPI für Projekt** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI für Projekt** = 24,5 / 110\
   **CPI für Projekt** = .22272\
   **CPI für Projekt** = 0,22

1. **EAC für Projekt** = EAC Aufgabe 1 + EAC Aufgabe 6\
   **EAC für Projekt** = 95 + 16,67\
   **EAC für Projekt** = 111.67 Std.

### PIM = Kostenbasiert {#pim-cost-based}

* [Einfaches Beispiel: Projekt ohne untergeordnete Aufgaben](#simple-example-project-has-no-children-tasks)

#### Einfaches Beispiel: Projekt ohne untergeordnete Aufgaben {#simple-example-project-has-no-children-tasks-1}

PIM = Kostenbasiert

EAC-Methode = Datenaggregation aus Aufgaben/Unteraufgaben

1. Erstellen Sie Projekt A mit drei Aufgaben (keine untergeordneten Aufgaben), die Benutzer 1 zugewiesen sind und deren Kosten/Std 100,00 USD beträgt.
1. Fügen Sie geplante/tatsächliche Stunden zu jeder Aufgabe hinzu und % Fertig stellen gemäß der unten stehenden Tabelle:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <br> <p><strong>Gpl. Std.</strong> </p> </th> 
   <th> <br> <p><strong>PLN LBR-Kosten</strong> </p> </th> 
   <th> <br> <p><strong>Tatsächliche Stunden</strong> </p> </th> 
   <th> <br> <p><strong>LBR-Kosten verwalten</strong> </p> </th> 
   <th> <p><strong>% Abgeschlossen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>5 Stunden</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 Std.</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 Std.</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>15 Stunden</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 Std.</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie den einzelnen Aufgaben die Ausgaben entsprechend der unten stehenden Tabelle hinzu:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <p><strong>Ausgabe</strong> </p> </th> 
   <th> <p><strong>Geplanter Betrag</strong> </p> </th> 
   <th> <p><strong>Tatsächlicher Betrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Exp1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Exp2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Exp</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>Aufgabe 3 Exp</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie dem Projekt zwei Ausgaben hinzu (d. h. nicht an eine Aufgabe gebunden):

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Ausgabe</strong> </p> </th> 
   <th> <p><strong>Geplanter Betrag</strong> </p> </th> 
   <th> <p><strong>Tatsächlicher Betrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projekt Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1 Exp2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Auf der Grundlage der obigen Werte werden die angefallenen/nicht angefallenen Kosten wie folgt ermittelt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <p><strong>Nicht eingetretene geplante Kosten</strong> </p> </th> 
   <th> <p><strong>Geplante Kosten</strong> </p> </th> 
   <th> <p><strong>Anfallende tatsächliche Kosten</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Führen Sie über Projektaktionen die Option Finanzen neu berechnen aus.
1. **CPI***für Aufgabe 1** = 0,14 berechnet wie folgt:\
   **CPI***für Aufgabe 1**  = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour\
   **CPI***für Aufgabe 1**  = (100+300) / (2500+400)\
   **CPI***für Aufgabe 1**  = 400/2900\
   **CPI***für Aufgabe 1**  = 0,14

1. **EAC*** für Aufgabe 1** = 13.400,00 $\
   **CPI-Arbeit***für Aufgabe 1** = WENN die tatsächlichen Arbeitskosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI-Arbeit***für Aufgabe 1** = 100/2500\
   **CPI-Arbeit***für Aufgabe 1** = 0,04

   **EAC für Arbeit***für Aufgabe 1** = *IF* CPI_Labour &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC-Arbeit = geplante Arbeitskosten + tatsächliche Arbeitskosten\
   **EAC für Arbeit***für Aufgabe 1** = 500.00/.04\
   **EAC für Arbeit***für Aufgabe 1** = 12.500,00 $

   **EAC-Ausgaben*** für Aufgabe 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgaben*** für Aufgabe 1** = 400,00 $ + 500,00 $\
   **EAC-Ausgaben*** für Aufgabe 1** = 900,00 $

   **EAC*** für Aufgabe 1** = Arbeitskosten der EAC und Ausgaben der EAC\
   **EAC*** für Aufgabe 1**  = 12.500,00 $ + 900,00 $\
   **EAC*** für Aufgabe 1**  = 13.400,00 $

1. Im Folgenden finden Sie die CPI-/EAC-Werte für Aufgabe 2 und Aufgabe 3:\
   Aufgabe 2 = 0,19 / 8.433,33 $\
   Aufgabe 3 = 0,44 / 6.950,00 $***

1. CPI für das Projekt = 0,32\
   **CPI***für Projekt** = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour\
   **CPI***für Projekt** = (1000 + 2300) / (7500 + 2700)\
   **CPI***für Projekt** = 3300/10200\
   **CPI***für Projekt** = 0,32

1. Der EAC für das Projekt beträgt 28.783,33 USD.\
   **EAC*** für Projekt** = EAC Aufgabe 1 + EAC Aufgabe 2 + EAC Aufgabe 3\
   **EAC*** für Projekt** = $13.400.00 + $8.433.33 + $6.950.00\
   **EAC*** für Projekt** = 28.783,33 $
