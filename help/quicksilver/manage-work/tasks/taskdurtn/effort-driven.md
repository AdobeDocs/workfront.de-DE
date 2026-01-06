---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Übersicht über den Dauertyp: Leistungsgesteuert'
description: Aufwandsgesteuert ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Dauertypen in Workfront finden Sie unter Übersicht über die Aufgabendauer und den Dauertyp.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 1%

---

# Übersicht über den Dauertyp: Leistungsgesteuert

Aufwandsgesteuert ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Dauertypen in Workfront finden Sie unter [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Übersicht über den Typ der leistungsgesteuerten Dauer

Ihr Workfront-Administrator oder ein Gruppenadministrator kann den Standarddauertyp Ihres Systems oder Ihrer Gruppe als leistungsgesteuert festlegen. In diesem Fall werden alle neuen Aufgaben mit diesem Dauertyp erstellt. Informationen zum Ändern der Voreinstellungen für Aufgaben und Probleme als Teil der Voreinstellungen für Projekte auf Systemebene oder Gruppenebene finden Sie unter [Konfigurieren von systemweiten Voreinstellungen für Aufgaben und Probleme](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

In diesem Szenario besteht die Gefahr einer willkürlichen Verkürzung des Projektplans, es sei denn, Sie als Projektmanager nehmen sich die Zeit zu überlegen, ob die Aufgabe tatsächlich eine leistungsgesteuerte Aufgabe ist.

Nutzung von Effort Driven für:

* Bestimmen Sie die geplante Dauer anhand der Anzahl der für die Arbeit an der Aufgabe verfügbaren Ressourcen. Dauer ist gleich den geplanten Stunden. Die geplante Dauer ist gleich der geplanten Stunden dividiert durch die Anzahl der zugewiesenen Personen.

  Die Arbeitsteilung und die Dauer hängen von dem Aufwand für die Aufgabe ab.

* Verfolgen Sie die Gesamtzahl der Stunden, die mit einer Aufgabe verbracht wurden, wenn mehrere Ressourcen zugewiesen sind.

  Durch das Hinzufügen von Ressourcen verringert sich die geplante Dauer der Aufgabe. (Das Prinzip „Viele Hände machen leichte Arbeit“ veranschaulicht den Effekt, den dieser Dauertyp auf die geplante Dauer einer Aufgabe hat.)

In den folgenden Abschnitten finden Sie genauere Informationen darüber, wie Workfront die geplante Dauer eines leistungsgesteuerten Vorgangs berechnet und welche Auswirkung das Hinzufügen von Ressourcen zu dem Vorgang mit diesem Dauertyp hat.

## Übersicht über die Formel für den leistungsgesteuerten Dauertyp

Die Formel zur Berechnung der geplanten Dauer für einen Vorgang mit dem Typ „Dauer“ des leistungsgesteuerten Vorgangs hängt vom Zuordnungsprozentsatz jeder Ressource ab, die dem Vorgang zugewiesen ist. Bei einem leistungsgesteuerten Vorgang berechnet Workfront die geplanten Stunden des Vorgangs, wobei diese immer mit der Aufgabendauer übereinstimmen:

```
Planned Hours (in hours) = Duration (in days)
```

Sie können die Dauer der Aufgabe manuell anpassen.

Workfront geht davon aus, dass ein Arbeitstag acht Arbeitsstunden hat. Der Workfront- oder Gruppenadministrator definiert die Stunden pro Arbeitstag mit der Einstellung „Typische Stunden pro Arbeitstag“ in den Projektvoreinstellungen im Setup. Weitere Informationen zum Ändern der Voreinstellungen für Aufgaben und Probleme im Rahmen der Projektvoreinstellungen auf Systemebene finden Sie unter [Konfigurieren von systemweiten Voreinstellungen für Aufgaben und Probleme](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront berücksichtigt den Zeitplan für jede Ressource, die dem Vorgang zugeordnet ist, um den Prozentsatz der Zuordnung für jede Ressource für den Vorgang zu bestimmen. Informationen zum Erstellen und Zuweisen von Zeitplänen zu Benutzern finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Betrachten Sie die folgenden Szenarien:

* [Ressourcen werden zu 100 % der Aufgabe zugewiesen](#resources-are-allocated-100-to-the-task)
* [Die Ressourcen werden der Aufgabe zu unterschiedlichen Prozentsätzen zugewiesen](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Ressourcen werden zu 100 % der Aufgabe zugewiesen {#resources-are-allocated-100-to-the-task}

Bei dieser Formel wird davon ausgegangen, dass alle Ressourcen zu 100 % der Aufgabe zugewiesen sind.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Bei dieser Berechnung wird davon ausgegangen, dass die Anzahl der Stunden an einem normalen Arbeitstag 8 beträgt. Die Gleichung enthält diesen Wert, sodass die geplante Dauer in Tagen angezeigt wird.

### Die Ressourcen werden der Aufgabe zu unterschiedlichen Prozentsätzen zugewiesen {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Da jede zugewiesene Ressource über eine eindeutige Zuordnungsebene verfügen kann, berücksichtigt die tatsächliche Formel diese Zuordnungswerte:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Bei dieser Berechnung wird davon ausgegangen, dass die Anzahl der Stunden an einem normalen Arbeitstag 8 beträgt. Die Gleichung enthält diesen Wert, sodass die geplante Dauer in Tagen angezeigt wird.

## Das Hinzufügen weiterer Ressourcen zu einer Aufgabe

Beim Hinzufügen oder Entfernen von Zugewiesenen zu einer Aufgabe mit dem Typ „Arbeitsgesteuerte Dauer“ ändern sich die Dauer und die geplanten Stunden nicht. Die geplante Dauer ändert sich jedoch.

Im folgenden Beispiel ist die Option Typische Stunden pro Arbeitstag in den Projektvoreinstellungen in Ihrem System-Setup auf 8 festgelegt. Da die Dauer 3 Tage beträgt, wird die geplante Stunde auf 24 festgelegt (3 Tage x 8 Stunden pro Arbeitstag = 24 geplante Stunden).

>[!NOTE]
>
>Bei Verwendung der Aufgabenbeschränkung Feste Daten bleibt die geplante Dauer beim Hinzufügen oder Entfernen von Beauftragten gleich. Stattdessen werden die Dauer und die geplanten Stunden angepasst. Bei Verwendung einer anderen Aufgabenbeschränkung als „Festes Datum“ wird die geplante Dauer angepasst.

Die folgende Tabelle zeigt, wie sich die geplante Dauer durch das Hinzufügen von Ressourcen zur Aufgabe ändert:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Anzahl der Zugewiesenen (jeweils 100 % zugewiesen)</strong> </p> </th> 
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
   <td> <p>3 Tage</p> <p>(24 geplante Stunden / 1 Verantwortlicher = 3 Tage)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 Tage</p> </td> 
   <td> <p>24 Stunden</p> <p>(3 Tage x 8 Stunden pro Arbeitstag = 24 geplante Stunden)</p> </td> 
   <td> <p>1,5 Tage</p> <p>(24 geplante Stunden / 2 Empfänger = 12 Stunden oder 1,5 Tage)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 Tage</p> </td> 
   <td> <p>24 Stunden</p> <p>(3 Tage x 8 Stunden pro Arbeitstag = 24 geplante Stunden)</p> </td> 
   <td> <p>1 Tag</p> <p>(24 geplante Stunden / 3 Bevollmächtigte = 8 Stunden oder 1 Tag)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändern des Dauertyps einer Aufgabe in „Leistungsgesteuert“

Informationen zum Ändern des Dauertyps einer Aufgabe finden Sie unter [Aktualisieren des Dauertyps einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
