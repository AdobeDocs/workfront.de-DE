---
product-area: agile-and-teams
navigation-topic: burndown
title: Verwenden eines alternativen Teamzeitplans für Startdiagramme
description: Zeitpläne, die in [!DNL Adobe Workfront] definiert sind, wirken sich auf die Abbruchgrafik aus, indem Tage (Wochenenden und Feiertage) vom Abbruch ausgeschlossen werden.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Verwenden eines alternativen Teamzeitplans für Startdiagramme

Zeitpläne, die in [!DNL Adobe Workfront] definiert sind, wirken sich auf das Abbruchdiagramm aus, indem Tage (Wochenenden und Feiertage) aus dem Abriss ausgeschlossen werden.

Standardmäßig verwendet das Diagramm den Standardzeitplan. Zusätzlich zum Standardzeitplan können agile Teams auch einen alternativen Zeitplan verwenden, um Team-spezifische, nicht-arbeitstägliche Tage zu integrieren. Dieser alternative Zeitplan spiegelt sich dann in der Abbruchgrafik aller Iterationen wider, die dem Team zugewiesen sind. Der alternative Zeitplan wirkt sich nur auf das Diagramm aus. (Weitere Informationen zum Standardzeitplan sowie dazu, wie der [!DNL Workfront]-Administrator einen teamspezifischen Zeitplan erstellen kann, finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Die Abbruchgrafik berücksichtigt keine partiellen Tage. Wenn Ihr Team beispielsweise jeden Freitag 4 Stunden arbeitet, wird es in der Abbruchgrafik als vollständiger Tag dargestellt.

Weitere Informationen zur Verwendung des Burndown-Diagramms finden Sie in der [Übersicht über das Agile Burndown-Diagramm](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md) .

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
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um herauszufinden, welchen Plan oder welchen Lizenztyp Sie haben.

## Verwenden eines alternativen Teamzeitplans für Startdiagramme

1. Stellen Sie sicher, dass der [!DNL Workfront] -Administrator den alternativen Zeitplan bereits erstellt hat, wie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) beschrieben.
1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

1. Wählen Sie im Bereich **[!UICONTROL Agile]** im Bereich **[!UICONTROL Plan]** den neuen Zeitplan aus dem Dropdown-Menü aus.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
