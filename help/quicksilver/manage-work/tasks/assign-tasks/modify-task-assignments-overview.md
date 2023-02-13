---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Übersicht über das Ändern von Aufgabenzuweisungen
description: Sie können Aufgaben Benutzern, Teams oder Auftragsrollen zuweisen oder deren Zuweisung aufheben. Sie können mehrere Ressourcen gleichzeitig oder nur eine Ressource zuweisen. Sie können eine Aufgabe gleichzeitig oder mehrere Aufgaben stapelweise zuweisen.
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Übersicht über das Ändern von Aufgabenzuweisungen

Sie können Aufgaben Benutzern, Teams oder Auftragsrollen zuweisen oder deren Zuweisung aufheben. Sie können mehrere Ressourcen gleichzeitig oder nur eine Ressource zuweisen. Sie können eine Aufgabe gleichzeitig oder mehrere Aufgaben stapelweise zuweisen.

>[!TIP]
>
>Sie können mehrere Benutzer, Auftragsrollen oder Teams zuweisen. Sie können nur aktive Benutzer, Stellenrollen und Teams zuweisen.
>
>Wenn ein Benutzer, eine Rolle oder ein Team zugewiesen wurde, bevor sie deaktiviert wurden, bleiben sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
>
>* Weisen Sie das Arbeitselement aktiven Ressourcen erneut zu.
>* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team erneut zu.
>


Dieser Artikel enthält allgemeine Informationen über die Auswirkungen der Änderung von Aufgabenzuweisungen. Informationen zum Zuweisen von Aufgaben finden Sie in den folgenden Artikeln:

