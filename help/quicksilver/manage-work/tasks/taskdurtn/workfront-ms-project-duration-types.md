---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Dauertypen in Adobe Workfront und Microsoft Project
description: Die in Adobe Workfront verfügbaren Dauertypen unterscheiden sich von ihren Gegenstücken im Microsoft-Projekt, die als Aufgabentypen bezeichnet werden. Dies kann beim Exportieren oder Importieren von Projekten zwischen Workfront und Microsoft Project manchmal verwirrend sein.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 11%

---

# Dauertypen in Adobe Workfront und Microsoft Project

Die in Adobe Workfront verfügbaren Dauertypen unterscheiden sich von ihren Gegenstücken im Microsoft-Projekt, die als Aufgabentypen bezeichnet werden. Dies kann beim Exportieren oder Importieren von Projekten zwischen Workfront und Microsoft Project manchmal verwirrend sein.

Informationen zum Importieren und Exportieren von Projekten zwischen Workfront und Microsoft Project finden Sie in den folgenden Artikeln:

* [Exportieren eines Projekts in das Microsoft-Projekt](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importieren eines Projekts aus Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

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
 
(drafting this because it is misleading)
 
</note>
-->
