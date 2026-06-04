---
content-type: reference
navigation-topic: boards
title: Agile-Team-Kanban-Karten zu Workfront-Boards migrieren
description: Sie können Ihre Arbeitselemente von einem Agile-Team-Kanban-Board auf ein neues oder vorhandenes Workfront-Board migrieren.
author: Courtney
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/RXk7PYF6JsdF71pRVwEA-Wk23h-UqbgLPXSyNR7VX5Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 360
ht-degree: 11%

---

# Migrieren von Agile-Team-Kanban-Karten zu Pinnwänden in Workfront

Sie können Ihre Arbeitselemente von einem Agile-Team-Kanban-Board auf ein neues oder vorhandenes Workfront-Board migrieren. Wenn Sie die Migration ausführen, werden alle Karten auf der Kanban-Pinnwand in die Workfront-Pinnwand kopiert. Es ist nicht erlaubt, bestimmte Karten auszuwählen.

Die Platzierung von Karten auf der Workfront-Pinnwand basiert auf Spaltenrichtlinien. (Eine Richtlinie kann beispielsweise alle Karten mit dem Status „In Bearbeitung“ in eine bestimmte Spalte verschieben. Weitere Informationen zu Spaltenrichtlinien finden Sie unter [Verwalten von ](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)). Wenn keine Richtlinien vorhanden sind oder die Karten nicht mit den Richtlinien übereinstimmen, werden die Karten in der Spalte ganz links auf der Pinnwand platziert. Derzeit werden die Karten in der Spalte „Rückstand“ auf der alten Pinnwand nicht zur Workfront-Pinnwand hinzugefügt.

Die Karten werden nicht aus dem Agile-Team-Kanban-Board entfernt und Kartenstatusänderungen werden mit beiden Boards synchronisiert. Sie können beide Pinnwände aktiviert lassen, bis Sie bereit sind, zu Workfront-Pinnwänden zu wechseln.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Kanban-Karten auf eine neue Pinnwand migrieren

{{step1-to-team}}

1. Zugriff auf ein Kanban-Board.
1. Klicken Sie auf [!UICONTROL **Zu Pinnwänden hinzufügen**] und wählen Sie [!UICONTROL **Neue Pinnwand**] aus.
1. Geben Sie im [!UICONTROL Zu neuer Pinnwand hinzufügen] einen Namen für die neue Pinnwand ein (der Name der aktuellen [!UICONTROL Kanban]-Pinnwand wird automatisch angezeigt) und klicken Sie auf [!UICONTROL **Hinzufügen**].

   ![Kanban-Karten zu neuer Pinnwand hinzufügen](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Optional) Klicken Sie auf der angezeigten Erfolgsmeldung auf den Link, um das neue Board zu öffnen.

## Kanban-Karten zu einer vorhandenen Pinnwand migrieren

{{step1-to-team}}

1. Zugriff auf ein Kanban-Board.
1. Klicken Sie auf [!UICONTROL **Zu Pinnwänden hinzufügen**] und wählen Sie &quot;[!UICONTROL **Pinnwand“**].
1. Suchen Sie im Dialogfeld [!UICONTROL Zu vorhandener Pinnwand hinzufügen] nach der Pinnwand, auf die die Karten migriert werden sollen, und wählen Sie diese aus. Klicken Sie dann auf [!UICONTROL **Hinzufügen**].

   ![Kanban-Karten zu vorhandener Pinnwand hinzufügen](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Optional) Klicken Sie auf der angezeigten Erfolgsmeldung auf den Link, um das Board zu öffnen.
