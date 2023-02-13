---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Erstellen einer agilen Geschichte in einer Iteration
description: In diesem Artikel wird beschrieben, wie Sie eine neue agile Geschichte erstellen, wenn Sie sich bereits in der Iteration befinden.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Erstellen einer agilen Geschichte in einer Iteration

In diesem Artikel wird beschrieben, wie Sie eine neue agile Geschichte erstellen, wenn Sie sich bereits in der Iteration befinden. Informationen zum Erstellen einer agilen Geschichte aus einer Aufgabe, einem Problem oder einem anderen Bereich von [!DNL Adobe Workfront], siehe [Hinzufügen von Meldungen zu einer vorhandenen Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Verwalten] Zugriff auf das Projekt, auf dem sich die Story befindet</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Erstellen einer agilen Geschichte in einer Iteration

1. Gehen Sie zur agilen Iteration, in der Sie die Geschichte erstellen möchten:

   1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe] Workfront, und klicken Sie dann auf **[!UICONTROL Teams]**.

   1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

   1. Wählen Sie im linken Bereich die Option **[!UICONTROL Iterationen]**.
   1. Klicken Sie auf den Namen der spezifischen Iteration, in der Sie eine Geschichte erstellen möchten.
   1. Wählen Sie im linken Bereich die Option **[!UICONTROL Meldungen]**.

1.  Klicken **[!UICONTROL Neue Geschichte].**
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
      <td>Wählen Sie diese Option aus, wenn die Story bereit ist, zu einer Iteration hinzugefügt zu werden. Wenn diese Option aktiviert ist, zeigt sie den Benutzern an, welche Meldungen im Backlog bereit sind, um zu einer Iteration hinzugefügt zu werden.<br>Eine Geschichte kann zu einer Iteration hinzugefügt werden, unabhängig davon, ob sie markiert ist oder nicht <strong>[!UICONTROL Bereit].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung] (Punkte)</strong></td>
      <td>Geben Sie die Schätzung für die Geschichte an. Wenn Ihr agile Team so konfiguriert ist, dass Geschichten in Punkten geschätzt werden, entspricht standardmäßig 1 Punkt 8 Stunden. Schätzungen werden in der Story als [!UICONTROL Planed Hours] hinzugefügt.<br>Wenn Sie beispielsweise eine Geschichte als 3 Punkte schätzen, wird standardmäßig die Meldung um 24 geplante Stunden erweitert.<br>Wenn eine Geschichte Unteraufgaben enthält, denken Sie daran, dass die kombinierten Schätzungen für alle Unteraufgaben die Schätzung der übergeordneten Meldung bestimmen. Weitere Informationen finden Sie unter <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Hinzufügen einer Unteraufgabe zu einer vorhandenen Geschichte auf der [!UICONTROL Scrum]-Pinnwand</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Übergeordnetes Projekt]</strong></td>
      <td>Beginnen Sie mit der Eingabe des Namens des Projekts, mit dem diese Geschichte verknüpft werden soll.<br>Standardmäßig wird die Story-Farbe als dieselbe Farbe wie andere Meldungen aus diesem Projekt angezeigt.<br>Der Status des Projekts muss auf [!UICONTROL Aktuell] eingestellt sein. Wenn der Projektstatus etwas Anderes als [!UICONTROL Aktuell] ist, wird er nicht im Dropdown-Menü angezeigt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Übergeordnete Aufgabe von [!UICONTROL]</strong></td>
      <td>Nachdem Sie ein übergeordnetes Projekt ausgewählt haben, können Sie eine übergeordnete Aufgabe auswählen. Wenn Sie eine übergeordnete Aufgabe auswählen, wird die Meldung als Unteraufgabe der übergeordneten Aufgabe des ausgewählten Projekts erstellt.<br>Beginnen Sie mit der Eingabe des Namens der übergeordneten Aufgabe für die Meldung und klicken Sie dann auf sie, wenn sie in der Dropdown-Liste angezeigt wird.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Benutzerdefinierter Forms]</strong></td>
      <td>Wählen Sie benutzerdefinierte Formulare aus, um sie dem Artikel hinzuzufügen.</td>
     </tr>
    </tbody>
   </table>

1. Klicken **[!UICONTROL Speichern von Meldungen]**.
