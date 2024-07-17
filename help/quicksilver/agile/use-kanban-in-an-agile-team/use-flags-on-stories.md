---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Verwenden Sie Flags auf Geschichten auf dem Kanban-Board
description: Auf der  [!DNL Kanban] Pinnwand bieten Flags einen visuellen Hinweis darauf, wann eine Geschichte bereit ist, zum nächsten Status zu wechseln. Dies ermöglicht Kanban-Teams, beim Verschieben von Geschichten über Status hinweg einen "Pull"-Ansatz anstelle eines "Push"-Ansatzes zu verwenden.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Verwenden Sie Flags auf Meldungen auf der [!UICONTROL Kanban]-Pinnwand

Auf der [!DNL Kanban]-Pinnwand bieten Flags einen visuellen Hinweis darauf, wann eine Geschichte bereit ist, zum nächsten Status zu wechseln. Dadurch können [!UICONTROL Kanban]-Teams beim Verschieben von Geschichten über Status hinweg einen Pull-Ansatz anstelle eines Push-Ansatzes verwenden.

**Beispiel:** Betrachten Sie das folgende Beispiel eines Teams, das einen Pull-Ansatz verwendet: Olivia, der Grafikdesigner im Team, beendet ihre Arbeit und setzt dann die Story-Markierung auf &quot;[!UICONTROL Bereit zum Pull]&quot;. Diese Fahne gibt Tony, dem Texter im Team, einen visuellen Hinweis, dass die Geschichte bereit ist, zum nächsten Status zu wechseln. Tony wechselt die Geschichte dann in den nächsten Status, wenn er bereit ist, damit zu beginnen.

Beachten Sie Folgendes bei der Verwendung von Flags für Meldungen:

* Flaggen sind kein Status, sondern ein visueller Hinweis darauf, dass die Geschichte bereit ist, von einem anderen Team in den nächsten Status versetzt zu werden.
* Flags werden nicht auf Storykarten angezeigt, die sich in der Spalte [!UICONTROL Rückprotokoll] oder in der Spalte [!UICONTROL Abgeschlossen] befinden (oder in einer Spalte, in der der Status der Spalte mit [!UICONTROL Abgeschlossen] übereinstimmt).

  Weitere Informationen zum Status von Meldungen finden Sie unter [Verwenden von Flags auf Geschichten auf der Kanban-Pinnwand](#updating-the-status-of-stories-and-subtasks)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Verwenden Sie Flags auf Meldungen auf der [!UICONTROL Kanban]-Pinnwand

So ändern Sie eine Markierung für eine Geschichte:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues [!UICONTROL Kanban]-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Gehen Sie zur [!UICONTROL Kanban]-Pinnwand, an der Sie eine Markierung für eine Geschichte ändern möchten.
1. Erweitern Sie den Bereich Geschichte , um das Flag anzuzeigen.\
   Die Markierung ist für jede Geschichte standardmäßig auf **[!UICONTROL Auf Track]** gesetzt.\
   ![Kanban-Karte](assets/agile-storycard-kanban-2021-350x308.png)

1. Klicken Sie auf die aktuelle Markierung und wählen Sie dann aus den folgenden Optionen aus:

   * **[!UICONTROL Auf Track]:** Die Meldung befindet sich im entsprechenden Status und es müssen derzeit keine Maßnahmen ergriffen werden.\

     Dies ist die Standardkennzeichnung für jede Geschichte auf dem Kanban-Board.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Ist blockiert]:** Die Meldung kann nicht zum nächsten Status übergehen. Wenn diese Markierung auf eine Geschichte gesetzt ist, zählt die Geschichte nicht zur WIP-Grenze. (Weitere Informationen zu WIP-Beschränkungen finden Sie im Artikel [Kanban konfigurieren](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

     ![kanban_flag_block.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Bereit zum Ziehen]:** Die Geschichte kann von einem anderen Team-Mitglied in den nächsten Status verschoben werden.\

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
