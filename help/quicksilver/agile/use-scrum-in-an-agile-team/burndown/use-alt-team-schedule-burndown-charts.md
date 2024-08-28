---
product-area: agile-and-teams
navigation-topic: burndown
title: Verwenden eines alternativen Team-Zeitplans für Niederschlagskarten
description: Zeitpläne, die in [!DNL Adobe Workfront] definiert sind, wirken sich auf die Abbruchgrafik aus, indem Tage (Wochenenden und Feiertage) vom Abbruch ausgeschlossen werden.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Verwenden eines alternativen Teamzeitplans für Startdiagramme

Zeitpläne, die in [!DNL Adobe Workfront] definiert sind, wirken sich auf das Abbruchdiagramm aus, indem Tage (Wochenenden und Feiertage) aus dem Abriss ausgeschlossen werden.

Standardmäßig verwendet das Diagramm den Standardzeitplan. Zusätzlich zum Standardzeitplan können agile Teams auch einen alternativen Zeitplan verwenden, um Team-spezifische, nicht-arbeitstägliche Tage zu integrieren. Dieser alternative Zeitplan spiegelt sich dann in der Abbruchgrafik aller Iterationen wider, die dem Team zugewiesen sind. Der alternative Zeitplan wirkt sich nur auf das Diagramm aus. (Weitere Informationen zum Standardzeitplan sowie dazu, wie der [!DNL Workfront]-Administrator einen teamspezifischen Zeitplan erstellen kann, finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Die Abbruchgrafik berücksichtigt keine partiellen Tage. Wenn Ihr Team beispielsweise jeden Freitag 4 Stunden arbeitet, wird es in der Abbruchgrafik als vollständiger Tag dargestellt.

Weitere Informationen zur Verwendung des Burndown-Diagramms finden Sie in der [Übersicht über das Agile Burndown-Diagramm](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md) .

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verwenden eines alternativen Teamzeitplans für Startdiagramme

1. Stellen Sie sicher, dass der [!DNL Workfront] -Administrator den alternativen Zeitplan bereits erstellt hat, wie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) beschrieben.

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das agile Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

1. Wählen Sie im Bereich **[!UICONTROL Agile]** im Bereich **[!UICONTROL Plan]** den neuen Zeitplan aus dem Dropdown-Menü aus.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
