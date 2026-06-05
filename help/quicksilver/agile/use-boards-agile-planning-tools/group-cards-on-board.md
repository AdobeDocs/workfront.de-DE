---
filename: group-cards-on-board
content-type: reference
navigation-topic: boards
title: Verwenden von Gruppen auf einem Board
description: Sie können Karten auf einer Pinnwand nach Verantwortlichem oder nach Tag gruppieren. Wenn Sie eine Option auswählen, nach der gruppiert werden soll, werden die Karten im SWMLANE-Format angezeigt.
author: Courtney
feature: Agile
exl-id: 6f57a20e-0e47-4457-8605-9bce55c013ec
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/SYKTSJJD64mValoUAfcz-bnHTj-AaKDQ7dSjAEweM0s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 317
ht-degree: 12%

---

# Verwenden von Gruppen auf einer Pinnwand

Sie können Karten auf einer Pinnwand nach Verantwortlichem oder nach Tag gruppieren. Wenn Sie eine Option auswählen, nach der gruppiert werden soll, werden die Karten im SWMLANE-Format angezeigt. Nicht zugewiesene Karten oder Karten ohne Tags werden in ihrem eigenen Swimlane angezeigt.

>[!NOTE]
>
>Alle Karten in der Aufnahmespalte sind nicht in einer Gruppe enthalten, und die Aufnahmespalte wird ausgeblendet, wenn eine Gruppe angewendet wird. Weitere Informationen zur Aufnahmespalte finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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

## Gruppieren von Karten auf einer Pinnwand

{{step1-to-boards}}

1. Zugriff auf eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie **[!UICONTROL Gruppe]**, um das Bedienfeld „Gruppe“ auf der linken Seite der Pinnwand zu öffnen.

   >[!NOTE]
   >
   >Die Standardeinstellung zum Gruppieren nach ist **[!UICONTROL Keine]**. Sie können diese Option jederzeit auswählen, um eine Gruppe zu entfernen und nur die Spalten auf der Pinnwand anzuzeigen.

1. Um die Karten zu gruppieren, wählen Sie **[!UICONTROL Verantwortliche]** oder **[!UICONTROL Tags]** aus.

   Die Karten werden automatisch gruppiert. Klicken Sie auf den Pfeil neben dem Gruppennamen, um die Gruppe zu reduzieren und zu erweitern.

   ![Gruppierte Karten auf einer Pinnwand](assets/group-by-assignee.png)

1. Auswählen, was passiert, wenn eine Karte in eine andere Gruppe verschoben wird.

   * **[!UICONTROL Bei Verantwortlichen hinzufügen]/[!UICONTROL Bei Tags hinzufügen]:** Die Verantwortlichen oder Tags in der neuen Gruppe werden der vorhandenen Liste der Verantwortlichen oder Tags auf der Karte hinzugefügt.
   * **[!UICONTROL Verantwortliche überschreiben]/[!UICONTROL Tags überschreiben]:** Die Verantwortlichen oder Tags in der neuen Gruppe überschreiben alle anderen Verantwortlichen oder Tags und werden die einzigen Verantwortlichen oder Tags auf der Karte.

   ![[!UICONTROL Gruppieren nach Optionen]](assets/group-by-rail.png)

1. Klicken Sie **[!UICONTROL Gruppen ausblenden]**, um das Gruppenbedienfeld auszublenden und die Vollpension anzuzeigen.
