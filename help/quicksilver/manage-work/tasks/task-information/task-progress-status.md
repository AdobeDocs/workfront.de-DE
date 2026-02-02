---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über den Aufgabenstatus
description: Adobe Workfront ermittelt den Fortschrittsstatus einer Aufgabe, indem es den Fortschritt der Aufgabe über die gesamte Zeitleiste hinweg betrachtet. Sie können Workfront so konfigurieren, dass die Bedingung eines Projekts auf der Grundlage des Fortschrittsstatus der Aufgaben bestimmt wird. Weitere Informationen zum Konfigurieren der Bedingung des Projekts finden Sie im Artikel Übersicht über Projektbedingung und Bedingungstyp .
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Übersicht über den Aufgabenstatus

<!-- Audited: 1/2024 -->

Adobe Workfront ermittelt den Fortschrittsstatus einer Aufgabe, indem es den Fortschritt der Aufgabe über die gesamte Zeitleiste hinweg betrachtet. Sie können Workfront so konfigurieren, dass die Bedingung eines Projekts auf der Grundlage des Fortschrittsstatus der Aufgaben bestimmt wird. Weitere Informationen zum Konfigurieren der Bedingung des Projekts finden Sie im Artikel [Übersicht über Projektbedingung und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Kriterien, die den Fortschrittsstatus von Aufgaben bestimmen

Informationen zum Fortschrittsstatus eines Projekts finden Sie unter [Übersicht über den Projektfortschritt](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Informationen zum Nachverfolgen des Fortschritts Ihrer Aufgaben finden Sie unter [Übersicht über den Aufgabenverfolgungsmodus](../../../manage-work/tasks/task-information/task-tracking-mode.md).

Die folgenden Kriterien bestimmen den Fortschrittsstatus einer Aufgabe:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Fortschrittsstatus</strong> </p> </th> 
   <th> <p><strong>Bestimmungskriterien</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>Einschaltzeit</strong> </p> </td> 
   <td scope="col"> <p>Eine Aufgabe gilt als <strong>Einschaltzeit</strong> wenn alle geplanten Termine mit den geplanten Terminen übereinstimmen. Dieser Fortschrittsstatus kann auch bedeuten, dass das Projekt dem Zeitplan voraus ist und die voraussichtlichen Termine vor den geplanten Terminen liegen.</p> <p>Weitere Informationen zu voraussichtlichen Terminen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme</a>.</p> <p>Weitere Informationen zum geplanten Abschlussdatum der Aufgabe finden Sie in den folgenden Artikeln:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Übersicht über das geplante Startdatum der Aufgabe</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Übersicht über das geplante Abschlussdatum der Aufgabe</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>Gefährdet</strong> </p> </td> 
   <td><p>Eine Aufgabe gilt als <strong>gefährdet</strong> wenn das geschätzte Abschlussdatum nach dem geplanten Abschlussdatum und nach dem erwarteten Abschlussdatum liegt. Dies kann vorkommen, wenn eine Aufgabe die Beschränkung <strong>Muss beendet sein am</strong> oder <strong>Muss beginnen am</strong> aufweist, aber der abgeschlossene Prozentwert oder die Vorgängerbeziehungen der Aufgabe zeigen, dass sie nicht zu den angegebenen Daten enden oder beginnen kann. </p><p> Wenn Sie die Aufgabenbeschränkung auf <strong>Muss abgeschlossen sein am</strong> setzen, wird das geplante Abschlussdatum manuell auf ein bestimmtes Datum festgelegt. Das voraussichtliche Abschlussdatum stimmt in diesem Fall mit dem geplanten Abschlussdatum überein. Im Falle dieser Einschränkung analysiert Workfront die Aufgabe und berechnet anhand des abgeschlossenen Prozentsatzes, wann sie abgeschlossen sein wird. Diese Berechnung wird als geschätztes Fälligkeitsdatum gespeichert. Wenn das voraussichtliche Fälligkeitsdatum nach dem voraussichtlichen Abschlussdatum liegt, besteht die Gefahr, dass die Aufgabe in Verzug gerät. </p> <p> Wenn Sie die Aufgabenbeschränkung auf <strong>Muss beginnen am</strong> setzen, wird das geplante Startdatum manuell auf ein bestimmtes Datum festgelegt. Das voraussichtliche Startdatum entspricht in diesem Fall dem geplanten Startdatum. Im Falle dieser Einschränkung analysiert Workfront die Aufgabe, um zu berechnen, wann sie auf der Grundlage der Vorgängerbeziehungen beginnen wird. Diese Berechnung wird als geschätztes Startdatum gespeichert. Wenn es einen erzwungenen Vorgänger gibt, der nicht zulässt, dass die Aufgabe am angegebenen Startdatum beginnt, kann das geschätzte Startdatum nach dem voraussichtlichen Abschlussdatum liegen. Es besteht die Gefahr, dass diese Aufgabe in Verzug gerät. </p> <p>Hinweis: In der Regel entsprechen die geschätzten Daten den voraussichtlichen Terminen, außer wenn <strong>Start erforderlich am</strong> oder <strong>Ende erforderlich am</strong> verwendet werden. In diesen Fällen werden die geschätzten Termine weiterhin auf der Grundlage des Prozentsatzes der Fertigstellung und anderer Faktoren (Vorgängerbeziehungen) berechnet, während die erwarteten Termine gezwungen sind, mit den geplanten Terminen übereinzustimmen, die manuell festgelegt wurden.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>hinter</strong> </p> </td> 
   <td> <p>Eine Aufgabe gilt als "<strong>", </strong> das voraussichtliche Abschlussdatum nach oder vor dem geplanten Abschlussdatum liegt.</p> <p>Das voraussichtliche Abschlussdatum ist eine Echtzeitansicht des Zeitpunkts, zu dem die Aufgabe je nach vorherigem Fortschritt abgeschlossen wird. Obwohl die Aufgabe verspätet gestartet wurde, wird dies noch nicht als verspätet betrachtet, da die geplanten und geplanten Abschlussdaten noch in der Zukunft liegen und die Aufgabe möglicherweise noch rechtzeitig abgeschlossen wird.</p> <p>Hinweis: Der <strong>Behind</strong>- und <strong>at</strong>-Fortschrittsstatus sind nahezu identisch. "<strong> Risiko“ </strong> jedoch an, dass es einige erzwungene Aufgabeneinschränkungen (Muss beendet sein am, Muss beginnen am, Feste Termine) für eines oder beide der geplanten Termine gibt. Wenn keine erzwungenen Einschränkungen für die Aufgabe vorhanden sind, sind die voraussichtlichen Termine mit den voraussichtlichen Terminen identisch und spiegeln die Systemberechnung des Abschlussdatums auf der Grundlage des aktuellen Fortschritts der Aufgabe wider. Die Aufgabe wird noch nicht als zu spät erachtet, da die geplanten und geplanten Abschlussdaten noch in der Zukunft liegen und die Aufgabe möglicherweise noch rechtzeitig abgeschlossen wird.<br>Weitere Informationen über das voraussichtliche und das voraussichtliche Datum finden Sie unter <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Übersicht über das voraussichtliche und das voraussichtliche Datum </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>spät</strong> </p> </td> 
   <td> <p>Eine Aufgabe ist <strong>spät</strong> wenn das geplante Abschlussdatum vor dem heutigen Datum liegt.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![On time progress status](assets/on-time-progress-status-350x233.png)

* At Risk

  ![At risk progress status](assets/at-risk-progress-status-350x233.png)

* Behind

  ![Behind progress status](assets/behind-progress-status-350x233.png)

* Late

  ![Late progress status](assets/late-progress-status-350x233.png)

-->
