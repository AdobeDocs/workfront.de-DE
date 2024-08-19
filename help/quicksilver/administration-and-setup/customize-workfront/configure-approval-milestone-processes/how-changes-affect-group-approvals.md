---
title: Auswirkungen der Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: In diesem Artikel wird erläutert, was passiert, wenn ein Genehmigungsprozess bereits verwendet wird, wenn ein Workfront-Administrator (oder ein Benutzer mit Administratorzugriff auf Genehmigungsprozesse) seine Zuordnung zu einer Gruppe ändert.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 77b2dce2-1523-4262-a659-0d301059a54c
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 1%

---

# Auswirkungen von Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse

In diesem Artikel wird erläutert, was passiert, wenn ein Genehmigungsprozess bereits mit Aufgaben, Problemen, Projekten, Vorlagen oder Vorlagenaufgaben verknüpft ist und ein Workfront-Administrator (oder ein Benutzer mit Administratorzugriff auf Genehmigungsprozesse) eine der folgenden Aktionen ausführt:

* Ändert den Validierungsprozess (Gruppenebene) von einer Gruppe in eine andere
* Ändert die dem Projekt zugeordnete Gruppe
* Ändert den Validierungsprozess von Gruppenebene zu Systemebene
* Ändert den Validierungsprozess von der Systemebene zur Gruppenebene

In diesem Artikel wird auch beschrieben, was beim Verschieben oder Kopieren von Aufgaben oder Problemen im Zusammenhang mit einem Genehmigungsprozess auf Gruppenebene zwischen zwei Projekten aus verschiedenen Gruppen geschieht.

Informationen zu den drei Arten von Genehmigungsprozessen, die Sie in Workfront verwenden können, finden Sie unter [Übersicht über den Genehmigungsprozess](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

>[!NOTE]
>
>Wenn das Projekt oder seine Aufgaben oder Probleme bereits mit einem Validierungsprozess auf Gruppenebene mithilfe benutzerdefinierter Status auf Gruppenebene verknüpft sind, kann das Ändern der Gruppe zu einem Konflikt zwischen den Genehmigungsstatus der vorherigen Gruppe und den auf Systemebene vorhandenen führen.
>
>Wenn beispielsweise ein Genehmigungsprozess zwei Pfade enthält, einen für den Status auf Systemebene und einen zweiten für den Status auf Gruppenebene, der dem gleichen Status auf Systemebene entspricht, führt das Ändern der Gruppe des Originalprojekts dazu, dass Workfront Schwierigkeiten hat, den gruppenspezifischen Status zu verstehen, der möglicherweise nicht in der zweiten Gruppe vorhanden ist. In diesem Fall tritt ein Fehler auf.
>
>Erwägen Sie, die Genehmigungsprozesse auf Gruppenebene für das Projekt oder dessen Aufgaben oder Probleme zu entfernen, bevor Sie die Projektgruppe aktualisieren.
>
>Informationen zum Erstellen von Genehmigungsprozessen auf Gruppenebene finden Sie unter [Genehmigungsprozesse auf Gruppenebene](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).
>
>Informationen zum Erstellen eines benutzerdefinierten Status auf Gruppenebene finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)

## Gruppenspezifische Validierungsprozesse von einer Gruppe zu einer anderen ändern

Die folgenden Szenarien treten auf, wenn bereits ein gruppenspezifischer Validierungsprozess für ein Objekt verwendet wird und es einer anderen Gruppe zugewiesen wird:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich oder Objekt, an das der Genehmigungsprozess angehängt wurde</th> 
   <th>Genehmigungs-Objekt</th> 
   <th>Änderung des Genehmigungsprozesses für das Objekt oder Gebiet</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt- oder Vorlagenvalidierung </td> 
   <td>Projekt</td> 
   <td>wird zu einem Genehmigungsprozess für den einmaligen Gebrauch</td> 
  </tr> 
  <tr> 
   <td>Aufgabenvalidierung oder Vorlagenvalidierung </td> 
   <td>Aufgabe</td> 
   <td>wird zu einem Genehmigungsprozess für den einmaligen Gebrauch </td> 
  </tr> 
  <tr> 
   <td>Genehmigung ausstellen</td> 
   <td>Problem</td> 
   <td>wird zu einem Genehmigungsprozess für den einmaligen Gebrauch</td> 
  </tr> 
  <tr> 
   <td>Aufgabenbereich im Feld "Projekt bearbeiten"oder "Vorlage bearbeiten"</td> 
   <td>Aufgabe</td> 
   <td> <p>Das Feld "Task Default Approval Process"wird auf N/A zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Aufgaben im Projekt verknüpft.</p> </td> 
  </tr> 
  <tr> 
   <td>Bereich "Queue Details"eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Das Feld Standardgenehmigung wird auf K/A zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anforderungen im Projekt verknüpft.</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Topic section of a project or template</td> 
   <td>Problem</td> 
   <td> <p>Das Feld Standardgenehmigung wird auf K/A zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anforderungen im Projekt verknüpft.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändern der mit einem Projekt verknüpften Gruppe

