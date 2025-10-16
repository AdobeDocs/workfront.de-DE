---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Verwalten der Stunden für die Zuweisung von Benutzenden und Rollen bei Aufgaben
description: Wenn Sie einer Aufgabe Benutzer oder Rollen zuweisen, wird ihnen eine bestimmte Anzahl von Stunden zugewiesen, um die Aufgabe abzuschließen. Sie können die Anzahl der Stunden, die jedem Benutzer bzw. jeder Aufgabenrolle zugewiesen werden, wenn er bzw. sie einer Aufgabe zugewiesen wird, manuell ändern, wenn der Aufgabendauer-Typ „Einfach“ ist.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: d0be569333b0454e26f4d0de1078b0425cf81707
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Verwalten der Stunden für die Zuordnung von Benutzern und Rollen bei Aufgaben

Zuordnungsstunden stellen die Gesamtzeit dar, in der eine zugewiesene Ressource an einem Vorgang arbeiten soll. Die Stunden stellen die Zeit dar, die einem Benutzer an einem bestimmten Tag oder Wochentag, einer bestimmten Woche oder einem bestimmten Monat während der Dauer der Aufgabe zugewiesen wird.

>[!NOTE]
>
>Wenn Sie Benutzende einer Arbeit zuweisen, wirkt sich ihre Verfügbarkeit entsprechend den Zeitplänen auf die geplanten und erwarteten Termine von Aufgaben und Problemen aus. Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Arbeit oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Aufgaben bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td>
   <td><p>Tragen Sie zur Aufgabe bei oder erhöhen Sie die Berechtigungen.</p>
   <p>Bearbeiten von Berechtigungen zum Aktualisieren von Zuordnungsstunden im Feld Aufgabe bearbeiten</p></td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Ändern der Zuordnungsstunden für eine Aufgabe

>[!IMPORTANT]
>
>Nachdem Sie die Zuordnungen für jede Zuweisung zu Aufgaben manuell geändert haben, werden die geplanten Stunden der Aufgaben möglicherweise entsprechend aktualisiert. Weitere Informationen finden Sie im Abschnitt [Aktualisieren der geplanten Stunden bei der Verwaltung von Benutzerzuweisungen](../../../manage-work/tasks/task-information/planned-hours.md#update) im Artikel [Geplante Stunden - Übersicht](../../../manage-work/tasks/task-information/planned-hours.md).

* Die Summe der Stunden, die einzelnen Ressourcen zugeordnet wurden, die der Aufgabe zugewiesen wurden, stellt die geplanten Stunden der Aufgabe dar.
* Wenn einer Aufgabe ein(e) Benutzende(r) oder eine Rollenzuweisung zugewiesen ist, entspricht die Anzahl der dem/r Benutzenden oder der Rolle zugewiesenen Stunden den geplanten Stunden der Aufgabe.
* Bei mehreren Zuweisungen wird jedem Benutzer bzw. jeder Aufgabenrolle standardmäßig dieselbe Anzahl von Stunden für die Arbeit an der Aufgabe zugewiesen, wenn der Dauertyp „Aufgabe“ „Einfach“ ist. Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Übersicht über den Dauertyp: Einfach](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Wenn die Aufgabe vom Typ Einfache Dauer ist, können Sie die Anzahl der zugewiesenen Stunden für jeden Benutzer oder jedes Aufgabengebiet manuell ändern, um anzugeben, dass einige der Aufgabenzugewiesenen mehr Zeit für die Arbeit an einer Aufgabe haben könnten als andere.
* Die Stundenanzahl, die Teams zugewiesen wurde, die Aufgaben zugewiesen wurden, kann nicht geändert werden.
* Sie können die Zuordnung von Benutzenden oder Aufgabengebieten für Probleme nicht manuell ändern.
* Mit dem Workload-Balancer können Sie auch die tägliche, wöchentliche oder monatliche Zuweisung von Benutzenden zu Aufgaben oder Problemen verwalten. Weitere Informationen finden Sie unter [Verwalten von Benutzerzuweisungen im Workload-Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Ändern der Benutzer- oder Rollenzuordnungsstunden für eine Aufgabe

1. Gehe zu einer Aufgabe, deren Zuweisungen die Zuordnungsstunden ändern sollen.
1. Klicken Sie auf das **Mehr**-![](assets/qs-more-icon-on-an-object.png) neben dem Namen der Aufgabe, klicken Sie dann auf **Bearbeiten** und dann auf **Arbeitsaufträge**.

   Oder

   Klicken Sie in **Aufgabenkopfzeile auf den** „Arbeitsaufträge“ und dann auf **Erweitert**.

1. Stellen Sie sicher **dass der „Dauertyp** der Aufgabe &quot;**&quot;**.
1. Ändern Sie **Zuweisungen** für jeden Aufgabenempfänger. Dies sind die Gesamtzuweisungen für jede Zuweisung zu dieser Aufgabe für die gesamte Dauer der Aufgabe. Dadurch werden möglicherweise auch die insgesamt geplanten Stunden der Aufgabe aktualisiert.

   ![Zuweisungen ändern](assets/advanced-assignments-duration-type-allocations.png)

1. Klicken Sie auf **Speichern**.
