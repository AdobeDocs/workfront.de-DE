---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Erstellen und Ändern der Teams einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit Teams arbeiten, die mit der Gruppe und ihren Untergruppen verknüpft sind.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 3%

---

# Erstellen und Ändern der Teams einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit Teams arbeiten, die mit der Gruppe und ihren Untergruppen verknüpft sind.

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Informationen dazu, wie Benutzer mit Planlizenz ein Team erstellen können, finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Informationen dazu, wie ein Workfront-Administrator ein Team erstellen kann, finden Sie unter [Erstellen eines Teams im Bereich „Setup“](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">einem Benutzer uneingeschränkten Administratorzugriff gewähren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie wissen möchten, über welchen Plan oder Lizenztyp Sie verfügen.

+++

## Im Bereich Gruppen können Sie Teams für Ihre Gruppe anzeigen, mit ihnen arbeiten und sie erstellen

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie Teams erstellen oder ändern möchten.
1. Klicken Sie im linken Bereich auf **Teams** ![](assets/teams.png) , um die mit der Gruppe und etwaigen Untergruppen verknüpften Teams aufzulisten.

1. Führen Sie einen der folgenden Schritte aus:

   * **Team hinzufügen**: Klicken Sie auf **Neues Team** und konfigurieren Sie es dann mit den folgenden Optionen:

   <!-- WRITER please check table below. I stripped out wonky conditions-->

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
       <td> <p> Das System füllt das Feld Gruppe für das neue Team mit der Gruppe aus, die Sie anzeigen. Wenn Sie das Team mit einer anderen Gruppe verknüpfen möchten, geben Sie den Namen der Gruppe ein und wählen Sie den Namen aus, wenn er angezeigt wird.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol <img src="assets/info-icon.png"> neben dem Team klicken. Dadurch wird eine QuickInfo angezeigt, die Informationen über die Gruppe auflistet, wie z. B. die Hierarchie der darüber liegenden Gruppen und deren Administratoren.</p> <p><b>HINWEIS</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können alle Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied dieses Teams zu sein. Gruppenadministratoren können im Hauptmenü zum Bereich Teams gehen und auf den <img src="assets/switch-team-icon.png" alt="Team-Symbol wechseln"> Teams wechseln klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
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

   * **Teams bearbeiten**: Wählen Sie mindestens ein Team aus, klicken Sie auf **das** Bearbeiten ![](assets/edit-icon.png) und verwenden Sie dann die folgenden Optionen, um es zu konfigurieren:

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
       <td> <p>Verknüpfen Sie das Team mit einer Gruppe. Beginnen Sie mit der Eingabe des Namens der Gruppe und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol <img src="assets/info-icon.png"> neben dem Team klicken. Dadurch wird eine QuickInfo angezeigt, die Informationen über die Gruppe auflistet, wie z. B. die Hierarchie der darüber liegenden Gruppen und deren Administratoren.</p> <p><b>HINWEIS</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können alle Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied dieses Teams zu sein. Gruppenadministratoren können im Hauptmenü zum Bereich Teams gehen und auf den <img src="assets/switch-team-icon.png" alt="Team-Symbol wechseln"> Teams wechseln klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Besitzerin bzw. Besitzer</td> 
       <td>Wählen Sie einen Verantwortlichen für das Team aus.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Team-Mitglieder</td> 
       <td> <p>Fügen Sie und Ihre Team-Mitglieder hinzu. Beginnen Sie mit der Eingabe des Benutzernamens und wählen Sie den Namen aus, wenn er angezeigt wird. Wiederholen Sie diesen Vorgang, um dem Team mehrere Benutzer hinzuzufügen.</p> <p><b>TIPP</b>: Es gibt keine Begrenzung dafür, wie viele Benutzer Sie einem Team hinzufügen können. Wir empfehlen jedoch, nicht zu viele Benutzer in einem Team zu haben, da die Arbeitsverwaltung des Teams zu komplex werden kann.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Beschreibung</td> 
       <td>Beschreibung für das Team eingeben.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Layoutvorlage</td> 
       <td> <p>Geben Sie den Namen der Layout-Vorlage ein, die das Team verwenden soll, und klicken Sie auf den Namen, wenn er angezeigt wird.</p> <p>Wenn Sie das Team mit dieser Layout-Vorlage als Home-Team der Benutzer festlegen, sehen alle Benutzer in diesem Team die Anpassungen in dieser Layout-Vorlage.<br>Ihre individuellen Layoutvorlageneinstellungen setzen die Einstellungen der Layoutvorlage „Home-Team“ außer Kraft. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Geben Sie an, ob es sich um ein Agile-Team handelt. Informationen zu agilen Teams und zur Verwaltung ihrer Arbeit finden Sie unter <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines agilen Teams</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Bearbeiten</td> 
       <td> <p>Schaltfläche „Bearbeiten“ in „Start“ ändern. Wenn ein(e) Benutzende(r) auf Start klickt, wird der Status des Elements automatisch aktualisiert.</p> <p>Weitere Informationen zum Konfigurieren der Schaltfläche „Start“ finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Starten“</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Schaltfläche „Fertig“</td> 
       <td> <p>Passen Sie die Schaltfläche Fertig an. Weitere Informationen finden Sie unter:</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Konfigurieren der Schaltfläche „Fertig“ für Aufgaben</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Konfigurieren der Schaltfläche „Fertig“ für Probleme</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **Teams löschen**: Wählen Sie mindestens ein Team aus und klicken Sie dann auf das Symbol Löschen ![](assets/delete.png).
   * **Teamliste exportieren**: Klicken Sie auf **Exportieren** ![](assets/export.png) und wählen Sie dann das Dateiformat für die exportierte Liste aus.