Wenn jemand die mit einem Projekt verknüpfte Gruppe in eine andere Gruppe ändert, geschieht Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich oder Objekt, an das bereits der Genehmigungsprozess angehängt ist</th> 
   <th>Genehmigungs-Objekt</th> 
   <th>Änderung des Validierungsprozesses des Objekts oder Gebiets</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt- oder Vorlagenvalidierung </td> 
   <td>Projekt</td> 
   <td>Wird zu einem Genehmigungsprozess für die einmalige Verwendung und der zugehörige Status wird aktualisiert und entspricht nun einem ähnlichen Status für die neue Gruppe.</td> 
  </tr> 
  <tr> 
   <td>Aufgabenvalidierung oder Vorlagenvalidierung </td> 
   <td>Aufgabe</td> 
   <td>Wird zu einem Genehmigungsprozess für die einmalige Verwendung und der zugehörige Status wird aktualisiert und entspricht nun einem ähnlichen Status für die neue Gruppe.</td> 
  </tr> 
  <tr> 
   <td>Genehmigung ausstellen</td> 
   <td>Problem</td> 
   <td>Wird zu einem Genehmigungsprozess für die einmalige Verwendung und der zugehörige Status wird aktualisiert und entspricht nun einem ähnlichen Status für die neue Gruppe.</td> 
  </tr> 
  <tr> 
   <td>Aufgabenbereich im Feld "Projekt bearbeiten"oder "Vorlage bearbeiten"</td> 
   <td>Aufgabe</td> 
   <td> <p>Das Feld "Task Default Approval Process"wird auf "N/A"zurückgesetzt</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Aufgaben im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Bereich "Queue Details"eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Das Feld Standardgenehmigungsprozess wird auf N/A zurückgesetzt</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anforderungen im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Topic section of a project or template</td> 
   <td>Problem</td> 
   <td> <p>Das Feld Standardgenehmigungsprozess wird auf N/A zurückgesetzt</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anforderungen im Projekt verknüpft</p> </td> 
  </tr> 
 </tbody> 
</table>

## Validierungsprozess von Gruppenebene zu Systemebene ändern

Wenn jemand die Gruppenoption in einem gruppenspezifischen Validierungsprozess in &quot;Alle Gruppen&quot;ändert, wird der Validierungsprozess systemweit durchgeführt und Folgendes geschieht:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich oder Objekt, an das der Genehmigungsprozess angehängt wurde</th> 
   <th>Genehmigungs-Objekt</th> 
   <th>Änderung des Validierungsprozesses des Objekts oder Gebiets</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt- oder Vorlagenvalidierung </td> 
   <td>Projekt</td> 
   <td>Keine Änderung</td> 
  </tr> 
  <tr> 
   <td>Aufgabenvalidierung oder Vorlagenvalidierung </td> 
   <td>Aufgabe</td> 
   <td>Keine Änderung</td> 
  </tr> 
  <tr> 
   <td>Genehmigung ausstellen</td> 
   <td>Problem</td> 
   <td>Keine Änderung</td> 
  </tr> 
  <tr> 
   <td>Aufgabenbereich im Feld "Projekt bearbeiten"oder "Vorlage bearbeiten"</td> 
   <td>Aufgabe</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, sondern standardmäßig mit neuen Aufgaben im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Bereich "Queue Details"eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, sondern standardmäßig mit neuen Problemen oder Anforderungen am Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Queue Topic section of a project or template</td> 
   <td>Problem</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, sondern standardmäßig mit neuen Problemen oder Anforderungen am Projekt verknüpft</p> </td> 
  </tr> 
 </tbody> 
</table>

## Validierungsprozess von der Systemebene zur Gruppenebene ändern

