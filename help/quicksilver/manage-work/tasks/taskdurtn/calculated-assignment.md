---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Dauertyp - Übersicht: Berechnete Zuweisung'
description: Berechnete Zuweisung ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Dauertypen in Workfront finden Sie unter Übersicht über die Aufgabendauer und den Dauertyp.
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Dauertyp - Übersicht: Berechnete Zuweisung

<!-- Audited: 5/2025 -->

Berechnete Zuweisung ist ein Dauertyp, den Sie für eine Aufgabe in Adobe Workfront festlegen können. Allgemeine Informationen zu den Dauertypen in Workfront finden Sie unter [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Übersicht über den Typ der berechneten Dauer der Zuweisung

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* Wenn Sie den Dauertyp Berechnete Zuweisung verwenden, müssen Sie sowohl eine Dauer als auch eine Anzahl geplanter Stunden für die Aufgabe angeben. Workfront teilt dann die Anzahl der geplanten Stunden durch die Anzahl der Stunden in der Duration und dann durch die Anzahl der Ressourcen, die der Aufgabe zugewiesen wurden, um den Zuordnungsprozentsatz für jede Ressource zu berechnen (berechnet die Zuordnung). Jede Ressource hat für ihren Zuordnungsprozentsatz denselben Wert. In diesem Fall können Sie die Zuordnungswerte für die einzelnen Ressourcen nicht ändern.
* Ihr Workfront-Administrator oder ein Gruppenadministrator kann den Standarddauertyp Ihres Systems oder Ihrer Gruppe als Berechnete Zuweisung festlegen. In diesem Fall werden alle neuen Aufgaben mit diesem Dauertyp erstellt. Informationen zum Ändern der Voreinstellungen für Aufgaben und Probleme als Teil der Voreinstellungen für Projekte auf Systemebene oder Gruppenebene finden Sie unter [Konfigurieren von systemweiten Voreinstellungen für Aufgaben und Probleme](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  In diesem Fall hat die Aufgabe den Standardwert einer eintägigen Dauer und 0 Stunden geplanter Stunden. Wenn der Projekt-Manager keine genauere Dauer festlegt und das Feld Geplante Stunden mit einer realistischen Schätzung ausfüllt, werden die Ressourcen nicht ausreichend zugewiesen.

Berechnete Zuweisung ist in folgenden Situationen der bevorzugte Dauertyp:

* Wenn Arbeitsaufträge ein Aktivitätsfenster haben, aber nicht die gesamte zugewiesene Dauer benötigen, um ihre Arbeit abzuschließen. Beispielsweise werden Sie beauftragt, Ihrem Vorgesetzten bis zum Ende der Woche einen Bericht zu übermitteln. Sie haben eine Dauer von fünf Tagen, aber es dauert nur 10 Stunden, um das Dokument zu entwerfen.
* Wenn einer Aufgabe eine einzelne Ressource zugewiesen wird, weil der Projektmanager die geplante Dauer und den geplanten Aufwand unabhängig voneinander schätzen kann.

  Sie können für dasselbe Ergebnis den Typ „Berechnete Arbeitsdauer“ verwenden. Der Projektmanager muss jedoch einen Prozentwert für die Zuordnung der Ressource eingeben, damit sich dies auf den berechneten Wert für „Geplante Stunden“ auswirkt. Dadurch wird die Projektplanung schwieriger und zeitaufwendiger.

Der Prozentsatz der Zuordnung für jede Ressource wird wie folgt berechnet:

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

Im unten beschriebenen Szenario hat beispielsweise jede Aufgabe eine Dauer von 3 Tagen. Der Projekt-Manager gibt manuell die Dauer (3 Tage oder 24 Stunden) und die geplanten Stunden ein. Infolgedessen wird der Prozentsatz der Zuordnung (oder der Zuweisungsprozentsatz) berechnet:

![Typ der berechneten ](assets/calcassign-350x80.png)

## Ändern des Dauertyps einer Aufgabe in „Berechnete Zuweisung“

Informationen zum Ändern des Dauertyps einer Aufgabe finden Sie unter [Aktualisieren des Dauertyps einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
