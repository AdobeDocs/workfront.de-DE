---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Erstellen einer Agile-Geschichte in einer Iteration
description: In diesem Artikel wird beschrieben, wie Sie eine neue agile Geschichte erstellen, wenn Sie sich bereits in der Iteration befinden.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Erstellen einer agilen Geschichte in einer Iteration

In diesem Artikel wird beschrieben, wie Sie eine neue agile Geschichte erstellen, wenn Sie sich bereits in der Iteration befinden. Informationen zum Erstellen eines agilen Verlaufs aus einer Aufgabe, einem Problem oder einem anderen Bereich von [!DNL Adobe Workfront] finden Sie unter [Hinzufügen von Geschichten zu einer vorhandenen Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>[!UICONTROL Verwalten] Zugriff auf das Projekt, auf dem sich die Story befindet </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer agilen Geschichte in einer Iteration

1. Gehen Sie zur agilen Iteration, in der Sie die Geschichte erstellen möchten:

   {{step1-to-team}}

   1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

   1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]** aus.
   1. Klicken Sie auf den Namen der spezifischen Iteration, in der Sie eine Geschichte erstellen möchten.
   1. Wählen Sie im linken Bereich **[!UICONTROL Meldungen]** aus.

1.  Klicken Sie auf **[!UICONTROL Neue Meldung]**.
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
      <td>Geben Sie die Schätzung für die Geschichte an. Wenn Ihr agile Team so konfiguriert ist, dass Geschichten in Punkten geschätzt werden, entspricht standardmäßig 1 Punkt 8 Stunden. Schätzungen werden in der Story als [!UICONTROL Planed Hours] hinzugefügt.<br>Wenn Sie z. B. eine Geschichte als 3 Punkte schätzen, besteht das Standardverhalten darin, der Meldung 24 geplante Stunden hinzuzufügen.<br>Wenn eine Geschichte Unteraufgaben enthält, denken Sie daran, dass die kombinierten Schätzungen für alle Unteraufgaben die Schätzung der übergeordneten Meldung bestimmen. Weitere Informationen finden Sie unter <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Hinzufügen einer Unteraufgabe zu einer bestehenden Meldung auf der [!UICONTROL Scrum]-Pinnwand</a>.</td>
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
