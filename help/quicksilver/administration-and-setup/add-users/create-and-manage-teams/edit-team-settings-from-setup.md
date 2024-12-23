---
title: Bearbeiten der Einstellungen eines Teams im Setup-Bereich
description: Als Adobe Workfront-Administrator können Sie die Einstellungen eines Teams im Bereich Einrichtung bearbeiten. Sie können Benutzer zu einem Team hinzufügen, die Layoutvorlage eines Teams festlegen und festlegen, wie der Status aufgezeichnet wird, wenn Arbeitselemente von einem Team abgeschlossen werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 6409f8fa5072413444545d2d3a80935dc6e04b4c
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 3%

---

# Bearbeiten Sie die Einstellungen eines Teams im Bereich &quot;Einrichtung&quot;.

Als Adobe Workfront-Administrator können Sie die Einstellungen eines Teams im Bereich Einrichtung bearbeiten. Sie können Benutzer zu einem Team hinzufügen, die Layoutvorlage eines Teams festlegen und festlegen, wie der Status aufgezeichnet wird, wenn Arbeitselemente von einem Team abgeschlossen werden.

Weitere Informationen zu Teams finden Sie unter [Übersicht über Teams](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Ein Gruppenadministrator kann die Einstellungen eines Teams für eine von ihm verwaltete Gruppe bearbeiten. Weitere Informationen finden Sie unter [Erstellen und Ändern von Teams einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Benutzer mit einer Standard- oder Planlizenz können die Einstellungen eines Teams im Bereich Teams bearbeiten. Weitere Informationen finden Sie unter [Bearbeiten von Teameinstellungen](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
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
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Team-Einstellungen bearbeiten

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Teams** .
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
       <td>Diese Option ist standardmäßig für neue und vorhandene Teams aktiviert. Deaktivieren Sie ihn, um das Team zu deaktivieren. Weitere Informationen finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Deaktivieren eines Teams</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Gruppe</td> 
      <td> <p>Verbinden Sie das Team mit einer Gruppe. Geben Sie den Namen der Gruppe ein und wählen Sie den Namen aus, wenn er angezeigt wird.</p> <p><b>HINWEIS</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied zu sein. Gruppenadministratoren können im Hauptmenü den Bereich Teams aufrufen und auf den Pfeil "Switch Teams"<img src="assets/switch-team-icon.png" alt="Symbol &quot;Team wechseln&quot;"> klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol "<img src="assets/info-icon.png">" klicken, das neben der Gruppe angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Besitzerin bzw. Besitzer</td> 
      <td>Wählen Sie einen Inhaber für das Team aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Team-Mitglieder</td> 
      <td> <p>Fügen Sie Mitglieder und Teams hinzu. Beginnen Sie mit der Eingabe des Namens eines Benutzers und wählen Sie dann den Namen aus, wenn er angezeigt wird. Wiederholen Sie diesen Vorgang, um mehrere Benutzer zum Team hinzuzufügen.</p> 
      <p><b>TIPP</b>: Sie können einer Gruppe eine beliebige Anzahl von Benutzern hinzufügen. Es wird jedoch empfohlen, in einem Team keine übermäßig große Anzahl hinzuzufügen, da das Arbeitsmanagement des Teams zu komplex werden könnte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie eine Beschreibung für das Team ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Layoutvorlage</td> 
      <td> <p>Beginnen Sie mit der Eingabe des Namens der Layoutvorlage, die das Team verwenden soll, und klicken Sie dann darauf, sobald sie angezeigt wird.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Geben Sie an, ob es sich um ein agiles Team handelt. Weitere Informationen zu agile Teams und zur Verwaltung ihrer Arbeit finden Sie unter <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines agilen Teams</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Bearbeiten</td> 
      <td> <p>Ändern Sie die Schaltfläche "Bearbeiten"in die Schaltfläche "Starten". Wenn ein Benutzer auf Start klickt, wird der Status des Elements automatisch aktualisiert.</p> <p>Weitere Informationen zum Konfigurieren der Schaltfläche "Start"finden Sie unter <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche "Work On It"durch eine Schaltfläche "Start"</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schaltfläche „Fertig“</td> 
      <td> <p>Passen Sie die Schaltfläche Fertig an. Weitere Informationen finden Sie unter</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Konfigurieren der Schaltfläche "Fertig"für Aufgaben</a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Konfigurieren der Schaltfläche "Fertig"für Probleme</a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Änderungen speichern**.
