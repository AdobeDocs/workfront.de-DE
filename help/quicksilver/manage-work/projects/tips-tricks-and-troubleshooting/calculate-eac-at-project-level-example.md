---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Berechnungsbeispiel - EAC auf Projektebene berechnen
description: In diesem Artikel finden Sie ein Beispiel für die Berechnung der Kalkulation bei Abschluss (EAC) eines Projekts auf Projektebene in Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '2214'
ht-degree: 1%

---

# Berechnungsbeispiel - EAC auf Projektebene berechnen

## EAC-Methode: Auf Projektebene berechnen

* [PIM = stundenbasiert](#pim-hour-based)
* [PIM= kostenbasiert](#pim-cost-based)

### PIM = stundenbasiert {#pim-hour-based}

* [Einfaches Beispiel: Das Projekt hat keine untergeordneten Aufgaben](#simple-example-project-has-no-children-tasks)
* [Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben](#complicated-example-project-has-children-tasks)

#### Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben {#simple-example-project-has-no-children-tasks}

PIM = stundenbasiert

EAC-Methode = Berechnung auf Projektebene **&#x200B;**

1. Erstellen Sie Projekt A mit drei Aufgaben (keine untergeordneten Aufgaben), die alle Benutzer 1 zugewiesen sind und deren Kosten/Std. 100,00 USD betragen.
1. Fügen Sie jeder Aufgabe die geplanten und tatsächlichen Stunden und % Abgeschlossen hinzu, wie in der folgenden Tabelle dargestellt:

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
      <td><p>5 Std</p></td>
      <td><p>25 Std</p></td>
      <td><p>20 %</p></td>
     </tr>
     <tr>
      <td><p>Aufgabe 2</p></td>
      <td><p>10 Std</p></td>
      <td><p>25 Std</p></td>
      <td><p>30 %</p></td>
     </tr>
     <tr>
      <td><p>Aufgabe 3</p></td>
      <td><p>15 Std</p></td>
      <td><p>25 Std</p></td>
      <td><p>40 %</p></td>
     </tr>
    </tbody>
   </table>

1. Finanzdaten für das Projekt neu berechnen
1. **CPI für Aufgabe 1** = .04 wie folgt berechnet:\
   **CPI für Aufgabe 1** = *IF* Tatsächliche Stunden > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
      *ELSE* CPI = 1\
   **CPI für Aufgabe 1** = 1 / 25\
   **CPI für Aufgabe 1** = .04

1. **EAC für Aufgabe 1** = 125 Stunden wie folgt berechnet:\
   **EAC für Aufgabe 1** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + tatsächlich  Stunden\
   **EAC für Aufgabe 1** = 5 / .04\
   **EAC für Aufgabe 1** = 125 Stunden&#x200B;**&#x200B;**

1. CPI/EAC für Aufgaben 2 und 3:\
   Aufgabe  2 = .12 / 83,33  Std.\
   Aufgabe 3 = .24 / 62,5 Stunden

1. **CPI für Projekt** = .13 wie folgt berechnet:\
   **CPI für Projekt** = *IF* Tatsächliche Stunden > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Projekt** = 10 / 75\
   **CPI für Projekt** = .13

1. **EAC für Projekt** = 225 Stunden wie folgt berechnet:\
   **EAC für Projekt** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + tatsächlich  Stunden\
   **EAC für Projekt** = 30 / .13333\
   **EAC für Projekt** = 225 Stunden

#### Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben {#complicated-example-project-has-children-tasks}

PIM = stundenbasiert

EAC-Methode = Berechnung auf Projektebene

1. Erstellen Sie Projekt A mit sechs Aufgaben, wobei Aufgabe 3 den Aufgaben 4 und 5 übergeordnet ist und Aufgabe 1 den Aufgaben 2 und 3 übergeordnet ist, wie unten dargestellt:\
   Aufgabe 1\
      Aufgabe 2\
      Aufgabe 3\
         Aufgabe 4\
         Aufgabe 5\
   Aufgabe 6

1. Weisen Sie Benutzer 1 die Aufgaben 2, 4, 5 und 6 zu, deren Kosten/Std.-Satz 100,00 $ beträgt.
1. Fügen Sie die geplanten/tatsächlichen Stunden für jede Aufgabe hinzu und % abgeschlossen gemäß der folgenden Tabelle.

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
   <td> </td> 
   <td> <p>10 Std</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>5 Std</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> </td> 
   <td> <p>10 Std</p> </td> 
   <td> </td> 
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

1. Fügen Sie 50 Stunden direkt zum Projekt hinzu (Mehr>Stunden>Stunden protokollieren).
1. **CPI für Aufgabe 2** = .1 Berechnet wie folgt:\
   **CPI für Aufgabe 2** = *IF* Tatsächliche Stunden > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Aufgabe 2** = 1 / 10\
   **CPI für Aufgabe 2** = .1

1. **EAC für Aufgabe 2** = 50 Stunden wie folgt berechnet:\
   **EAC für Aufgabe 2** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + tatsächlich  Stunden\
   **EAC für Aufgabe 2** = 5 / .1\
   **EAC für Aufgabe 2** = 50 Stunden

1. CPI/EAC für Aufgaben 4, 5 und 6:\
   Aufgabe 4: .4 / 25 Stunden\
   Aufgabe 5: .75 / 20 Std\
   Aufgabe 6: 1,2/16,67 Uhr

1. **CPI für Aufgabe 3** = .38  Wird wie folgt berechnet:\
   **CPI für Aufgabe 3** = *IF* Tatsächliche Stunden > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Aufgabe 3** = 11,5 / 30\
   **CPI für Aufgabe 3** = .38

1. **EAC für Aufgabe 3** = 65,22 Stunden wie folgt berechnet:\
   **EAC für Aufgabe 3** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + tatsächlich  Stunden\
   **EAC für Aufgabe 3** =  25 / .383333\
   **EAC für Aufgabe 3** = 65,22 Stunden

1. **CPI für Aufgabe 1** = .25 wie folgt berechnet:\
   **CPI für Aufgabe 1** = *IF* Tatsächliche Stunden > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Aufgabe 1** = 12,5 / 50\
   **CPI für Aufgabe 1** = .25

1. **EAC für Aufgabe 1** = 120 Stunden wie folgt berechnet:\
   **EAC für Aufgabe 1** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden / CPI\
       *ELSE* EAC = Geplant  Stunden + tatsächlich  Stunden\
   **EAC für Aufgabe 1** =  30/.25\
   **EAC für Aufgabe 1** = 120 Stunden

1. **CPI für Projekt** = .22 wie folgt berechnet:\
   **CPI für Projekt** = *IF* Tatsächliche Stunden > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI für Projekt** = 24,5 / 110\
   **CPI für Projekt** = .22272\
   **CPI für Projekt** = .22

1. **EAC für Projekt** = 224,49  Std. wie folgt berechnet:\
   **EAC für Projekt** = *IF* CPI &lt;> 0 *THEN* EAC = Geplante Stunden/CPI\
       *ELSE* EAC = Geplant  Stunden + tatsächlich  Stunden\
   **EAC für Projekt** =  50 / .22272\
   **EAC für Projekt** = 224,49 Stunden

### PIM= kostenbasiert {#pim-cost-based}

* [Einfaches Beispiel: Das Projekt hat keine untergeordneten Aufgaben](#simple-example-project-has-no-children-tasks)
* [Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben](#complicated-example-project-has-children-tasks)

#### Einfaches Beispiel: Projekt hat keine untergeordneten Aufgaben {#simple-example-project-has-no-children-tasks-1}

PIM = kostenbasiert

EAC-Methode = Berechnung auf Projektebene

1. Erstellen Sie Projekt A mit drei Aufgaben (keine untergeordneten Aufgaben), die alle Benutzer 1 zugewiesen sind und deren Kosten/Std. 100,00 USD betragen.
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
   <td> <p> 2 700,00 $ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Führen Sie in Projektaktionen die Option Finanzen neu berechnen aus.
1. **CPI für Aufgabe 1** = .14
1. **CPI**&#x200B;**für Aufgabe 1** = .14 wie folgt berechnet:\
   **CPI**  **für Aufgabe 1** = *IF* Ist-Lohnkosten + IncurredActualExpenseCost  &lt;> 0 *DANN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labour\
   **CPI**&#x200B;**für Aufgabe 1** = (100+300) / (2500+400)\
   **CPI**  **für Aufgabe 1** = 400 / 2900\
   **CPI**  **für Aufgabe 1**  = .14&#x200B;**&#x200B;**

1. **EAC**&#x200B;**für Aufgabe 1** = 13.400,00 $\
   **CPI Labor**  **für Aufgabe 1** = WENN Ist-Lohnkosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI Labor**  **für Aufgabe 1** = 100/2500\
   **CPI Labor**  **für Aufgabe 1** = .04 **&#x200B;**&#x200B;**&#x200B; EAC Arbeit &#x200B;**&#x200B;**für Aufgabe 1 &#x200B;**=*IF *CPI_Labor &lt;> 0*THEN *EAC Arbeit = Geplante Lohnkosten/CPI_Labor\
   *    SONST* EAC  Arbeit = Geplante Arbeitskosten + Ist-Arbeitskosten\
   **EAC Arbeit &#x200B;**&#x200B;**für Aufgabe 1** = 500.00/.04\
   **EAC Labor**&#x200B;**für Aufgabe 1** = 12.500,00 $\
   **EAC-Ausgabe**&#x200B;**für Aufgabe 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-**&#x200B;**&#x200B; für Aufgabe 1** = 400,00 $ + 500,00 $\
   **EAC-Ausgabe**&#x200B;**für Aufgabe 1** = 900,00 $\
   **EAC**&#x200B;**für Aufgabe 1** = EAC-Arbeitsaufwand + EAC-Ausgaben\
   **EAC**&#x200B;**für Aufgabe 1**  = 12 500,00 $ + 900,00 $\
   **EAC**&#x200B;**für Aufgabe 1**  = 13 400,00 $

1. Im Folgenden finden Sie die CPI-/EAC-Werte für Aufgabe 2 und Aufgabe 3:\
   Task 2 = .19 / $ 8.433,33\
   Task 3 = .44 / $6.950.00

1. **CPI für Projekt** = .32 wie folgt berechnet:\
   **CPI**&#x200B;**für Projekt** = *IF* Ist-Lohnkosten + IncurredActualExpenseCost  &lt;> 0 *DANN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour\
   **CPI**&#x200B;**für Projekt** = (1000 + 2300) / (7500 + 2700)\
   **CPI**&#x200B;**für Projekt** = 3300 / 10200\
   **CPI**&#x200B;**for Project** = .32

1. **EAC für Projekt** = 28.200,00 $ wie folgt berechnet:\
   **CPI Arbeit**&#x200B;**für Projekt** = WENN Ist-Lohnkosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI Labor**&#x200B;**für Projekt** = 1000 / 7500\
   **CPI Labor**&#x200B;**for Project** = .13333\
   **CPI Labor**&#x200B;**for Project** = .13

   **EAC Labor**&#x200B;**for Project** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   SONST* EAC  Arbeit = Geplante Arbeitskosten + Ist-Arbeitskosten\
   **EAC Labor**&#x200B;**for Project** = 3000/ .13333\
   **EAC Labor**&#x200B;**for Project** = 22.500,00 $

   **EAC-Ausgaben**&#x200B;**Projekt** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC-Ausgaben**&#x200B;**Projekt** = 3.000,00 $ + 2.700,00 $\
   **EAC-Ausgaben**&#x200B;**Projekt** = 5.700,00 $

   **EAC**&#x200B;**PROJECT** = EAC-Arbeitsaufwand + EAC-Ausgaben\
   **EAC**&#x200B;**PROJECT**  = 22 500,00 $ + 5 700,00 $\
   **EAC**&#x200B;**PROJECT**  = 28 200,00 $

#### Kompliziertes Beispiel: Projekt hat untergeordnete Aufgaben {#complicated-example-project-has-children-tasks-1}

PIM = kostenbasiert

EAC-Methode = Berechnung auf Projektebene

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
   <td> </td> 
   <td> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>5 Std</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>20 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>40 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>15 Std</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>50 %</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>20 Std</p> </td> 
   <td> <p>2 000,00 $</p> </td> 
   <td> <p>10 Std</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
   <td> <p>60 %</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Fügen Sie 50 Stunden direkt zum Projekt hinzu (Mehr>Stunden>Stunden protokollieren), sodass 5.000,00 USD der tatsächlichen Lohnkosten direkt im Projekt erfasst werden. **&#x200B;**
1. Aufwendungen zu jeder Aufgabe gemäß der folgenden Tabelle hinzufügen (Zwischen jeder Aufgabe habe ich eine leere Zeile hinzugefügt, um die Lesbarkeit zu erleichtern):

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
   <td> <p>- 400,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Ausl. 2</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 1</p> </td> 
   <td> <p>Aufgabe 1 Ausl. 3</p> </td> 
   <td> <p>400,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Ausl. 1</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Ausl. 2</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Ausl. 3</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>Aufgabe 2 Ausl. 4</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>Aufgabe 3 Ausl</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>Aufgabe 4 Ausl. 1</p> </td> 
   <td> <p>800,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>Aufgabe 4 Ausl. 2</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4 </p> </td> 
   <td> <p>Aufgabe 4 Ausl. 3</p> </td> 
   <td> <p>-200,00</p> </td> 
   <td> <p>0,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>Aufgabe 5 Ausl. 1</p> </td> 
   <td> <p>700,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>Aufgabe 5 Ausl. 2</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>Aufgabe 5 Ausl. 3</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>- 200,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>Aufgabe 6 Ausl. 1</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>Aufgabe 6 Ausl. 2</p> </td> 
   <td> <p>500,00 $</p> </td> 
   <td> <p>- 300,0 $</p> </td> 
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
   <td> <p> 0,00 $ <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Auf der Grundlage der oben genannten Werte werden die angefallenen/nicht angefallenen Kosten wie folgt ermittelt:

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
   <td> <p>400,00 $</p> </td> 
   <td> <p>- 500,00 $</p> </td> 
   <td> <p>800,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 2</p> </td> 
   <td> <p>- 400,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
   <td> <p>1 300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 3</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>1 000,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 4</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>- 100,00 $</p> </td> 
   <td> <p>300,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 5</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>1 100,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe 6</p> </td> 
   <td> <p>0,00 $</p> </td> 
   <td> <p>600,00 $</p> </td> 
   <td> <p>700,00 $</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>2 500,00 $</p> </td> 
   <td> <p>1000,00 $</p> </td> 
   <td> <p>1 500,00 $</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Führen Sie in Projektaktionen die Option Finanzen neu berechnen aus.
1. **CPI** für Aufgabe 2 = .17 wie folgt berechnet:\
   **CPI Aufgabe 2** = *IF* Ist-Lohnkosten + IncurredActualExpenseCost  &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLabourCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labour\
   **CPI**&#x200B;**Task 2** = (100+300) / (1000+1300)\
   **CPI**&#x200B;**Task 2**  = 400 / 2300\
   **CPI**&#x200B;**Task 2**  = .17

1. **EAC** für Aufgabe 2 = 5.900,00 $\
   **CPI Arbeit**&#x200B;**Aufgabe 2** = WENN Ist-Lohnkosten &lt;> 0 DANN CPI_Arbeit = TotalBudgetedCostWorkPerformed / Ist-Lohnkosten\
      ELSE CPI_Labour = 1\
   **CPI Labor**&#x200B;**Task 2** = 100/1000\
   **CPI Labor**&#x200B;**Task 2** = .1

   **EAC Labor**&#x200B;**Task 2** = *IF* CPI_Labour &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   SONST* EAC  Arbeit = Geplante Arbeitskosten + Ist-Arbeitskosten\
   **EAC Labor**&#x200B;**Task 2** = 500.00/.1\
   **EAC Labor**&#x200B;**Task 2** = $5.000.00 **&#x200B;**&#x200B;**&#x200B; EAC Expense &#x200B;**&#x200B;**Task 2 &#x200B;**= IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgabe &#x200B;**&#x200B;**Aufgabe 2** = 1.300,00 $ + - 400,00 $\
   **EAC-Ausgabe**&#x200B;**Aufgabe 2** = 900,00 $

   **EAC**&#x200B;**Aufgabe 2** = EAC-Arbeitsaufwand + EAC-Ausgaben\
   **EAC**&#x200B;**Task 2**  = 5 000,00 $ + 900,00 $\
   **EAC**&#x200B;**Task 2**  = 5 900,00 $

1. Die CPI/EAC für die Aufgaben 4, 5 und 6 werden auf die gleiche Weise festgelegt, sodass ich nur die folgenden Werte angeben werde:\
   Aufgabe 4: .23 / 3.400,00 $\
   Aufgabe 5: .64 / $3.100.00\
   Aufgabe 6: 1,06 / 2.366,67 $

1. CPI für Aufgabe 3 = .31 wie folgt berechnet:\
   **CPI**&#x200B;**Aufgabe 3** = *IF* Ist-Lohnkosten + IncurredActualExpenseCost  &lt;> 0 *DANN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour\
   **CPI**&#x200B;**Task 3**  = (1 150 + 500) / (3 000 + 2 400)\
   **CPI**&#x200B;**Task 3**  =  1650/5400\
   **CPI**&#x200B;**Task 3**  = .31 **&#x200B;**&#x200B;**&#x200B; EAC für Aufgabe 3 &#x200B;**= 9.521,74 $ wie folgt berechnet:\
   **CPI Labor &#x200B;**&#x200B;**Task 3** = WENN die tatsächlichen Lohnkosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI Labor**&#x200B;**Task 3** = 1150/3000\
   **CPI Labor**&#x200B;**Task 3** = .383333\
   **CPI Labor**&#x200B;**Task 3** = .38

   **EAC Labor**&#x200B;**Task 3** = *IF* CPI_Labour &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   SONST* EAC  Arbeit = Geplante Arbeitskosten + Ist-Arbeitskosten\
   **EAC Labor**&#x200B;**Task 3** = $2.500.00 / .383333\
   **EAC Labor**&#x200B;**Task 3** = 6.521,74 $

   **EAC-Ausgabe**&#x200B;**Aufgabe 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgabe**&#x200B;**Aufgabe 3** = 2.400,00 $ + 600,00 $\
   **EAC-Ausgabe**&#x200B;**Aufgabe 3** = 3.000,00 $

   **EAC**&#x200B;**Aufgabe 3** = EAC-Arbeitsaufwand + EAC-Ausgaben\
   **EAC**&#x200B;**Task 3**  = 6 521,74 $ + 3 000,00 $\
   **EAC**&#x200B;**Task 3**  = 9 521,74 $

1. CPI für Aufgabe 1 = .16 berechnet wie folgt:\
   **CPI**&#x200B;**Task 1** = *IF* Ist-Lohnkosten + IncurredActualExpenseCost  &lt;> 0 *DANN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour\
   **CPI**&#x200B;**Task 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI**&#x200B;**Task 1**  =  1550 / 9500=\
   **CPI**&#x200B;**Task 1**  = .16

1. EAC für Aufgabe 1 beträgt 17.100,00 US-Dollar und wird wie folgt berechnet:\
   **CPI Labor**&#x200B;**Task 1** = WENN die tatsächlichen Lohnkosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI Labor**&#x200B;**Task 1** = 1250 / 5000\
   **CPI Labor**&#x200B;**Task 1** = .25

   **EAC Labor**&#x200B;**Task 1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC Labor = Geplante Lohnkosten / CPI_Labor\
   *   SONST* EAC  Arbeit = Geplante Arbeitskosten + Ist-Arbeitskosten\
   **EAC Labor**&#x200B;**Task 1** = 3.000,00 $ / .25\
   **EAC Labor**&#x200B;**Task 1** = 12.000,00 $

   **EAC-Ausgabe**&#x200B;**Aufgabe 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC Ausgabe**&#x200B;**Aufgabe 1** = 4500 $ + 600 $\
   **EAC-Ausgabe**&#x200B;**Aufgabe 1** = 5.100,00 $

   **EAC**&#x200B;**Aufgabe 1** = EAC-Arbeitsaufwand + EAC-Ausgaben\
   **EAC**&#x200B;**Task 1**  = 12 000,00 $ + 5 100,00 $\
   **EAC**&#x200B;**Task 1**  = 17 100,00 $

1. CPI für Projekt ist .25\
   **CPI**&#x200B;**für Projekt** = *IF* Ist-Lohnkosten + IncurredActualExpenseCost  &lt;> 0 *DANN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labour

   **CPI**&#x200B;**für Projekt** = (2450 + 1900) / (11000 + 6700)\
   **CPI**&#x200B;**für Projekt** =   4350/17700\
   **CPI**&#x200B;**for Project** = .25

1. **EAC für Projekt** = 32.248,98 $ wie folgt berechnet:\
   **CPI Arbeit**&#x200B;**für Projekt** = WENN Ist-Lohnkosten &lt;> 0 DANN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labour = 1\
   **CPI Labor**&#x200B;**für Projekt** = 2450 / 11000\
   **CPI Labor**&#x200B;**for Project** = .22272\
   **CPI Labor**&#x200B;**for Project** = .22

   **EAC Labor**&#x200B;**for Project** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   SONST* EAC  Arbeit = Geplante Arbeitskosten + Ist-Arbeitskosten\
   **EAC Labor**&#x200B;**für Projekt** = 5.000,00 $ / .22272\
   **EAC Labor**&#x200B;**for Project** = 22.448,97959 $\
   **EAC Labor**&#x200B;**for Project** = 22.448,98 $

   **EAC-Ausgabe**&#x200B;**Projekt** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-Ausgaben**&#x200B;**Projekt** = 3.100,00 $ + 6.700,00 $\
   **EAC-Ausgaben**&#x200B;**Projekt** = 9.800,00 $

   **EAC**&#x200B;**PROJECT** = EAC-Arbeitsaufwand + EAC-Ausgaben\
   **EAC**&#x200B;**PROJECT**  = $ 22.448,98 + 9.800,00\
   **EAC**&#x200B;**PROJECT**  = 32 248,98 $
