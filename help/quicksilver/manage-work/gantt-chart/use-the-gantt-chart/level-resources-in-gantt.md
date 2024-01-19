---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Level-Ressourcen in  [!UICONTROL Gantt-Diagramm]
description: Informationen zum Level von Ressourcen im Gantt-Diagramm.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Level-Ressourcen in [!UICONTROL Gantt-Diagramm]

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

Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL] Zugriff auf das Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Übersicht über die Ressourcenebene

Wenn dieselbe Ressource zwei verschiedenen Aufgaben zugewiesen ist, können Sie die Ressourcenebene verwenden, um die Zeitleiste der Aufgaben so anzupassen, dass sie nicht gleichzeitig ausgeführt werden.

Beachten Sie Folgendes beim Einbinden von Ressourcen auf ein Projekt:

* Die Ressourcenebene gilt nur für ein Projekt. [!DNL Adobe Workfront] verwaltet Ressourcen nicht mehr als ein Projekt gleichzeitig.
* Wenn **[!UICONTROL Aufwandsorientiert]** wird als **[!UICONTROL Dauer Typ]**, [!DNL Workfront] wird die Ressourcen nicht ausdehnen.
* Wenn mehrere Benutzer derselben Aufgabe zugewiesen sind, wird die Einteilung abgebrochen.
* Bedingungen für den Typ **[!UICONTROL Aufgabenbegrenzung]** wird Vorrang vor der Ressourcenebene haben. Wenn beispielsweise **[!UICONTROL Feste Datumswerte]** wird als [!UICONTROL Aufgabenbegrenzung], ändert die Ressourcenebene die Aufgabendaten nicht.
* Vorläufige Beziehungen haben Vorrang vor der Ressourcenebene.
* **[!UICONTROL Ressourcenebene]** muss auf **[!UICONTROL Manuell]** für das Projekt zur Anpassung der Ebene in der [!UICONTROL Gantt-Diagramm]. Wenn Sie über Verwaltungsberechtigungen für das Projekt verfügen, können Sie die Ressourcen des Systems automatisch auf Ebene des Projekts platzieren, indem Sie diese Einstellung im Projekt anpassen und **[!UICONTROL Automatisch]** anstelle von **[!UICONTROL Manuell]** im **[!UICONTROL Projekt bearbeiten]** ankreuzen.

  ![](assets/resource-leveling-mode-350x177.png)

* Als Projekteigentümer oder Aufgabenverantwortlicher können Sie eine Zeitverzögerung für eine Aufgabe einführen, um anzuzeigen, dass eine große Wahrscheinlichkeit besteht, dass die Aufgabe möglicherweise mehr Zeit benötigt. Informationen zum Hinzufügen einer Zeitverzögerung zu einer Aufgabe finden Sie unter [Zeitverzögerung für Aufgabenebene aktualisieren](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Anwenden der Ressourcenebene in der [!UICONTROL Gantt-Diagramm]

Sie können die Aufgabenliste verwenden [!UICONTROL Gantt-Diagramm] , um Ressourcen zu sammeln.

1. Wechseln Sie zu dem Projekt, das Sie unterteilen möchten.
1. Im **[!UICONTROL Aufgaben]** Bereich, klicken Sie auf die **[!UICONTROL Gantt-Diagramm]** Symbol.

   Alle Änderungen werden automatisch gespeichert, wenn die Variable **[!UICONTROL Automatische Speicherung]** aktiviert ist. Sie ist standardmäßig aktiviert.

1. (Optional) Klicken Sie auf die **[!UICONTROL Plan] mode** Symbol und wählen Sie **[!UICONTROL Manuelles Speichern Standard]** oder **[!UICONTROL Timeline-Planung]** , um Ihre Änderungen manuell zu speichern.

   >[!TIP]
   >
   >Ressourcen können nicht in der  [!UICONTROL Gantt-Diagramm] wenn die [!UICONTROL Automatische Speicherung] aktiviert ist.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Klicken Sie auf **[!UICONTROL Level Resources]** Dropdown-Menü.

   ![Level_resources.png](assets/level-resouces.png)

1. Wählen Sie eine der folgenden Optionen aus:

   * **[!UICONTROL Level Now]**: Wendet die Ressourcenebene auf die ausgewählte Aufgabe an.
   * **[!UICONTROL Klare Ebene]**: Entfernt alle Ressourcenebenen aus der ausgewählten Aufgabe.

   >[!NOTE]
   >
   >Ihre Ressourcen werden möglicherweise überzugewiesen, wenn sie mehreren Aufgaben zugewiesen werden, die im selben Zeitrahmen stattfinden.

1. (Optional und bedingt) Wenn Sie die Option Automatisches Speichern deaktiviert haben, klicken Sie auf die **[!UICONTROL Rückgängig]** oder &#x200B;**[!UICONTROL Wiederholen]** -Symbole, wenn Sie eine der Änderungen abbrechen oder duplizieren möchten.

   >[!TIP]
   >
   >Sie können die folgenden Tastaturbefehle verwenden, um Änderungen an der [!UICONTROL Gantt-Diagramm]:
   >
   >* [!DNL Mac]: Verwenden Sie [!UICONTROL Befehl + Z] zum Rückgängigmachen und [!UICONTROL Befehl + Umschalt + Z] zurück.
   >* Windows: Verwenden Sie [!UICONTROL Strg + Z] zum Rückgängigmachen und [!UICONTROL Strg + Y] zurück.


1. Klicks **[!UICONTROL Speichern]** in der oberen rechten Ecke des [!UICONTROL Gantt-Diagramm].

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
