---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 'Übersicht über die Aufgabe: Originaldauer und ursprünglich geplante Stunden'
description: Bei der Planung eines Projekts sollten Sie die Werte für die geplanten Stunden und die Dauer (oder geplante Dauer) jeder Aufgabe im Projekt festlegen.
author: Alina
feature: Work Management
exl-id: 96d77d9f-3d5f-457e-a4ad-10edc371a991
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 1%

---

# Übersicht über die Aufgabe: Originaldauer und ursprünglich geplante Stunden

Bei der Planung eines Projekts sollten Sie die Werte für die geplanten Stunden und die Dauer (oder geplante Dauer) jeder Aufgabe im Projekt festlegen.

Weitere Informationen zu geplanten Stunden zu Aufgaben finden Sie unter [Übersicht über geplante Stunden](../../../manage-work/tasks/task-information/planned-hours.md).

Weitere Informationen zur Aufgabendauer finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Sie können diese Werte auf der Registerkarte &quot;Aufgabendetails&quot;oder beim Bearbeiten einer Aufgabe sehen.

Wenn Sie eine Ansicht für eine Aufgabenliste oder einen Aufgabenbericht erstellen, können Sie zusätzlich die Felder &quot;Ursprüngliche geplante Stunden&quot;und &quot;Ursprüngliche Dauer&quot;für die Aufgaben anzeigen.

## Ursprünglich erforderlicher Arbeitsaufwand

Die ursprünglich geplanten Stunden einer Aufgabe stellen die Anzahl der geplanten Stunden dar, die eine Aufgabe hatte, bevor sie zur übergeordneten Aufgabe wurde. Wenn eine Aufgabe eine übergeordnete Aufgabe wird, werden die geplanten Stunden der untergeordneten Aufgaben in die übergeordnete Aufgabe aggregiert, um die geplanten Stunden der übergeordneten Aufgabe anzugeben.

Wenn Sie das Feld Ursprünglich geplante Stunden in einem Aufgabenbericht oder einer Aufgabenliste anzeigen, können Sie die Originalanzahl der geplanten Stunden anzeigen, bevor die Aufgabe die Anzahl der geplanten Stunden ihrer untergeordneten Elemente geerbt hat.

>[!NOTE]
>
>Wenn Sie eine Aufgabe erstellen, beträgt die Anzahl der ursprünglich geplanten Stunden null. Wenn die Aufgabe eine übergeordnete Aufgabe wird, wird der Wert dieses Felds mit der Anzahl der geplanten Stunden der Aufgabe ausgefüllt, bevor sie in eine übergeordnete Aufgabe geändert wurde. Dieser Wert verbleibt in diesem Feld, selbst wenn die Aufgabe wieder zu einer eigenständigen Aufgabe zurückgesetzt wird.

## Ursprüngliche Dauer

Die ursprüngliche Dauer einer Aufgabe ist die Dauer in Minuten, die eine Aufgabe hatte, bevor sie zur übergeordneten Aufgabe wurde. Wenn eine Aufgabe übergeordnet wird, wird die Dauer zwischen dem geplanten Startdatum des frühesten untergeordneten Elements und dem geplanten Abschlussdatum des letzten untergeordneten Elements in die übergeordnete Aufgabe aggregiert und wird zur Dauer der übergeordneten Aufgabe. Dadurch wird die Dauer der ursprünglichen Aufgabe ersetzt.

Wenn Sie das Feld Ursprüngliche Dauer in einem Aufgabenbericht oder einer Aufgabenliste anzeigen, können Sie die Originalanzahl der Tage für die Dauer der Aufgabe anzeigen, bevor die Dauer der untergeordneten Aufgaben übernommen wurde.

>[!NOTE]
>
>Wenn Sie eine Aufgabe erstellen, ist die ursprüngliche Dauer null. Wenn die Aufgabe eine übergeordnete Aufgabe wird, wird der Wert dieses Felds mit der Dauer der Aufgabe ausgefüllt, bevor sie in eine übergeordnete Aufgabe geändert wurde. Dieser Wert verbleibt in diesem Feld, selbst wenn die Aufgabe wieder zu einer eigenständigen Aufgabe zurückgesetzt wird. Dieser Wert wird in Minuten angezeigt.

## Beispiel

Wenn zwei Aufgaben beispielsweise eigenständige Aufgaben sind, sind ihre ursprüngliche Dauer und die ursprünglich geplanten Stunden null.

![original_scheduled_hours_and_duration_without_parent.png](assets/original-planned-hours-and-duration-without-parent-350x38.png)

Wenn die erste Aufgabe übergeordnet wird, werden die Felder &quot;Originaldauer&quot;und &quot;Ursprünglich geplante Stunden&quot;mit den Werten für Dauer und Geplante Stunden der Aufgabe ausgefüllt, bevor sie übergeordnet wurde. Die ursprüngliche Dauer wird in Minuten angezeigt. Die Dauer und die geplanten Stunden des Kindes werden zur Dauer und den geplanten Stunden des Elternteils.

![original_and_scheduled_hours_with_a_parent_task.png](assets/original-and-planned-hours-with-a-parent-task-350x38.png)

Wenn das übergeordnete Element wieder zu einer eigenständigen Aufgabe wird, kehren die Dauer und die geplanten Stunden wieder zu den ursprünglichen Werten zurück, während die ursprüngliche Dauer und die ursprünglich geplanten Stunden ausgefüllt bleiben. Sie kehren nicht auf null zurück.

![original_duration_and_scheduled_hours_after_reversal_of_a_parent.png](assets/original-duration-and-planned-hours-after-reversal-of-a-parent-350x39.png)
