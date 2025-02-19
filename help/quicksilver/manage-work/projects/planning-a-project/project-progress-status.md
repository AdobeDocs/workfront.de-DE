---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über den Projektfortschritt
description: Adobe Workfront ermittelt den Fortschrittsstatus eines Projekts anhand des Fortschritts des Projekts in der gesamten Zeitleiste. Sie können Workfront so konfigurieren, dass die Bedingung eines Projekts auf der Grundlage des Fortschrittsstatus der Aufgaben bestimmt wird. Weitere Informationen zum Projektfortschritt finden Sie in diesem Artikel .
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: d85ccb9dbef343ecc8808412e89264b3ea6ab25e
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 1%

---

# Übersicht über den Projektfortschritt

<!--Audited: 12/2023-->

Adobe Workfront ermittelt den Fortschrittsstatus eines Projekts anhand des Fortschritts des Projekts in der gesamten Zeitleiste. Sie können Workfront so konfigurieren, dass die Bedingung eines Projekts auf der Grundlage des Fortschrittsstatus der Aufgaben bestimmt wird. Weitere Informationen zum Konfigurieren der Bedingung des Projekts finden Sie im Artikel [Übersicht über Projektbedingung und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Im Folgenden finden Sie den Fortschrittsstatus von Projekten in Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Im Zeitplan</td> 
   <td> Der Fortschrittsstatus eines Projekts ist "<strong>", </strong>:<ul><li>Wenn sowohl das geplante als auch das geschätzte Abschlussdatum vor dem geplanten Abschlussdatum des Projekts liegen oder damit übereinstimmen</li></ul> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Gefährdet</td> 
   <td> Der Fortschrittsstatus eines Projekts ist <strong>Gefährdet</strong> wenn <strong>alle</strong> der folgenden Bedingungen zutreffen:<ul><li>Sowohl die geschätzten als auch die erwarteten Abschlussdaten liegen in der Zukunft</li><li> Das geschätzte Abschlussdatum liegt sowohl nach dem geplanten Abschlussdatum als auch nach dem voraussichtlichen Abschlussdatum </li></ul><p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>In Verzug</td> 
   <td> Der Fortschrittsstatus eines Projekts ist "<strong>"</strong> wenn <strong>alle</strong> der folgenden Bedingungen zutreffen:<ul><li>Sowohl die geschätzten als auch die erwarteten Abschlussdaten liegen in der Zukunft</li><li> Sowohl das geschätzte als auch das voraussichtliche Abschlussdatum liegen hinter dem geplanten Abschlussdatum des Projekts</li><li> Das voraussichtliche Abschlussdatum liegt nicht nach dem voraussichtlichen Abschlussdatum</li></ul> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Verspätet</td> 
   <td> 
     Der Fortschrittsstatus eines Projekts ist <strong>Verspätet</strong> wenn <strong> der folgenden </strong> zutrifft:<ul><li>Das Projekt ist abgeschlossen und das tatsächliche Abschlussdatum liegt hinter dem geplanten Abschlussdatum <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Das Projekt ist noch nicht abgeschlossen und das geplante Abschlussdatum liegt in der Vergangenheit <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie Folgendes:

* Das voraussichtliche Abschlussdatum des Projekts wird von der Aufgabe auf dem kritischen Pfad mit dem neuesten voraussichtlichen Abschlussdatum bestimmt.
* Das geschätzte Abschlussdatum des Projekts wird von der Aufgabe auf dem kritischen Pfad mit dem neuesten geschätzten Abschlussdatum gesteuert.

Informationen zum projektkritischen Pfad finden Sie unter [Übersicht über den projektkritischen Pfad](../../../manage-work/tasks/manage-tasks/critical-path.md).

Informationen zu voraussichtlichen Abschlussdaten finden Sie unter [Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
