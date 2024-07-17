---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Berechnungsbeispiel - EAC auf Projektebene berechnen
description: PIM = Stunde-basiert
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# Berechnungsbeispiel - EAC auf Projektebene berechnen

## EAC-Methode: Auf Projektebene berechnen

* [PIM = Stunde-basiert](#pim-hour-based)
* [PIM = Kostenbasiert](#pim-cost-based)

### PIM = Stunde-basiert {#pim-hour-based}

* [Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben](#simple-example-project-has-no-children-tasks)
* [Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben](#complicated-example-project-has-children-tasks)

#### Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben {#simple-example-project-has-no-children-tasks}

PIM = Stunde-basiert

EAC-Methode = Auf Projektebene berechnen ****

1. Erstellen Sie Projekt A mit drei Aufgaben (keine untergeordneten Aufgaben), die Benutzer 1 zugewiesen sind und deren Kosten/Stunde 100,00 USD beträgt.
1. Fügen Sie für jede Aufgabe geplante und tatsächliche Stunden hinzu und % Fertig stellen gemäß der unten stehenden Tabelle:

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>Aufgabe</strong></p></th>
      <th><br><p><strong>Gpl. Std.</strong></p></th>
      <th><br><p><strong>Tatsächliche Stunden</strong></p></th>
      <th><p><strong>% abgeschlossen</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>Aufgabe 1</p></td>
      <td><p>5 Stunden</p></td>
      <td><p>25 Stunden</p></td>
      <td><p>20 %</p></td>
     </tr>
     <tr>
      <td><p>Aufgabe 2</p></td>
      <td><p>10 Stunden</p></td>
      <td><p>25 Stunden</p></td>
      <td><p>30 %</p></td>
     </tr>
     <tr>
      <td><p>Aufgabe 3</p></td>
      <td><p>15 Stunden</p></td>
      <td><p>25 Stunden</p></td>
      <td><p>40 %</p></td>
     </tr>
    </tbody>
   </table>

1. Führen Sie eine Neuberechnung der Finanzierungen für das Projekt durch.
1. **CPI für Aufgabe 1** = .04, berechnet wie folgt:\
   **CPI für Aufgabe 1** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
      *ELSE* CPI = 1\
   **CPI für Aufgabe 1** = 1/25\
   **CPI für Aufgabe 1** = 0,04

1. **EAC für Aufgabe 1** = 125 Stunden, berechnet wie folgt:\
   **EAC für Aufgabe 1** = *IF* CPI &lt;> 0 *DANN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + realisiert  Stunden\
   **EAC für Aufgabe 1** = 5 / .04\
   **EAC für Aufgabe 1** = 125 Stunden***

1. CPI/EAC für die Aufgaben 2 und 3 sind:\
   Aufgabe  2 = 0,12 / 83,33  hrs\
   Aufgabe 3 = 0,24 / 62,5 Std.

1. **CPI für Projekt** = .13, berechnet wie folgt:\
   **CPI für Projekt** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Projekt** = 10 / 75\
   **CPI für Projekt** = 0,13

1. **EAC für Projekt** = 225 Stunden, berechnet wie folgt:\
   **EAC für Projekt** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + realisiert  Stunden\
   **EAC für Projekt** = 30 / .13333\
   **EAC für Projekt** = 225 Stunden

#### Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben {#complicated-example-project-has-children-tasks}

PIM = Stunde-basiert

EAC-Methode = Auf Projektebene berechnen

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
   <th> <br> <p><strong>Akt hrs</strong> </p> </th> 
   <th> <p><strong>% Complete</strong> </p> </th> 
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
   <td> <p>20 %</p> </td> 
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
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>15 Stunden</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>20 Stunden</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie dem Projekt 50 Stunden direkt hinzu (Mehr > Stunden > Protokollzeiten).
1. **CPI für Aufgabe 2** = .1, berechnet wie folgt:\
   **CPI für Aufgabe 2** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Aufgabe 2** = 1/10\
   **CPI für Aufgabe 2** = .1

1. **EAC für Aufgabe 2** = 50 Stunden, berechnet wie folgt:\
   **EAC für Aufgabe 2** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + realisiert  Stunden\
   **EAC für Aufgabe 2** = 5 / .1\
   **EAC für Aufgabe 2** = 50 Stunden

1. CPI/EAC für die Aufgaben 4, 5 und 6 lauten wie folgt:\
   Aufgabe 4: 0,4 / 25 Stunden\
   Aufgabe 5: 0,75 / 20 Stunden\
   Aufgabe 6: 1.2 / 16.67 Std.

1. **CPI für Aufgabe 3** = 0,38  berechnet wie folgt:\
   **CPI für Aufgabe 3** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Aufgabe 3** = 11,5 / 30\
   **CPI für Aufgabe 3** = 0,38

1. **EAC für Aufgabe 3** = 65,22 Std. berechnet wie folgt:\
   **EAC für Aufgabe 3** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + realisiert  Stunden\
   **EAC für Aufgabe 3** =  25 / 383333\
   **EAC für Aufgabe 3** = 65,22 Stunden

1. **CPI für Aufgabe 1** = .25, berechnet wie folgt:\
   **CPI für Aufgabe 1** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Aufgabe 1** = 12,5 / 50\
   **CPI für Aufgabe 1** = 0,25

1. **EAC für Aufgabe 1** = 120 Stunden, berechnet wie folgt:\
   **EAC für Aufgabe 1** = *IF* CPI &lt;> 0 *DANN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + realisiert  Stunden\
   **EAC für Aufgabe 1** =  30.25\
   **EAC für Aufgabe 1** = 120 Stunden

1. **CPI für Projekt** = .22, berechnet wie folgt:\
   **CPI für Projekt** = *IF* Actual Hours > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Projekt** = 24,5 / 110\
   **CPI für Projekt** = .2272\
   **CPI für Projekt** = 0,22

1. **EAC für Projekt** = 224.49  wird wie folgt berechnet:\
   **EAC für Projekt** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + realisiert  Stunden\
   **EAC für Projekt** =  50 / .22272\
   **EAC für Projekt** = 224,49 Stunden

### PIM = Kostenbasiert {#pim-cost-based}

* [Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben](#simple-example-project-has-no-children-tasks)
* [Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben](#complicated-example-project-has-children-tasks)

#### Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben {#simple-example-project-has-no-children-tasks-1}

PIM = Kostenbasiert

EAC-Methode = Auf Projektebene berechnen

1. Erstellen Sie Projekt A mit drei Aufgaben (keine untergeordneten Aufgaben), die Benutzer 1 zugewiesen sind und deren Kosten/Stunde 100,00 USD beträgt.
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
   <th> <br> <p><strong>PLN-LBR-Kosten</strong> </p> </th> 
   <th> <br> <p><strong>Akt hrs</strong> </p> </th> 
   <th> <br> <p><strong>LBR-Kosten verwalten</strong> </p> </th> 
   <th> <p><strong>% Complete</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>5 Stunden</p> </td> 
   <td> <p>500,00$</p> </td> 
   <td> <p>25 Stunden</p> </td> 
   <td> <p>2.500,00$</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>25 Stunden</p> </td> 
   <td> <p>2.500,00$</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>15 Stunden</p> </td> 
   <td> <p>1.500,00$</p> </td> 
   <td> <p>25 Stunden</p> </td> 
   <td> <p>2.500,00$</p> </td> 
   <td> <p>40 %</p> </td> 
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
   <th> <p><strong>Kosten</strong> </p> </th> 
   <th> <p><strong>Geplanter Betrag</strong> </p> </th> 
   <th> <p><strong>Tatsächlicher Betrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Exp1</p> </td> 
   <td> <p>300,00$</p> </td> 
   <td> <p>400,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Exp2</p> </td> 
   <td> <p>500,00$</p> </td> 
   <td> <p>0,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Exp</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>Aufgabe 3 Exp</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>$ 700.00</p> </td> 
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
   <th> <p><strong>Kosten</strong> </p> </th> 
   <th> <p><strong>Geplanter Betrag</strong> </p> </th> 
   <th> <p><strong>Tatsächlicher Betrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projekt Exp 1</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>1.500,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1 Exp2</p> </td> 
   <td> <p>2.500,00$</p> </td> 
   <td> <p>0,00$</p> </td> 
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
   <th> <p><strong>Vorgesehene Ausgaben</strong> </p> </th> 
   <th> <p><strong> Anfallende tatsächliche Kosten</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>500,00$</p> </td> 
   <td> <p>300,00$</p> </td> 
   <td> <p>400,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>0,00$</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>0,00$</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>$ 700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>3.000,00 $</p> </td> 
   <td> <p>2.300,00$</p> </td> 
   <td> <p> 2.700,00$ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Führen Sie über Projektaktionen die Option Finanzen neu berechnen aus.
1. **CPI für Aufgabe 1** = 0,14
1. **CPI*** für Aufgabe 1** = .14 berechnet wie folgt:\
   **CPI**  **für Aufgabe 1** = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labour\
   **CPI***für Aufgabe 1** = (100+300) / (2500+400)\
   **CPI**  **für Aufgabe 1** = 400 / 2900\
   **CPI**  **für Aufgabe 1**  = .14****

1. **EAC***für Aufgabe 1** = 13.400,00 USD\
   **CPI-Arbeit**  **für Aufgabe 1** = WENN die tatsächlichen Arbeitskosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI-Arbeit**  **für Aufgabe 1** = 100/2500\
   **CPI-Arbeit**  **für Aufgabe 1** = .04 ****** EAC Labour ****für Aufgabe 1 **=*IF *CPI_Labour &lt;> 0*DANN *EAC Labour = Geplante Arbeitskosten/CPI_Labour\
   *    ELSE* EAC  Arbeit = Geplante Arbeitskosten + tatsächliche Arbeitskosten\
   **EAC-Arbeit ****für Aufgabe 1** = 500.00/.04\
   **EAC Labour***für Aufgabe 1** = 12.500,00 USD\
   **EAC-Ausgaben*** für Aufgabe 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgaben****für Aufgabe 1** = 400,00 $ + 500,00 $\
   **EAC-Ausgaben*** für Aufgabe 1** = 900,00 USD\
   **EAC***für Aufgabe 1** = EAC-Arbeitskosten + EAC-Ausgaben\
   **EAC***für Aufgabe 1**  = 12.500,00 $ + 900,00 $\
   **EAC***für Aufgabe 1**  = 13.400,00 $

1. Im Folgenden finden Sie die CPI-/EAC-Werte für Aufgabe 2 und Aufgabe 3:\
   Aufgabe 2 = 0,19 / 8.433,33 $\
   Aufgabe 3 = 0,44 / 6.950,00 $

1. **CPI für Projekt** = .32, berechnet wie folgt:\
   **CPI*** für Projekt** = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour\
   **CPI*** für Projekt** = (1000 + 2300) / (7500 + 2700)\
   **CPI*** für Projekt** = 3300 / 10200\
   **CPI*** für Projekt** = .32

1. **EAC für Projekt** = 28.200,00 USD, berechnet wie folgt:\
   **CPI-Arbeit*** für Projekt** = WENN die tatsächlichen Arbeitskosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI-Arbeit*** für Projekt** = 1000 / 7500\
   **CPI-Arbeit*** für Projekt** = .13333\
   **CPI-Arbeit*** für Projekt** = .13

   **EAC Labour*** für Projekt** = *IF* CPI_Labour &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Arbeit = Geplante Arbeitskosten + tatsächliche Arbeitskosten\
   **EAC-Arbeit*** für Projekt** = 3000/ .13333\
   **EAC-Arbeit*** für Projekt** = 22.500,00 USD

   **EAC-Ausgaben***Projekt** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC-Ausgaben***Projekt** = 3000,00 $ + 2.700,00 $\
   **EAC-Ausgaben***Projekt** = 5.700,00 USD

   **EAC***Projekt** = EAC-Arbeitskosten + EAC-Ausgaben\
   **EAC***Projekt**  = 22.500,00 $ + 5.700,00 $\
   **EAC***Projekt**  = 28.200,00 $

#### Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben {#complicated-example-project-has-children-tasks-1}

PIM = Kostenbasiert

EAC-Methode = Auf Projektebene berechnen

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
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <br> <p><strong>Gpl. Std.</strong> </p> </th> 
   <th> <br> <p><strong>PLN-LBR-Kosten</strong> </p> </th> 
   <th> <br> <p><strong>Akt hrs</strong> </p> </th> 
   <th> <br> <p><strong>LBR-Kosten verwalten</strong> </p> </th> 
   <th> <p><strong>% Complete</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>5 Stunden</p> </td> 
   <td> <p>500,00$</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>15 Stunden</p> </td> 
   <td> <p>1.500,00$</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>20 Stunden</p> </td> 
   <td> <p>2.000,00 $</p> </td> 
   <td> <p>10 Stunden</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie dem Projekt 50 Stunden direkt hinzu (Mehr > Stunden > Protokollzeiten), sodass 5.000,00 USD der tatsächlichen Arbeitskosten direkt im Projekt erfasst werden. ****
1. Fügen Sie den Aufgaben die Ausgaben entsprechend der unten stehenden Tabelle hinzu (ich habe zwischen den einzelnen Aufgaben eine leere Zeile eingefügt, um das Lesen zu erleichtern):

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <p><strong>Kosten</strong> </p> </th> 
   <th> <p><strong>Geplanter Betrag</strong> </p> </th> 
   <th> <p><strong>Tatsächlicher Betrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Exp1</p> </td> 
   <td> <p>300,00$</p> </td> 
   <td> <p>- $ 400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Exp2</p> </td> 
   <td> <p>- 500,00$</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Exp3</p> </td> 
   <td> <p>400,00$</p> </td> 
   <td> <p>0,00$</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Exp 1</p> </td> 
   <td> <p>500,00$</p> </td> 
   <td> <p>$ 700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Exp 2</p> </td> 
   <td> <p>- $ 400.00</p> </td> 
   <td> <p>0,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Exp 3</p> </td> 
   <td> <p>- 200,00$</p> </td> 
   <td> <p>600,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Exp 4</p> </td> 
   <td> <p>$ 700.00</p> </td> 
   <td> <p>- 200,00$</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>Aufgabe 3 Exp</p> </td> 
   <td> <p>0,00$</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>Aufgabe 4 Exp 1</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>0,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>Aufgabe 4 Exp 2</p> </td> 
   <td> <p>- 100,00$</p> </td> 
   <td> <p>300,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4 </p> </td> 
   <td> <p>Aufgabe 4 Exp 3</p> </td> 
   <td> <p>-200,00</p> </td> 
   <td> <p>0,00$</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>Aufgabe 5 Exp 1</p> </td> 
   <td> <p>$ 700.00</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>Aufgabe 5 Exp 2</p> </td> 
   <td> <p>- 100,00$</p> </td> 
   <td> <p>300,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>Aufgabe 5 Exp 3</p> </td> 
   <td> <p>- $ 400.00</p> </td> 
   <td> <p>- 200,00$</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>Aufgabe 6 Exp 1</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>$ 700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>Aufgabe 6 Exp 2</p> </td> 
   <td> <p>500,00$</p> </td> 
   <td> <p>-$ 300.0</p> </td> 
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
   <th> <p><strong>Kosten</strong> </p> </th> 
   <th> <p><strong>Geplanter Betrag</strong> </p> </th> 
   <th> <p><strong>Tatsächlicher Betrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projekt Exp 1</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
   <td> <p>1.500,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1 Exp2</p> </td> 
   <td> <p>2.500,00$</p> </td> 
   <td> <p> 0,00$ <strong></strong></p> </td> 
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
   <th> <p><strong>Vorgesehene Ausgaben</strong> </p> </th> 
   <th> <p><strong> Anfallende tatsächliche Kosten</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>400,00$</p> </td> 
   <td> <p>- 500,00$</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>- $ 400.00</p> </td> 
   <td> <p>300,00$</p> </td> 
   <td> <p>1.300,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>0,00$</p> </td> 
   <td> <p>0,00$</p> </td> 
   <td> <p>1.000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>- 100,00$</p> </td> 
   <td> <p>300,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>0,00$</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>1.100,00$</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>0,00$</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>$ 700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>2.500,00$</p> </td> 
   <td> <p>1000,00$</p> </td> 
   <td> <p>1.500,00$</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Führen Sie über Projektaktionen die Option Finanzen neu berechnen aus.
1. **CPI** für Aufgabe 2 = .17, berechnet wie folgt:\
   **CPI-Aufgabe 2** = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost  &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLabourCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labour\
   **CPI***Aufgabe 2** = (100+300) / (1000+1300)\
   **CPI***Aufgabe 2**  = 400/2300\
   **CPI***Aufgabe 2**  = 0,17

1. **EAC** für Aufgabe 2 = 5.900,00 USD\
   **CPI-Arbeit***Aufgabe 2** = IF Tatsächliche Arbeitskosten &lt;> 0 DANN CPI_Labour = TotalBudgetedCostWorkPerformed/Tatsächliche Arbeitskosten\
      ELSE CPI_Labour = 1\
   **CPI-Arbeit***Aufgabe 2** = 100/1000\
   **CPI Labour***Aufgabe 2** = .1

   **EAC Labour***Aufgabe 2** = *IF* CPI_Labour &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Arbeit = Geplante Arbeitskosten + tatsächliche Arbeitskosten\
   **EAC Labour***Aufgabe 2** = 500.00/.1\
   **EAC Labour***Aufgabe 2** = 5.000,00 $****** EAC-Ausgaben ****Aufgabe 2 **= IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgaben ****Aufgabe 2** = 1.300,00 $ + -$400,00\
   **EAC-Ausgaben***Aufgabe 2** = 900,00 USD

   **EAC***Aufgabe 2** = EAC-Arbeitskosten + EAC-Ausgaben\
   **EAC***Aufgabe 2**  = 5.000,00 $ + 900,00 $\
   **EAC***Aufgabe 2**  = 5.900,00 $

1. Der CPI/EAC für die Aufgaben 4, 5 und 6 wird auf die gleiche Weise bestimmt, sodass ich nur die folgenden Werte bereitstellen werde:\
   Aufgabe 4: 0,23 / 3.400,00 $\
   Aufgabe 5: 0,64 / 3.100,00 $\
   Aufgabe 6: 1.06 / 2.366,67 $

1. CPI für Aufgabe 3 = .31, berechnet wie folgt:\
   **CPI***Aufgabe 3** = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour\
   **CPI***Aufgabe 3**  = (1.150 + 500) / (3000 + 2400)\
   **CPI***Aufgabe 3**  =  1650/5400\
   **CPI***Aufgabe 3**  = .31 ****** EAC für Aufgabe 3 **= 9.521,74 USD, berechnet wie folgt:\
   **CPI-Arbeit ****Aufgabe 3** = WENN die tatsächlichen Arbeitskosten &lt;> 0

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI-Arbeit***Aufgabe 3** = 1150/3000\
   **CPI-Arbeit***Aufgabe 3** = .383333\
   **CPI-Arbeit***Aufgabe 3** = .38

   **EAC Labour***Aufgabe 3** = *IF* CPI_Labour &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Arbeit = Geplante Arbeitskosten + tatsächliche Arbeitskosten\
   **EAC-Arbeit***Aufgabe 3** = 2.500,00 $ / .383333 $\
   **EAC-Arbeit***Aufgabe 3** = 6.521,74 USD

   **EAC-Ausgaben***Aufgabe 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgaben***Aufgabe 3** = 2.400,00 $ + 600,00 $\
   **EAC-Ausgaben***Aufgabe 3** = 3.000,00 $

   **EAC***Aufgabe 3** = EAC-Arbeitskosten + EAC-Ausgaben\
   **EAC***Aufgabe 3**  = 6.521,74 $ + 3.000,00 $\
   **EAC***Aufgabe 3**  = 9.521,74 $

1. CPI für Aufgabe 1 = .16, berechnet wie folgt:\
   **CPI***Aufgabe 1** = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour\
   **CPI***Aufgabe 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI***Aufgabe 1**  =  1550 / 9500=\
   **CPI***Aufgabe 1**  = 0,16

1. Der EAC für Aufgabe 1 beträgt 17.100,00 $ und wird wie folgt berechnet:\
   **CPI-Arbeit***Aufgabe 1** = WENN die tatsächlichen Arbeitskosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI-Arbeit***Aufgabe 1** = 1250 / 5000\
   **CPI-Arbeit***Aufgabe 1** = .25

   **EAC Labour***Aufgabe 1** = *IF* CPI_Labour &lt;> 0 *DANN* EAC Labour = Geplante Arbeitskosten / CPI_Labour\
   *   ELSE* EAC  Arbeit = Geplante Arbeitskosten + tatsächliche Arbeitskosten\
   **EAC-Arbeit***Aufgabe 1** = 3.000,00 $ / 0,25\
   **EAC-Arbeit***Aufgabe 1** = 12.000,00 $

   **EAC-Ausgaben***Aufgabe 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgaben***Aufgabe 1** = 4500 $ + 600 $\
   **EAC-Ausgaben***Aufgabe 1** = 5.100,00 USD

   **EAC***Aufgabe 1** = EAC-Arbeitskosten + EAC-Ausgaben\
   **EAC***Aufgabe 1**  = $12.000.00 + 5.100.00\
   **EAC***Aufgabe 1**  = 17.100,00 $

1. CPI für Projekt ist 0,25\
   **CPI*** für Projekt** = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour

   **CPI*** für Projekt** = (2450 + 1900) / (11000 + 6700)\
   **CPI*** für Projekt** =   4350/17700\
   **CPI*** für Projekt** = .25

1. **EAC für Projekt** = 32.248,98 USD, berechnet wie folgt:\
   **CPI-Arbeit*** für Projekt** = WENN die tatsächlichen Arbeitskosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI-Arbeit*** für Projekt** = 2450 / 11000\
   **CPI-Arbeit*** für Projekt** = .2272\
   **CPI-Arbeit*** für Projekt** = .22

   **EAC Labour*** für Projekt** = *IF* CPI_Labour &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Arbeit = Geplante Arbeitskosten + tatsächliche Arbeitskosten\
   **EAC-Arbeit*** für Projekt** = 5.000,00 $ / .22272\
   **EAC-Arbeit*** für Projekt** = 22.448,97959 $\
   **EAC-Arbeit*** für Projekt** = 22.448,98 USD

   **EAC-Ausgaben***Projekt** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgaben***Projekt** = 3.100,00 $ + 6.700,00 $\
   **EAC-Ausgaben***Projekt** = 9.800,00 USD

   **EAC***Projekt** = EAC-Arbeitskosten + EAC-Ausgaben\
   **EAC***Projekt**  = 22.448,98 $ + 9.800,00 $\
   **EAC***Projekt**  = 32.248,98 $
