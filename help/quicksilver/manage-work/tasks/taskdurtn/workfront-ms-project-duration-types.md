---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Dauertypen in Adobe Workfront- und Microsoft-Projekten
description: Die in Adobe Workfront verfügbaren Dauertypen unterscheiden sich von ihren Gegenstücken im Microsoft-Projekt, die als Aufgabentypen bezeichnet werden. Dies kann beim Exportieren oder Importieren von Projekten zwischen Workfront und Microsoft Project manchmal verwirrend sein.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Dauertypen in Adobe Workfront- und Microsoft-Projekten

Die in Adobe Workfront verfügbaren Dauertypen unterscheiden sich von ihren Gegenstücken im Microsoft-Projekt, die als Aufgabentypen bezeichnet werden. Dies kann beim Exportieren oder Importieren von Projekten zwischen Workfront und Microsoft Project manchmal verwirrend sein.

Informationen zum Importieren und Exportieren von Projekten zwischen Workfront und Microsoft Project finden Sie in den folgenden Artikeln:

* [Exportieren eines Projekts in das Microsoft-Projekt](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importieren eines Projekts aus dem Microsoft-Projekt](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Dauertypen in Workfront- und Microsoft-Projekten

Workfront verfügt über vier Typen von Aufgabendauer:

* Einfach
* Leistungsgesteuert
* Berechnete Arbeit
* Berechnete Zuweisung

Weitere Informationen finden Sie unter [Übersicht über Aufgabendauer und -typ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Diese Dauertypen werden vom Microsoft-Projekt nicht erkannt. Derzeit verfügt Microsoft Project über drei Aufgabentypen, die den Dauertypen in Workfront ähneln:

* Feste Einheiten
* Festarbeit
* Feste Dauer

## Der Dauertyp ändert sich beim Exportieren aus Workfront in MS Project

Beim Exportieren von Projekten aus Workfront in Microsoft Project werden leistungsgesteuerte Aufgaben zu Festaufgaben. Einfache, berechnete Arbeit und berechnete Zuordnung werden zu festen Einheiten.

## Der Dauertyp ändert sich beim Importieren aus MS Project in Workfront

Beim Importieren von Projekten aus Microsoft Project in Workfront werden feste Einheiten leistungsgesteuert. Feste Arbeit und Feste Dauer erhalten den Standarddauertyp, den Ihr Workfront-Administrator für Ihr System ausgewählt hat. Weitere Informationen finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
