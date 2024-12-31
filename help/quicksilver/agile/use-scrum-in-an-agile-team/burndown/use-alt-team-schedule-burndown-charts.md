---
product-area: agile-and-teams
navigation-topic: burndown
title: Verwenden eines alternativen Team-Zeitplans für Burndown-Diagramme
description: Zeitpläne, die in definiert sind [!DNL Adobe Workfront]  wirken sich auf das Burndown-Diagramm aus, indem sie Urlaubstage (Wochenenden und Feiertage) vom Burndown ausschließen.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Verwenden eines alternativen Team-Zeitplans für Burndown-Diagramme

Zeitpläne, die in definiert sind, [!DNL Adobe Workfront] sich auf das Burndown-Diagramm auswirken, indem sie Urlaubstage (Wochenenden und Feiertage) vom Burndown ausschließen.

Standardmäßig verwendet das Burndown-Diagramm den Standardzeitplan. Zusätzlich zum Standardzeitplan können Agile-Teams auch einen alternativen Zeitplan verwenden, um teamspezifische arbeitsfreie Tage einzubinden. Dieser alternative Zeitplan wird dann im Burndown-Diagramm jeder Iteration angezeigt, die dem Team zugewiesen ist. Der alternative Zeitplan wirkt sich nur auf das Burndown-Diagramm aus. (Weitere Informationen zum Standardzeitplan sowie dazu, wie der [!DNL Workfront] einen teamspezifischen Zeitplan erstellen kann, finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Das Burndown-Diagramm berücksichtigt keine partiellen Tage. Wenn Ihr Team beispielsweise jeden Freitag 4 Stunden arbeitet, wird dies im Burndown-Diagramm als ganzer Tag dargestellt.

Weitere Informationen zur Verwendung des Burndown-Diagramms finden Sie unter [Agile Burndown-Diagramm - Übersicht](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Work] oder höher</p> </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verwenden eines alternativen Team-Zeitplans für Burndown-Diagramme

1. Stellen Sie sicher, dass der [!DNL Workfront]-Administrator den alternativen Zeitplan bereits erstellt hat, wie in [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) beschrieben.

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Agile-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

1. Wählen Sie **[!UICONTROL Abschnitt]** im Bereich **[!UICONTROL Zeitplan]** den neuen Zeitplan aus dem Dropdown-Menü aus.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
