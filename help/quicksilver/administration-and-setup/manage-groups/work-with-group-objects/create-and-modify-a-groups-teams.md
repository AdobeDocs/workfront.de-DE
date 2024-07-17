---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Erstellen und Ändern von Teams einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die mit der Gruppe und ihren Untergruppen verknüpften Teams anzeigen und mit ihnen arbeiten.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 6f9eddd46430990e11d5d661ea09f0595a9acebc
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# Erstellen und Ändern von Teams einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie die mit der Gruppe und ihren Untergruppen verknüpften Teams anzeigen und mit ihnen arbeiten.

Wenn es Gruppen über Ihrer Gruppe gibt, können ihre Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Informationen dazu, wie Benutzer mit einer Planungslizenz ein Team erstellen können, finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Weitere Informationen dazu, wie ein Workfront-Administrator ein Team erstellen kann, finden Sie unter [Erstellen eines Teams aus dem Einrichtungsbereich](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Gewähren eines vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben.

## Anzeigen, Arbeiten mit und Erstellen von Teams für Ihre Gruppe über den Bereich Gruppen

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie Teams erstellen oder ändern möchten.
1. Klicken Sie im linken Bereich auf **Teams** ![](assets/teams.png) , um die Teams aufzulisten, die der Gruppe und etwaigen Untergruppen zugeordnet sind.

1. Führen Sie einen der folgenden Schritte aus:

   * **Team hinzufügen**: Klicken Sie auf **Neues Team** und verwenden Sie dann die folgenden Optionen, um es zu konfigurieren:

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
       <td> <p> Das System füllt das Feld Gruppe für das neue Team mit der Gruppe aus, die Sie anzeigen. Wenn Sie das Team mit einer anderen Gruppe verknüpfen möchten, geben Sie den Namen der Gruppe ein und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol "<img src="assets/info-icon.png">" klicken, das neben der Gruppe angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> <p><b>HINWEIS</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied zu sein. Gruppenadministratoren können im Hauptmenü den Bereich Teams aufrufen und auf den Pfeil "Switch Teams"<img src="assets/switch-team-icon.png" alt="Symbol &quot;Team wechseln&quot;"> klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Team-Mitglieder</td> 
       <td> <p>Beginnen Sie mit der Eingabe des Namens eines Benutzers für das Team und wählen Sie dann den Namen aus, wenn in der Dropdown-Liste angezeigt wird. Wiederholen Sie diesen Vorgang, um mehrere Benutzer zum Team hinzuzufügen.</p> <p>Es gibt keine Beschränkung dafür, wie viele Benutzer Sie einem Team hinzufügen können. Es wird jedoch empfohlen, nicht zu viele Benutzer in einem Team zu haben, da das Arbeitsmanagement des Teams zu komplex werden könnte.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Beschreibung</td> 
       <td>Geben Sie eine Beschreibung für das Team ein.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Kalender</td> 
       <td>Wählen Sie, welches Kalenderregister für dieses Team angezeigt wird.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Bearbeiten</td> 
       <td>Ändern Sie die Schaltfläche "Bearbeiten"in die Schaltfläche "Starten". Wenn ein Benutzer auf Start klickt, wird der Status des Elements automatisch aktualisiert.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Schaltfläche „Fertig“</td> 
       <td>Wählen Sie den Status aus, den Sie für Elemente festlegen möchten, wenn Sie auf die Schaltfläche Fertig klicken.</td> 
       </tr> 
      </tbody> 
     </table>

   * **Teams bearbeiten**: Wählen Sie mindestens ein Team aus, klicken Sie auf **das** Bearbeitungssymbol ![](assets/edit-icon.png) und verwenden Sie dann die folgenden Optionen, um es zu konfigurieren:

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
       <td> <p>Verbinden Sie das Team mit einer Gruppe. Geben Sie den Namen der Gruppe ein und wählen Sie den Namen aus, wenn er angezeigt wird.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol "<img src="assets/info-icon.png">" klicken, das neben der Gruppe angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> <p><b>HINWEIS</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied zu sein. Gruppenadministratoren können im Hauptmenü den Bereich Teams aufrufen und auf den Pfeil "Switch Teams"<img src="assets/switch-team-icon.png" alt="Symbol &quot;Team wechseln&quot;"> klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Besitzerin bzw. Besitzer</td> 
       <td>Wählen Sie einen Inhaber für das Team aus.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Team-Mitglieder</td> 
       <td> <p>Fügen Sie Mitglieder und Teams hinzu. Beginnen Sie mit der Eingabe des Namens eines Benutzers und wählen Sie dann den Namen aus, wenn er angezeigt wird. Wiederholen Sie diesen Vorgang, um mehrere Benutzer zum Team hinzuzufügen.</p> <p><b>TIPP</b>: Es gibt keine Beschränkung dafür, wie viele Benutzer Sie einem Team hinzufügen können. Es wird jedoch empfohlen, nicht zu viele Benutzer in einem Team zu haben, da das Arbeitsmanagement des Teams zu komplex werden könnte.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Beschreibung</td> 
       <td>Geben Sie eine Beschreibung für das Team ein.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Layoutvorlage</td> 
       <td> <p>Beginnen Sie mit der Eingabe des Namens der Layoutvorlage, die das Team verwenden soll, und klicken Sie dann darauf, sobald sie angezeigt wird.</p> <p>Wenn Sie das Team mit dieser Layoutvorlage als Startseite der Benutzer festlegen, sehen alle Benutzer in diesem Team die Anpassungen in dieser Layoutvorlage.<br>Die individuellen Layoutvorlageneinstellungen überschreiben die Einstellungen der Startseiten-Team-Layoutvorlage. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Geben Sie an, ob es sich um ein agiles Team handelt. Weitere Informationen zu agile Teams und zur Verwaltung ihrer Arbeit finden Sie unter <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines agilen Teams</a>.</td> 
       </tr> 
       <tr> 
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

   * **Teams löschen**: Wählen Sie mindestens ein Team aus und klicken Sie dann auf das Löschsymbol ![](assets/delete.png).
   * **Exportieren der Teamliste**: Klicken Sie auf **Export** ![](assets/export.png) und wählen Sie dann das Dateiformat für die exportierte Liste aus.
