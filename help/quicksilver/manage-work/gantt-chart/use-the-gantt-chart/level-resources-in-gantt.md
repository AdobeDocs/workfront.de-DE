---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Abgleichen von Ressourcen im [!UICONTROL Gantt-Diagramm]
description: Informationen zum Abgleichen von Ressourcen im Gantt-Diagramm.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# Abgleichen von Ressourcen im [!UICONTROL Gantt-Diagramm]

Die Abgleichung Ihrer Ressourcen in einem Projekt dient zwei Zwecken:

* So passen Sie automatisch die Zeitüberschreitung für Zugewiesene an.
* So erstellen Sie automatisch einen realistischen Aufgabenplan für ein Projekt.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf Projekte</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festlegt. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Manage]-Zugriff auf das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Übersicht über den Abgleich von Ressourcen

Wenn dieselbe Ressource zwei verschiedenen Vorgängen zugewiesen ist, können Sie die Zeitleiste der Vorgänge mit dem Abgleich der Ressourcen anpassen, sodass sie nicht gleichzeitig ausgeführt werden.

Beachten Sie beim Abgleichen von Ressourcen für ein Projekt Folgendes:

* Der Ressourcenabgleich gilt nur für ein Projekt, sodass [!DNL Adobe Workfront] Ressourcen nicht für mehr als ein Projekt gleichzeitig abgleicht.
* Wenn **[!UICONTROL Aufwandsgesteuert]** als **[!UICONTROL Dauertyp]** ausgewählt ist, gleichen [!DNL Workfront] die Ressourcen nicht ab.
* Wenn mehrere Benutzer derselben Aufgabe zugewiesen sind, wird der Abgleich abgebrochen.
* Bedingungen für den Typ **[!UICONTROL Aufgabenbeschränkung]** haben Vorrang vor dem Abgleich von Ressourcen. Wenn beispielsweise **[!UICONTROL Feste Termine]** als [!UICONTROL Aufgabenbeschränkung] ausgewählt ist, ändert der Ressourcenabgleich die Aufgabentermine nicht.
* Vorgängerbeziehungen haben Vorrang vor dem Abgleich von Ressourcen.
* **[!UICONTROL Ressourcenabgleich]** muss für das Projekt auf **[!UICONTROL Manuell]** gesetzt werden, um den Abgleich im [!UICONTROL Gantt-Diagramm] anzupassen. Wenn Sie über Verwaltungsberechtigungen für das Projekt verfügen, können Sie die Ressourcen automatisch auf Systemebene verwalten, indem Sie diese Einstellung für das Projekt anpassen und **[!UICONTROL Automatisch]** anstelle von **[!UICONTROL Manuell]** im **[!UICONTROL Projekt bearbeiten]** auswählen.

  ![Abgleichsmodus für Ressourcen](assets/resource-leveling-mode-350x177.png)

* Als Projektbesitzer oder Aufgabenbevollmächtigter können Sie eine Abgleichsverzögerung für eine Aufgabe einführen, um anzugeben, dass die Aufgabe möglicherweise zusätzliche Zeit benötigt. Informationen zum Hinzufügen einer Abgleichsverzögerung zu einer Aufgabe finden Sie unter [Aktualisieren der Abgleichsverzögerung für Aufgaben](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Anwenden des Ressourcenabgleichs im [!UICONTROL Gantt-Diagramm]

Sie können die Aufgabenliste (Gantt[!UICONTROL Diagramm) verwenden] um Ihre Ressourcen abzugleichen.

1. Navigieren Sie zu dem Projekt, das Sie abgleichen möchten.
1. Klicken Sie im Bereich **[!UICONTROL Aufgaben]** auf das Symbol **[!UICONTROL Gantt-Diagramm]**.

   Alle Änderungen werden automatisch gespeichert, wenn die Option **[!UICONTROL Automatisches Speichern]** aktiviert ist. Sie ist standardmäßig aktiviert.

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Plan]Modus** und wählen Sie **[!UICONTROL Manuelles Speichern von Standard]** oder **[!UICONTROL Timeline Planning]**, um Ihre Änderungen manuell zu speichern.

   >[!TIP]
   >
   >Sie können Ressourcen im [!UICONTROL Gantt-Diagramm“ nicht abgleichen] wenn die Option [!UICONTROL Automatisches Speichern] aktiviert ist.

   ![Manuelle Einstellung aktiviert](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Klicken Sie auf **[!UICONTROL Dropdown-Menü]** Ressourcen abgleichen“.

   ![Level_Resources.png](assets/level-resouces.png)

1. Eine der folgenden Optionen auswählen:

   * **[!UICONTROL Jetzt abgleichen]**: Wendet den Ressourcenabgleich auf die ausgewählte Aufgabe an.
   * **[!UICONTROL Abgleich aufheben]**: Entfernt alle Ressourcenabgleiche aus der ausgewählten Aufgabe.

   >[!NOTE]
   >
   >Ihre Ressourcen können überlastet sein, wenn sie mehreren Aufgaben zugewiesen sind, die im selben Zeitrahmen auftreten.

1. (Optional und bedingt) Wenn Sie die Option Automatisches Speichern deaktiviert haben, klicken Sie auf die Symbole **[!UICONTROL Rückgängig]** oder &#x200B;**[!UICONTROL Wiederholen]**, wenn Sie Änderungen rückgängig machen oder duplizieren möchten.

   >[!TIP]
   >
   >Mit den folgenden Tastaturbefehlen können Sie Änderungen im [!UICONTROL Gantt-Diagramm“ rückgängig machen oder ]:
   >
   >* [!DNL Mac]: Verwenden Sie [!UICONTROL Befehl + Z], um den Vorgang rückgängig zu machen, und [!UICONTROL Befehl + Umschalt + Z], um ihn wiederherzustellen.
   >* Windows: Verwenden Sie [!UICONTROL Strg + Z], um den Vorgang rückgängig zu machen, und [!UICONTROL Strg + Y], um ihn wiederherzustellen.


1. Klicken **[!UICONTROL oben rechts]** &quot;[!UICONTROL &quot; auf „Speichern].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
