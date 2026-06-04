---
product-area: agile-and-teams
navigation-topic: burndown
title: Verwenden eines alternativen Team-Zeitplans für Burndown-Diagramme
description: Zeitpläne, die in definiert sind [!DNL Adobe Workfront]  wirken sich auf das Burndown-Diagramm aus, indem sie Urlaubstage (Wochenenden und Feiertage) vom Burndown ausschließen.
author: Courtney
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/BWnnytUMaoygpGpDdjQ5dmdBZrR1IWAu7onkwVizvUc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 16%

---

# Verwenden eines alternativen Team-Zeitplans für Burndown-Diagramme

Zeitpläne, die in definiert sind, [!DNL Adobe Workfront] sich auf das Burndown-Diagramm auswirken, indem sie Urlaubstage (Wochenenden und Feiertage) vom Burndown ausschließen.

Standardmäßig verwendet das Burndown-Diagramm den Standardzeitplan. Zusätzlich zum Standardzeitplan können Agile-Teams auch einen alternativen Zeitplan verwenden, um teamspezifische arbeitsfreie Tage einzubinden. Dieser alternative Zeitplan wird dann im Burndown-Diagramm jeder Iteration angezeigt, die dem Team zugewiesen ist. Der alternative Zeitplan wirkt sich nur auf das Burndown-Diagramm aus. (Weitere Informationen zum Standardzeitplan sowie dazu, wie der [!DNL Workfront] einen teamspezifischen Zeitplan erstellen kann, finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Das Burndown-Diagramm berücksichtigt keine partiellen Tage. Wenn Ihr Team beispielsweise jeden Freitag 4 Stunden arbeitet, wird dies im Burndown-Diagramm als ganzer Tag dargestellt.

Weitere Informationen zur Verwendung des Burndown-Diagramms finden Sie unter [Agile Burndown-Diagramm - Übersicht](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

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
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Verwenden eines alternativen Team-Zeitplans für Burndown-Diagramme

1. Stellen Sie sicher, dass der [!DNL Workfront]-Administrator den alternativen Zeitplan bereits erstellt hat, wie in [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) beschrieben.

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Agile-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

1. Wählen Sie **[!UICONTROL Abschnitt]** im Bereich **[!UICONTROL Zeitplan]** den neuen Zeitplan aus dem Dropdown-Menü aus.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
