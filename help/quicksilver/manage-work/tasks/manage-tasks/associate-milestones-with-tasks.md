---
product-area: projects
navigation-topic: manage-tasks
title: Verknüpfen von Meilensteinen mit Aufgaben
description: Sie können Meilensteine mit Aufgaben verknüpfen, um anzugeben, wann Sie während der Lebensdauer des Projekts wichtige Schritte erreichen. Sie müssen einen Meilensteinpfad mit einem Projekt verknüpfen, bevor Sie Meilensteine mit Aufgaben im Projekt verknüpfen können.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Verknüpfen von Meilensteinen mit Aufgaben

<!--Audited: 01/2024-->

Sie können Meilensteine mit Aufgaben verknüpfen, um anzugeben, wann Sie während der Lebensdauer des Projekts wichtige Schritte erreichen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neue Lizenz: Standard</p> 
   <p>Aktuelle Lizenz: Arbeite oder höher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgabe verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Voraussetzungen

Bevor Sie einen Meilenstein mit einer Aufgabe verknüpfen können, muss Folgendes vorhanden sein:

* Der Workfront-Administrator muss einen Meilensteinpfad erstellen, wie unter [Meilensteinpfad erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) beschrieben.

* Sie müssen einem Projekt einen Meilensteinpfad zuweisen.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Um einen Meilensteinpfad mit einem Projekt zu verknüpfen, muss sich das Projekt im Status Planung oder Aktuell befinden.

  >[!TIP]
  >
  >Um mithilfe der Milestone-Ansicht den bestmöglichen Überblick über den Fortschritt von Meilensteinen in Ihren Projekten zu erhalten, sollten Sie übergeordnete Aufgaben erstellen und sie mit jeder Hauptphase Ihres Projekts verknüpfen. Verknüpfen Sie dann diese übergeordneten Aufgaben mit jedem der Meilensteine Ihres Meilensteinpfads.

## Zuweisen eines Meilensteins zu einer Aufgabe

Nachdem ein Meilensteinpfad mit einem Projekt verknüpft wurde, kann Aufgaben ein Meilenstein zugewiesen werden.

1. Wechseln Sie zu einer Aufgabe, klicken Sie auf das Symbol **Mehr** ![](assets/more-icon.png) rechts neben dem Aufgabennamen und dann auf **Bearbeiten**.

   Aufgaben und Meilensteine haben eine 1:1-Beziehung. Sie können nicht denselben Meilenstein an mehrere Aufgaben anhängen. Jede Aufgabe kann mit einem einzigen Meilenstein verknüpft werden oder jeder Meilenstein kann einer Aufgabe zugeordnet werden.

1. Klicken Sie auf **Einstellungen** und wählen Sie dann einen Meilenstein im Feld **Meilenstein** für die Aufgabe aus.
1. Klicken Sie auf **Speichern**.
1. (Optional) Fügen Sie in einer Aufgabenliste die Spalte **Statussymbole** hinzu, um zu ermitteln, welche Aufgaben Meilensteine aufweisen. Der Meilensteindiamantenindikator wird in der Spalte Statussymbole angezeigt.

   Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![](assets/amwt3.png)

1. (Optional) Markieren Sie in einer Liste von Projekten die Ansicht **Milestone** , um den Fortschritt Ihrer Meilensteinaufgaben zu ermitteln.

   ![](assets/milestone-view-project-list.png)
