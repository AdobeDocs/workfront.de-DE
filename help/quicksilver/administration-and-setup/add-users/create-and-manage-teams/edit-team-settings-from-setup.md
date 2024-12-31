---
title: Bearbeiten der Einstellungen eines Teams im Bereich „Setup“
description: Als Adobe Workfront-Administrator können Sie die Einstellungen eines Teams im Bereich „Setup“ bearbeiten. Sie können Benutzer zu einem Team hinzufügen, die Layout-Vorlage eines Teams festlegen und festlegen, wie der Status aufgezeichnet wird, wenn Arbeitselemente von einem Team abgeschlossen werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 6409f8fa5072413444545d2d3a80935dc6e04b4c
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 3%

---

# Bearbeiten der Einstellungen eines Teams im Bereich Setup

Als Adobe Workfront-Administrator können Sie die Einstellungen eines Teams im Bereich „Setup“ bearbeiten. Sie können Benutzer zu einem Team hinzufügen, die Layout-Vorlage eines Teams festlegen und festlegen, wie der Status aufgezeichnet wird, wenn Arbeitselemente von einem Team abgeschlossen werden.

Informationen zu Teams finden Sie unter [Teams - Übersicht](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Ein Gruppenadministrator bzw. eine Gruppenadministratorin kann die Einstellungen eines Teams für eine von ihm verwaltete Gruppe bearbeiten. Weitere Informationen finden Sie [Erstellen und Ändern der Teams einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Ein Benutzer mit einer Standard- oder Plan-Lizenz kann die Einstellungen eines Teams im Bereich Teams bearbeiten. Weitere Informationen finden Sie unter [Teameinstellungen bearbeiten](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
       <p>Oder</p>
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

## Bearbeiten der Einstellungen eines Teams

{{step-1-to-setup}}

1. Klicken Sie **linken** auf „Teams“.
1. Wählen Sie ein Team aus und klicken Sie dann auf **Bearbeiten** ![](assets/edit-icon.png).

1. Nehmen Sie eine der folgenden Änderungen vor:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Team-Name</td> 
      <td>Geben Sie einen Namen für das Team ein.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Ist aktiv </td> 
       <td>Diese Option ist standardmäßig für neue und vorhandene Teams aktiviert. Deaktivieren, um das Team zu deaktivieren. Weitere Informationen finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Team deaktivieren</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Gruppe</td> 
      <td> <p>Verknüpfen Sie das Team mit einer Gruppe. Beginnen Sie mit der Eingabe des Namens der Gruppe und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> <p><b>HINWEIS</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können alle Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied dieses Teams zu sein. Gruppenadministratoren können im Hauptmenü zum Bereich Teams gehen und auf den <img src="assets/switch-team-icon.png" alt="Team-Symbol wechseln"> Teams wechseln klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol <img src="assets/info-icon.png"> neben dem Team klicken. Dadurch wird eine QuickInfo angezeigt, die Informationen über die Gruppe auflistet, wie z. B. die Hierarchie der darüber liegenden Gruppen und deren Administratoren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Besitzerin bzw. Besitzer</td> 
      <td>Wählen Sie einen Verantwortlichen für das Team aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Team-Mitglieder</td> 
      <td> <p>Fügen Sie und Ihre Team-Mitglieder hinzu. Beginnen Sie mit der Eingabe des Benutzernamens und wählen Sie den Namen aus, wenn er angezeigt wird. Wiederholen Sie diesen Vorgang, um dem Team mehrere Benutzer hinzuzufügen.</p> 
      <p><b>TIPP</b>: Sie können einem Team eine beliebige Anzahl von Benutzern hinzufügen. Es wird jedoch empfohlen, nicht zu viele Teammitglieder hinzuzufügen, da die Arbeitsverwaltung des Teams zu komplex werden könnte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Beschreibung für das Team eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Layoutvorlage</td> 
      <td> <p>Geben Sie den Namen der Layout-Vorlage ein, die das Team verwenden soll, und klicken Sie auf den Namen, wenn er angezeigt wird.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Geben Sie an, ob es sich um ein Agile-Team handelt. Informationen zu agilen Teams und zur Verwaltung ihrer Arbeit finden Sie unter <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines agilen Teams</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. Klicken Sie auf **Änderungen speichern**.
