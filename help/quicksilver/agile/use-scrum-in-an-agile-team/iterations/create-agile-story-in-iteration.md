---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Erstellen einer Agile-Story in einer Iteration
description: In diesem Artikel wird beschrieben, wie Sie eine neue Agile-Story erstellen, wenn Sie sich bereits in der Iteration befinden.
author: Jenny
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 4%

---

# Erstellen einer Agile-Story in einer Iteration

In diesem Artikel wird beschrieben, wie Sie eine neue Agile-Story erstellen, wenn Sie sich bereits in der Iteration befinden. Informationen zum Erstellen einer Agile-Story aus einer Aufgabe, einem Problem oder einem anderen [!DNL Adobe Workfront] finden Sie unter [Hinzufügen von Stories zu einer vorhandenen Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Agile-Story in einer Iteration

1. Wechseln Sie zur agilen Iteration, in der Sie die Story erstellen möchten:

   {{step1-to-team}}

   1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

   1. Wählen Sie im linken Bedienfeld **[!UICONTROL Iterationen]** aus.
   1. Klicken Sie auf den Namen der spezifischen Iteration, für die Sie eine Story erstellen möchten.
   1. Wählen Sie im linken Bereich die Option **[!UICONTROL Storys]** aus.

1.  Klicken Sie auf **[!UICONTROL Neue Story]**.
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
      <td>Geben Sie den Schätzwert für die Story an. Wenn Ihr agiles Team so konfiguriert ist, dass Geschichten in Punkten geschätzt werden, entspricht standardmäßig 1 Punkt 8 Stunden. Die Schätzungen werden als [!UICONTROL Geplante Stunden] zur Story hinzugefügt.<br>Wenn Sie beispielsweise eine Story als 3 Punkte schätzen, fügt das Standardverhalten der Story 24 geplante Stunden hinzu.<br>Wenn eine Story Unteraufgaben enthält, denken Sie daran, dass die kombinierten Schätzungen für alle Unteraufgaben die Schätzung der übergeordneten Story bestimmen. Weitere Informationen finden Sie unter <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Hinzufügen einer Unteraufgabe zu einer vorhandenen Story auf dem [!UICONTROL Scrum]-Board</a>.</td>
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
