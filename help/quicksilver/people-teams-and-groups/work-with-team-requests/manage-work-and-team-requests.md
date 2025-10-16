---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Arbeits- und Teamanfragen verwalten
description: Eine Anfrage stellt eine ausstehende Aufgaben- oder Problemzuweisung dar. Arbeitsanfragen werden an Einzelpersonen und Teamanfragen an Teams gesendet.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: dd47158a4c2e1b7372af6c9450b2d277d1ca8c6f
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Arbeits- und Teamanfragen verwalten

Eine Anfrage stellt eine ausstehende Aufgaben- oder Problemzuweisung dar. Arbeitsanfragen werden an Einzelpersonen und Teamanfragen an Teams gesendet.

>[!NOTE]
>
>Agile-Teams haben keine Teamanfragen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <p>Arbeit oder höher</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
