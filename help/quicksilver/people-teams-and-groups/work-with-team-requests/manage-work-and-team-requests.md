---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Verwalten von Arbeits- und Team-Anforderungen
description: Eine Anfrage stellt eine ausstehende Aufgabe oder Problemzuweisung dar. Arbeitsanfragen werden an Einzelpersonen gesendet und Team-Anfragen werden an Teams gesendet.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Verwalten von Arbeits- und Teamanfragen

Eine Anfrage stellt eine ausstehende Aufgabe oder Problemzuweisung dar. Arbeitsanfragen werden an Einzelpersonen gesendet und Team-Anfragen werden an Teams gesendet.

>[!NOTE]
>
>Agile Teams verfügen nicht über Teamanfragen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>So weisen Sie eine Anforderung zu oder bearbeiten sie sie:
   <p>Neu: Licht oder höher</br>
    oder</br>
   Aktuell: Überprüfen oder höher</p>
   <p>So weisen Sie eine Anforderung erneut zu:
   <p>Neu: Standard</br>
    oder</br>
   Aktuell: Arbeit oder höher</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zuweisen einer Anforderung zu einem Team {#assign-a-request-to-a-team}

Projektmanager und Problemanfragen können Teams Arbeit zuweisen, wenn sie nicht wissen, welche Ressource für die Arbeit geeignet ist oder wenn es nicht wichtig ist, wer die Arbeit abschließt.

Die dem Team zugewiesenen Aufgaben verbleiben auf der Registerkarte [!UICONTROL Team-Anforderungen] , bis ein Benutzer des Teams sich bereit erklärt, an der Anfrage zu arbeiten.

Wenn eine Anforderung sowohl einem Team als auch einem Benutzer zugewiesen wird, der nicht Mitglied des Teams ist, ist die Anforderung sowohl auf der Registerkarte [!UICONTROL Team-Anforderungen] als auch im Arbeitsanforderungsbereich des Benutzers sichtbar. Wenn der Benutzer, der nicht im Team ist, sich bereit erklärt, an der Aufgabe zu arbeiten, bleibt die Aufgabe auf der Registerkarte [!UICONTROL Team-Anforderungen], bis ein Benutzer des Teams sich bereit erklärt, daran zu arbeiten.

Teams können Aufgaben und Problemen auf eine der folgenden Arten zugewiesen werden:

* Durch das [!UICONTROL Gantt-Diagramm]
* Über eine Aufgaben- oder Problemliste (einzeln oder in Stapeln)
* Wenn eine Aufgabe oder ein Problem erstellt oder geändert wird
* Über Routing-Regeln für eine Anfrage (nur Probleme)

Sie können eine Anforderung manuell über die Team-Seite einem Team zuweisen, wie in diesem Abschnitt beschrieben.

So weisen Sie einem Team manuell über die Team-Seite eine Anforderung zu:

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Klicken Sie auf das Symbol **[!UICONTROL Mehr]** ![](assets/more-icon.png) und wählen Sie dann **[!UICONTROL Arbeitserfordernis senden]** aus.

   ![](assets/edit-team-settings-350x205.png)

1. Füllen Sie die Informationen in dem sich öffnenden Feld aus.
1. Klicken Sie auf **[!UICONTROL Anfrage senden]**.\
   Dem Team wird nun eine neue Aufgabe zugewiesen, die auf der Registerkarte Team-Anforderungen angezeigt wird. Diese Aufgabe ist derzeit nicht mit einem Projekt verknüpft, kann jedoch verschoben werden, wie unter [Aufgaben verschieben](../../manage-work/tasks/manage-tasks/move-tasks.md) beschrieben.

## Anforderungen neu zuweisen {#reassign-requests}

Sie können Anforderungen, die Ihrem Team zugewiesen wurden, neu zuweisen:

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie im linken Navigationsbereich **[!UICONTROL Team Requests]** aus.
1. Klicken Sie auf das Symbol **[!UICONTROL Neu zuweisen]** .

1. Beginnen Sie mit der Eingabe des Namens des Benutzers, der Gruppe oder des Teams, dem Sie die Anforderung neu zuweisen möchten, und klicken Sie dann auf **[!UICONTROL Zuweisen]**.\
   Die Anfrage wird neu zugewiesen.
