---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Erstellen einer Agile-Story
description: Sie können eine agile Story bei einer Iteration auf verschiedene Arten erstellen. Nachdem Sie eine Agile-Story erstellt haben, können Sie der Story Unteraufgaben hinzufügen.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# Erstellen einer agilen Story

Sie können eine agile Story bei einer Iteration auf verschiedene Arten erstellen. Nachdem Sie eine Agile-Story erstellt haben, können Sie der Story Unteraufgaben hinzufügen.

Wenn Sie eine Story oder eine Unteraufgabe in einer Iteration hinzufügen, wird der Dauertyp auf [!UICONTROL Einfach] und die Aufgabenbeschränkung auf Feste Datumswerte festgelegt, wobei die Datumswerte innerhalb der Iteration gesperrt sind. Sie können den Dauertyp oder die Aufgabenbeschränkung in einer Iteration nicht ändern. Außerdem muss die Aufgabendauer größer als 0 Minuten sein.

Informationen zum Verwalten der Story, nachdem sie der Iteration hinzugefügt wurde, finden Sie unter [Iterationen](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <p>Arbeit oder höher</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Zugriff auf das Projekt verwalten, an dem sich die Story befindet </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Agile-Story in einer Iteration

1. Wechseln Sie zur agilen Iteration, in der Sie die Story erstellen möchten:

   {{step1-to-team}}

   1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

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
      <td role="rowheader"><strong>[!UICONTROL bereit]</strong></td>
      <td>Wählen Sie diese Option, wenn die Story bereit zum Hinzufügen zu einer Iteration ist. Wenn diese Option ausgewählt ist, zeigt sie den Benutzenden an, welche Storys im Rückstand bereit zum Hinzufügen zu einer Iteration sind.<br>Eine Story kann zu einer Iteration hinzugefügt werden, unabhängig davon, ob sie <strong>[!UICONTROL Ready] markiert ist oder nicht.</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung] (Punkte)</strong></td>
      <td>Geben Sie den Schätzwert für die Story an. Wenn Ihr agiles Team so konfiguriert ist, dass Geschichten in Punkten geschätzt werden, entspricht standardmäßig 1 Punkt 8 Stunden. Die Schätzungen werden als [!UICONTROL Geplante Stunden] zur Story hinzugefügt.<br>Wenn Sie beispielsweise eine Story als 3 Punkte schätzen, fügt das Standardverhalten der Story 24 [!UICONTROL Geplante Stunden] hinzu.<br>Wenn eine Story Unteraufgaben enthält, denken Sie daran, dass die kombinierten Schätzungen für alle Unteraufgaben die Schätzung der übergeordneten Story bestimmen. Weitere Informationen finden Sie unter <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Hinzufügen von Storys zu einer vorhandenen Iteration</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Übergeordnetes Projekt]</strong></td>
      <td>Geben Sie den Namen des Projekts ein, mit dem diese Story verknüpft werden soll.<br>Standardmäßig wird die Farbe der Story mit derselben Farbe angezeigt wie bei anderen Stories aus diesem Projekt.<br>Der Status des Projekts muss auf [!UICONTROL Current] gesetzt werden. Wenn der Status des Projekts alles andere als [!UICONTROL Current] ist, wird er nicht im Dropdown-Menü angezeigt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Übergeordnete Aufgabe]</strong></td>
      <td>Nachdem Sie ein übergeordnetes Projekt ausgewählt haben, haben Sie die Möglichkeit, eine übergeordnete Aufgabe auszuwählen. Wenn Sie eine übergeordnete Aufgabe auswählen, wird die Story als Teilaufgabe der übergeordneten Aufgabe für das ausgewählte Projekt erstellt.<br>Beginnen Sie mit der Eingabe des Namens der übergeordneten Aufgabe für die Story und klicken Sie dann darauf, wenn sie in der Dropdown-Liste angezeigt wird.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Wählen Sie benutzerdefinierte Formulare aus, die der Story hinzugefügt werden sollen.</td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie **[!UICONTROL Story speichern]**.

## Erstellen einer Agile-Story im Auftragsbestand

Aus dem agilen Rückstand können Sie eine agile Story erstellen, wie im Abschnitt [Erstellen neuer Stories im Rückstand](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) im Artikel [[!UICONTROL Verwalten] des agilen Rückstands](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) beschrieben.

## Aufgabe oder Problem als agile Story hinzufügen

Sie können einer Iteration eine vorhandene Aufgabe oder ein vorhandenes Problem als Story hinzufügen. Weitere Informationen finden Sie unter [Hinzufügen von Storys zu einer vorhandenen Iteration](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) oder [Hinzufügen von Storys und Problemen vom [!UICONTROL Scrum]-Board](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Erstellen von Teilaufgaben in einer agilen Story

Sie können eine Unteraufgabe zu einer Agile-Story erstellen, indem Sie eine der folgenden Methoden verwenden:

* Verwenden Sie dazu die Registerkarte **[!UICONTROL Teilaufgaben]**, wie unter [Erstellen von Teilaufgaben](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [Erstellen von Teilaufgaben](../../manage-work/tasks/create-tasks/create-subtasks.md) beschrieben.

* Direkt über das Story Board, wie in [Erstellen einer Iteration](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) beschrieben.
