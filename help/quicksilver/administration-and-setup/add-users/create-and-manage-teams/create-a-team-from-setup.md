---
title: Erstellen eines Teams im Bereich „Setup“
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Als Adobe Workfront-Administrator können Sie im Bereich „Setup“ ein Team erstellen.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 8%

---

# Erstellen eines Teams im Bereich Setup

Als Adobe Workfront-Administrator können Sie im Bereich „Setup“ ein Team erstellen. Informationen zu Teams finden Sie unter [Teams - Übersicht](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Ein Gruppenadministrator bzw. eine Gruppenadministratorin kann im Bereich „Setup“ ein Team für eine von ihm bzw. ihr verwaltete Gruppe erstellen. Weitere Informationen finden Sie [Erstellen und Ändern der Teams einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Ein Benutzer mit einer Standard- oder Plan-Lizenz kann auch ein Team aus dem Bereich Teams erstellen. Weitere Informationen finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>ODER</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Teams

{{step-1-to-setup}}

1. Klicken Sie auf **Teams** und dann auf **Neues Team**.

1. Geben Sie im **Neues Team** angezeigten Feld die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Team-Name</td> 
      <td>Geben Sie einen Namen für das Team ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppe</td> 
      <td> <p>Wenn Sie das Team mit einer Gruppe verknüpfen möchten, geben Sie den Namen der Gruppe ein und wählen Sie den Namen aus, wenn er angezeigt wird.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol <img src="assets/info-icon.png"> neben dem Team klicken. Dadurch wird eine QuickInfo angezeigt, die Informationen über die Gruppe auflistet, wie z. B. die Hierarchie der darüber liegenden Gruppen und deren Administratoren.</p> <p><b>HINWEIS</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können alle Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied dieses Teams zu sein. Gruppenadministratoren können im Hauptmenü zum Bereich Teams gehen und auf den <img src="assets/switch-team-icon.png" alt="Team-Symbol wechseln"> Teams wechseln klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Team-Mitglieder</td> 
      <td> <p>Geben Sie den Namen eines Benutzers ein, der dem Team angehören soll, und wählen Sie dann den Namen aus, wenn in der Dropdown-Liste angezeigt wird. Wiederholen Sie diesen Vorgang, um dem Team mehrere Benutzer hinzuzufügen.</p> <p>Es gibt keine Begrenzung dafür, wie viele Benutzer Sie einem Team hinzufügen können. Wir empfehlen jedoch, nicht zu viele Benutzer in einem Team zu haben, da die Arbeitsverwaltung des Teams zu komplex werden kann.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Beschreibung für das Team eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kalender</td> 
      <td>Wählen Sie, welches Kalenderregister für dieses Team angezeigt wird.</td> 
     </tr> 
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Dies ist ein Agile-Team</td> 
      <td>Wählen Sie dieses Element aus, wenn Sie dieses neue Team als agiles Team konfigurieren möchten. Weitere Informationen zu Agile-Teams finden Sie unter <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines Agile-Teams</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bearbeiten</td> 
      <td>Schaltfläche „Bearbeiten“ in „Start“ ändern. Wenn ein(e) Benutzende(r) auf Start klickt, wird der Status des Elements automatisch aktualisiert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schaltfläche „Fertig“</td> 
      <td>Wählen Sie den Status aus, den Sie für Elemente festlegen möchten, wenn auf die Schaltfläche Fertig geklickt wird.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Team erstellen**.

## Teambesitzer

Wenn Sie ein Team erstellen, werden Sie standardmäßig zum Teambesitzer.

Sie können Teambesitzer für alle Teams anzeigen, wenn Sie einen Bericht für Teams erstellen, und das Feld „Name des Verantwortlichen“ in Ihren Bericht aufnehmen. (Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
