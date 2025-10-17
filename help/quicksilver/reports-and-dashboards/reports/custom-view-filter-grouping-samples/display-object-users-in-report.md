---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Berichte oder Listen: Zeigt Benutzer an, die mit einem Objekt verknüpft sind'
description: Sie können Benutzer, Aufgabengebiete und Teams, die mit Objekten in Berichten oder Listen verknüpft sind, anzeigen und in Filtern auf diese verweisen. Sie können nicht nach Benutzern, Aufgabengebieten oder Teams gruppieren, die mit Objekten verknüpft sind.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 2%

---

# Berichte oder Listen: Zeigt Benutzer an, die mit einem Objekt verknüpft sind

Sie können Benutzer, Aufgabengebiete und Teams, die mit Objekten in Berichten oder Listen verknüpft sind, anzeigen und in Filtern auf diese verweisen. Sie können nicht nach Benutzern, Aufgabengebieten oder Teams gruppieren, die mit Objekten verknüpft sind.

Sie können nach Benutzern, Aufgabengebieten oder Teams filtern, die mit den folgenden Objekten verknüpft sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Objekt</td> 
   <td>Zugeordnete Benutzer oder Aufgabengebiete</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Projekt</td> 
   <td> <p>Sie können alle Benutzenden und die Aufgabengebiete, die sie für das Projekt erfüllen, in einem Projektbericht anzeigen. Sie können nicht nach Benutzern oder deren zugehörigen Aufgabengebieten in einem Projektbericht filtern. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aufgaben</td> 
   <td>Sie können in einem Aufgabenbericht nach allen Benutzern, Aufgabengebieten und Teams filtern, die einer Aufgabe zugewiesen sind.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Probleme</td> 
   <td>Sie können in einem Problembericht nach allen Benutzern, Aufgabengebieten und Teams filtern, die einem Problem zugewiesen sind.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Portfolios</td> 
   <td>Sie können alle Benutzenden und die Aufgabengebiete, die sie für das Projekt erfüllen, in einem Projektbericht anzeigen und den Bericht nach Portfolio gruppieren. Sie können nicht nach Benutzern oder deren zugehörigen Aufgabengebieten in einem Projektbericht filtern.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Programme</td> 
   <td>Sie können alle Benutzenden und die Aufgabengebiete, die sie für das Projekt erfüllen, in einem Projektbericht anzeigen und den Bericht nach Programm gruppieren. Sie können nicht nach Benutzern oder deren zugehörigen Aufgabengebieten in einem Projektbericht filtern.</td> 
  </tr> 
 </tbody> 
</table>

## Alle mit einem Projekt verknüpften Benutzer und Aufgabengebiete anzeigen

Sie können alle Benutzenden, die mit im Projekt verknüpft sind, in der Ansicht einer Projektliste oder eines Berichts anzeigen. Dazu gehören alle Benutzenden, die im Abschnitt Personen des Projekts aufgeführt sind. Sie können auch die Rollen anzeigen, denen sie zugeordnet sind, wenn sie Aufgaben oder Problemen im Projekt zugewiesen wurden, und zwar in einem Projektbericht.

![Projekt mit Benutzer- und Rolleninformationen](assets/project-with-user-and-role-information-report-350x100.png)

Informationen zum Erstellen eines Projektberichts, in dem alle Benutzenden und ihre Rollen im Projekt angezeigt werden, finden Sie [Ansicht: Liste der Projektbenutzenden mit Aufgabengebieten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Sie können nicht nach Benutzern oder Aufgabengebieten filtern, die mit Projekten in einem Projektfilter verknüpft sind.

## Alle Benutzer, Aufgabengebiete oder Teams anzeigen, die einer Aufgabe zugewiesen sind

Sie können alle Benutzer, Rollen oder Teams, die einer Aufgabe zugewiesen sind, in der Ansicht einer Aufgabenliste oder eines Berichts anzeigen, indem Sie das Feld Zuweisungen zur Ansicht hinzufügen.

![Zuweisungsfeld](assets/assignments-field-task-view-350x124.png)

Sie können nach Benutzern, Aufgabengebieten oder Teams filtern, die Aufgaben zugewiesen wurden, indem Sie in einem Aufgabenfilter auf die folgenden Felder verweisen:

* Arbeitsauftrag – Benutzer
* Arbeitsauftrag – Aufgabengebiete
* Team

![Arbeitsauftrag - Benutzer und Rollen im Aufgabenfilter](assets/assignment-users-roles-task-filter-350x334.png)

## Alle Benutzer, Aufgabengebiete oder Teams anzeigen, die einem Problem zugewiesen sind

Sie können alle Benutzenden, Rollen oder Teams, die einem Problem zugewiesen sind, in der Ansicht einer Problemliste oder eines Berichts anzeigen, indem Sie das Feld Zuweisungen zur Ansicht hinzufügen.

Sie können nach Benutzern, Aufgabengebieten oder Teams filtern, die Problemen zugewiesen sind, indem Sie in einem Problemfilter auf die folgenden Felder verweisen:

* Arbeitsauftrag – Benutzer
* Arbeitsauftrag – Aufgabengebiete
* Team

## Alle mit einem Portfolio verbundenen Benutzer und Aufgabengebiete anzeigen

Sie können alle mit einem Portfolio verbundenen Benutzer und Rollen anzeigen, indem Sie sie in einem Projektbericht anzeigen und dann den Bericht nach Portfolio gruppieren.

Informationen zum Erstellen eines Projektberichts, in dem alle Benutzenden und ihre Rollen im Projekt angezeigt werden, finden Sie [Ansicht: Liste der Projektbenutzenden mit Aufgabengebieten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Sie können nicht nach Benutzern oder Aufgabengebieten filtern, die mit Projekten in einem Portfolio oder Projektfilter verknüpft sind.

## Alle mit einem Programm verknüpften Benutzer und Aufgabengebiete anzeigen

Sie können alle mit einem Programm verbundenen Benutzer und Rollen anzeigen, indem Sie sie in einem Projektbericht anzeigen und dann den Bericht nach Programm gruppieren.

Informationen zum Erstellen eines Projektberichts, in dem alle Benutzenden und ihre Rollen im Projekt angezeigt werden, finden Sie [Ansicht: Liste der Projektbenutzenden mit Aufgabengebieten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

Sie können nicht nach Benutzern oder Aufgabengebieten filtern, die mit Projekten in einem Programm- oder Projektfilter verknüpft sind.
