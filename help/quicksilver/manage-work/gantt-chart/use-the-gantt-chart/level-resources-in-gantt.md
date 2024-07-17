---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Level-Ressourcen im [!UICONTROL Gantt-Diagramm]
description: Informationen zum Level von Ressourcen im Gantt-Diagramm.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Level-Ressourcen im [!UICONTROL Gantt-Diagramm]

Die Nutzung Ihrer Ressourcen für ein Projekt hat zwei Ziele:

* Automatische Anpassung der Zeitüberzuteilung für Bevollmächtigte.
* So erstellen Sie automatisch einen realistischen Aufgabenzeitplan für ein Projekt.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL] Zugriff auf das Projekt verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Übersicht über die Ressourcenebene

Wenn dieselbe Ressource zwei verschiedenen Aufgaben zugewiesen ist, können Sie die Ressourcenebene verwenden, um die Zeitleiste der Aufgaben so anzupassen, dass sie nicht gleichzeitig ausgeführt werden.

Beachten Sie Folgendes beim Einbinden von Ressourcen auf ein Projekt:

* Die Ressourcenebene gilt nur für ein Projekt, sodass [!DNL Adobe Workfront] Ressourcen nicht für mehr als ein Projekt auf einer Ebene einstuft.
* Wenn **[!UICONTROL Anstrengung gesteuert]** als **[!UICONTROL Dauer-Typ]** ausgewählt ist, werden die Ressourcen nicht auf [!DNL Workfront] gesetzt.
* Wenn mehrere Benutzer derselben Aufgabe zugewiesen sind, wird die Einteilung abgebrochen.
* Bedingungen für den Typ von **[!UICONTROL Task Constraint]** haben Vorrang vor der Ebene der Ressourcen. Wenn beispielsweise **[!UICONTROL Feste Datumswerte]** als [!UICONTROL Aufgabenbegrenzung] ausgewählt ist, ändert die Ressourcenebene die Aufgabendaten nicht.
* Vorläufige Beziehungen haben Vorrang vor der Ressourcenebene.
* **[!UICONTROL Ressourcenebene]** muss für das Projekt auf **[!UICONTROL Manuell]** gesetzt werden, um die Ebene im [!UICONTROL Gantt-Diagramm] anzupassen. Wenn Sie über Verwaltungsberechtigungen für das Projekt verfügen, können Sie festlegen, dass Ressourcen automatisch vom System verwaltet werden, indem Sie diese Einstellung im Projekt anpassen und im Feld **[!UICONTROL Projekt bearbeiten]** die Option **[!UICONTROL Automatisch]** anstelle von **[!UICONTROL Manuell]** auswählen.

  ![](assets/resource-leveling-mode-350x177.png)

* Als Projekteigentümer oder Aufgabenverantwortlicher können Sie eine Zeitverzögerung für eine Aufgabe einführen, um anzuzeigen, dass eine große Wahrscheinlichkeit besteht, dass die Aufgabe möglicherweise mehr Zeit benötigt. Weitere Informationen zum Hinzufügen einer Zeitverzögerung zu einer Aufgabe finden Sie unter [Verzögerung der Aufgabenebene aktualisieren](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Anwenden der Ressourcenebene im [!UICONTROL Gantt-Diagramm]

Sie können die Aufgabenliste [!UICONTROL Gantt-Diagramm] verwenden, um Ihre Ressourcen zu unterteilen.

1. Wechseln Sie zu dem Projekt, das Sie unterteilen möchten.
1. Klicken Sie im Bereich **[!UICONTROL Aufgaben]** auf das Symbol **[!UICONTROL Gantt-Diagramm]**.

   Alle Änderungen werden automatisch gespeichert, wenn die Option **[!UICONTROL Autosave]** aktiviert ist. Sie ist standardmäßig aktiviert.

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Planen] mode** und wählen Sie **[!UICONTROL Manuelles Speichern von Standard]** oder **[!UICONTROL Timeline-Planung]** aus, um Ihre Änderungen manuell zu speichern.

   >[!TIP]
   >
   >Sie können keine Ressourcen im [!UICONTROL Gantt-Diagramm] ausrichten, wenn die Option [!UICONTROL Autosave] aktiviert ist.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Klicken Sie auf das Dropdown-Menü **[!UICONTROL Level Resources]** .

   ![Level_resources.png](assets/level-resouces.png)

1. Wählen Sie eine der folgenden Optionen aus:

   * **[!UICONTROL Level Now]**: Wendet die Ressourcenebene auf die ausgewählte Aufgabe an.
   * **[!UICONTROL Levellierungsgrad löschen]**: Entfernt alle Ressourcenebenen aus der ausgewählten Aufgabe.

   >[!NOTE]
   >
   >Ihre Ressourcen werden möglicherweise überzugewiesen, wenn sie mehreren Aufgaben zugewiesen werden, die im selben Zeitrahmen stattfinden.

1. (Optional und bedingt) Wenn Sie die Option &quot;Automatisches Speichern&quot;deaktiviert haben, klicken Sie auf die Symbole **[!UICONTROL Rückgängig]** oder &#x200B;**[!UICONTROL Wiederholen]** , wenn Sie eine der Änderungen abbrechen oder duplizieren möchten.

   >[!TIP]
   >
   >Sie können die folgenden Tastaturbefehle verwenden, um Änderungen am [!UICONTROL Gantt-Diagramm] rückgängig zu machen oder wiederherzustellen:
   >
   >* [!DNL Mac]: Verwenden Sie [!UICONTROL Befehl + Z], um das Rückgängigmachen rückgängig zu machen, und [!UICONTROL Befehl + Umschalt + Z], um es erneut auszuführen.
   >* Windows: Verwenden Sie [!UICONTROL Strg + Z], um das Rückgängigmachen rückgängig zu machen, und [!UICONTROL Strg + Y], um es erneut auszuführen.


1. Klicken Sie oben rechts im [!UICONTROL Gantt-Diagramm] auf **[!UICONTROL Speichern]**.

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
