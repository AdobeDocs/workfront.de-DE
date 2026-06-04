---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Arbeits- und Teamanfragen verwalten
description: Eine Anfrage stellt eine ausstehende Aufgaben- oder Problemzuweisung dar. Arbeitsanfragen werden an Einzelpersonen und Teamanfragen an Teams gesendet.
author: Courtney
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/h9ebMyu8AQNPQTzfYkEMbEbHtghIj-wegaml3cM3RMY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: be65ef36-43e4-48e1-a062-caa3778e15beid: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 488
ht-degree: 9%

---

# Verwalten von Arbeits- und Team-Anfragen

Eine Anfrage stellt eine ausstehende Aufgaben- oder Problemzuweisung dar. Arbeitsanfragen werden an Einzelpersonen und Teamanfragen an Teams gesendet.

>[!NOTE]
>
>Agile-Teams haben keine Teamanfragen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>So weisen Sie eine Anforderung zu oder bearbeiten sie:
   <p>Licht oder höher</p>
  <p>Überprüfen oder höher</p>
   <p>So weisen Sie eine Anfrage neu zu:
   <p>Standard</p>
   <p>Work oder höher</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anforderung einem Team zuweisen {#assign-a-request-to-a-team}

Projektmanager und Problemanfragende können Teams Arbeit zuweisen, wenn sie nicht wissen, welche Ressource die richtige für die Arbeit ist, oder wenn es unerheblich ist, wer die Arbeit abschließt.

Aufgaben, die dem Team zugewiesen wurden, bleiben auf der Registerkarte [!UICONTROL Teamanfragen], bis ein(e) Benutzende(r) im Team die Anfrage freiwillig bearbeitet.

Wenn eine Anfrage sowohl einem Team als auch einem Benutzer zugewiesen wird, der nicht zum Team gehört, ist die Anfrage sowohl auf der Registerkarte [!UICONTROL Team-Anfragen] als auch im Bereich für Arbeitsanfragen des Benutzers sichtbar. Wenn der/die Benutzende, der/die nicht zum Team gehört, freiwillig an der Aufgabe arbeitet, bleibt die Aufgabe weiterhin auf der Registerkarte [!UICONTROL Team-Anfragen], bis ein(e) Benutzende(r) im Team die Aufgabe freiwillig übernimmt.

Teams können auf eine der folgenden Arten Aufgaben und Problemen zugewiesen werden:

* Über das [!UICONTROL Gantt-Diagramm]
* Aus einer Aufgaben- oder Problemliste (einzeln oder in großen Mengen)
* Wenn eine Aufgabe oder ein Problem erstellt oder geändert wird
* Durch Routing-Regeln für eine Anfrage (nur Probleme)

Sie können eine Anforderung manuell einem Team über die Seite „Team“ zuweisen, wie in diesem Abschnitt beschrieben.

So weisen Sie einem Team manuell eine Anforderung über die Seite „Team“ zu:

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Klicken Sie auf das **[!UICONTROL Mehr]**-Symbol ![](assets/more-icon.png) und wählen Sie dann **[!UICONTROL Arbeitsauftrag senden]** aus.

   ![](assets/edit-team-settings-350x205.png)

1. Füllen Sie die Informationen in das sich öffnende Feld ein.
1. Klicken Sie **[!UICONTROL Anfrage senden]**.\
   Dem Team wird jetzt eine neue Aufgabe zugewiesen, die auf der Registerkarte Team-Anfragen angezeigt wird. Diese Aufgabe ist derzeit keinem Projekt zugeordnet, kann jedoch verschoben werden, wie unter [Aufgaben verschieben](../../manage-work/tasks/manage-tasks/move-tasks.md) beschrieben.

## Anforderungen neu zuweisen {#reassign-requests}

Sie können Anfragen, die Ihrem Team zugewiesen wurden, neu zuweisen:

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Navigationsbereich die Option **[!UICONTROL Teamanfragen]** aus.
1. Klicken Sie auf **[!UICONTROL Symbol „Neu zuweisen]**.

1. Geben Sie den Namen des Benutzers, der Gruppe oder des Teams ein, dem bzw. dem Sie die Anfrage neu zuweisen möchten, und klicken Sie dann auf **[!UICONTROL Zuweisen]**.\
   Die Anfrage wurde neu zugewiesen.
