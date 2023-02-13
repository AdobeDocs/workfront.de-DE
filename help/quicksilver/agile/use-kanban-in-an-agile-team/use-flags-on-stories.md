---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Verwenden Sie Flags auf Geschichten auf dem Kanban-Board
description: Im [!DNL Kanban] -Pinnwand und -Flags bieten einen visuellen Hinweis darauf, wann eine Geschichte bereit ist, zum nächsten Status zu wechseln. Dies ermöglicht Kanban-Teams, beim Verschieben von Geschichten über Status hinweg einen "Pull"-Ansatz anstelle eines "Push"-Ansatzes zu verwenden.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Verwenden Sie Flags für Meldungen auf [!UICONTROL Kanban] Pinnwand

Im [!DNL Kanban] -Pinnwand und -Flags bieten einen visuellen Hinweis darauf, wann eine Geschichte bereit ist, zum nächsten Status zu wechseln. Dies ermöglicht [!UICONTROL Kanban] Teams verwenden einen Pull-Ansatz anstelle eines Push-Ansatzes, wenn Geschichten über Status hinweg verschoben werden.

**Beispiel:** Betrachten Sie das folgende Beispiel eines Teams, das einen Pull-Ansatz verwendet: Olivia, der Grafikdesigner des Teams, beendet ihre Arbeit und setzt dann die Story-Markierung auf &quot;[!UICONTROL Bereit zum Abruf].&quot; Diese Fahne gibt Tony, dem Texter im Team, einen visuellen Hinweis, dass die Geschichte bereit ist, zum nächsten Status zu wechseln. Tony wechselt die Geschichte dann in den nächsten Status, wenn er bereit ist, damit zu beginnen.

Beachten Sie Folgendes bei der Verwendung von Flags für Meldungen:

* Flaggen sind kein Status, sondern ein visueller Hinweis darauf, dass die Geschichte bereit ist, von einem anderen Team in den nächsten Status versetzt zu werden.
* Flags werden nicht auf Storykarten angezeigt, die sich in der [!UICONTROL Rückstand] oder in der Spalte [!UICONTROL Fertig] Spalte (oder in einer Spalte, in der der Status der Spalte [!UICONTROL Fertig]).

   Weitere Informationen zum Status von Meldungen finden Sie unter [Verwenden Sie Flags auf Geschichten auf dem Kanban-Board](#updating-the-status-of-stories-and-subtasks)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Verwenden Sie Flags für Meldungen auf [!UICONTROL Kanban] Pinnwand

So ändern Sie eine Markierung für eine Geschichte:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder eine neue [!UICONTROL Kanban] Team aus dem Dropdown-Menü oder suchen Sie in der Suchleiste nach einem Team.

1. Navigieren Sie zu [!UICONTROL Kanban] Pinnwand, auf der Sie eine Markierung für eine Geschichte ändern möchten.
1. Erweitern Sie den Bereich Geschichte , um das Flag anzuzeigen.\
   Das Flag ist auf **[!UICONTROL Auf Tracking]** für jede Geschichte standardmäßig.\
   ![Kanban-Karte](assets/agile-storycard-kanban-2021-350x308.png)

1. Klicken Sie auf das aktuelle Flag und wählen Sie dann aus den folgenden Flag-Optionen aus:

   * **[!UICONTROL Auf Tracking]:** Die Geschichte befindet sich in einem geeigneten Status und es müssen derzeit keine Maßnahmen ergriffen werden.\

      Dies ist die Standardkennzeichnung für jede Geschichte auf dem Kanban-Board.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Ist blockiert]:** Die Geschichte kann nicht zum nächsten Status übergehen. Wenn diese Markierung auf eine Geschichte gesetzt ist, zählt die Geschichte nicht zur WIP-Grenze. (Weitere Informationen zu WIP-Beschränkungen finden Sie im Artikel [Kanban konfigurieren](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_block.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Bereit zum Abruf]:** Die Geschichte kann von einem anderen Team in den nächsten Status verschoben werden.\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
