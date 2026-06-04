---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Eine Agile-Story verschieben
description: Sie können eine Agile-Story entweder in eine andere Iteration (für Scrum-Teams) oder in den Rückstand (für Kanban- und Scrum-Teams) verschieben.
author: Courtney
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/gVEWRh4iiYdy6CwzLubaY3GZ4EE5C5diJ-RvsYFFtE4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 343
ht-degree: 11%

---

# Verschieben einer Agile-Story

Sie können eine Agile-Story entweder in eine andere Iteration (für Scrum-Teams) oder in den Rückstand (für Kanban- und Scrum-Teams) verschieben.

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
   <td>Zugriff auf die Story verwalten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Story aus einer Iteration oder Kanban-Pinnwand in den Rückstand verschieben

1. Gehen Sie zur Iteration oder zum Kanban-Board, das die Story enthält, die Sie in den Rückstand verschieben möchten.
1. Klicken Sie oben auf der Seite auf die Überschrift „Iteration“.
1. Wählen Sie auf **[!UICONTROL Registerkarte]** Storys“ die Storys aus, die Sie verschieben möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** > **[!UICONTROL Verschieben nach]**. Das **[!UICONTROL Verschieben nach]** wird angezeigt.

   ![Dialogfeld „Story verschieben“](assets/iteration-story-move.png)

1. Wählen Sie **Team_name&#39;s Backlog**. Im obigen Beispiel lautet der Name des Teams **Marketing**.

1. Klicken Sie **[!UICONTROL Verschieben]**.

## Story in eine andere Iteration verschieben

Sie können eine Story für Ihr Scrum-Team in eine andere Iteration verschieben, wenn Sie Systemadministrator oder Mitglied des Teams sind, mit dem die Iteration verknüpft ist.

>[!NOTE]
>
> Die **[!UICONTROL Verschieben nach]** ist nicht für übergeordnete Storys in einer Iteration verfügbar. Sie können Teilaufgaben nur in eine andere Iteration verschieben.


1. Wechseln Sie zur Iteration, die die Story enthält, die Sie verschieben möchten.
1. Klicken Sie oben auf der Seite auf die Überschrift „Iteration“.
1. Wählen Sie auf **[!UICONTROL Registerkarte]** Storys“ die Storys aus, die Sie verschieben möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** > **[!UICONTROL Verschieben nach]**. Das **[!UICONTROL Verschieben nach]** wird angezeigt.

   ![Dialogfeld „Story verschieben“](assets/iteration-story-move.png)

1. Wählen Sie **[!UICONTROL eine weitere Iteration]**.
1. Wählen Sie im angezeigten Dropdown-Menü die Iteration aus, in die Sie die Story verschieben möchten.

   >[!NOTE]
   >
   >Die Einstellungen [!UICONTROL  Arbeitselement ]Geplantes Startdatum) und [!UICONTROL Geplantes Abschlussdatum] werden von einer Einstellung auf der Seite [!UICONTROL Team bearbeiten] beeinflusst. Weitere Informationen finden Sie im Abschnitt [[!UICONTROL Konfigurieren], wie Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration angewendet werden](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) im Artikel [Konfigurieren von Scrum](../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

1. Klicken Sie **[!UICONTROL Verschieben]**.
