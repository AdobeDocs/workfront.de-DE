---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Verwalten von Benutzer- und Rollenzuordnungsstunden für Aufgaben
description: Beim Zuweisen von Benutzern oder Rollen zu einer Aufgabe werden sie einer bestimmten Anzahl von Stunden zugewiesen, um die Aufgabe abzuschließen. Sie können die Anzahl der Stunden, die jedem Benutzer oder jeder Auftragsrolle zugewiesen werden, wenn sie einer Aufgabe zugewiesen werden, manuell ändern, wenn der Aufgabendauer-Typ einfach ist.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 830ad0411084844ace1e1e543c3ebefcb558af80
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Verwalten von Benutzer- und Rollenzuordnungsstunden für Aufgaben

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p>
   <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute oder höhere Berechtigungen für die Aufgabe</p> <p>Berechtigungen bearbeiten, um die Zuordnungszeiten im Feld "Aufgabe bearbeiten"zu aktualisieren</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Ändern der Zuordnungszeiten für eine Aufgabe

>[!IMPORTANT]
>
>Nachdem Sie die Zuordnungen für jede Aufgabenzuweisung manuell geändert haben, werden die geplanten Stunden der Aufgaben möglicherweise entsprechend aktualisiert. Weitere Informationen finden Sie im Abschnitt &quot;[Geplante Stunden bei der Verwaltung von Benutzerzuweisungen aktualisieren](../../../manage-work/tasks/task-information/planned-hours.md#update)&quot;im Artikel [Übersicht über geplante Stunden](../../../manage-work/tasks/task-information/planned-hours.md)&quot;.

* Die Gesamtstunden, die den einzelnen Ressourcen, die der Aufgabe zugewiesen sind, zugewiesen werden, stellen die geplanten Stunden der Aufgabe dar.
* Wenn einer Aufgabe ein Benutzer oder eine Rollenzuweisung zugewiesen ist, entspricht die dem Benutzer bzw. der Rolle zugewiesene Zeitdauer den geplanten Stunden der Aufgabe.
* Bei mehreren Zuweisungen wird jedem Benutzer bzw. jeder Vorgangsrolle standardmäßig eine gleiche Anzahl von Stunden für die Arbeit an der Aufgabe zugewiesen, wenn der Aufgabendauer-Typ einfach ist. Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Überblick über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Übersicht über den Dauer-Typ: Einfach](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Wenn die Aufgabe den Typ Einfache Dauer aufweist, können Sie die Anzahl der zugewiesenen Stunden für jeden Benutzer oder jede Aufgabenrolle manuell ändern, um anzugeben, dass einige der Aufgabenverantwortlichen möglicherweise mehr Zeit für die Bearbeitung einer Aufgabe haben als andere.
* Sie können die den Aufgaben zugewiesenen Teams zugewiesenen Stunden nicht ändern.
* Sie können die Benutzer- oder Aufgabenrollenzuordnung für Probleme nicht manuell ändern.
* Sie können auch die tägliche, wöchentliche oder monatliche Zuordnung von Benutzern zu Aufgaben oder Problemen mithilfe des Workload Balancer verwalten. Weitere Informationen finden Sie unter [Verwalten von Benutzerzuordnungen im Arbeitslade-Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Ändern der Benutzer- oder Rollenzuordnungszeiten für eine Aufgabe

1. Gehen Sie zu einer Aufgabe, für deren Zuweisungen Sie die Zuordnungszeiten ändern möchten.
1. Klicken Sie auf das Menü **Mehr** neben dem Namen der Aufgabe, dann auf **Bearbeiten** und dann auf **Zuweisungen**.![](assets/qs-more-icon-on-an-object.png)

   Oder

   Klicken Sie in der Aufgabenüberschrift auf den Bereich **Zuweisungen** und dann auf **Erweitert**.

1. Stellen Sie sicher, dass der **Dauer-Typ** der Aufgabe **einfach** ist.
1. Ändern Sie die **Zuordnungen** für jeden Aufgabenverantwortlichen. Dies sind die Gesamtzuweisungen für jede Zuweisung zu dieser Aufgabe während der gesamten Dauer der Aufgabe. Dadurch kann auch die Gesamtdauer der geplanten Aufgaben aktualisiert werden.

   ![Ändern der Zuordnungen](assets/advanced-assignments-duration-type-allocations.png)

1. Klicken Sie auf **Speichern**.
