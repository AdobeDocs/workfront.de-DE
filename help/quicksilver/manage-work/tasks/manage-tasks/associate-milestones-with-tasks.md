---
product-area: projects
navigation-topic: manage-tasks
title: Verknüpfen von Meilensteinen mit Aufgaben
description: Sie können Meilensteine mit Aufgaben verknüpfen, um anzugeben, wann Sie während der Lebensdauer des Projekts wichtige Schritte erreichen.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Verknüpfen von Meilensteinen mit Aufgaben

Sie können Meilensteine mit Aufgaben verknüpfen, um anzugeben, wann Sie während der Lebensdauer des Projekts wichtige Schritte erreichen.

## Zugriffsanforderungen

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
  <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgabe verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie einen Meilenstein mit einer Aufgabe verknüpfen können, muss Folgendes vorhanden sein:

* Der Workfront-Administrator muss einen Meilensteinpfad erstellen, wie unter [Meilensteinpfad erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Um einen Meilensteinpfad mit einem Projekt zu verknüpfen, muss sich das Projekt im Status Planung oder Aktuell befinden.

>[!TIP]
>
>Um mithilfe der Milestone-Ansicht den bestmöglichen Überblick über den Fortschritt von Meilensteinen in Ihren Projekten zu erhalten, sollten Sie übergeordnete Aufgaben erstellen und sie mit jeder Hauptphase Ihres Projekts verknüpfen. Verknüpfen Sie dann diese übergeordneten Aufgaben mit jedem der Meilensteine Ihres Meilensteinpfads.

## Zuweisen eines Meilensteins zu einer Aufgabe

1. Wechseln Sie zu einem Projekt und klicken Sie dann auf das **Mehr** icon ![](assets/more-icon.png), dann **Bearbeiten**.
1. Verwenden der **Einstellungen** festlegen, legen Sie den Meilensteinpfad fest, der für das Projekt verwendet werden soll.
1. Klicken Sie auf **Speichern**.

   Nachdem ein Meilensteinpfad mit einem Projekt verknüpft wurde, kann Aufgaben ein Meilenstein zugewiesen werden.

1. Wechseln Sie zu einer Aufgabe und klicken Sie auf die Schaltfläche **Mehr** icon ![](assets/more-icon.png), dann **Bearbeiten**.

   Aufgaben und Meilensteine haben eine 1:1-Beziehung. Sie können nicht denselben Meilenstein an mehrere Aufgaben anhängen. Jede Aufgabe kann mit einem einzigen Meilenstein verknüpft werden oder jeder Meilenstein kann einer Aufgabe zugeordnet werden.

1. Klicken **Einstellungen** und wählen Sie dann einen Meilenstein in der **Milestone** -Feld für die Aufgabe.
1. Klicken **Speichern**.
1. (Optional) Fügen Sie in einer Liste von Aufgaben die **Statussymbole** -Spalte, um zu ermitteln, welche Aufgaben Meilensteine aufweisen.

   ![](assets/amwt3.png)

1. (Optional) Wählen Sie in einer Liste von Projekten die **Milestone** anzeigen, um den Fortschritt Ihrer Meilensteinaufgaben zu ermitteln.

   ![screen_shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)