Wenn jemand die Verfügbarkeit eines systemweiten Validierungsprozesses von &quot;Alle Gruppen&quot;in eine bestimmte Gruppe ändert, wird der Validierungsprozess gruppenspezifisch und Folgendes geschieht:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich oder Objekt, an das der Genehmigungsprozess angehängt wurde</th> 
   <th>Genehmigungs-Objekt</th> 
   <th>Änderung des Validierungsprozesses des Objekts oder Gebiets</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt-, Aufgaben-, Problem-, Vorlagen- oder Vorlagenaufgabe, die zur Gruppe des Validierungsprozesses gehört</td> 
   <td> <p>Projekt, Aufgabe oder Problem</p> </td> 
   <td>Keine Änderung</td> 
  </tr> 
  <tr> 
   <td>Aufgabenbereich im Feld "Projekt bearbeiten"oder "Vorlage bearbeiten"für ein Projekt oder eine Vorlage, das/die zur Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Aufgabe</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, sondern standardmäßig mit neuen Aufgaben im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Bereich "Queue Details"für ein Projekt oder eine Vorlage, das/die zur Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Problem</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, sondern standardmäßig mit neuen Problemen oder Anforderungen am Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Bereich "Warteschlangenthema"für ein Projekt oder eine Vorlage, das/die zur Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Problem</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, sondern standardmäßig mit neuen Problemen oder Anforderungen am Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Projekt-, Aufgaben-, Problem-, Vorlagen- oder Vorlagenaufgabe, die zu einer anderen Gruppe als der Gruppe des Validierungsprozesses gehört</td> 
   <td> <p>Projekte</p> <p>Aufgaben</p> <p>Probleme</p> </td> 
   <td>wird zu einem Genehmigungsprozess für den einmaligen Gebrauch</td> 
  </tr> 
  <tr> 
   <td>Aufgabenbereich im Feld "Projekt bearbeiten"oder "Vorlage bearbeiten"für ein Projekt oder eine Vorlage, das/die zu einer anderen Gruppe als der Gruppe des Validierungsprozesses gehört</td> 
   <td>Aufgaben</td> 
   <td> <p>Das Feld "Task Default Approval Process"wird auf N/A zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Aufgaben im Projekt verknüpft.</p> </td> 
  </tr> 
  <tr> 
   <td>Bereich "Queue Details"für ein Projekt oder eine Vorlage, das/die zu einer anderen Gruppe als der Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Probleme</td> 
   <td> <p>Das Feld Standardgenehmigung wird auf K/A zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anforderungen im Projekt verknüpft.</p> </td> 
  </tr> 
  <tr> 
   <td>Bereich "Warteschlangenthema"für ein Projekt oder eine Vorlage, das/die zu einer anderen Gruppe als der Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Probleme</td> 
   <td> <p>Das Feld Standardgenehmigung wird auf K/A zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anforderungen im Projekt verknüpft.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verschieben oder Kopieren einer Aufgabe oder eines Problems in ein Projekt mit einer anderen Gruppe als der des Genehmigungsprozesses

Das Verschieben oder Kopieren einer Aufgabe oder eines Problems von einem Projekt in ein anderes kann sich je nach den Gruppen der beiden Projekte auf bestehende Genehmigungsprozesse für die Aufgabe oder das Problem auswirken. Die folgende Tabelle zeigt die möglicherweise vorhandenen Szenarien:

| Vorgang zur ursprünglichen Aufgabe oder zur Genehmigung eines Problems | Gruppen der beiden Projekte | Änderungen im Genehmigungsprozess, nachdem die Aufgabe oder das Problem in ein anderes Projekt verschoben wurde |
|---|---|---|
| Genehmigungsprozess für den einmaligen Gebrauch, der mit einem systemweiten Status verknüpft ist | Projekte befinden sich in derselben oder unterschiedlichen Gruppen | Keine Änderung |
| Validierungsprozess für die einmalige Verwendung, der mit einem gruppenspezifischen Status verknüpft ist | Projekte befinden sich in verschiedenen Gruppen | Die Genehmigung bleibt ein Genehmigungsprozess für die einmalige Verwendung, und der mit der Genehmigung verknüpfte Status wird entsprechend dem Status für die neue Gruppe aktualisiert. |
| Systemweiter Genehmigungsprozess | Projekte befinden sich in derselben oder unterschiedlichen Gruppen | Keine Änderung |
| Gruppenspezifischer Validierungsprozess | Projekte befinden sich in derselben Gruppe | Keine Änderung |
| Gruppenspezifischer Validierungsprozess | Projekte befinden sich in verschiedenen Gruppen und die Gruppen haben unterschiedliche gruppenspezifische Status | Die Genehmigung wird zu einem Validierungsprozess für die einmalige Verwendung, und der mit der Genehmigung verknüpfte Status wird entsprechend dem Status für die neue Gruppe aktualisiert. |
| Gruppenspezifischer Validierungsprozess | Projekte befinden sich in verschiedenen Gruppen und es gibt einen Status mit demselben Schlüssel in der neuen Gruppe wie der Status, der dem Genehmigungsprozess der ersten Gruppe zugeordnet ist | Keine Änderung |
