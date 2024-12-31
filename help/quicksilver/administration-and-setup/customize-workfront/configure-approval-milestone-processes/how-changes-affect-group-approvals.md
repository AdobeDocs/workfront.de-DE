---
title: Auswirkungen von Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: In diesem Artikel wird erläutert, was passiert, wenn ein Genehmigungsprozess bereits verwendet wird, wenn ein Workfront-Administrator (oder ein Benutzer mit administrativem Zugriff auf Genehmigungsprozesse) seine Zuordnung zu einer Gruppe ändert.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 77b2dce2-1523-4262-a659-0d301059a54c
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 1%

---

# Auswirkungen von Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse

In diesem Artikel wird erläutert, was passiert, wenn ein Genehmigungsprozess bereits mit Aufgaben, Problemen, Projekten, Vorlagen oder Vorlagenaufgaben verknüpft ist und ein Workfront-Administrator (oder ein Benutzer mit administrativem Zugriff auf Genehmigungsprozesse) eine der folgenden Aktionen ausführt:

* Ändert den Genehmigungsprozess (auf Gruppenebene) von einer Gruppe in eine andere
* Ändert die dem Projekt zugeordnete Gruppe.
* Ändert den Genehmigungsprozess von der Gruppenebene zur Systemebene
* Ändert den Genehmigungsprozess von der Systemebene zur Gruppenebene

In diesem Artikel wird auch beschrieben, was passiert, wenn Aufgaben oder Probleme, die mit einem Genehmigungsprozess auf Gruppenebene zwischen zwei Projekten aus verschiedenen Gruppen verbunden sind, verschoben oder kopiert werden.

Informationen zu den drei Genehmigungsprozesstypen, die Sie in Workfront verwenden können, finden Sie unter [Übersicht über Genehmigungsprozesse](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

>[!NOTE]
>
>Wenn das Projekt bzw. seine Aufgaben oder Probleme bereits mit einem Genehmigungsprozess auf Gruppenebene unter Verwendung benutzerdefinierter Status auf Gruppenebene verknüpft sind, kann eine Änderung der Gruppe zu einem Konflikt zwischen den Genehmigungsstatus der vorherigen Gruppe und den auf Systemebene vorhandenen Status führen.
>
>Wenn beispielsweise ein Genehmigungsprozess zwei Pfade enthält, einen für einen Status auf Systemebene und einen zweiten für einen Status auf Gruppenebene, der demselben Status auf Systemebene entspricht, führt das Ändern der Gruppe des ursprünglichen Projekts dazu, dass Workfront Schwierigkeiten hat, den gruppenspezifischen Status zu verstehen, der möglicherweise nicht in der zweiten Gruppe vorhanden ist. In diesem Fall tritt ein Fehler auf.
>
>Erwägen Sie, die Genehmigungsprozesse auf Gruppenebene für das Projekt oder seine Aufgaben oder Probleme zu entfernen, bevor Sie die Gruppe des Projekts aktualisieren.
>
>Informationen zum Erstellen von Genehmigungsprozessen auf Gruppenebene finden Sie unter [Genehmigungsprozesse auf Gruppenebene](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).
>
>Informationen zum Erstellen eines benutzerdefinierten Status auf Gruppenebene finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)

## Gruppenspezifischer Genehmigungsprozess von einer Gruppe in eine andere ändern

Die folgenden Szenarien treten auf, wenn bereits ein gruppenspezifischer Genehmigungsprozess für ein Objekt verwendet wird und dieser von jemandem einer anderen Gruppe zugewiesen wird:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich oder Objekt, an den der Genehmigungsprozess angehängt wurde</th> 
   <th>Validierungsobjekt</th> 
   <th>Änderung des Genehmigungsprozesses für das Objekt oder den Bereich</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt- oder Vorlagenvalidierung </td> 
   <td>Projekt</td> 
   <td>Wird zu einem Genehmigungsprozess für den einmaligen Gebrauch</td> 
  </tr> 
  <tr> 
   <td>Aufgabenvalidierung oder Vorlagenaufgabe </td> 
   <td>Aufgabe</td> 
   <td>Wird zu einem Genehmigungsprozess für den einmaligen Gebrauch </td> 
  </tr> 
  <tr> 
   <td>Anfragegenehmigung</td> 
   <td>Problem</td> 
   <td>Wird zu einem Genehmigungsprozess für den einmaligen Gebrauch</td> 
  </tr> 
  <tr> 
   <td>Aufgaben im Bereich Projekt bearbeiten oder Vorlage bearbeiten</td> 
   <td>Aufgabe</td> 
   <td> <p>Das Feld Standardmäßiger Genehmigungsprozess der Aufgabe wird auf Nicht zutreffend zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Aufgaben im Projekt verknüpft.</p> </td> 
  </tr> 
  <tr> 
   <td>Abschnitt „Warteschlangendetails“ eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Das Feld Standardgenehmigung wird auf Nicht zutreffend zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anfragen im Projekt verknüpft.</p> </td> 
  </tr> 
  <tr> 
   <td>Warteschlangenthema-Abschnitt eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Das Feld Standardgenehmigung wird auf Nicht zutreffend zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anfragen im Projekt verknüpft.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändern der mit einem Projekt verknüpften Gruppe

