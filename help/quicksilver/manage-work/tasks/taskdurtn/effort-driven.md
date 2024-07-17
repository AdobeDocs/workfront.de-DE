---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Duration Type overview: Effort Driven'
description: '"Anstrengung gesteuert"ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Durationstypen in Workfront finden Sie unter Übersicht über die Aufgabendauer und -dauer.'
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 1%

---

# Übersicht über den Durationstyp: Aufwandsorientiert

&quot;Anstrengung gesteuert&quot;ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Durationstypen in Workfront finden Sie unter [Übersicht über die Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Übersicht über die Dauer des Aufwands

Ihr Workfront- oder Gruppenadministrator kann den Standardtyp für die Dauer Ihres Systems oder Ihrer Gruppe auf &quot;Aufwandsgesteuert&quot;festlegen. In diesem Fall werden alle neuen Aufgaben mit diesem Typ Dauer erstellt. Informationen zum Ändern der Aufgaben- und Ausgabevoreinstellungen als Teil Ihrer Projektanforderungen auf System- oder Gruppenebene finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

In diesem Szenario besteht die Gefahr, den Projektplan willkürlich zu verkürzen, es sei denn, Sie als Projektmanager sollten sich die Zeit nehmen, um zu überlegen, ob es sich bei der Aufgabe tatsächlich um eine Aufgabe handelt, die von Effort geleitet wird.

Verwenden Sie die Aufwandsanalyse für Folgendes:

* Bestimmen Sie die geplante Dauer basierend auf der Anzahl der Ressourcen, die für die Bearbeitung der Aufgabe verfügbar sind. Die Dauer entspricht den geplanten Stunden. Die geplante Dauer entspricht der Anzahl der geplanten Stunden dividiert durch die Anzahl der Bevollmächtigten.

  Der auf die Aufgabe angewendete Aufwand bestimmt die Arbeitsteilung und Dauer.

* Verfolgen Sie die Gesamtzahl der Stunden, die für eine Aufgabe verbracht wurden, wenn mehrere Ressourcen zugewiesen sind.

  Wenn Ressourcen hinzugefügt werden, nimmt die geplante Dauer der Aufgabe ab. (Der Grundsatz &quot;Viele Hände machen Licht funktionieren&quot;zeigt die Auswirkungen dieses Typs auf die geplante Dauer einer Aufgabe.)

In den folgenden Abschnitten finden Sie detailliertere Informationen dazu, wie Workfront die geplante Dauer einer anstrengenden Aufgabe berechnet und wie sich das Hinzufügen von Ressourcen auf die Aufgabe mit diesem Dauerhaltungstyp auswirkt.

## Übersicht über die Formel für die Aufwandsgesteuerte Dauer

Die Formel zur Berechnung der geplanten Dauer einer Aufgabe mit dem Typ Dauer des Aufwands hängt vom Zuordnungsprozentsatz jeder Ressource ab, die der Aufgabe zugewiesen ist. Im Falle einer anstrengenden Aufgabe berechnet Workfront die geplanten Stunden der Aufgabe und sie entsprechen immer der Dauer der Aufgabe:

```
Planned Hours (in hours) = Duration (in days)
```

Sie können die Dauer der Aufgabe manuell anpassen.

Workfront geht davon aus, dass ein Arbeitstag acht Arbeitsstunden umfasst. Ihr Workfront- oder Gruppenadministrator definiert die Arbeitsstunden pro Arbeitstag mit der Einstellung &quot;Typische Stunden pro Arbeitstag&quot;in den Projektanvoreinstellungen im Setup. Weitere Informationen zum Ändern der Aufgaben- und Problemvoreinstellungen als Teil Ihrer Projektanforderungen auf Systemebene finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront berücksichtigt den Zeitplan für jede der Aufgabe zugewiesene Ressource, um den Prozentsatz der Zuordnung für jede Ressource für die Aufgabe zu bestimmen. Informationen zum Erstellen und Zuweisen von Zeitplänen für Benutzer finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Betrachten Sie die folgenden Szenarien:

* [Die Ressourcen werden zu 100 % der Aufgabe zugewiesen](#resources-are-allocated-100-to-the-task)
* [Ressourcen werden für verschiedene Zeitprozentsätze für die Aufgabe zugewiesen](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Die Ressourcen werden zu 100% der Aufgabe zugewiesen. {#resources-are-allocated-100-to-the-task}

Bei dieser Formel wird davon ausgegangen, dass der Aufgabe alle Ressourcen zu 100 % zugewiesen sind.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Bei dieser Berechnung wird davon ausgegangen, dass die Anzahl der Stunden an einem normalen Arbeitstag 8 beträgt. Die Gleichung enthält diesen Wert, sodass die geplante Dauer in Tagen angezeigt wird.

### Ressourcen werden für verschiedene Zeitprozentsätze für die Aufgabe zugewiesen {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Da jede zugewiesene Ressource über eine eindeutige Zuordnungsebene verfügen kann, berücksichtigt die aktuelle Formel die folgenden Zuordnungswerte:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Bei dieser Berechnung wird davon ausgegangen, dass die Anzahl der Stunden an einem normalen Arbeitstag 8 beträgt. Die Gleichung enthält diesen Wert, sodass die geplante Dauer in Tagen angezeigt wird.

## Das Hinzufügen von mehr Ressourcen zu einer Aufgabe

Beim Hinzufügen oder Entfernen von Bevollmächtigten zu einer Aufgabe mit dem Typ &quot;Aufwandsgesteuerte Dauer&quot;, &quot;Dauer&quot;und &quot;Geplante Stunden&quot;ändern sich nicht. Die geplante Dauer ändert sich jedoch.

Im folgenden Beispiel ist die Standardzeit pro Arbeitstag in den Projekteinstellungen in Ihrem System-Setup auf 8 gesetzt. Da die Dauer 3 Tage beträgt, wird die geplante Stunde auf 24 Tage eingestellt (3 Tage x 8 Stunden pro Arbeitstag = 24 geplante Stunden).

>[!NOTE]
>
>Bei der Verwendung der Task-Beschränkung &quot;Feste Datumswerte&quot;bleibt die geplante Dauer beim Hinzufügen oder Entfernen von Bevollmächtigten gleich. Stattdessen werden die Dauer und die geplanten Stunden angepasst. Bei Verwendung einer anderen Aufgabenbegrenzung als &quot;Feste Datumswerte&quot;wird die geplante Dauer angepasst.

Die folgende Tabelle zeigt, wie sich die geplante Dauer ändert, indem Ressourcen zur Aufgabe hinzugefügt werden:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Anzahl der zugewiesenen Personen (jeweils 100 %)</strong> </p> </th> 
   <th> <p><strong>Dauer</strong> </p> </th> 
   <th> <p><strong>Geplante Stunden</strong> </p> </th> 
   <th><strong>Geplante Dauer</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 Tage</p> </td> 
   <td> <p>24 Stunden</p> <p>(3 Tage x 8 Stunden pro Arbeitstag = 24 geplante Stunden)</p> </td> 
   <td> <p>3 Tage</p> <p>(24 geplante Stunden / 1 Bevollmächtigter = 3 Tage)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 Tage</p> </td> 
   <td> <p>24 Stunden</p> <p>(3 Tage x 8 Stunden pro Arbeitstag = 24 geplante Stunden)</p> </td> 
   <td> <p>1,5 Tage</p> <p>(24 geplante Stunden/ 2 Zuweisung = 12 Stunden oder 1,5 Tage)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 Tage</p> </td> 
   <td> <p>24 Stunden</p> <p>(3 Tage x 8 Stunden pro Arbeitstag = 24 geplante Stunden)</p> </td> 
   <td> <p>1 Tag</p> <p>(24 geplante Stunden/ 3 Zuweisung = 8 Stunden oder 1 Tag)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändern Sie die Dauer einer Aufgabe in &quot;Anstrengung gesteuert&quot;

Weitere Informationen zum Ändern des Dauer-Typs einer Aufgabe finden Sie unter [Aktualisieren des Dauer-Typs einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
