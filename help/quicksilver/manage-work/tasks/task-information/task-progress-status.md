---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über den Task Progress Status
description: Adobe Workfront ermittelt den Fortschrittsstatus einer Aufgabe, indem es den Fortschritt der Aufgabe über ihre Zeitleiste hinweg betrachtet. Sie können Workfront so konfigurieren, dass die Bedingung eines Projekts basierend auf dem Wert des Fortschrittsstatus der Aufgaben bestimmt wird. Weitere Informationen zum Konfigurieren der Bedingung des Projekts finden Sie im Artikel Überblick über Projektbedingungen und Bedingungstyp.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Übersicht über den Task Progress Status

<!-- Audited: 1/2024 -->

Adobe Workfront ermittelt den Fortschrittsstatus einer Aufgabe, indem es den Fortschritt der Aufgabe über ihre Zeitleiste hinweg betrachtet. Sie können Workfront so konfigurieren, dass die Bedingung eines Projekts basierend auf dem Wert des Fortschrittsstatus der Aufgaben bestimmt wird. Weitere Informationen zum Konfigurieren der Bedingung des Projekts finden Sie im Artikel [Überblick über Projektbedingungen und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Kriterien, die den Fortschrittsstatus von Aufgaben bestimmen

Informationen zum Fortschrittsstatus eines Projekts finden Sie unter [Überblick über den Projektfortschritt](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Informationen zum Tracking des Fortschritts Ihrer Aufgaben finden Sie unter [Übersicht über den Task Tracking Mode](../../../manage-work/tasks/task-information/task-tracking-mode.md).

Die folgenden Kriterien bestimmen den Fortschrittsstatus einer Aufgabe:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Fortschrittsstatus</strong> </p> </th> 
   <th> <p><strong>Bestimmen von Kriterien</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>Einschaltzeit</strong> </p> </td> 
   <td scope="col"> <p>Eine Aufgabe wird als <strong>Einschaltzeit</strong> betrachtet, wenn alle geplanten Daten mit den geplanten Daten übereinstimmen. Dieser Fortschrittsstatus könnte auch bedeuten, dass das Projekt planmäßig überholt ist und die geplanten Daten vor den geplanten Daten liegen könnten.</p> <p>Weitere Informationen zu den prognostizierten Daten finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Überblick über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme</a>.</p> <p>Weitere Informationen zum geplanten Abschlussdatum der Aufgabe finden Sie in den folgenden Artikeln:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Überblick über die geplante Aufgabe, Startdatum</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Übersicht über das geplante Abschlussdatum der Aufgabe</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>Risiko</strong> </p> </td> 
   <td><p>Eine Aufgabe wird als <strong>Risiko</strong> betrachtet, wenn das geschätzte Abschlussdatum nach dem geplanten Abschlussdatum und nach dem geplanten Abschlussdatum liegt. Dies kann vorkommen, wenn eine Aufgabe die Beschränkung <strong>Must Finish On</strong> oder <strong>Must Start On</strong> hat, aber der Prozentsatz complete oder die Vorgängerbeziehungen der Aufgabe zeigen, dass sie nicht an den angegebenen Daten beendet oder gestartet werden kann. </p><p> Durch manuelles Festlegen der Aufgabenbegrenzung auf <strong>Must Finish on</strong> wird das geplante Abschlussdatum auf ein bestimmtes Datum gesetzt. Das vorgeschlagene Abschlussdatum stimmt in diesem Fall mit dem geplanten Abschlussdatum überein. Im Falle dieser Einschränkung analysiert Workfront die Aufgabe, um anhand des abgeschlossenen Prozentsatzes zu berechnen, wann sie abgeschlossen sein wird. Diese Berechnung wird als geschätztes Fälligkeitsdatum gespeichert. Wenn das geschätzte Fälligkeitsdatum nach dem geplanten Abschlussdatum liegt, besteht die Gefahr, dass die Aufgabe verspätet ist. </p> <p> Wenn Sie die Aufgabenbegrenzung auf <strong>Muss am</strong> manuell festlegen, wird das geplante Startdatum auf ein bestimmtes Datum gesetzt. Das vorgeschlagene Startdatum entspricht in diesem Fall dem geplanten Startdatum. Im Falle dieser Einschränkung analysiert Workfront die Aufgabe, um zu berechnen, wann sie basierend auf ihren Vorgängerbeziehungen starten wird. Diese Berechnung wird als geschätztes Startdatum gespeichert. Wenn es einen erzwungenen Vorgänger gibt, der nicht zulässt, dass die Aufgabe am angegebenen Startdatum beginnt, kann das geschätzte Startdatum nach dem geplanten Abschlussdatum liegen. Die Aufgabe wird als zu spät angesehen. </p> <p>Hinweis: In der Regel stimmen die geschätzten Datumswerte mit den prognostizierten Datumswerten überein, außer wenn <strong>am</strong> beginnen muss oder <strong>am</strong> beendet werden muss. In diesen Fällen werden die geschätzten Datumswerte weiterhin auf der Grundlage der prozentualen Vollständigkeit und anderer Faktoren (Vorgängerbeziehungen) berechnet, während die prognostizierten Datumswerte gezwungen sind, die manuell festgelegten geplanten Datumswerte abzugleichen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Hinter</strong> </p> </td> 
   <td> <p>Eine Aufgabe gilt als <strong>Hinter </strong>, wenn das geschätzte Abschlussdatum später oder gleich dem geplanten Abschlussdatum und früher als das prognostizierte Abschlussdatum liegt.</p> <p>Das geplante Abschlussdatum ist eine Echtzeitansicht des Zeitpunkts, zu dem die Aufgabe auf der Grundlage des vorherigen Fortschritts abgeschlossen wird. Obwohl die Aufgabe verspätet gestartet wurde, wird sie noch nicht als spät betrachtet, da die geplanten und geplanten Abschlussdaten noch in der Zukunft liegen und die Aufgabe möglicherweise noch rechtzeitig abgeschlossen werden kann.</p> <p>Hinweis: Die Fortschrittsstatus <strong>hinter</strong> und <strong>auf Risiko</strong> sind fast identisch. <strong>Risiko</strong> gibt jedoch an, dass einige erzwungene Aufgabenbegrenzungen (Muss abgeschlossen werden, Muss am, Feste Datumswerte beginnen) an einem oder beiden der geplanten Daten vorhanden sind. Wenn für die Aufgabe keine erzwungenen Beschränkungen bestehen, sind die prognostizierten Datumswerte mit den geschätzten Datumswerten identisch und spiegeln die Systemberechnung des Abschlussdatums basierend auf dem aktuellen Fortschritt der Aufgabe wider. Die Aufgabe wird noch nicht als spät angesehen, da die geplanten und geplanten Abschlussdaten noch in der Zukunft liegen und die Aufgabe möglicherweise noch rechtzeitig abgeschlossen werden kann.<br>Weitere Informationen zu den prognostizierten und geschätzten Datumswerten finden Sie unter <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Überblick über die prognostizierten und geschätzten Datumswerte </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Late</strong> </p> </td> 
   <td> <p>Eine Aufgabe ist <strong>überfällig</strong>, wenn das geplante Abschlussdatum vor dem heutigen Datum liegt.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![](assets/on-time-progress-status-350x233.png)

* At Risk

  ![](assets/at-risk-progress-status-350x233.png)

* Behind

  ![](assets/behind-progress-status-350x233.png)

* Late

  ![](assets/late-progress-status-350x233.png)

-->