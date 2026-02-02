---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Dauertyp - Übersicht: Berechnete Arbeit'
description: Berechnete Arbeit ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Dauertypen in Workfront finden Sie unter Übersicht über die Aufgabendauer und den Dauertyp.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 2%

---

# Dauertyp - Übersicht: Berechnete Arbeit

Berechnete Arbeit ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Dauertypen in Workfront finden Sie unter [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Übersicht über den Typ der berechneten Arbeitsdauer

Berechnete Arbeit bestimmt den Aufwand (geplante Stunden), der für die Erfüllung der Aufgabe erforderlich ist. Es wird empfohlen, den Typ Berechnete Arbeitsdauer zu verwenden, wenn die der Aufgabe zugewiesenen Ressourcen für die gesamte Dauer der Aufgabe zugewiesen sind.

Ihr Workfront-Administrator oder ein Gruppenadministrator kann den Standarddauertyp Ihres Systems oder Ihrer Gruppe als berechnete Arbeit festlegen. In diesem Fall werden alle neuen Aufgaben mit diesem Dauertyp erstellt. Informationen zum Ändern der Voreinstellungen für Aufgaben und Probleme als Teil der Voreinstellungen für Projekte auf Systemebene oder Gruppenebene finden Sie unter [Konfigurieren von systemweiten Voreinstellungen für Aufgaben und Probleme](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Beim Hinzufügen von Ressourcen zu einer Aufgabe kann ein Projektmanager erwarten, dass der geplante Aufwand zunimmt. Beispiel: Ein einstündiges Planungstreffen mit drei Ressourcen stellt insgesamt drei Arbeitsstunden dar, und ein einstündiges Planungstreffen mit zehn Ressourcen stellt zehn Arbeitsstunden dar. Dabei wird davon ausgegangen, dass jede Ressource der Aufgabe mit 100%iger Zuordnung zugeordnet ist.

## Formel zur Berechnung des erforderlichen Arbeitsaufwands bei Verwendung des Typs Berechnete Arbeitsdauer überprüfen

Wenn Sie den Typ „Berechnete Arbeitsdauer“ für eine Aufgabe verwenden, berechnet Workfront den Arbeitsaufwand für jede Aufgabe anhand der beiden folgenden Formeln. Die Formeln unterscheiden sich je nachdem, wie viel Prozent der Zeit jede Ressource der Aufgabe zugewiesen ist und wie viele Ressourcen Sie jeder Aufgabe zugewiesen haben:

* Vereinfachte Formel: Angenommen, dem Vorgang ist eine Ressource zugeordnet und sie wird dem Vorgang zu 100 % ihrer verfügbaren Zeit zugeordnet, wird der Wert Arbeit erforderlich für jeden Vorgang anhand der folgenden Formel berechnet:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Komplexe Formel: Wenn Sie jede Ressource mit verschiedenen Zuteilungen zuordnen, berücksichtigt die Formel diese Zuteilungen und berücksichtigt diese Varianten:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Überprüfen der Auswirkungen des Hinzufügens oder Entfernens von Ressourcen aus der Aufgabe

Beim Hinzufügen oder Entfernen von Zugewiesenen zu einer Aufgabe mit dem Typ „Berechnete Arbeitsdauer“ kann die Dauer manuell bearbeitet werden. Wenn zugewiesene Personen zur Aufgabe hinzugefügt oder daraus entfernt werden, ändern sich die geplanten Stunden.

Im folgenden Beispiel wird in den Projektvoreinstellungen unter „Setup“ für „Typische Stunden pro Arbeitstag“ der Wert 8 festgelegt. Jede Aufgabe hat eine Dauer von 1 Tag. Wenn sich die Anzahl der Bevollmächtigten ändert, ändert sich die geplante Arbeitszeit entsprechend der Anzahl der Bevollmächtigten für eine bestimmte Aufgabe:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Anzahl der Zugewiesenen (jeweils 100 % zugewiesen)</strong> </p> </th> 
   <th> <p><strong>Dauer</strong> </p> </th> 
   <th> <p><strong>Geplante Stunden</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 Tag</p> </td> 
   <td> <p>8 Stunden</p> <p>(1 Tag x 8 Stunden pro Arbeitstag x 1 Verantwortlicher = 8 geplante Stunden)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 Tag</p> </td> 
   <td> <p>16 Stunden</p> <p>(1 Tag x 8 Stunden pro Arbeitstag x 2 Beauftragte = 16 geplante Stunden)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 Tag</p> </td> 
   <td> <p>24 Stunden</p> <p>(1 Tag x 8 Stunden pro Arbeitstag x 3 Beauftragte = 24 geplante Stunden)</p> </td> 
  </tr> 
 </tbody> 
</table>

In diesem Fall wird jeder Verantwortliche zu 100 % der Aufgabe „Berechnete Arbeit“ zugewiesen.

![Typ der berechneten Arbeitsdauer](assets/calcwork-350x71.png)

## Ändern des Dauertyps einer Aufgabe in „Berechnete Arbeit“

Informationen zum Ändern des Dauertyps einer Aufgabe finden Sie unter [Aktualisieren des Dauertyps einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
