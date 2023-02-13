---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Verwalten von Benutzer- und Rollenzuordnungsstunden für Aufgaben
description: Beim Zuweisen von Benutzern oder Rollen zu einer Aufgabe werden sie einer bestimmten Anzahl von Stunden zugewiesen, um die Aufgabe abzuschließen. Sie können die Anzahl der Stunden, die jedem Benutzer oder jeder Auftragsrolle zugewiesen werden, wenn sie einer Aufgabe zugewiesen werden, manuell ändern, wenn der Aufgabendauer-Typ einfach ist.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Verwalten von Benutzer- und Rollenzuordnungsstunden für Aufgaben

Beim Zuweisen von Benutzern oder Rollen zu einer Aufgabe werden sie einer bestimmten Anzahl von Stunden zugewiesen, um die Aufgabe abzuschließen. Sie können die Anzahl der Stunden, die jedem Benutzer oder jeder Auftragsrolle zugewiesen werden, wenn sie einer Aufgabe zugewiesen werden, manuell ändern, wenn der Aufgabendauer-Typ einfach ist.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen oder höhere Berechtigungen zur Aufgabe</p> <p>Berechtigungen bearbeiten, um die Zuordnungszeiten im Feld "Aufgabe bearbeiten"zu aktualisieren</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Ändern der Zuordnungszeiten für eine Aufgabe

>[!IMPORTANT]
>
>Nachdem Sie die Zuordnungen für jede Aufgabenzuweisung manuell geändert haben, werden die geplanten Stunden der Aufgaben möglicherweise entsprechend aktualisiert. Weitere Informationen finden Sie im Abschnitt . [Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen](../../../manage-work/tasks/task-information/planned-hours.md#update) im Artikel [Übersicht über geplante Stunden](../../../manage-work/tasks/task-information/planned-hours.md).

* Die Gesamtstunden, die den einzelnen Ressourcen, die der Aufgabe zugewiesen sind, zugewiesen werden, entsprechen den geplanten Stunden der Aufgabe.
* Wenn einer Aufgabe ein Benutzer oder eine Rollenzuweisung zugewiesen ist, entspricht die dem Benutzer bzw. der Rolle zugewiesene Zeitdauer den geplanten Stunden der Aufgabe.
* Bei mehreren Zuweisungen wird jedem Benutzer bzw. jeder Vorgangsrolle standardmäßig eine gleiche Anzahl von Stunden für die Arbeit an der Aufgabe zugewiesen, wenn der Aufgabendauer-Typ einfach ist. Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Übersicht über den Durationstyp: Einfach](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Wenn die Aufgabe den Typ Einfache Dauer aufweist, können Sie die Anzahl der zugewiesenen Stunden für jeden Benutzer oder jede Aufgabenrolle manuell ändern, um anzugeben, dass einige der Aufgabenverantwortlichen möglicherweise mehr Zeit für die Bearbeitung einer Aufgabe haben als andere.
* Sie können die den Aufgaben zugewiesenen Teams zugewiesenen Stunden nicht ändern.
* Sie können die Benutzer- oder Aufgabenrollenzuordnung für Probleme nicht manuell ändern.
* Sie können auch die tägliche, wöchentliche oder monatliche Zuordnung von Benutzern zu Aufgaben oder Problemen mithilfe des Workload Balancer verwalten. Weitere Informationen finden Sie unter [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Ändern der Benutzer- oder Rollenzuordnungszeiten für eine Aufgabe

1. Gehen Sie zu einer Aufgabe, für deren Zuweisungen Sie die Zuordnungszeiten ändern möchten.
1. Klicken Sie auf **Mehr** Menü ![](assets/qs-more-icon-on-an-object.png) neben dem Namen der Aufgabe klicken Sie auf **Bearbeiten**, dann **Zuweisungen**.

   Oder

   Klicken Sie auf **Zuweisungen** Bereich in der Aufgabenüberschrift und klicken Sie dann auf **Erweitert**.

1. Stellen Sie sicher, dass **Dauer Typ** der Aufgabe **Einfach**.
1. Ändern Sie die **Zuordnungen** für jeden Aufgabenverantwortlichen. Dies sind die Gesamtzuweisungen für jede Zuweisung zu dieser Aufgabe während der gesamten Dauer der Aufgabe. Dadurch kann auch die Gesamtdauer der geplanten Aufgaben aktualisiert werden.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Klicken Sie auf **Speichern**.
