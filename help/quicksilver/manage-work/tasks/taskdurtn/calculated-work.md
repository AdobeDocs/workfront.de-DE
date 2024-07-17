---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Duration Type overview: Calculated Work'
description: '"Berechnete Arbeit"ist eine Dauer, die Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Durationstypen in Workfront finden Sie unter Übersicht über die Aufgabendauer und -dauer.'
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# Übersicht über den Dauer-Typ: Berechnete Arbeit

&quot;Berechnete Arbeit&quot;ist eine Dauer, die Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Durationstypen in Workfront finden Sie unter [Übersicht über die Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Übersicht über den Typ der berechneten Arbeitsdauer

Berechnete Arbeit bestimmt den Aufwand (geplante Stunden), der zum Abschluss der Aufgabe erforderlich ist. Es wird empfohlen, den Typ &quot;Berechnete Arbeitsdauer&quot;zu verwenden, wenn die der Aufgabe zugewiesenen Ressourcen für die gesamte Dauer der Aufgabe zugewiesen sind.

Ihr Workfront- oder Gruppenadministrator kann den Standardtyp für die Dauer Ihres Systems oder Ihrer Gruppe als &quot;Berechnete Arbeit&quot;festlegen. In diesem Fall werden alle neuen Aufgaben mit diesem Typ Dauer erstellt. Informationen zum Ändern der Aufgaben- und Ausgabevoreinstellungen als Teil Ihrer Projektanforderungen auf System- oder Gruppenebene finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Wenn Ressourcen zu einer Aufgabe hinzugefügt werden, kann ein Projektmanager mit einer geplanten Erhöhung des Aufwands rechnen. Ein einstündiges Planungstreffen mit drei Ressourcen stellt beispielsweise drei Gesamtarbeitsstunden dar, und ein einstündiges Planungstreffen mit zehn Ressourcen stellt zehn Arbeitsstunden dar. Dabei wird davon ausgegangen, dass jede Ressource der Aufgabe mit 100 % Zuordnung zugewiesen ist.

## Überprüfen Sie die Formel zur Berechnung der erforderlichen Arbeit bei Verwendung des Typs &quot;Berechnete Arbeitsdauer&quot;.

Wenn Sie den Typ &quot;Berechnete Arbeitsdauer&quot;für eine Aufgabe verwenden, berechnet Workfront die Arbeitsleistung für jede Aufgabe anhand der folgenden beiden Formeln. Die Formeln variieren je nachdem, welcher Prozentsatz der Zeit der Zuweisung der einzelnen Ressourcen zu der Aufgabe entspricht und wie viele Ressourcen Sie den einzelnen Aufgaben zugewiesen haben:

* Vereinfachte Formel: Wenn Sie der Aufgabe eine Ressource zugewiesen haben und sie der Aufgabe für 100 % ihrer verfügbaren Zeit zugewiesen sind, wird der Wert für &quot;Arbeit erforderlich&quot;für jede Aufgabe anhand der folgenden Formel berechnet:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Komplexe Formel: Wenn Sie jede Ressource mit verschiedenen Zuordnungen zuweisen, berücksichtigt die Formel diese Zuordnungen und berücksichtigt diese Varianten:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Überprüfen Sie den Effekt des Hinzufügens oder Entfernen von Ressourcen aus der Aufgabe

Beim Hinzufügen oder Entfernen von Bevollmächtigten zu einer Aufgabe mit dem Typ &quot;Berechnete Arbeitsdauer&quot;kann die Dauer manuell bearbeitet werden. Wenn Zuweisung hinzugefügt oder aus der Aufgabe entfernt werden, ändern sich die geplanten Stunden.

Im folgenden Beispiel wird unter &quot;Projektvoreinstellungen&quot;unter &quot;Einrichtung&quot;für &quot;Typische Stunden pro Arbeitstag&quot;der Wert &quot;8&quot;festgelegt. Jede Aufgabe hat eine Dauer von 1 Tag. Da sich die Anzahl der Bevollmächtigten ändert, hängt die Anzahl der geplanten Stunden von der Anzahl der Bevollmächtigten für eine bestimmte Aufgabe ab:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Anzahl der zugewiesenen Personen (jeweils 100 %)</strong> </p> </th> 
   <th> <p><strong>Dauer</strong> </p> </th> 
   <th> <p><strong>Geplante Stunden</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 Tag</p> </td> 
   <td> <p>8 Stunden</p> <p>(1 Tag x 8 Stunden pro Arbeitstag x 1 Bevollmächtigter = 8 geplante Stunden)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 Tag</p> </td> 
   <td> <p>16 Stunden</p> <p>(1 Tag x 8 Stunden pro Arbeitstag x 2 Zuweisung = 16 geplante Stunden)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 Tag</p> </td> 
   <td> <p>24 Stunden</p> <p>(1 Tag x 8 Stunden pro Arbeitstag x 3 Zuweisung = 24 geplante Stunden)</p> </td> 
  </tr> 
 </tbody> 
</table>

In diesem Fall wird jedem Bevollmächtigten 100 % der Aufgabe &quot;Berechnete Arbeit&quot;zugewiesen.

![](assets/calcwork-350x71.png)

## Ändern Sie den Aufgabentyp in &quot;Berechnete Arbeit&quot;

Weitere Informationen zum Ändern des Dauer-Typs einer Aufgabe finden Sie unter [Aktualisieren des Dauer-Typs einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
