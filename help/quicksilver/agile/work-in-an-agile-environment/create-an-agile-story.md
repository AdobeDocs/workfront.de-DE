---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Erstellen einer Agile-Story
description: Sie können eine Agile-Story bei einer Iteration auf verschiedene Arten erstellen. Nachdem Sie eine Agile-Story erstellt haben, können Sie der Story Unteraufgaben hinzufügen.
author: Courtney
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 8%

---

# Erstellen einer Agile-Story

Sie können eine Agile-Story bei einer Iteration auf verschiedene Arten erstellen. Nachdem Sie eine Agile-Story erstellt haben, können Sie der Story Unteraufgaben hinzufügen.

Wenn Sie eine Story oder eine Unteraufgabe in einer Iteration hinzufügen, wird der Dauertyp auf [!UICONTROL Einfach] und die Aufgabenbeschränkung auf Feste Datumswerte festgelegt, wobei die Datumswerte innerhalb der Iteration gesperrt sind. Sie können den Dauertyp oder die Aufgabenbeschränkung in einer Iteration nicht ändern. Außerdem muss die Aufgabendauer größer als 0 Minuten sein.

Informationen zum Verwalten der Story, nachdem sie der Iteration hinzugefügt wurde, finden Sie unter [Iterationen](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Zugriff auf das Projekt verwalten, an dem sich die Story befindet </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Agile-Story in einer Iteration

1. Wechseln Sie zur agilen Iteration, in der Sie die Story erstellen möchten:

   {{step1-to-team}}

   1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

   1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]**, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
   1. Klicken Sie auf den Namen der spezifischen Iteration, für die Sie eine Story erstellen möchten.

   ![Neue Story zur Iteration hinzufügen](assets/iteration-stories-list.png)

1. Klicken Sie auf **[!UICONTROL Neue Story].**
1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story-Name]</strong></td>
      <td>Geben Sie einen Namen für die Story ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td>
      <td>Geben Sie eine Beschreibung für die Story ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Bereit]</strong></td>
      <td>Wählen Sie diese Option, wenn die Story bereit zum Hinzufügen zu einer Iteration ist. Wenn diese Option ausgewählt ist, zeigt sie den Benutzenden an, welche Storys im Rückstand bereit zum Hinzufügen zu einer Iteration sind.<br>Ein Story kann einer Iteration hinzugefügt werden, unabhängig davon, ob er als <strong>[!UICONTROL Ready] markiert ist.</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL-Schätzung] (Punkte)</strong></td>
      <td>Geben Sie die Schätzung für den Textabschnitt an. Wenn Ihr agiles Team so konfiguriert ist, dass Geschichten in Punkten geschätzt werden, entspricht standardmäßig 1 Punkt 8 Stunden. Die Schätzungen werden als [!UICONTROL Planned Hours] auf der Story hinzugefügt.<br>Wenn Sie beispielsweise einen Textabschnitt auf 3 Punkte schätzen, ist das Standardverhalten, der Textabschnitt um 24 [!UICONTROL Planned Hours] (Geplante Stunden) zu erweitern.<br>Wenn ein Textabschnitt Unteraufgaben enthält, denken Sie daran, dass die kombinierten Schätzungen für alle Unteraufgaben die Schätzung des übergeordneten Textabschnitts bestimmen. Weitere Informationen finden Sie unter <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Storys zu einer vorhandenen Iteration hinzufügen</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Übergeordnetes [!UICONTROL-Projekt]</strong></td>
      <td>Beginnen Sie mit der Eingabe des Namens des Projekts, dem diese Story zugeordnet werden soll.<br>Standardmäßig wird die Textabschnittsfarbe in derselben Farbe wie die anderen Textabschnitte aus diesem Projekt angezeigt.<br>Der Status des Projekts muss auf [!UICONTROL Current] festgelegt werden. Wenn der Status des Projekts etwas Anderes als [!UICONTROL Current] ist, wird er nicht im Dropdown-Menü angezeigt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Übergeordnete Aufgabe]</strong></td>
      <td>Nachdem Sie ein übergeordnetes Projekt ausgewählt haben, haben Sie die Möglichkeit, eine übergeordnete Aufgabe auszuwählen. Wenn Sie eine übergeordnete Aufgabe auswählen, wird die Story als Unteraufgabe der übergeordneten Aufgabe für das ausgewählte Projekt erstellt.<br>Beginnen Sie mit der Eingabe des Namens der übergeordneten Aufgabe für die Story und klicken Sie dann darauf, wenn sie in der Dropdown-Liste angezeigt wird.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Benutzerdefinierte Formulare]</strong></td>
      <td>Wählen Sie benutzerdefinierte Formulare aus, die der Story hinzugefügt werden sollen.</td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie **[!UICONTROL Story speichern]**.

## Erstellen einer Agile-Story im Auftragsbestand

Sie können eine Agile-Story aus dem Agile-Rückstand erstellen, wie im Abschnitt [Erstellen neuer Stories im Rückstand](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) im Artikel [[!UICONTROL Verwalten] des Agile-Rückstands](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) beschrieben.

## Aufgabe oder Problem als agile Story hinzufügen

Sie können einer Iteration eine vorhandene Aufgabe oder ein Problem als Story hinzufügen. Weitere Informationen finden Sie unter [Storys zu einer vorhandenen Iteration hinzufügen](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) oder [Storys und Probleme aus dem [!UICONTROL Scrum]-Board hinzufügen](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Agile Textabschnitte mit Unteraufgaben versehen

Sie können eine Unteraufgabe für eine agile Story mit einer der folgenden Methoden erstellen:

* Durch Verwendung der Registerkarte **[!UICONTROL Teilaufgaben]**, wie in [Teilaufgaben erstellen](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [Teilaufgaben erstellen](../../manage-work/tasks/create-tasks/create-subtasks.md) beschrieben.

* Direkt aus dem Storyboard, wie in [Erstellen einer Iteration](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) beschrieben.
