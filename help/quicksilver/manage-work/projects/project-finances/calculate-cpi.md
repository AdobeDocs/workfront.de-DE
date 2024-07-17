---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: CPI (Cost Performance Index) berechnen
description: Der Cost Performance Index (CPI) beschreibt die Beziehung auf Projekt- oder Aufgabenebene zwischen den geplanten und den tatsächlichen Kosten. Projektmanager überprüfen diese Metrik, um Aufgaben oder Projekte zu identifizieren, die derzeit unter oder über den Kosten an einem bestimmten Punkt nachverfolgen.
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# CPI (Cost Performance Index) berechnen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

Der Cost Performance Index (CPI) beschreibt die Beziehung auf Projekt- oder Aufgabenebene zwischen den geplanten und den tatsächlichen Kosten. Projektmanager überprüfen diese Metrik, um Aufgaben oder Projekte zu identifizieren, die derzeit unter oder über den Kosten an einem bestimmten Punkt nachverfolgen. Die Kosten können in Stunden oder Dollar gemessen werden, je nach Performance Index Method (PIM). Weitere Informationen zum Festlegen der Leistungsindex-Methode finden Sie unter [Festlegen der Leistungsindex-Methode (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Nur Organisationen, die eine Zeiteingabe benötigen, können CPI verwenden. Darüber hinaus sind kostenbasierte PIM-Werte nur in Unternehmen exakt, die über definierte Kostensätze für Aufgabenverantwortliche verfügen (Stellenrollen oder Benutzer).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten anzeigen</p> <p> Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für das Projekt mit Berechtigungen zum Anzeigen von Finanzen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Übersicht über den CPI (Cost Performance Index)

* [Der CPI-Wert](#the-cpi-value)
* [Berechnung des CPI](#how-cpi-is-calculated)

### CPI-Wert {#the-cpi-value}

Projektmanager wissen, dass ein CPI-Wert von 1 bedeutet, dass das Projekt genau im Budget liegt. Werte, die größer als 1 sind, weisen darauf hin, dass ein Projekt im Budget liegt (weniger Stunden oder Ausgaben wurden als ursprünglich geplant verzeichnet), und Werte unter 1 bedeuten, dass ein Projekt über dem Budget liegt (mehr Stunden oder Ausgaben wurden verzeichnet als ursprünglich geplant). Je weiter von 1, desto größer ist die Abweichung vom Plan.

| **CPI-Wert** | **Anzeige für Budget** |
|---|---|
| 1 | Über Plan oder Budget |
| > 1 (größer als 1) | Haushaltsmittel |
| &lt; 1 (weniger als 1) | Budget |


### Berechnung des CPI {#how-cpi-is-calculated}

In Adobe Workfront hängt die Berechnung des CPI von der für das Projekt ausgewählten Leistungsindex-Methode ab. Weitere Informationen zum Festlegen der Leistungsindex-Methode finden Sie unter [Festlegen der Leistungsindex-Methode (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [CPI-Berechnungen bei Verwendung von stündbasiertem PIM](#cpi-calculations-when-using-hour-based-pim)
* [CPI-Berechnungen bei Verwendung kostenbasierter PIM](#cpi-calculations-when-using-cost-based-pim)

#### CPI-Berechnungen bei Verwendung von stündbasiertem PIM {#cpi-calculations-when-using-hour-based-pim}

Wenn

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Sonst

```
CPI = 1
```

* **Für eine nicht übergeordnete Aufgabe:**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **Für eine übergeordnete Aufgabe:**
Gesamtsumme der durchgeführten budgetierten Kostenarbeit = die Summe des Felds Gesamtsumme der durchgeführten budgetierten Kosten für alle direkten untergeordneten Aufgaben.

* **Für ein Projekt:**
Gesamtsumme der durchgeführten budgetierten Kostenarbeit = die Summe des Felds &quot;Gesamtkostenarbeit&quot;für alle Aufgaben auf oberster Ebene (Eltern und eigenständige Aufgaben).

Weitere Informationen über die insgesamt durchgeführten budgetierten Kosten (BCWP) finden Sie unter [Berechnung der durchgeführten budgetierten Kosten (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

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



Sonst

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

Die in dieser Berechnung enthaltenen Felder werden im Folgenden beschrieben:

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Versicherungsbezogene Ausgaben sind die Ausgaben, auf die sich tatsächliche Kosten > 0 belaufen

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* Geplante Kosten der durchgeführten Arbeit werden anhand der folgenden Formel berechnet:

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

Die Gesamtsumme der durchgeführten budgetierten Kosten wird für Folgendes berechnet:

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

Sie können den CPI eines Projekts oder einer Aufgabe in einer Projekt-, Aufgabenliste oder einem Bericht anzeigen. Darüber hinaus können Sie sie auf Projekt- oder Aufgabenebene anzeigen.

1. Wechseln Sie zu dem Projekt oder der Aufgabe, in dem/der die CPI angezeigt werden soll.
1. Erweitern Sie im linken Bereich **Projektdetails** oder **Aufgabendetails**, je nachdem, ob Sie die CPI für ein Projekt oder eine Aufgabe anzeigen.

1. Klicken Sie auf **Finance**.

   Der CPI wird im Feld **CPI/SPI/CSI** angezeigt.

   ![](assets/cpi-on-project-nwe.png)
