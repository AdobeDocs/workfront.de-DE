---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Schätzung nach Abschluss berechnen (EAC)
description: Als Leistungsmetrik stellt die Schätzung bei Abschluss (EAC) die voraussichtlichen Gesamtkosten Ihres Projekts oder Ihrer Aufgabe nach Abschluss dar.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Schätzung nach Abschluss berechnen (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Als Leistungsmetrik stellt die Schätzung bei Abschluss (EAC) die voraussichtlichen Gesamtkosten Ihres Projekts oder Ihrer Aufgabe nach Abschluss dar.

Als Einstellung können Sie damit festlegen, wie der EAC-Wert berechnet werden soll. 

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
   <td> <p>Zugriff auf Projekte und Finanzdaten anzeigen</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für das Projekt mit Berechtigungen zum Anzeigen von Finanzen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Definieren der EAC-Berechnung

Im Rahmen der Voreinstellungen des Projektsystems kann der Adobe Workfront-Administrator definieren, wie die EAC berechnet werden soll. Die EAC kann auf eine der folgenden beiden Arten berechnet werden:

* [Berechnen auf Projektebene](#calculate-at-the-project-level)
* [Zusammenführen von Aufgaben und Unteraufgaben](#roll-up-from-tasks-and-subtasks)

Weitere Informationen zum Einrichten von Projektvoreinstellungen in Workfront, einschließlich der Berechnung der Schätzung nach Abschluss, finden Sie unter [Systemweite Projektanvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Als Projektmanager können Sie diese Voreinstellung auch auf Projektebene im Untertab Finanzen des Projekts ändern. Weitere Informationen zum Bearbeiten der Unterregisterkarte &quot;Finanzen&quot;eines Projekts finden Sie unter [Verwalten von Informationen im Bereich &quot;Projekt-Finanzen&quot;](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Auf Projektebene berechnen {#calculate-at-the-project-level}

Die EAC für die übergeordnete Aufgabe und das Projekt werden durch Eingabe der tatsächlichen Stunden/tatsächlichen Arbeitskosten in die EAC-Formeln bestimmt. Diese Berechnung umfasst die tatsächlichen Stunden/ Kosten und Ausgaben, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.

### Zusammenführen von Aufgaben und Unteraufgaben {#roll-up-from-tasks-and-subtasks}

Die EAC für die übergeordnete Aufgabe und das Projekt werden durch Addieren der EAC für jede untergeordnete Aufgabe bestimmt. Diese Berechnung schließt tatsächliche Stunden/-kosten und -aufwendungen aus, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.

## Berechnung der EAC auf Grundlage der Leistungsindex-Methode (PIM)

In Workfront hängt die EAC-Berechnung von der ausgewählten Leistungsindex-Methode (PIM) des Projekts ab. Weitere Informationen zum Festlegen des PIM für Ihr System oder Ihr Projekt finden Sie unter [Festlegen der Leistungsindex-Methode (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Berechnen der EAC mithilfe der stündbasierten PIM](#calculate-eac-using-hour-based-pim)
* [Berechnung der EAC mit kostenbasiertem PIM](#calculate-eac-using-cost-based-pim)

### Berechnung der EAC mit stündbasiertem PIM {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Wenn der Kosten-Leistungs-Index [ den Kosten-Leistungs-Index (CPI) berechnen](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Gesamtgeplante Stunden + tatsächliche Stunden. Dies tritt auf, wenn Stunden erfasst wurden, das Projekt/die Aufgabe jedoch zu 0 % abgeschlossen ist.

Weitere Informationen zur Berechnung des CPI finden Sie unter [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Berechnung der EAC mit kostenbasiertem PIM {#calculate-eac-using-cost-based-pim}

Die EAC eines Projekts wird anhand der folgenden Formel berechnet:

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC-Arbeit =  <em>IF</em> CPI-Arbeit &lt;&gt; 0 DANN EAC-Arbeit = geplante Arbeitskosten/CPI-Arbeit</pre><pre><em>ELSE</em> EAC  Arbeit = Geplante Arbeitskosten + tatsächliche Arbeitskosten</pre><pre>CPI-Arbeit = WENN tatsächliche Arbeitskosten &lt;&gt; 0 DANN CPI-Arbeitskosten = TotalBudgetedCostWorkPerformed / Tatsächliche Arbeitskosten</pre><pre>ELSE CPI Labour = 1 </pre>Bei der Berechnung des EAC werden die folgenden Felder berücksichtigt:

* Gesamtsumme der durchgeführten budgetierten Kosten (BCWP) = Ergebnis der Multiplikation der veranschlagten Kosten der geplanten Arbeit (veranschlagte Kosten) und des Prozentsatzes der bisher abgeschlossenen Aufgabe.

  Weitere Informationen über die insgesamt durchgeführten budgetierten Kosten (BCWP) finden Sie unter [Berechnung der durchgeführten budgetierten Kosten (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Für eine nicht übergeordnete Aufgabe:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **Für eine übergeordnete Aufgabe:**
Gesamtsumme der durchgeführten budgetierten Kostenarbeit = die Summe des Felds Gesamtsumme der durchgeführten budgetierten Kosten für alle direkten untergeordneten Aufgaben.

   * **Für ein Projekt:**
Gesamtsumme der durchgeführten budgetierten Kostenarbeit = die Summe des Felds &quot;Gesamtkostenarbeit&quot;für alle Aufgaben auf oberster Ebene (Eltern und eigenständige Aufgaben). 

* EAC-Ausgaben = das Ergebnis der Hinzufügung der tatsächlichen Aufwendungen zu den nicht anfallenden geplanten Kosten. Sie wird mit der folgenden Formel berechnet:

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Incurred Tatsächliche Kosten = Die Summe des Felds &quot;Geplanter Betrag&quot;für alle Ausgaben, für die das Feld &quot;Tatsächlicher Betrag&quot;> 0 ist. Wenn Sie beispielsweise eine Ausgabe für Aufgabe 1 erstellen und 500,00 USD im Feld &quot;Geplanter Betrag&quot;und einen Betrag > 0 im Feld &quot;Tatsächlicher Betrag&quot;eingeben (d. h. 600,00 USD), belaufen sich die Kosten für geplante geplante Ausgaben für diese Aufgabe auf 500,00 USD.
   * Nicht eingeplante Ausgaben = Die Summe des Felds &quot;Geplanter Betrag&quot;für alle Ausgaben, für die das Feld &quot;Tatsächlicher Betrag&quot;= 0 ist. Wenn Sie beispielsweise zwei Ausgaben für Aufgabe 1 erstellen, wobei der Wert im Feld Geplanter Betrag für die erste Ausgabe 500,00 USD und der Wert im tatsächlichen Betrag 600,00 USD und für die zweite Ausgabe der Wert im Feld Geplanter Betrag 300,00 USD und der Wert des Felds &quot;Tatsächlicher Betrag&quot;0,00 USD beträgt, lautet der Wert des Nicht eingeplante Kosten für diese Aufgabe belaufen sich auf 300,00 USD. 

## Suchen Sie die EAC in einem Projekt oder einer Aufgabe

1. Wechseln Sie zu dem Projekt oder der Aufgabe, in dem/der Sie die EAC anzeigen möchten.
1. Erweitern Sie **Projektdetails** oder **Aufgabendetails** im linken Bereich des Projekts oder der Aufgabe, je nachdem, wo Sie die EAC anzeigen.

1. Klicken Sie auf **Finance**. 

   Der EAC-Wert wird im Feld **Schätzung bei Abschluss** angezeigt.

   ![](assets/eac-highlighted-on-project-350x112.png)
