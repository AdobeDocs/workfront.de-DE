---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Flags für Storys im Kanban-Board verwenden
description: Auf dem  [!DNL Kanban]  bieten Flags einen visuellen Hinweis darauf, wann eine Story bereit ist, zum nächsten Status zu wechseln. Dadurch können Kanban-Teams beim Verschieben von Storys über Status hinweg einen „Pull“-Ansatz anstelle eines „Push“-Ansatzes verwenden.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Flags auf Storys auf dem Kanban[!UICONTROL Board ]

Auf der [!DNL Kanban] bieten Flags einen visuellen Hinweis darauf, wann eine Story bereit ist, zum nächsten Status zu wechseln. Dadurch können [!UICONTROL Kanban]-Teams beim Verschieben von Storys über Status hinweg einen „Pull“-Ansatz anstelle eines „Push“-Ansatzes verwenden.

**Beispiel:** Betrachten Sie das folgende Beispiel eines Teams, das einen „Pull“-Ansatz verwendet: Olivia, die Grafikdesignerin im Team, beendet ihre Arbeit und setzt dann das Story-Flag auf &quot;[!UICONTROL Ready to Pull].“ Diese Flagge gibt Tony, dem Texter im Team, einen visuellen Hinweis darauf, dass die Geschichte bereit ist, zum nächsten Status zu wechseln. Tony bewegt die Geschichte dann in den nächsten Status, wenn er bereit ist, mit der Arbeit daran zu beginnen.

Beachten Sie Folgendes, wenn Sie -Flags für Storys verwenden:

* Markierungen sind kein Status, sondern ein visueller Hinweis darauf, dass die Story bereit ist, von einem anderen Team-Mitglied in den nächsten Status verschoben zu werden.
* Flags werden nicht auf Story-Karten angezeigt, die sich in der Spalte [!UICONTROL Rückstand] oder in der Spalte [!UICONTROL Fertigstellen] (oder in einer Spalte, in der der Status der Spalte mit [!UICONTROL Fertigstellen] entspricht) befinden.

  Weitere Informationen über den Status von Storys finden Sie unter [Verwenden von Flags auf Storys auf dem Kanban-Board](#updating-the-status-of-stories-and-subtasks)

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
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Flags auf Storys auf dem Kanban[!UICONTROL Board ]

So ändern Sie eine Markierung für eine Story:

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues [!UICONTROL Kanban]-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wechseln Sie zum [!UICONTROL Kanban]-Board, auf dem Sie eine Markierung für eine Story ändern möchten.
1. Erweitern Sie die Story-Kachel, um die Markierung anzuzeigen.
Die Markierung ist standardmäßig auf **[!UICONTROL Auf Kurs]** für jede Story festgelegt.
   ![Kanban-Karte](assets/agile-storycard-kanban-2021-350x308.png)

1. Klicken Sie auf die aktuelle Markierung und wählen Sie dann eine der folgenden Markierungsoptionen aus:

   * **[!UICONTROL Auf Kurs]:** Die Story befindet sich im entsprechenden Status und es müssen derzeit keine Maßnahmen ergriffen werden.

     Dies ist die Standardmarkierung für jede Story auf dem Kanban-Board.
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Ist blockiert]:** Die Story kann nicht mit dem nächsten Status fortfahren. Wenn diese Markierung für eine Story gesetzt wird, zählt die Story nicht zum WIP-Limit. (Weitere Informationen zu Fertigstellungsbeschränkungen finden Sie im Artikel [Konfigurieren von ](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)).

     ![kanban_flag_block.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Bereit zum ]:** Die Story kann von einem anderen Teammitglied in den nächsten Status verschoben werden.

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
