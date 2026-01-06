---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Berechnungsbeispiel - EAC als Rollup aus Aufgaben berechnen
description: In diesem Artikel finden Sie ein Beispiel für die Berechnung der Kalkulation bei Abschluss (EAC) eines Projekts als Datenaggregation aus allen Projektaufgaben in Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 2%

---

# Berechnungsbeispiel - EAC als Rollup aus Aufgaben berechnen

## EAC-Methode: aus Aufgaben oder Teilaufgaben aggregieren

* [PIM= stundenbasiert](#pim-hour-based)
* [PIM= kostenbasiert](#pim-cost-based)

### PIM= stundenbasiert {#pim-hour-based}

* [Einfaches Beispiel: Das Projekt hat keine untergeordneten Aufgaben](#simple-example-project-has-no-children-tasks)
* [Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben](#complicated-example-project-has-children-tasks)

#### Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben {#simple-example-project-has-no-children-tasks}

PIM = stundenbasiert

EAC-Methode = Datenaggregation aus Aufgaben/Teilaufgaben

1. Erstellen Sie Projekt A mit drei Aufgaben (keine untergeordneten Aufgaben), die alle Benutzer 1 zugewiesen sind und deren Kosten/Std. 100,00 USD betragen.
1. Fügen Sie jeder Aufgabe die geplanten/tatsächlichen Stunden hinzu und % abgeschlossen gemäß nachstehender Tabelle:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <br> <p><strong>Gpl. Std.</strong> </p> </th> 
   <th> <br> <p><strong>Tats. Std</strong> </p> </th> 
   <th> <p><strong>% abgeschlossen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>5 Std</p> </td> 
   <td> <p>25 Std</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>25 Std</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>15 Std</p> </td> 
   <td> <p>25 Std</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Finanzdaten neu berechnen
1. **CPI für Aufgabe 1** = .04 wie folgt berechnet:\
   **CPI für Aufgabe 1** = *IF* Tatsächliche Stunden > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
   *ELSE* CPI = 1\
   **CPI für Aufgabe 1** = 1 / 25\
   **CPI für Aufgabe 1** = .04

1. **EAC für Aufgabe 1** = 125 Stunden wie folgt berechnet:\
   **EAC für Aufgabe 1** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/ CPI\
   *SONST*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC für Aufgabe 1** = 5 / .04\
   **EAC für Aufgabe 1** = 125 Stunden

1. CPI/EAC für Aufgaben 2 und 3:\
   Aufgabe 2 = .12 / 83.33 Uhr\
   Aufgabe 3 = .24 / 62,5 Stunden

1. **CPI für Projekt** = .13 wie folgt berechnet:\
   **CPI für Projekt** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI für Projekt** = 10 / 75\
   **CPI für Projekt** = .13

1. **EAC für Projekt** = 270,83 Stunden wie folgt berechnet\
   **EAC für Projekt** = EAC-Aufgabe 1 + EAC-Aufgabe 2 + EAC-Aufgabe 3\
   **EAC für Projekt** = 125 + 83,33 + 62,5\
   **EAC für Projekt** = 270,83 Stunden

#### Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben {#complicated-example-project-has-children-tasks}

PIM = stundenbasiert

EAC-Methode = Datenaggregation aus Aufgaben/Teilaufgaben

1. Erstellen Sie Projekt A mit sechs Aufgaben, wobei Aufgabe 3 den Aufgaben 4 und 5 übergeordnet ist und Aufgabe 1 den Aufgaben 2 und 3 übergeordnet ist, wie unten dargestellt:\
   Aufgabe 1\
   Aufgabe 2\
   Aufgabe 3\
   Aufgabe 4\
   Aufgabe 5\
   Aufgabe 6

1. Weisen Sie Benutzer 1 die Aufgaben 2, 4, 5 und 6 zu, deren Kosten/Std.-Satz 100,00 $ beträgt.
1. Fügen Sie die geplanten/tatsächlichen Stunden für jede Aufgabe und % Abgeschlossen gemäß der folgenden Tabelle hinzu.

   >[!NOTE]
   >
   >Für die Aufgaben 1 und 3 werden nur die tatsächlichen Stunden hinzugefügt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <br> <p><strong>Gpl. Std.</strong> </p> </th> 
   <th> <br> <p><strong>Tats. Std</strong> </p> </th> 
   <th> <p><strong>% abgeschlossen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> </td> 
   <td> <p>10 Std</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>5 Std</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> </td> 
   <td> <p>10 Std</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>15 Std</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>20 Std</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie 50 Stunden direkt zum Projekt hinzu (Mehr>Stunden>Stunden protokollieren), sodass 5.000,00 USD der tatsächlichen Lohnkosten direkt im Projekt erfasst werden.
1. Neuberechnung der Finanzen ausführen
1. **CPI für Aufgabe 2** = .1 Berechnet wie folgt:\
   **CPI für Aufgabe 2** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI für Aufgabe 2** = 1 / 10\
   **CPI für Aufgabe 2** = .1

1. **EAC für Aufgabe 2** = 50 Stunden wie folgt berechnet:\
   **EAC für Aufgabe 2** = *IF* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = Geplante Stunden + Tatsächliche Stunden
   **EAC für Aufgabe 2** = 5 / .1\
   **EAC für Aufgabe 2** = 50 Stunden

1. CPI/EAC für Aufgabe 4, Aufgabe 5 und Aufgabe 6:\
   Aufgabe 4 = .4 / 25 Stunden\
   Aufgabe 5 = .75 / 20 Stunden\
   Aufgabe 6 = 1,2 / 16,67 Stunden

1. **CPI für Aufgabe 3** = .38\
   **CPI für Aufgabe 3** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI für Aufgabe 3** = 11,5 / 30\
   **CPI für Aufgabe 3** = .38

1. **EAC für Aufgabe 3** = EAC-Aufgabe 4 + EAC-Aufgabe 5\
   **BK für Aufgabe 3** = 25 + 20\
   **EAC für Aufgabe 3** = 45 Stunden

1. **CPI für Aufgabe 1** = .25 wie folgt berechnet:\
   **CPI für Aufgabe 1** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI für Aufgabe 1** = 12,5 / 50\
   **CPI für Aufgabe 1** = .25

1. **EAC für Aufgabe 1** = EAC-Aufgabe 2 + EAC-Aufgabe 3\
   **BK für Aufgabe 1** = 50 + 45\
   **EAC für Aufgabe 1** = 95 Stunden

1. CPI für Projekt = .22 wie folgt berechnet:\
   **CPI für Projekt** = *IF* Tatsächliche Stunden > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1
   **CPI für Projekt** = 24,5 / 110\
   **CPI für Projekt** = .22272\
   **CPI für Projekt** = .22

1. **EAC für Projekt** = EAC Aufgabe 1 + EAC Aufgabe 6\
   **EAC für Projekt** = 95 + 16,67\
   **EAC für Projekt** = 111,67 Stunden

### PIM= kostenbasiert {#pim-cost-based}

* [Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben](#simple-example-project-has-no-children-tasks)

#### Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben {#simple-example-project-has-no-children-tasks-1}

PIM = kostenbasiert

EAC-Methode = Datenaggregation aus Aufgaben/Teilaufgaben

1. Erstellen Sie Projekt A mit drei Aufgaben (keine untergeordneten Aufgaben), die alle Benutzer 1 zugewiesen sind, deren Kosten/Std. 100,00 USD beträgt.
1. Fügen Sie jeder Aufgabe die geplanten/tatsächlichen Stunden hinzu und % abgeschlossen gemäß nachstehender Tabelle:

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
   <th> <br> <p><strong>Gpl. Lohnkosten</strong> </p> </th> 
   <th> <br> <p><strong>Tats. Std</strong> </p> </th> 
   <th> <br> <p><strong>Ist-Lohnkosten</strong> </p> </th> 
   <th> <p><strong>% abgeschlossen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>5 Std</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>25 Std</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>25 Std</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>30 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>15 Std</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
   <td> <p>25 Std</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie jeder Aufgabe Ausgaben gemäß der folgenden Tabelle hinzu:

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
   <td> <p>Aufgabe 1 Ausl. 1</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Ausl. 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Ausl</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>Aufgabe 3 Ausl</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie dem Projekt zwei Ausgaben hinzu (d. h., die nicht an eine Aufgabe gebunden sind):

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
   <td> <p>Projektausgabe 1</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1 Ausl. 2</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Anhand der oben genannten Werte werden die angefallenen/nicht angefallenen Kosten wie folgt ermittelt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aufgabe</strong> </p> </th> 
   <th> <p><strong>Keine geplanten Ausgaben angefallen</strong> </p> </th> 
   <th> <p><strong>Geplante Ausgaben</strong> </p> </th> 
   <th> <p><strong>Ist-Kosten angefallen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>200,00 $</p> </td> 
   <td> <p>100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>3 000,00 $</p> </td> 
   <td> <p>2 300,00 $</p> </td> 
   <td> <p>2 700,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Führen Sie in Projektaktionen die Option Finanzen neu berechnen aus.
1. **CPI****für Aufgabe 1** = .14 wie folgt berechnet:\
   **CPI****für Aufgabe 1** = *IF* Ist-Lohnkosten + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labour\
     **CPI****für Aufgabe 1** = (100+300) / (2500+400)\
     **CPI****für Aufgabe 1** = 400 / 2900\
     **CPI****für Aufgabe 1** = .14

1. **EAC****für Aufgabe 1** = 13.400,00 $\
   **CPI Labor****for Task 1** = IF Actual Labour Cost &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labour = 1\
   **CPI Labor****für Aufgabe 1** = 100/2500\
   **CPI Labor****für Aufgabe 1** = .04

   **EAC Labor****für Aufgabe 1** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * SONSTIGE* EAC-Arbeitskosten = Geplante Arbeitskosten + Ist-Arbeitskosten\
     **EAC Arbeit****für Aufgabe 1** = 500.00/.04\
     **EAC Labor****für Aufgabe 1** = 12.500,00 $

   **EAC-Ausgabe****für Aufgabe 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-**** für Aufgabe 1** = 400,00 $ + 500,00 $\
   **EAC-Ausgabe****für Aufgabe 1** = 900,00 $

   **EAC****für Aufgabe 1** = EAC-Arbeitsaufwand + EAC-Ausgaben\
   **EAC****für Aufgabe 1** = 12.500,00 $ + 900,00 $\
   **EAC****für Aufgabe 1** = 13.400,00 $

1. Im Folgenden finden Sie die CPI-/EAC-Werte für Aufgabe 2 und Aufgabe 3:\
   Task 2 = .19 / $ 8.433,33\
   Task 3 = .44 / $6.950.00****

1. Der CPI für das Projekt = .32\
   **CPI****für Projekt** = *IF* Tatsächliche Arbeitskosten + IncurredActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labour\
     **CPI****für Projekt** = (1000 + 2300) / (7500 + 2700)\
     **CPI****für Projekt** = 3300 / 10200\
     **CPI****for Project** = .32

1. EAC für das Projekt beträgt $28.783,33\
   **EAC****für Projekt** = EAC Aufgabe 1 + EAC Aufgabe 2 + EAC Aufgabe 3\
   **EAC****für Projekt** = 13.400,00 $ + 8.433,33 $ + 6.950,00 $\
   **EAC****für Projekt** = 28.783,33 $
