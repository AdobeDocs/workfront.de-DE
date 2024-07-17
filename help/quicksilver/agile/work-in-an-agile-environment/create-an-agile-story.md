---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Erstellen einer agilen Geschichte
description: Sie können auf verschiedene Weise eine agile Geschichte über eine Iteration erstellen. Nachdem Sie eine agile Geschichte erstellt haben, können Sie der Geschichte Unteraufgaben hinzufügen.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# Erstellen einer agilen Geschichte

Sie können auf verschiedene Weise eine agile Geschichte über eine Iteration erstellen. Nachdem Sie eine agile Geschichte erstellt haben, können Sie der Geschichte Unteraufgaben hinzufügen.

Wenn Sie eine Geschichte oder Unteraufgabe in einer Iteration hinzufügen, wird der Dauer-Typ auf [!UICONTROL Einfach] und die Aufgabenbegrenzung auf Feste Datumswerte gesetzt, wobei die Daten innerhalb der Iteration gesperrt sind. Sie können in einer Iteration weder den Duration Type noch die Task Constraint ändern. Außerdem muss die Dauer der Aufgabe größer als 0 Minuten sein.

Informationen zum Verwalten der Geschichte nach dem Hinzufügen zur Iteration finden Sie unter [Iterationen](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Verwalten] Zugriff auf das Projekt, auf dem sich die Story befindet</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen einer agilen Geschichte in einer Iteration

1. Gehen Sie zur agilen Iteration, in der Sie die Geschichte erstellen möchten:

   1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

   1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

   1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]** aus, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
   1. Klicken Sie auf den Namen der spezifischen Iteration, in der Sie eine Geschichte erstellen möchten.

   ![Neue Geschichte zur Iteration hinzufügen](assets/iteration-add-story.png)

1. Klicken Sie auf **[!UICONTROL New Story].**
1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Geben Sie einen Namen für die Geschichte ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td>
      <td>Geben Sie eine Beschreibung für die Geschichte ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Bereit]</strong></td>
      <td>Wählen Sie diese Option aus, wenn die Story bereit ist, zu einer Iteration hinzugefügt zu werden. Wenn diese Option aktiviert ist, zeigt sie den Benutzern an, welche Meldungen im Backlog bereit sind, um zu einer Iteration hinzugefügt zu werden.<br>Eine Geschichte kann zu einer Iteration hinzugefügt werden, unabhängig davon, ob sie <strong>[!UICONTROL Ready] markiert ist oder nicht.</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung] (Punkte)</strong></td>
      <td>Geben Sie die Schätzung für die Geschichte an. Wenn Ihr agile Team so konfiguriert ist, dass Geschichten in Punkten geschätzt werden, entspricht standardmäßig 1 Punkt 8 Stunden. Schätzungen werden in der Story als [!UICONTROL Planed Hours] hinzugefügt.<br>Wenn Sie beispielsweise eine Geschichte als 3 Punkte schätzen, wird standardmäßig 24 geplante [!UICONTROL Stunden] zur Geschichte hinzugefügt.<br>Wenn eine Geschichte Unteraufgaben enthält, denken Sie daran, dass die kombinierten Schätzungen für alle Unteraufgaben die Schätzung der übergeordneten Meldung bestimmen. Weitere Informationen finden Sie unter <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Meldungen zu einer vorhandenen Iteration hinzufügen</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Übergeordnetes Projekt]</strong></td>
      <td>Beginnen Sie mit der Eingabe des Namens des Projekts, mit dem diese Geschichte verknüpft werden soll.<br>Standardmäßig wird die Story-Farbe als dieselbe Farbe wie andere Meldungen aus diesem Projekt angezeigt.<br>Der Status des Projekts muss auf [!UICONTROL Aktuell] festgelegt sein. Wenn der Projektstatus etwas Anderes als [!UICONTROL Aktuell] ist, wird er nicht im Dropdown-Menü angezeigt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Übergeordnete Aufgabe von [!UICONTROL]</strong></td>
      <td>Nachdem Sie ein übergeordnetes Projekt ausgewählt haben, können Sie eine übergeordnete Aufgabe auswählen. Wenn Sie eine übergeordnete Aufgabe auswählen, wird die Meldung als Unteraufgabe der übergeordneten Aufgabe des ausgewählten Projekts erstellt.<br>Beginnen Sie mit der Eingabe des Namens der übergeordneten Aufgabe für die Geschichte und klicken Sie dann auf sie, wenn sie in der Dropdown-Liste angezeigt wird.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Wählen Sie benutzerdefinierte Formulare aus, um sie dem Artikel hinzuzufügen.</td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie auf **[!UICONTROL Geschichte speichern]**.

## Erstellen Sie einen agilen Artikel im Backlog.

Sie können einen agilen Artikel aus dem agilen Backlog erstellen, wie im Abschnitt [Erstellen neuer Meldungen im Backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) im Artikel [[!UICONTROL Verwalten] des agile Backlog](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) beschrieben.

## Hinzufügen einer Aufgabe oder eines Problems als agile Geschichte

Sie können eine vorhandene Aufgabe oder ein Problem als Geschichte zu einer Iteration hinzufügen. Weitere Informationen finden Sie unter [Meldungen zu einer vorhandenen Iteration hinzufügen](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) oder [Meldungen und Probleme aus der [!UICONTROL Scrum]-Pinnwand hinzufügen](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Erstellen von Unteraufgaben für einen agilen Verlauf

Sie können eine Unteraufgabe für eine agile Geschichte mit einer der folgenden Methoden erstellen:

* Verwenden Sie die Registerkarte **[!UICONTROL Unteraufgaben]**, wie in [Unteraufgaben erstellen](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [Unteraufgaben erstellen](../../manage-work/tasks/create-tasks/create-subtasks.md) beschrieben.

* Direkt vom Story-Forum aus, wie unter [Iteration erstellen](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) beschrieben.
