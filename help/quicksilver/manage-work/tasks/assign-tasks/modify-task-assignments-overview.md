---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Übersicht über das Ändern von Aufgabenzuweisungen
description: Sie können Benutzern, Teams oder Aufgabengebieten Aufgaben zuweisen oder die Zuweisung von Aufgaben aufheben. Sie können mehrere Ressourcen oder nur eine Ressource gleichzeitig zuweisen. Sie können jeweils eine Aufgabe oder mehrere Aufgaben gleichzeitig zuweisen.
author: Lisa
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Übersicht über das Ändern von Aufgabenzuweisungen

Sie können Benutzern, Teams oder Aufgabengebieten Aufgaben zuweisen oder die Zuweisung von Aufgaben aufheben. Sie können mehrere Ressourcen oder nur eine Ressource gleichzeitig zuweisen. Sie können jeweils eine Aufgabe oder mehrere Aufgaben gleichzeitig zuweisen.

>[!TIP]
>
>Sie können mehrere Benutzer, Aufgabengebiete oder Teams zuweisen. Sie können nur aktive Benutzer, Aufgabengebiete und Teams zuweisen.
>
>Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team zugewiesen wurde, bevor sie/er deaktiviert wurden, bleiben sie/sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
>
>* Weisen Sie das Arbeitselement den aktiven Ressourcen neu zu.
>* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team zu.
>

Dieser Artikel enthält allgemeine Informationen über die Auswirkungen der Änderung von Aufgabenzuweisungen. Informationen zum Zuweisen von Aufgaben finden Sie in den folgenden Artikeln:

* Informationen zum Zuweisen von Aufgaben finden Sie unter [Aufgaben zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks.md) und [Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Informationen zum Ändern von Zuweisungen für mehrere Aufgaben im Planungsbereich finden Sie unter „Ändern von Zuweisungen für mehrere Benutzer zu Aufgaben in den Planungsbereichen“.
* Informationen zum Zuweisen von Aufgaben mit dem Workload Balancer finden Sie unter [Übersicht über das Zuweisen von Arbeit im Workload Balancer](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Einige Informationen in diesem Artikel gelten auch für Zuweisungen an Probleme. Weitere Informationen zum Zuweisen von Problemen und weitere Überlegungen finden Sie unter [Übersicht über das Ändern von Problemzuweisungen](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Wann Benutzerzuweisungen für Aufgaben geändert werden sollten

Möglicherweise möchten Sie die Benutzerzuweisungen für Aufgaben aus verschiedenen Gründen ändern, z. B.:

* Benutzer können Ihrem Team beitreten oder es verlassen
* Ein(e) Benutzende(r) macht Urlaub, der über die Fälligkeitsdaten der Aufgabe hinausgeht

  >[!NOTE]
  >
  >Wenn Sie Benutzende einer Arbeit zuweisen, wirkt sich ihre Verfügbarkeit entsprechend den Zeitplänen auf die geplanten und geplanten Termine von Aufgaben aus. Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Eine bestimmte Rolle oder ein bestimmter Benutzer wird für mehrere Aufgaben als Verantwortlicher festgelegt, und Sie möchten schnell alle Elemente ändern, die einem anderen Benutzer oder einer anderen Rolle zugewiesen werden sollen

## Überlegungen zu mehreren Zuweisungen an Aufgabengebiete, Teams und Benutzer

Beachten Sie Folgendes, wenn Sie einem Arbeitselement mehrere Ressourcen zuweisen:

* Benutzern kann mehr als ein Aufgabengebiet mit ihrem Profil zugeordnet sein. Informationen zum Verknüpfen von Benutzern mit Aufgabengebieten finden Sie unter [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Aufgaben oder Probleme werden in der Regel zuerst einem oder mehreren Aufgabengebieten oder einem Team zugewiesen. Wenn Projekte startbereit sind, müssen sie möglicherweise auch Benutzern zugewiesen werden.\
  Wenn eine Aufgabe oder ein Problem einer oder mehreren Rollen zugewiesen ist und Sie dann auch einen Benutzer zuweisen, entscheidet Adobe Workfront gemäß den folgenden Regeln, welches Aufgabengebiet mit dem zusätzlichen Benutzer (falls vorhanden) verknüpft werden soll:

   * Wenn nur ein Aufgabengebiet zugewiesen ist und es mit der Primären Rolle des Benutzers übereinstimmt, wird die Aufgabe oder das Problem nur dem Benutzer zugewiesen, der seine Primäre Rolle erfüllt.
   * Wenn mehrere Rollen zugewiesen sind und mindestens eine der Rollen mit den sekundären Rollen des Benutzers übereinstimmt, wird die Aufgabe oder das Problem dem Benutzer zugewiesen, der eine der anderen Rollen erfüllt (die Workfront zufällig auswählt, wenn mehrere Übereinstimmungen vorliegen), sowie allen zusätzlichen Rollen, die zugewiesen werden.
   * Wenn mindestens ein Aufgabengebiet zugewiesen ist und es keine Übereinstimmungen mit den Rollen des Benutzers gibt, wird die Aufgabe oder das Problem sowohl der Rolle bzw. den Rollen als auch dem Benutzer zugewiesen.

* Wenn eine Aufgabe oder ein Problem einem Team zugewiesen wird und Sie auch einen Benutzer zuweisen, bleibt die Aufgabe oder das Problem sowohl dem Team als auch dem Benutzer zugewiesen.

## Wie sich das Entfernen von Verantwortlichen auf die Aufgabenstunden und Zuordnungsprozentsätze auswirkt

Das Entfernen von Benutzern kann sich auf die Aufgabenstunden und Zuordnungsprozentsätze auswirken. Welche Auswirkungen das Entfernen eines Benutzers auf die Aufgabe hat, hängt vom für die Aufgabe ausgewählten Dauertyp ab. Informationen zum Dauertyp finden Sie unter [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Wenn Sie einen Benutzer aus einer Aufgabe mit den folgenden Dauertypen löschen:

* **Einfach** Die diesem Benutzer zugewiesenen geplanten Stunden werden von den geplanten Gesamtstunden der Aufgabe abgezogen.

  >[!IMPORTANT]
  >
  >Dies könnte sich negativ auf Ihren Projektplan auswirken, da es die geplanten Gesamtstunden für die Aufgabe und das Projekt ändert.

* **Leistungsgesteuert:** Der Zuordnungsprozentsatz ändert sich für andere Benutzer nicht.
* **Berechnete Zuweisung:** Die Zuordnungsprozentsätze anderer Benutzer werden so angepasst, dass die Gesamtsumme 100% entspricht.
* **Berechnete Arbeit:** Der Zuordnungsprozentsatz ändert sich für andere Benutzer nicht.

## Überlegungen zum Aufheben der Zuweisung von Aufgaben

Sie können Zuweisungen aus jeweils einer Aufgabe entfernen oder Sie können Zuweisungen aus mehreren Aufgaben zusammen entfernen.

Weitere Informationen zum Massenentfernen von Zuweisungen aus Aufgaben finden Sie unter [Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Beachten Sie beim Entfernen von Zuweisungen aus Aufgaben Folgendes:

* Wenn Sie die Zuweisung eines Benutzers zu einer Aufgabe aufheben, bleibt die Aufgabe dem Aufgabengebiet zugewiesen, das der Benutzer bei der Aufgabe erfüllt hat.
* Wenn Sie die Zuweisung eines Aufgabengebiets oder Teams zu einer Aufgabe aufheben, bleibt die Zuweisung der Aufgabe aufgehoben, sofern sie keiner anderen Ressource zugewiesen ist.
