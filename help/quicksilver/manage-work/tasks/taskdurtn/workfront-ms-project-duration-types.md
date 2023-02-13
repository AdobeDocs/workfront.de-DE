---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Arten von Dauer in Adobe Workfront- und Microsoft-Projekten
description: Die in Adobe Workfront verfügbaren Durationstypen unterscheiden sich von den entsprechenden Typen im Microsoft-Projekt, die als Aufgabentypen bezeichnet werden. Dies kann beim Exportieren oder Importieren von Projekten zwischen Workfront und Microsoft Project manchmal verwirrend sein.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Arten von Dauer in Adobe Workfront- und Microsoft-Projekten

Die in Adobe Workfront verfügbaren Durationstypen unterscheiden sich von den entsprechenden Typen im Microsoft-Projekt, die als Aufgabentypen bezeichnet werden. Dies kann beim Exportieren oder Importieren von Projekten zwischen Workfront und Microsoft Project manchmal verwirrend sein.

Informationen zum Importieren und Exportieren von Projekten zwischen Workfront und Microsoft Project finden Sie in den folgenden Artikeln:

* [Projekt in ein Microsoft-Projekt exportieren](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importieren eines Projekts aus einem Microsoft-Projekt](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Arten von Dauer in Workfront- und Microsoft-Projekten

Workfront verfügt über vier Aufgabenlaufzeittypen:

* Einfach
* Leistungsgesteuert
* Berechnete Arbeit
* Berechnete Zuweisung

Weitere Informationen finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Diese Dauertypen werden vom Microsoft-Projekt nicht erkannt. Derzeit gibt es in Microsoft Project drei Aufgabentypen, die den Duration Types in Workfront ähneln:

* Feste Einheiten
* Feste Arbeit
* Feste Dauer

## Änderungen am Durationstyp beim Export von Workfront in MS Project

Beim Export von Projekten aus Workfront in Microsoft Project werden anstrengende Aufgaben zu &quot;Feste Arbeit&quot;. Einfache, berechnete Arbeit und berechnete Zuweisung werden zu festen Einheiten.

## Änderungen des Durationstyps beim Import aus MS Project in Workfront

Beim Importieren von Projekten aus Microsoft Project in Workfront werden feste Einheiten zu Aufwandsorientiert. Feste Arbeit und feste Dauer erhalten den Standardlaufzeittyp, den Ihr Workfront-Administrator für Ihr System ausgewählt hat. Weitere Informationen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