Wenn jemand die einem Projekt zugeordnete Gruppe in eine andere Gruppe ändert, geschieht Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich oder Objekt, an den der Genehmigungsprozess bereits angehängt ist</th> 
   <th>Validierungsobjekt</th> 
   <th>Änderung des Genehmigungsprozesses für das Objekt oder den Bereich</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt- oder Vorlagenvalidierung </td> 
   <td>Projekt</td> 
   <td>Wird zu einem einmaligen Genehmigungsprozess und der damit verknüpfte Status wird aktualisiert, damit er einem ähnlichen Status für die neue Gruppe entspricht.</td> 
  </tr> 
  <tr> 
   <td>Aufgabenvalidierung oder Vorlagenaufgabe </td> 
   <td>Aufgabe</td> 
   <td>Wird zu einem einmaligen Genehmigungsprozess und der damit verknüpfte Status wird aktualisiert, damit er einem ähnlichen Status für die neue Gruppe entspricht.</td> 
  </tr> 
  <tr> 
   <td>Anfragegenehmigung</td> 
   <td>Problem</td> 
   <td>Wird zu einem einmaligen Genehmigungsprozess und der damit verknüpfte Status wird aktualisiert, damit er einem ähnlichen Status für die neue Gruppe entspricht.</td> 
  </tr> 
  <tr> 
   <td>Aufgaben im Bereich Projekt bearbeiten oder Vorlage bearbeiten</td> 
   <td>Aufgabe</td> 
   <td> <p>Das Feld „Standardmäßiger Genehmigungsprozess für Aufgabe“ wird auf „Nicht zutreffend“ zurückgesetzt</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Aufgaben im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Abschnitt „Warteschlangendetails“ eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Das Feld Standardgenehmigungsprozess wird auf Nicht zutreffend zurückgesetzt</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anfragen im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Warteschlangenthema-Abschnitt eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Das Feld Standardgenehmigungsprozess wird auf Nicht zutreffend zurückgesetzt</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anfragen im Projekt verknüpft</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändern eines Genehmigungsprozesses von der Gruppenebene in die Systemebene

Wenn jemand in einem gruppenspezifischen Genehmigungsprozess die Gruppenoption in „Alle Gruppen“ ändert, wird der Genehmigungsprozess systemweit und es passiert Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich oder Objekt, an den der Genehmigungsprozess angehängt wurde</th> 
   <th>Validierungsobjekt</th> 
   <th>Änderung des Genehmigungsprozesses für das Objekt oder den Bereich</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt- oder Vorlagenvalidierung </td> 
   <td>Projekt</td> 
   <td>Keine Änderung</td> 
  </tr> 
  <tr> 
   <td>Aufgabenvalidierung oder Vorlagenaufgabe </td> 
   <td>Aufgabe</td> 
   <td>Keine Änderung</td> 
  </tr> 
  <tr> 
   <td>Anfragegenehmigung</td> 
   <td>Problem</td> 
   <td>Keine Änderung</td> 
  </tr> 
  <tr> 
   <td>Aufgaben im Bereich Projekt bearbeiten oder Vorlage bearbeiten</td> 
   <td>Aufgabe</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, aber standardmäßig ist er mit neuen Aufgaben im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Abschnitt „Warteschlangendetails“ eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, aber standardmäßig ist er mit neuen Problemen oder Anfragen im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Warteschlangenthema-Abschnitt eines Projekts oder einer Vorlage</td> 
   <td>Problem</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, aber standardmäßig ist er mit neuen Problemen oder Anfragen im Projekt verknüpft</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändern eines Genehmigungsprozesses von der Systemebene zur Gruppenebene

