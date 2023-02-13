---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über den Projektstatus
description: Adobe Workfront ermittelt den Fortschrittsstatus eines Projekts, indem es den Fortschritt des Projekts über seine Zeitleiste hinweg betrachtet. Sie können Workfront so konfigurieren, dass die Bedingung eines Projekts basierend auf dem Wert des Fortschrittsstatus der Aufgaben bestimmt wird. Weitere Informationen zum Konfigurieren der Bedingung des Projekts finden Sie im Artikel Überblick über Projektbedingungen und Bedingungstyp.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# Übersicht über den Projektstatus

Adobe Workfront ermittelt den Fortschrittsstatus eines Projekts, indem es den Fortschritt des Projekts über seine Zeitleiste hinweg betrachtet. Sie können Workfront so konfigurieren, dass die Bedingung eines Projekts basierend auf dem Wert des Fortschrittsstatus der Aufgaben bestimmt wird. Weitere Informationen zum Konfigurieren der Projektbedingung finden Sie im Artikel [Übersicht über Projektbedingung und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Im Folgenden werden die Fortschrittsstatus von Projekten in Workfront beschrieben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Einschaltzeit</td> 
   <td> <p>Wenn sowohl das prognostizierte als auch das geschätzte Abschlussdatum vor dem geplanten Abschlussdatum des Projekts liegen, lautet der Fortschrittsstatus des Projekts <strong>Einschaltzeit</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Gefährdet</td> 
   <td> <p>Wenn sowohl das geschätzte als auch das prognostizierte Abschlussdatum in der Zukunft liegen, aber später als das geplante Abschlussdatum des Projekts und das geschätzte Abschlussdatum nach dem geplanten Abschlussdatum liegt, lautet der Projektfortschrittsstatus <strong>Risiko</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>In Verzug</td> 
   <td> <p>Wenn sowohl das geschätzte als auch das prognostizierte Abschlussdatum in der Zukunft liegen, aber später als das geplante Abschlussdatum des Projekts, das geschätzte Abschlussdatum jedoch nicht später als das geplante Abschlussdatum ist, lautet der Projektfortschrittsstatus <strong>Hinter</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>In Verzug</td> 
   <td> 
    <ul> 
     <li> <p>Wenn das Projekt abgeschlossen ist und das tatsächliche Abschlussdatum nach dem geplanten Abschlussdatum liegt, lautet der Fortschrittsstatus des Projekts: <strong>Verspätet</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Wenn das Projekt nicht abgeschlossen ist und das geplante Abschlussdatum des Projekts in der Vergangenheit liegt, lautet der Projektfortschrittsstatus . <strong>Verspätet</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Beachten Sie Folgendes:

* Das geplante Abschlussdatum des Projekts wird von der Aufgabe auf dem kritischen Pfad mit dem neuesten geplanten Abschlussdatum bestimmt.
* Das geschätzte Abschlussdatum des Projekts wird von der Aufgabe auf dem kritischen Pfad mit dem neuesten geschätzten Abschlussdatum bestimmt.

Weitere Informationen zum kritischen Pfad des Projekts finden Sie unter [Überblick über das Projekt - Kritischer Pfad](../../../manage-work/tasks/manage-tasks/critical-path.md).

Weitere Informationen zu den prognostizierten Abschlussdaten finden Sie unter [Übersicht über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
