---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über geplante Stunden
description: Die mit einer Aufgabe, einem Problem oder einem Projekt verknüpften geplanten Stunden stellen die Zeit dar, die die zugewiesenen Benutzer zum Abschließen der Aufgabe, des Problems oder des Projekts benötigen.
author: Alina
feature: Work Management
exl-id: 0b86c760-691a-436e-9beb-31e9ac36440a
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# Übersicht über geplante Stunden

Die mit einer Aufgabe, einem Problem oder einem Projekt verknüpften geplanten Stunden stellen die Zeit dar, die die zugewiesenen Benutzer zum Abschließen der Aufgabe, des Problems oder des Projekts benötigen.

## Überlegungen zu geplanten Stunden in Adobe Workfront

* Geplante Stunden sind in erster Linie mit Arbeitselementen (Aufgaben und Problemen) in Adobe Workfront verknüpft. Die geplanten Stunden von Arbeitselementen führen zu den geplanten Stunden ihrer Projekte.
* Standardmäßig verteilt Workfront Aufgaben und Ausgaben für geplante Stunden gleichmäßig auf alle Tage der Dauer der Aufgabe oder des Problems.
* Wenn Benutzer und Rollen Aufgaben und Problemen zugewiesen werden, werden die geplanten Stunden aus den Aufgaben und Problemen mit Benutzer- oder Rollenzuweisungen verknüpft.
* Sie müssen den Wert für &quot;Geplante Stunden&quot;für Aufgaben und Probleme definieren, wenn Sie die Tools für die Ressourcenverwaltung in Workfront verwenden möchten.
* Sie können den Wert für &quot;Geplante Stunden&quot;für Aufgaben nur für einige Dauer-Typen ändern.

  Weitere Informationen zum Ändern der geplanten Stunden für Aufgaben im Verhältnis zum Aufgabentyp finden Sie im Abschnitt . [Aktualisieren der geplanten Aufgaben auf Grundlage des Durationstyps](#update-task-planned-hours-based-on-duration-type) in diesem Artikel.

* Sie können den Wert von &quot;Geplante Stunden&quot;für Probleme jederzeit ändern.
* Sie können den Wert der geplanten Stunden von Projekten oder übergeordneten Aufgaben nicht ändern, da es sich um eine berechnete Gesamtsumme aller geplanten Stunden aller Aufgaben und Unteraufgaben handelt.
* Die Verwaltung von Benutzerzuordnungen mithilfe von Tools zur Ressourcenverwaltung kann die Anzahl der geplanten Stunden für Aufgaben, Probleme, Projekte und die Anzahl der Zuweisungen ändern, die mit Arbeitselementen verknüpft sind.

## Geplante Stunden für Aufgaben vs. geplante Stunden für Projekte {#planned-hours-on-tasks-vs-planned-hours-on-projects}

Geplante Stunden von Aufgaben rollen zu den geplanten Stunden des Projekts. Die geplanten Stunden aus den Problemen führen nicht immer zu den geplanten Stunden des Projekts.

In diesem Abschnitt werden die Unterschiede zwischen der geplanten und der Aufgabe beschrieben. Außerdem wird beschrieben, wo Sie Probleme mit geplanten Stunden anzeigen können, die zum Projekt gehören.

* [Geplante Stunden für Aufgaben](#planned-hours-on-tasks)
* [Geplante Stunden für Projekte](#planned-hours-on-projects)

### Geplante Stunden für Aufgaben {#planned-hours-on-tasks}

Die geplanten Stunden einer Aufgabe geben an, wie lange die tatsächliche Arbeit an der Aufgabe vermutlich dauern wird. Standardmäßig verteilt Workfront die Gesamtdauer der geplanten Stunden für jeden Tag innerhalb der Dauer jeder Aufgabe gleichmäßig. Die tägliche geplante Zeitdauer wird zur täglichen Zuteilung für die Aufgabe. Wenn die Aufgabe mehreren Ressourcen zugewiesen ist, wird standardmäßig jeder Ressource die gleiche Anzahl von Stunden pro Tag zugeordnet.

Mithilfe des Lastenausgleichs können Sie die täglichen Zuordnungen für die den Aufgaben zugewiesenen Benutzer ändern. Auf diese Weise können auch die geplanten Stunden der Aufgabe aktualisiert werden, wenn der Aufgabendauertyp einfach ist. Weitere Informationen finden Sie im Abschnitt &quot;Aktualisierung der geplanten Aufgaben bei der Verwaltung von Benutzerzuweisungen&quot;im Artikel [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Wenn eine Aufgabe Unteraufgaben enthält, entsprechen die geplanten Stunden der übergeordneten Aufgabe der Summe aller geplanten Stunden für alle Unteraufgaben. Sie können die geplanten Stunden einer übergeordneten Aufgabe nicht aktualisieren.

>[!NOTE]
>
>Im Gegensatz zu &quot;Geplante Stunden&quot;werden die tatsächlichen Stunden einer übergeordneten Aufgabe direkt bei der übergeordneten Aufgabe protokolliert. Sie stellen keine Summe der tatsächlichen Stunden der untergeordneten Aufgaben dar.\
>Weitere Informationen zu den tatsächlichen Stunden finden Sie unter [Tatsächliche Stunden anzeigen](../../../manage-work/tasks/task-information/actual-hours.md).

### Geplante Stunden für Projekte {#planned-hours-on-projects}

Sie können die geplante Stundenzahl eines Projekts nicht bearbeiten. &quot;Geplante Stunden&quot;für ein Projekt sind eine berechnete Summe aller geplanten Stunden aus allen Aufgaben im Rahmen des Projekts.

Ob in der Berechnung für geplante Stunden Probleme enthalten sind, hängt von der Position im Projekt ab, an der Sie geplante Stunden anzeigen. Sie können geplante Projektstunden an den folgenden Stellen in einem Projekt anzeigen:

* **Projektdetails und das Feld &quot;Projekt bearbeiten&quot;**: Nur die geplanten Stunden für die Aufgaben im Rahmen des Projekts werden berücksichtigt. Die geplanten Stunden für die Probleme im Projekt werden bei der Anzeige der Gesamtanzahl der geplanten Stunden für das Projekt im Abschnitt Projektdetails oder im Feld Projekt bearbeiten nicht berücksichtigt.

* **Der Lastenausgleich**: Nur die geplanten Stunden, die mit den Aufgaben verknüpft sind, die im Lastenausgleich sichtbar sind, werden im Arbeitslastausgleich für Projekte angezeigt. Die tägliche Zuordnung von Benutzern kann das Projekt täglich geplante Stunden im Arbeitslastausgleich ändern.
* **Abschnitt &quot;Nutzung&quot;**: Die mit den den Aufgaben zugeordneten Benutzern verknüpften geplanten Stunden und die Probleme im Projekt werden bei der Anzeige der Gesamtanzahl der geplanten Stunden für das Projekt im Abschnitt &quot;Nutzung&quot;berücksichtigt.
* **Bereich &quot;Rollenzuweisung&quot;** in der Aufgabenliste: Die geplanten Stunden für die Aufgaben und die Probleme im Projekt, die einer Auftrags- oder Benutzerrolle zugeordnet sind, werden in diesem Bereich angezeigt. Geplante Stunden, die mit Aufgaben und Problemen verknüpft sind, die nicht zugewiesen oder Teams zugewiesen sind, werden in diesem Bereich nicht angezeigt. Weitere Informationen finden Sie unter [Anzeigen von geplanten Projektstunden im Bereich &quot;Rollenzuweisung&quot;](../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md).

## Verteilung der geplanten Stunden über die Dauer einer Aufgabe

Standardmäßig verteilt Workfront die geplanten Stunden gleichmäßig auf die Dauer einer Aufgabe und weist je nach Verfügbarkeit des Projektzeitplans für jeden Tag der Aufgabe eine identische Anzahl geplanter Stunden zu.

Wenn beispielsweise eine Aufgabe auf 16 Uhr eingestellt ist und der Zeitplan am ersten Tag der Aufgabe eine Stunde verbleibt, teilt Workfront eine geplante Stunde am ersten Tag der Aufgabendauer und dann die restlichen geplanten Stunden gleichmäßig auf die restlichen Tage der Aufgabendauer auf.

>[!NOTE]
>
>Die geplante Stunde pro Tag oder die tägliche Zuweisung ist die Zuweisung der geplanten Stunden für jeden Tag während der Dauer der Aufgabe. Wenn die Aufgabe eine Zuweisung hat, stellt diese Zahl die geplanten Stunden pro Tag pro Zuweisung dar. Wenn die Aufgabe mehrere Zuweisungen aufweist, unterscheiden sich die geplanten Stunden pro Tag pro Zuweisung von den geplanten Stunden pro Tag für die Aufgabe. Es gibt keine visuelle Darstellung in Workfront für die geplanten Stunden pro Tag pro Zuweisung für Aufgaben mit mehreren Zuweisungen.

## Werte für geplante Stunden suchen und verstehen

Die Werte für geplante Stunden finden Sie in verschiedenen Bereichen von Workfront. 

Die angezeigte Anzahl der geplanten Stunden stammt entweder aus den Arbeitselementen im Projekt oder wird je nach Bereich und Objekt, in dem Sie sie anzeigen, unterschiedlich berechnet.

Geplante Stunden finden Sie in den folgenden Bereichen von Workfront:

* [Der Bereich Details eines Projekts, einer Aufgabe oder eines Problems](#the-details-section-of-a-project-task-or-issue)
* [Das Feld &quot;Aufgabe bearbeiten&quot;oder &quot;Problem bearbeiten&quot;](#the-edit-task-or-edit-issue-box)
* [Berichte](#reports)
* [Der Lastenausgleich](#the-workload-balancer)
* [Der Ressourcen-Planer](#the-resource-planner)
* [Der Nutzungsbericht](#the-utilization-report)
* [Bereich &quot;Rollenzuweisung&quot;](#The%C2%A0Role)

### Der Bereich Details eines Projekts, einer Aufgabe oder eines Problems {#the-details-section-of-a-project-task-or-issue}

![](assets/planned-hours-on-details-for-project-nwe-350x138.png)

Die im Abschnitt &quot;Details&quot;einer Aufgabe, eines Problems oder eines Projekts unter &quot;Geplante Stunden&quot;angegebenen Gesamtstunden sind mit dem jeweiligen Element verknüpft.

Weitere Informationen zu geplanten Projektstunden finden Sie im Abschnitt [Geplante Stunden für Aufgaben vs. geplante Stunden für Projekte](#planned-hours-on-tasks-vs-planned-hours-on-projects) in diesem Artikel beschrieben.

### Das Feld &quot;Aufgabe bearbeiten&quot;oder &quot;Problem bearbeiten&quot; {#the-edit-task-or-edit-issue-box}

![](assets/planned-hours-on-edit-task-box-nwe-350x70.png)

Die geplanten Stunden im Feld &quot;Bearbeiten&quot;einer Aufgabe oder eines Problems entsprechen der Gesamtanzahl der geplanten Stunden des jeweiligen Elements.

Weitere Informationen zu geplanten Projektstunden finden Sie im Abschnitt [Geplante Stunden für Aufgaben vs. geplante Stunden für Projekte](#planned-hours-on-tasks-vs-planned-hours-on-projects) in diesem Artikel beschrieben.

Für Aufgaben können Sie die geplante Stundenanzahl nur für bestimmte Arten von Dauer bearbeiten. Weitere Informationen finden Sie unter [Aktualisieren der geplanten Aufgaben auf Grundlage des Durationstyps](#update-task-planned-hours-based-on-duration-type) in diesem Artikel beschrieben.

Sie können die individuelle Zuweisung der geplanten Stunden für jeden Benutzer oder jede Auftragsrolle, die der Aufgabe oder dem Problem zugewiesen ist, im Bereich Zuweisungen anzeigen.

### Berichte {#reports}

![](assets/planned-hours-on-task-repot-nwe-350x99.png)

Sie können das Feld &quot;Geplante Stunden&quot;zu Projekt-, Aufgaben- und Problemberichten hinzufügen.

Die Spalte Geplante Stunden ist standardmäßig in der Standardansicht einer Aufgabenliste enthalten.

Der Bericht &quot;Geplante Stunden&quot;in einer Aufgabe, einem Problem oder einem Projekt entspricht der Gesamtanzahl der geplanten Stunden des jeweiligen Elements, wie sie im Bereich Details oder im Feld Bearbeiten der Elemente angezeigt werden.

Informationen zum Erstellen von Berichten finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

>[!NOTE]
>
>Wenn Sie einen Bericht zum Projekt (Finanzdaten) erstellen und nach Datum gruppieren, zeigen die geplanten Stunden je nach Zeitablauf der Aufgaben für das Projekt möglicherweise einen Teil der geplanten Stunden des Projekts an. Standardmäßig verteilt Workfront die geplanten Stunden der Aufgaben gleichmäßig auf jeden Tag der Aufgabendauer. Die geplanten Stunden für einen bestimmten Zeitraum stimmen mit der gleichen Verteilung überein, die Workfront für diesen Zeitraum im Bericht Projekt (Finanzdaten) festgelegt hat.

<!--
### The Scheduling areas  {#the-scheduling-areas}

![](assets/task-detail-expanded-in-scheduler-with-planned-hours-and-adjusted-daily-allocations-nwe-350x323.png)

The Planned Hours for tasks and issues display in the Scheduling areas in the Planned Hours field.

You can view the daily allocation of Planned Hours for each user assigned to a task or an issue in the Scheduling areas.

The daily hour amount represents one of the following:

* the default amount equally distributed by Workfront for each day of the Duration of the tasks or issues
* the adjusted daily allocation managed by resource managers.

  For information about adjusting daily allocations in the Scheduling tools, see [Manage user allocations in the Scheduling areas](../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).
-->

### Der Lastenausgleich {#the-workload-balancer}

![](assets/planned-hours-on-wb-expanded-with-pti-info-nwe-350x114.png)

Die folgenden geplanten Stunden für Aufgaben, Probleme und Projekte werden rechts neben der Aufgabe, dem Problem oder dem Projektnamen im Arbeitslastausgleich angezeigt:

* Für Aufgaben und Probleme werden die ihnen zugeordneten Planungszeiten angezeigt.
* Für Projekte wird eine Gesamtanzahl von geplanten Stunden aus den Aufgaben und Problemen angezeigt, die auf dem Bildschirm angezeigt werden.

  >[!TIP]
  >
  >Der Lastenausgleich zeigt nicht alle geplanten Stunden eines Projekts im Bereich Projektdetails an.

Sie können die tägliche Zuweisung von geplanten Stunden für jeden Benutzer, der einer Aufgabe zugewiesen ist, oder ein Problem im Arbeitslastausgleich anzeigen.

Die tägliche Stundenanzahl der geplanten Stunden stellt eine der folgenden dar: 

* den von Workfront gleichmäßig verteilten Standardbetrag für jeden Tag der Dauer der Aufgaben, Probleme oder des Projekts
* die von Ressourcenmanagern verwaltete angepasste tägliche Zuordnung.

  Informationen zum Anpassen der täglichen Zuordnungen im Arbeitslastausgleich finden Sie unter [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

### Der Ressourcen-Planer {#the-resource-planner}

![](assets/planned-hours-on-all-objects-in-resource-planned-expanded-nwe-350x204.png)

Der Ressourcenplaner zeigt geplante Stunden für Projekte, Aufgaben, Probleme an.

Sie können die wöchentlichen Zuordnungen von geplanten Stunden für die mit Arbeitselementen verknüpften Benutzer und Stellenrollen in der Spalte PLN des Resource Planers anzeigen.

>[!TIP]
>
>Tägliche Zuordnungsanpassungen im Arbeitslasten-Balancer beeinflussen die wöchentlichen Zuordnungen für Aufgaben und Probleme im Ressourcenplaner.

Die Anzahl der geplanten Stunden für jedes Objekt hängt davon ab, welche Ansicht Sie auf den Ressourcenplaner anwenden. Weitere Informationen finden Sie unter [Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

Die wöchentliche Stundenzahl für geplante Aufgaben und Probleme stellt eine der folgenden dar:

* den von Workfront gleichmäßig verteilten wöchentlichen Standardbetrag für jeden Tag der Dauer der Aufgaben oder Probleme
* die angepasste wöchentliche Zuordnung, die von Ressourcenmanagern im Workload Balancer verwaltet wird.

  Informationen zum Anpassen der täglichen Zuordnungen im Arbeitslastausgleich finden Sie unter [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Der wöchentliche Betrag für Projekte, Benutzer und Rollen wird durch die wöchentlichen Beträge der geplanten Stunden für die damit verbundenen Aufgaben und Probleme beeinflusst.

### Der Nutzungsbericht {#the-utilization-report}

Das Projekt &quot;Geplante Stunden&quot;ist mit den Zuweisungen für jede Aufgabe und jedes Problem verknüpft.

>[!IMPORTANT]
>
>Beachten Sie, dass die im Bericht &quot;Dienstprogramme&quot;geplanten Stunden mit den Zuweisungen und nicht mit den Aufgaben und Problemen selbst verknüpft sind. Die im Bericht &quot;Nutzung&quot;geplanten Stunden stimmen nicht immer mit den geplanten Stunden zu den Aufgaben und Problemen des Projekts überein. Die geplanten Stunden stimmen jedoch mit den Stunden überein, die mit den Zuweisungen zu Aufgaben und Problemen verknüpft sind.

Sie können die folgenden Arten von geplanten Stunden im Nutzungsbericht anzeigen:

* die Gesamtdauer der geplanten Zeiträume aller Zuweisungen für das Projekt während der gesamten Dauer der einbezogenen Projekte;
* die insgesamt geplanten Stunden aller Zuweisungen nur für den angegebenen Datumsbereich (Sie können eine einzelne Woche oder einen einzelnen Monat angeben).

  Wenn die tägliche Zuweisung der Stunden durch den Benutzer mithilfe des Workload Balancer angepasst wurde, kann sich dies auf die geplanten Stunden für einen bestimmten Datumsbereich auswirken, wenn die im Auslastungsbericht ausgewählten Daten nur einen Teil der Dauer einer Aufgabe oder eines Problems enthalten. Informationen zur Anpassung der täglichen Zuordnungen für Benutzer finden Sie unter [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Weitere Informationen finden Sie unter [Informationen zur Ressourcenauslastung anzeigen](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

### Bereich &quot;Rollenzuweisung&quot;

Die im Bereich &quot;Rollenzuweisung&quot;unter &quot;Geplante Stunden&quot;angegebenen Stunden geben die Anzahl der geplanten Stunden an, die mit jeder den Aufgaben oder Problemen des Projekts zugewiesenen Auftragsrolle für die Gesamtdauer des Projekts verbunden sind. Die Zahl entspricht der Rolle Geplante Stunden im Ressourcen-Planer.

>[!TIP]
>
Beachten Sie, dass die mit Benutzern verknüpften geplanten Stunden nicht im Bereich Rollenzuweisung angezeigt werden.

Weitere Informationen finden Sie unter [Rollenzuweisung für Projekte und Initiativen im Arbeitslastausgleich anzeigen](../../../scenario-planner/show-role-allocation-workload-balancer.md).

## Aktualisieren der geplanten Aufgaben auf Grundlage des Durationstyps {#update-task-planned-hours-based-on-duration-type}

Sie können die Gesamtanzahl der geplanten Stunden für Aufgaben beim Bearbeiten von Aufgaben nur aktualisieren, wenn die Aufgaben einen bestimmten Dauerhaltungstyp aufweisen.

Die folgenden Szenarien existieren:

* Sie können geplante Stunden für Aufgaben nur ändern, wenn Sie beim Bearbeiten einer Aufgabe die Typen &quot;Berechnete Zuweisung&quot;oder &quot;Einfache Dauer&quot;verwenden.

  Weitere Informationen zum Typ der berechneten Zuweisungsdauer finden Sie unter [Übersicht über den Dauer-Typ: Berechnete Zuweisung](../../../manage-work/tasks/taskdurtn/calculated-assignment.md).

  Weitere Informationen zum Typ &quot;Einfache Dauer&quot;finden Sie unter [Übersicht über den Dauer-Typ: Einfach](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).

* Sie können die Aufgaben Geplante Stunden im Arbeitslastausgleich nur für Aufgaben vom Typ Einfache Dauer aktualisieren, wenn Sie die Zuordnung der Benutzer zu Aufgaben verwalten. Informationen zum Verwalten von Benutzerzuordnungen im Arbeitslastausgleich finden Sie unter [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
* Sie können die geplanten Stunden für Aufgaben mit einer Dauer vom Typ &quot;Aufwandsorientiert&quot;oder &quot;Berechnete Arbeit&quot;nicht ändern. In diesen Fällen bestimmt Workfront geplante Stunden anhand der Dauer der Aufgabe. In diesem Fall sind die geplanten Stunden jedoch immer gleich der Dauer (in Stunden) und werden von der Prozentzuweisung der zugewiesenen Ressourcen nicht beeinflusst.

  Weitere Informationen zum Typ der anfechtbaren Dauer finden Sie unter [Übersicht über den Durationstyp: Aufwandsorientiert](../../../manage-work/tasks/taskdurtn/effort-driven.md).

  Weitere Informationen zum Typ der berechneten Arbeitsdauer finden Sie unter [Übersicht über den Dauer-Typ: Berechnete Arbeit](../../../manage-work/tasks/taskdurtn/calculated-work.md).

## Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen

Sie können geplante Stunden für Aufgaben aktualisieren, wenn Sie die Zuweisung von Benutzer- oder Auftragsrollen zu Aufgaben manuell aktualisieren. Dies ist nur möglich, wenn für Aufgaben der Typ &quot;Dauer&quot;einfach ist.

Weitere Informationen finden Sie unter [Übersicht über den Dauer-Typ: Einfach](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).

Sie können entweder die Gesamtzuordnung der Benutzer und Rollen, die der Aufgabe zugewiesen sind, oder die tägliche Zuordnung des Benutzers bei Verwendung des Workload Balancer aktualisieren.

Informationen zum Verwalten der Gesamtzahl der Benutzer- und Stellenzuweisungen für Aufgaben finden Sie unter [Verwalten von Benutzer- und Rollenzuordnungsstunden für Aufgaben](../../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md).

Informationen zur Verwaltung der täglichen Zuweisung von Aufgaben finden Sie unter [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Die folgenden Szenarien bestehen beim manuellen Aktualisieren der Zuweisung von Benutzer- oder Auftragsrollen für Aufgaben:

* Wenn Sie die Zuordnung der einzelnen Benutzer oder Rollen nicht manuell aktualisiert haben, um eine Änderung an der Aufgabe Geplante Stunden Trigger, bleiben die geplanten Stunden beim Hinzufügen, Entfernen oder Ersetzen von Zuweisungen für die Aufgabe unverändert. Beim Hinzufügen einer neuen Zuweisung zur Aufgabe werden die einzelnen Zuordnungen zwischen allen Zuweisungsberechtigten neu verteilt.
* Wenn Sie die Zuweisungen manuell aktualisiert haben, um eine Änderung an der Aufgabe Geplante Stunden Trigger, werden die geplanten Stunden reduziert, wenn Sie Zuweisungen aus der Aufgabe entfernen. Sie bleiben unverändert, wenn Sie eine Zuweisung ersetzen.
* Wenn Sie die Zuweisungen manuell aktualisiert haben, um eine Änderung an der Aufgabe Geplante Stunden Trigger, und Sie der Aufgabe eine Zuweisung hinzufügen, wird der neuen Zuweisung standardmäßig 0 Stunden zugewiesen. Sie müssen die Zuordnung der Aufgaben manuell aktualisieren, was sich auf die geplanten Stunden auswirken kann.
* Wenn Sie die Zuweisungen nicht manuell aktualisiert haben, um eine Änderung an der Aufgabe Geplante Stunden Trigger, und Sie alle Zuweisungen für die Aufgabe entfernen, bleiben die geplanten Stunden unverändert.
* Wenn Sie die Zuweisungen manuell aktualisiert haben, um eine Änderung an der Aufgabe Geplante Stunden Trigger, und Sie alle Zuweisungen für die Aufgabe entfernen, werden auch die geplanten Stunden entfernt und die geplanten Stunden der Aufgabe werden 0.

>[!NOTE]
>
Wenn eine Aufgabe beispielsweise 10 geplante Stunden hat und Sie zwei Bevollmächtigte haben, wird ihnen standardmäßig jeweils fünf Stunden zugewiesen.
>
* Wenn Sie die Zuordnung der einzelnen Benutzer oder die täglichen Zuordnungen nicht mit dem Arbeitslastausgleich aktualisieren und einen oder alle Verantwortlichen aus der Aufgabe entfernen, bleibt die Aufgabe Geplant Stunden 10 Stunden.
* Wenn Sie die Zuweisung der Aufgaben manuell auf 4 bzw. 6 Stunden ändern und den Benutzer, der 6 Stunden zugewiesen ist, sowie die Rolle des Auftrags entfernen, wird die Aufgabe Geplante Stunden auf 4 Stunden aktualisiert. Wenn Sie auch den Benutzer entfernen, der 4 Stunden zugewiesen ist, aber die mit dem entfernten Benutzer verknüpfte Auftragsrolle beibehalten, bleiben die geplanten Stunden der Aufgabe 4 Stunden. Wenn Sie den letzten Benutzer entfernen, der 4 Stunden zugewiesen ist, sowie dessen Rolle als Job und die Aufgabe nicht zugewiesen ist, wird die Aufgabe Planed Hours der Aufgabe zu 0.




## Automatisches Aktualisieren von geplanten Aufgaben mithilfe von Arbeitsaufwand

Wenn Sie die Arbeitsaufgabe verwenden, um den für den Abschluss einer Aufgabe erforderlichen Aufwand zu schätzen, wird die Anzahl der geplanten Stunden für die Aufgaben automatisch aktualisiert. Dies ist nur für Aufgaben mit dem Typ Einfache Dauer möglich.

Informationen zur Verwendung von &quot;Arbeitsaufwand&quot;zur Schätzung des Aufgabenaufwands finden Sie unter [Übersicht über den Arbeitsaufwand](../../../manage-work/tasks/task-information/work-effort.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this issue has the explanation of how Planned Hours should work - from Vazgen and Anna: https://hub.workfront.com/issue/6217dced00730b7034c4b808339a35ce/</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Details of their comments: </p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Anna Asatryan</p>
<p>3/22/2022 At 3:16 PM</p>
<p>&nbsp;</p>
<p>to Mark Paul, Corrie Butler, Arman Simonyan, Gagik Khalatyan, Alina Wilson, Artur Sargsyan, Vazgen Babayan, Anna Asatryan</p>
<p>I have done some rough calculations on what the planned hours/revenues should look like Book.xlsx . And if we look, for example at the 2 users highlighted in one of the screenshots their planned hours look way off from what the calculation looks like in the spreadsheet (i.e. equally distributed allocation). When looking at the Workload balancer (the second screenshot), as an example for the user Yashas Mitta, I can see that the allocation has been modified. Obviously the utilization report calculates the allocations based on the modified contouring using the new work per day calculation. The project financial report uses the old, equal distribution of allocation along the full duration of the task. Hence. there is a difference when grouping per periods.</p>
<p>Vazgen Babayan</p>
<p>I believe we will need to prioritise syncing the project financial data report with the new work per day.</p>
<p>Alina Wilson</p>
<p>@Anna Asatryan , do you have a definition of what we should say in documentation (glossary, for example) for how the Planned Hours (or Planned Revenue) is calculated, keeping in mind that we don't document the concept of "workPerDay". We call them "daily allocations", for example, but let me know if that's accurate, too.</p>
<p>Vazgen Babayan</p>
<p>Last Thursday at 3:13 PM</p>
<p>I think an important note here is that regardless the calculation, even if the both views used the same formula, they will not display the same data, because the underlying data sources are different. The Financial Data report does not respect user-entered allocations in Workload Balancer at this moment. So there will be a clear discrepancy, as Anna showed in her message. My recommendation for communication will be to explain that the data sources are different so there can be a mismatch in data and that we will look into addressing that on our roadmap.</p>
<p>Alina Wilson</p>
<p>So far, I hear you guys say this (with my questions for confirmation/ comments in bold):</p>
<p>- the utilization report calculates the allocations based on the modified contouring using the new work per day calculation (so this is what we see in the Workload Balancer, right?)</p>
<p>- the project financial report uses the old, equal distribution of allocation along the full duration of the task (this is before the daily allocations for example were modified in the WB, right?)</p>
<p>I have these additional questions:</p>
<p>- what does the Project Details show? Which Planned Hours, for instance - because earlier, we had a question about this also. - which numbers?</p>
<p>- what does any Planned Hours/ Planned Revenue field that can be pulled in any other report (outside of Financial Data and Utilization reports) show? - which numbers?</p>
<p>- are there any other areas I am not thinking of that we need to document, @Corrie Butler</p>
<p>I will try to document all the possible areas where these display but please help. Thanks!</p>
<p>Vazgen Babayan</p>
<p>Last Saturday at 3:41 PM</p>
<ul>
<li> <p>Confirming the first two points </p> </li>
</ul>
<p>For the following questions</p>
<ul>
<li> <p>Project details show an aggregated sum of task planned hours. It doesn't have anything to do with the work per day because it always deals with total numbers for the whole duration of the Project/Task.</p> </li>
<li> <p>Same thing applies to the Planned Hours and Planned Revenue fields in reports - they show totals for the whole Project/Task duration and thus have no use of work per day.</p> </li>
<li> <p>Can't think of any other fields related to this right now.</p> </li>
<li> <p>In general, if I were to summarize the system behavior, it's as follows:</p> </li>
<li> <p>Every area that only deals with total numbers of Planned Hours / Planned Revenue, uses the numbers entered on the tasks. Those are Task / Project Details, reports exposing those fields.</p> </li>
<li> <p>Areas that deal with time-sensitive portions of Planned Hours / Planned Revenue, use work per day. Those are all Resource Management tools - Workload Balancer, Resource Planner, Utilization Report, importing projects via Scenario Planner.</p> </li>
<li> <p>All the areas in the second point support user-edited allocations made in Workload Balancer.</p> </li>
<li> <p>Scheduling area and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from Workload Balancer.</p> </li>
<li> <p>Scheduling will be removed this year, and we need to do work to move the Project Financial Data reports to the new work per day sometime after Q3.</p> </li>
</ul>
<p>Alina Wilson</p>
<p>@Vazgen Babayan , one clarifying question: when you say "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" - you mean that those use the system default which spreads the allocations evenly, correct? Because you can edit (daily) allocations in Scheduling tools, but it doesn't use that, correct? It uses the default of the daily allocation that the system figures out when dividing the Planned Hours by the number of days in the Duration. Please let me know. And thanks!</p>
<p>Anna Asatryan</p>
<p>Yesterday at 11:42 AM</p>
<p>@Alina Wilson , that's correct, when saying "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" Vazgen meant that it spreads the allocation evenly.</p>
<p>As for the scheduling, the allocation modification that's being done there isn't reflected anywhere else in the application other than in the Scheduling itself. That's probably one of the reasons it's being deprecated.</p>
</div>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <br> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below is drafted because I replaced it with the table above)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can find the Planned Hours information on tasks, issues, or projects in the following locations:</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours in the Details  section  of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours in the Details  section  is identical for tasks, issues, and projects. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the Planned Hours value on the Details  section  of a task: </p>
<ol>
<li value="1">Go to a task for which you want to review the Planned Hours.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Overview</strong> area and notice the Planned Hours value.</p> <p>This value represents the time it would take the user assigned to the task to complete it. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3> </h3>
<p>The Planned Hours in the Edit box of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours while editing a task or an issue is identical. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the value of Planned Hours while editing a task:</p>
<ol>
<li value="1">Go to the task or issue you want to view Planned Hours for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> <p>The Planned Hours are located in the <strong>Overview</strong> section. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours column is included in the Standard view of a task list, by default. For issues and projects, you can add it to the view, when you are editing the view or when you build a report. </p>
<p>The Planned Hours in a task, issue, or project report are the total Planned Hours of the respective item as they display in the Details  section  or the Edit box of the items. </p>
<p>Adding the Planned Hours column to a project view is similar to building a view in a project report. </p>
<p>To show Planned Hours in a project report:</p>
<ol>
<li value="1"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Workfront, then click <strong>Reports</strong>. </p> </li>
<li value="2">Click <strong>New Report</strong>, then choose <strong>Project</strong> as your object.</li>
<li value="3">Click <strong>Add Column</strong>, and start typing <strong>Planned Hours</strong> when the <strong>Show in this column</strong> drop-down field is displayed. Select the field when it appears in the list.</li>
<li value="4"> <p>Click <strong>Save + Close</strong> to save the report. </p> <p>The Planned Hours column shows the total number of Planned Hours on each project. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Planned Hours in Resource Management tools</p> <note type="important">
When viewing Planned Hours in the Resource Management tools by a specific time frame, the daily allocations for each work item and the daily allocations for the resources assigned to the work items during that time frame can influence the daily Planned Hours of projects or work items.
</note>
<p>You can see the value of Planned Hours for your tasks, issues, or projects when using the following Resource Management tools:</p>
<ul>
<li> <p>Resource Planner</p> <p>For information about using the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p> </li>
<li> <p>Utilization Report.</p> <p>For information about the utilization report, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </li>
<li>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Workload Balancer or Scheduling areas in the following sections:</p>
<ul>
<li>Scheduling or Workload Balancer sections in the Resourcing area</li>
<li>Scheduling or Workload Balancer section at the project level</li>
<li>Schedule or Workload Balancer section at the team level</li>
</ul>
</div> <p>For information about scheduling resources, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p> <p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Workload Balancer overview</a>. </p> </li>
<li> <p><b>Role Allocation panel</b> in the project  task list or  Workload Balancer: The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see <a href="../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md" class="MCXref xref">View project Planned Hours in the Role Allocation panel</a>. </p> </li>
</ul>
</div>
-->