Wenn jemand die Verfügbarkeit eines systemweiten Genehmigungsprozesses von „Alle Gruppen“ in eine bestimmte Gruppe ändert, wird der Genehmigungsprozess gruppenspezifisch und es geschieht Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich oder Objekt, an den der Genehmigungsprozess angehängt wurde</th> 
   <th>Validierungsobjekt</th> 
   <th>Änderung des Genehmigungsprozesses für das Objekt oder den Bereich</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt, Aufgabe, Problem, Vorlage oder Vorlagenaufgabe, das/die zur Gruppe des Genehmigungsprozesses gehört</td> 
   <td> <p>Projekt, Aufgabe oder Problem</p> </td> 
   <td>Keine Änderung</td> 
  </tr> 
  <tr> 
   <td>Aufgaben im Bereich Projekt bearbeiten oder Vorlage bearbeiten für ein Projekt oder eine Vorlage, das/die zur Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Aufgabe</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, aber standardmäßig ist er mit neuen Aufgaben im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Abschnitt „Warteschlangendetails“ für ein Projekt oder eine Vorlage, das/die zur Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Problem</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, aber standardmäßig ist er mit neuen Problemen oder Anfragen im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Warteschlangenthema-Abschnitt für ein Projekt oder eine Vorlage, das/die zur Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Problem</td> 
   <td> <p>Keine Änderung am Genehmigungsprozess, aber standardmäßig ist er mit neuen Problemen oder Anfragen im Projekt verknüpft</p> </td> 
  </tr> 
  <tr> 
   <td>Projekt, Aufgabe, Problem, Vorlage oder Vorlagenaufgabe, das zu einer anderen Gruppe als der Gruppe des Genehmigungsprozesses gehört</td> 
   <td> <p>Projekte</p> <p>Aufgaben</p> <p>Probleme</p> </td> 
   <td>Wird zu einem Genehmigungsprozess für den einmaligen Gebrauch</td> 
  </tr> 
  <tr> 
   <td>Aufgaben im Bereich Projekt bearbeiten oder Vorlage bearbeiten für ein Projekt oder eine Vorlage, das/die zu einer anderen Gruppe als der Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Aufgaben</td> 
   <td> <p>Das Feld Standardmäßiger Genehmigungsprozess der Aufgabe wird auf Nicht zutreffend zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Aufgaben im Projekt verknüpft.</p> </td> 
  </tr> 
  <tr> 
   <td>Abschnitt „Warteschlangendetails“ für ein Projekt oder eine Vorlage, das/die zu einer anderen Gruppe als der Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Probleme</td> 
   <td> <p>Das Feld Standardgenehmigung wird auf Nicht zutreffend zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anfragen im Projekt verknüpft.</p> </td> 
  </tr> 
  <tr> 
   <td>Warteschlangenthema-Abschnitt für ein Projekt oder eine Vorlage, das/die zu einer anderen Gruppe als der Gruppe des Genehmigungsprozesses gehört</td> 
   <td>Probleme</td> 
   <td> <p>Das Feld Standardgenehmigung wird auf Nicht zutreffend zurückgesetzt.</p> <p>Standardmäßig sind keine Genehmigungsprozesse mit neuen Problemen oder Anfragen im Projekt verknüpft.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verschieben oder Kopieren einer Aufgabe oder eines Problems in ein Projekt mit einer anderen Gruppe als der des Genehmigungsprozesses

Das Verschieben oder Kopieren einer Aufgabe oder eines Problems aus einem Projekt in ein anderes kann sich je nach Gruppe der beiden Projekte auf die vorhandenen Genehmigungsprozesse für die Aufgabe oder das Problem auswirken. Die folgende Tabelle zeigt die möglichen Szenarien:

| Genehmigungsprozess für ursprüngliche Aufgabe oder Anfrage | Gruppen der beiden Projekte | Änderungen im Genehmigungsprozess, nachdem die Aufgabe oder das Problem in ein anderes Projekt verschoben wurde |
|---|---|---|
| Genehmigungsprozess für den einmaligen Gebrauch, der mit einem systemweiten Status verknüpft ist | Projekte befinden sich in derselben oder in verschiedenen Gruppen | Keine Änderung |
| Genehmigungsprozess für den einmaligen Gebrauch, der mit einem gruppenspezifischen Status verknüpft ist | Projekte sind in verschiedenen Gruppen | Die Genehmigung bleibt ein einmaliger Genehmigungsprozess und der mit der Genehmigung verknüpfte Status wird aktualisiert, damit er einem ähnlichen Status für die neue Gruppe entspricht. |
| Systemweiter Genehmigungsprozess | Projekte befinden sich in derselben oder in verschiedenen Gruppen | Keine Änderung |
| Gruppenspezifischer Genehmigungsprozess | Projekte gehören derselben Gruppe an | Keine Änderung |
| Gruppenspezifischer Genehmigungsprozess | Projekte befinden sich in verschiedenen Gruppen und die Gruppen haben unterschiedliche gruppenspezifische Status | Die Genehmigung wird zu einem einmaligen Genehmigungsprozess und der mit der Genehmigung verknüpfte Status wird aktualisiert, damit er einem ähnlichen Status für die neue Gruppe entspricht. |
| Gruppenspezifischer Genehmigungsprozess | Projekte befinden sich in verschiedenen Gruppen und es gibt einen Status mit demselben Schlüssel in der neuen Gruppe wie der Status, der mit dem Genehmigungsprozess der ersten Gruppe verknüpft ist | Keine Änderung |