* Informationen zum Zuweisen von Aufgaben finden Sie unter [Aufgaben zuweisen](../../../manage-work/tasks/assign-tasks/assign-tasks.md) und [Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* Informationen zum Ändern von Zuweisungen für mehrere Aufgaben im Bereich &quot;Planung&quot;finden Sie unter [Mehrere Benutzerzuweisungen zu Aufgaben in den Planungsbereichen ändern](../../../resource-mgmt/resource-scheduling/modify-multipl-assignments-scheduling-areas.md).
* Informationen zum Zuweisen von Aufgaben mithilfe des Lastenausgleichs finden Sie unter [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Einige Informationen in diesem Artikel gelten auch für die Zuweisung von Problemen. Weitere Informationen zum Zuweisen von Problemen sowie weitere Überlegungen finden Sie unter [Übersicht über Problemzuweisungen ändern](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## Wann sollten Benutzerzuweisungen für Aufgaben geändert werden?

Sie können die Benutzerzuweisungen für Aufgaben aus verschiedenen Gründen ändern, z. B. aus den folgenden:

* Benutzer treten dem Team bei oder verlassen es.
* Ein Benutzer nimmt einen Urlaub, der über die Fälligkeitsdaten der Aufgaben hinausgeht

   >[!NOTE]
   >
   >Wenn Benutzer zur Arbeit zugewiesen werden, wirkt sich ihre Verfügbarkeit entsprechend ihren Zeitplänen auf die geplanten und geplanten Termine der Aufgaben aus. Weitere Informationen zu Zeitplänen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Eine bestimmte Rolle oder ein bestimmter Benutzer wird als Verantwortlicher für mehrere Aufgaben festgelegt und Sie möchten schnell alle Elemente ändern, die einem anderen Benutzer oder einer anderen Rolle zugewiesen werden sollen

## Überlegungen zur Mehrfachzuweisung von Stellenrollen, Teams und Benutzern

Beachten Sie beim Zuweisen mehrerer Ressourcen zu einem Arbeitselement Folgendes:

* Benutzern kann mehr als eine Auftragsrolle mit ihrem Profil zugeordnet sein. Informationen zum Zuordnen von Benutzern zu Aufgabenrollen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Aufgaben oder Probleme werden normalerweise zuerst einer oder mehreren Auftragsrollen oder einem Team zugewiesen. Wenn Projekte startbereit sind, müssen sie möglicherweise auch Benutzern zugewiesen werden.\
   Wenn eine Aufgabe oder ein Problem einer oder mehreren Rollen zugewiesen ist und Sie dann auch einen Benutzer zuweisen, bestimmt Adobe Workfront gemäß den folgenden Regeln, welche Vorgangsrolle dem zusätzlichen Benutzer zugeordnet werden soll (falls vorhanden):

   * Wenn nur eine Auftragsrolle zugewiesen ist und sie mit der Primären Rolle des Benutzers übereinstimmt, wird die Aufgabe bzw. das Problem nur dem Benutzer zugewiesen, der seine Primäre Rolle erfüllt.
   * Wenn mehrere Rollen zugewiesen sind und mindestens eine der Rollen mit den sekundären Rollen des Benutzers übereinstimmt, wird die Aufgabe bzw. das Problem dem Benutzer zugewiesen, der eine seiner &quot;Sonstige Rollen&quot;(die Workfront zufällig auswählt, wenn mehrere Übereinstimmungen vorliegen) erfüllt, sowie allen weiteren zugewiesenen Rollen.
   * Wenn eine oder mehrere Aufgabenrollen zugewiesen sind und die Benutzerrollen nicht übereinstimmen, wird die Aufgabe bzw. das Problem sowohl den Rollen oder Rollen als auch dem Benutzer zugewiesen.

* Wenn eine Aufgabe oder ein Problem einem Team zugewiesen ist und Sie auch einen Benutzer zuweisen, bleibt die Aufgabe bzw. das Problem sowohl dem Team als auch dem Benutzer zugewiesen.

## Wie sich das Entfernen von Bevollmächtigten auf die Aufgabenzeiten und Zuordnungsprozentsätze auswirkt

Das Entfernen von Benutzern kann sich auf die Aufgabenzeiten und Zuordnungsprozentsätze auswirken. Die Auswirkungen, die das Entfernen eines Benutzers auf die Aufgabe hat, hängen vom Typ Dauer ab, der für die Aufgabe ausgewählt wurde. Weitere Informationen zum Typ der Dauer finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Wenn Sie einen Benutzer aus einer Aufgabe mit den folgenden Ereignistypen löschen:

* **Einfach:** Die diesem Benutzer zugewiesenen geplanten Stunden werden von den geplanten Gesamtstunden der Aufgabe abgezogen.

   >[!IMPORTANT]
   >
   >Dies könnte sich negativ auf Ihren Projektplan auswirken, da sich dadurch die Gesamtdauer der geplanten Aufgaben und des Projekts ändert.

* **Aufwandsorientiert:** Der Zuordnungsprozentsatz ändert sich für andere Benutzer nicht.
* **Berechnete Zuweisung:** Die Zuordnungsprozentsätze anderer Benutzer werden so angepasst, dass die Gesamtsumme 100 % entspricht.
* **Berechnete Arbeit:** Der Zuordnungsprozentsatz ändert sich für andere Benutzer nicht.

## Überlegungen zum Aufheben der Zuweisung von Aufgaben

Sie können Zuweisungen aus einer Aufgabe gleichzeitig entfernen oder Zuweisungen aus mehreren Aufgaben gleichzeitig entfernen.

Weitere Informationen zum Entfernen von Zuweisungen aus Aufgaben in Stapeln finden Sie unter [Mehrere Benutzerzuweisungen in einer Aufgabenliste ändern](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

Beachten Sie beim Entfernen von Zuweisungen aus Aufgaben Folgendes:

* Wenn Sie die Zuweisung eines Benutzers zu einer Aufgabe aufheben, bleibt die Aufgabe der Auftragsrolle zugewiesen, die der Benutzer für die Aufgabe erfüllt hat.
* Wenn Sie die Zuweisung einer Auftrags- oder Team-Rolle zu einer Aufgabe aufheben, bleibt die Aufgabe nicht zugewiesen, wenn sie keiner anderen Ressource zugewiesen ist.
