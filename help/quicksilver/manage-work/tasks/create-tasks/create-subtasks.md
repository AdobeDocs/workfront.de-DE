---
product-area: projects
navigation-topic: create-tasks
title: Teilaufgaben erstellen
description: In Adobe Workfront können Aufgaben über hierarchische Beziehungen verfügen. Untergeordnete Aufgaben werden als Teilaufgaben bezeichnet. Sie können Teilaufgaben in der Aufgabenliste erstellen, indem Sie eine Hauptaufgabe zu einer Teilaufgabe machen. Sie können eine Teilaufgabe auch zu einer Hauptaufgabe machen.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 3%

---

# Teilaufgaben erstellen

<!-- Audited: 01/2025 -->

In Adobe Workfront können Aufgaben über hierarchische Beziehungen verfügen. Untergeordnete Aufgaben werden als Teilaufgaben bezeichnet. Sie können Teilaufgaben in der Aufgabenliste erstellen, indem Sie eine Hauptaufgabe zu einer Teilaufgabe einer anderen Aufgabe machen. Sie können eine Teilaufgabe auch zu einer Hauptaufgabe machen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt mit der Möglichkeit zum Hinzufügen von Aufgaben oder höher hinzufügen</p> 
   <p>Wenn Sie eine Aufgabe erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für die Aufgabe</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project and the parent task with ability to Add Tasks or higher</p> <p>You automatically receive Manage permissions to the task after you create it.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Teilaufgaben erstellen

Sie können Teilaufgaben aus der Aufgabenliste oder dem Abschnitt Teilaufgaben erstellen.

>[!TIP]
>
>Das Erstellen von Teilaufgaben für ein Projekt ähnelt dem Erstellen von Vorlagenteilaufgaben zu Vorlagenaufgaben in einer Vorlage.


### Erstellen von Teilaufgaben aus der Aufgabenliste {#create-subtasks-from-the-task-list}

1. Wechseln Sie zu dem Projekt, in dem Sie Teilaufgaben erstellen möchten.
1. Klicken Sie auf **Abschnitt** Aufgaben“ im linken Bereich.
1. (Bedingt) Wenn sich die Aufgabe, die Sie als untergeordnete Aufgabe festlegen möchten, nicht bereits direkt unter der Aufgabe befindet, die Sie als übergeordnete Aufgabe festlegen möchten, ziehen Sie sie per Drag-and-Drop an die entsprechende Position in der Aufgabenliste.
1. Wählen Sie die Aufgabe aus, die Sie zu einer Teilaufgabe machen möchten, und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Einrückungssymbol** ![Einrückungssymbol](assets/indent-icon-nwe-33x29.png), um die ausgewählte Aufgabe zu einer Unteraufgabe für die Aufgabe direkt darüber zu machen.
   * Wenn Sie eine standardmäßige englische QWERTY-Tastatur verwenden, drücken Sie Wahltaste + > (Mac) oder Alt + > (Windows) auf der Tastatur. In anderen Sprachen können Sie die Befehle + , (Mac) oder Alt + , (Windows) zum Einrücken verwenden.

     >[!TIP]
     >
     >Die Tastaturbefehle funktionieren nicht, wenn Sie Aufgaben im Inline-Bearbeitungsmodus bearbeiten. Verwenden Sie in diesem Fall das Einrückungssymbol ![Einrückungssymbol](assets/indent-icon-nwe-33x29.png) um Teilaufgaben zu erstellen.

   * Ziehen Sie die Aufgabe per Drag-and-Drop auf die Aufgabe, die Sie als übergeordnete Aufgabe festlegen möchten.

     >[!NOTE]
     >
     >Aufgaben können nur dann eingezogen werden, wenn die Aufgabenliste nach Aufgabennummer sortiert ist und auf die Aufgabenliste keine Gruppierungen angewendet wurden.

### Erstellen von Teilaufgaben aus dem Abschnitt „Aufgaben-Teilaufgaben“ {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>Der Workfront- oder Gruppenadministrator kann den Abschnitt Teilaufgaben in der Umgebung mithilfe einer Layout-Vorlage entfernen.

1. Wechseln Sie zu dem Projekt, in dem Sie Teilaufgaben erstellen möchten.
1. Klicken Sie auf **Abschnitt** Aufgaben“ im linken Bereich.
1. Klicken Sie auf den Namen der Aufgabe, für die Sie eine Unteraufgabe erstellen möchten.
1. Klicken Sie auf **Abschnitt** Teilaufgaben“ im linken Bedienfeld, falls verfügbar.
1. Klicken Sie auf **Neue Aufgabe.**

   Informationen zum Erstellen von Aufgaben finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Klicken Sie auf **Aufgabe erstellen.**

   Die neue Aufgabe wird als Teilaufgabe zu der in Schritt 3 ausgewählten Aufgabe erstellt. <!--ensure this is accurate-->

## Teilaufgabe zu einer Hauptaufgabe machen

1. Wechseln Sie zu dem Projekt, in dem eine Teilaufgabe zu einer Hauptaufgabe gemacht werden soll.
1. Klicken Sie auf **Abschnitt** Aufgaben“ im linken Bereich.
1. Wählen Sie die Teilaufgabe aus, die Sie zu einer Hauptaufgabe machen möchten.
1. Klicken Sie auf **Ausrücken**-Symbol ![Ausrücken](assets/outdent-icon-nwe-31x29.png), um die Unteraufgabe zu einer Hauptaufgabe zu machen.

   ODER

   Drücken Sie auf einer standardmäßigen englischen QWERTY-Tastatur die Wahltaste + &lt; (Mac) oder Alt + &lt; (Windows). Andere Sprachen können die Befehle Option + verwenden. (Mac) oder Alt + . (Windows) zum Ausrücken.

   >[!NOTE]
   >
   >Sie können Aufgaben nur dann ausrücken, wenn die Aufgabenliste nach Aufgabennummer sortiert ist und wenn auf die Aufgabenliste keine Gruppierungen angewendet werden.
