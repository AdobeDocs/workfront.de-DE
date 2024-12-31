---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Kostenentwicklungsindex (CPI) berechnen
description: Der Kostenentwicklungsindex (Cost Performance Index, CPI) beschreibt die Beziehung zwischen den geplanten Kosten und den Ist-Kosten auf Projekt- oder Vorgangsebene. Projektmanager überprüfen diese Metrik, um Aufgaben oder Projekte zu identifizieren, die zu einem bestimmten Zeitpunkt unter oder über den Kosten liegen.
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Kostenentwicklungsindex (CPI) berechnen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

Der Kostenentwicklungsindex (Cost Performance Index, CPI) beschreibt die Beziehung zwischen den geplanten Kosten und den Ist-Kosten auf Projekt- oder Vorgangsebene. Projektmanager überprüfen diese Metrik, um Aufgaben oder Projekte zu identifizieren, die zu einem bestimmten Zeitpunkt unter oder über den Kosten liegen. Die Kosten können je nach Leistungsindexmethode (PIM) in Stunden oder Dollar angegeben werden. Weitere Informationen zum Festlegen der Leistungsindexmethode finden Sie unter [Festlegen der Leistungsindexmethode (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Nur Organisationen, die eine Zeiteingabe benötigen, können CPI verwenden. Darüber hinaus sind kostenbasierte PIM-Werte nur in Organisationen korrekt, die Kostensätze für Aufgabenzugewiesene (Aufgabengebiete oder Benutzer) definiert haben.

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

## Überblick über den Kostenentwicklungsindex (Cost Performance Index, CPI)

* [Der CPI-Wert](#the-cpi-value)
* [So wird der CPI berechnet](#how-cpi-is-calculated)

### Der CPI-Wert {#the-cpi-value}

Projektmanager wissen, dass ein CPI-Wert von 1 bedeutet, dass das Projekt exakt im Budget liegt. Werte über 1 zeigen an, dass ein Projekt unter dem Budget liegt (es wurden weniger Stunden oder Ausgaben erfasst als ursprünglich geplant), und Werte unter 1 bedeuten, dass ein Projekt das Budget überschreitet (es wurden mehr Stunden oder Ausgaben erfasst als ursprünglich geplant). Je weiter von 1, desto größer die Abweichung vom Plan.

| **CPI-Wert** | **Angaben zum Budget** |
|---|---|
| 1 | Auf Plan oder Budget |
| > 1 (größer als 1) | Unter Budget |
| &lt; 1 (weniger als 1) | Über Budget |


### So wird der CPI berechnet {#how-cpi-is-calculated}

In Adobe Workfront hängt die Berechnung des VPI von der für das Projekt ausgewählten Leistungsindexmethode ab. Weitere Informationen zum Festlegen der Leistungsindexmethode finden Sie unter [Festlegen der Leistungsindexmethode (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [CPI-Berechnungen bei Verwendung eines stundenbasierten PIM](#cpi-calculations-when-using-hour-based-pim)
* [CPI-Berechnungen bei Verwendung kostenbasierter PIM](#cpi-calculations-when-using-cost-based-pim)

#### CPI-Berechnungen bei Verwendung eines stundenbasierten PIM {#cpi-calculations-when-using-hour-based-pim}

Wenn

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Andernfalls

```
CPI = 1
```

* **Für eine nicht übergeordnete Aufgabe:**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **Für eine übergeordnete Aufgabe:**
Gesamte budgetierte Kosten Ausgeführte Arbeit = Summe der insgesamt budgetierten Kosten Ausgeführte Arbeit für alle direkt untergeordneten Aufgaben.

* **Für ein Projekt:**
Gesamte budgetierte Kosten Ausgeführte Arbeit = Summe der insgesamt budgetierten Kosten Ausgeführte Arbeit für alle Aufgaben der obersten Ebene (übergeordnete und eigenständige Aufgaben).

Informationen über die insgesamt budgetierten Kosten der durchgeführten Arbeit (SKAA) finden Sie unter [Budgetierte Kosten der durchgeführten Arbeit (SKAA) berechnen](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### CPI-Berechnungen bei Verwendung kostenbasierter PIM {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

Wenn

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



Andernfalls

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

Die Felder in dieser Berechnung werden nachfolgend beschrieben:

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Aufgetretene Ausgaben sind die Ausgaben, für die die Ist-Kosten > 0 sind.

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* Die geplanten Kosten der geleisteten Arbeit werden nach folgender Formel berechnet:

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

Die insgesamt budgetierten Kosten der durchgeführten Arbeit werden für Folgendes berechnet:

* **Für eine nicht übergeordnete Aufgabe:**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **Für eine übergeordnete Aufgabe:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* **Für ein Projekt:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
  ```



## CPI in einem Projekt oder einer Aufgabe suchen

Sie können den CPI eines Projekts oder einer Aufgabe in einem Projekt, einer Aufgabenliste oder einem Bericht anzeigen. Darüber hinaus können Sie sie auf Projekt- oder Aufgabenebene anzeigen.

1. Wechseln Sie zu dem Projekt oder der Aufgabe, in dem bzw. der Sie den CPI anzeigen möchten.
1. Erweitern Sie **Projektdetails** oder **Aufgabendetails** im linken Bereich, je nachdem, ob Sie den CPI für ein Projekt oder eine Aufgabe anzeigen.

1. Klicken Sie auf **Finanzen**.

   Der CPI wird im Feld **CPI/SPI/CSI** angezeigt.

   ![](assets/cpi-on-project-nwe.png)
