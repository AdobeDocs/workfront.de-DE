---
title: Erstellen eines Teams im Bereich "Einrichtung"
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Als Adobe Workfront-Administrator können Sie im Bereich "Einrichtung"ein Team erstellen.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---

# Erstellen eines Teams im Bereich &quot;Einrichtung&quot;

Als Adobe Workfront-Administrator können Sie im Bereich &quot;Einrichtung&quot;ein Team erstellen. Weitere Informationen zu Teams finden Sie unter [Teams - Übersicht](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Ein Gruppenadministrator kann ein Team für eine Gruppe erstellen, die er verwaltet, und zwar über den Bereich Einrichtung . Weitere Informationen finden Sie unter [Erstellen und Ändern von Teams einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Ein Benutzer mit einer Planungslizenz kann auch ein Team aus dem Bereich Personen erstellen. Weitere Informationen finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
>


## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Team erstellen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Teams** Klicken Sie auf **Neues Team**.

1. Im **Neues Team** die folgenden Informationen angeben:

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
      <td> <p>Wenn Sie das Team mit einer Gruppe verknüpfen möchten, geben Sie den Namen der Gruppe ein und wählen Sie den Namen aus, wenn er angezeigt wird.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber halten und auf das Informationssymbol klicken <img src="assets/info-icon.png"> , das daneben angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> <p><b>NOTE</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied zu sein. Gruppenadministratoren können im Hauptmenü den Bereich Teams aufrufen und auf den Pfeil Switches klicken <img src="assets/switch-team-icon.png" alt="Symbol "Team wechseln""> , um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Dies ist ein Agile-Team</td> 
      <td>Wählen Sie dieses Element aus, wenn Sie dieses neue Team als agiles Team konfigurieren möchten. Weitere Informationen zu agilen Teams finden Sie unter <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines agilen Teams</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bearbeiten</td> 
      <td>Ändern Sie die Schaltfläche "Bearbeiten"in die Schaltfläche "Starten". Wenn ein Benutzer auf Start klickt, wird der Status des Elements automatisch aktualisiert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schaltfläche „Fertig“</td> 
      <td>Wählen Sie den Status aus, den Sie für Elemente festlegen möchten, wenn auf die Schaltfläche Fertig geklickt wird.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Team erstellen**.

## Team-Eigentümer

Wenn Sie ein Team erstellen, werden Sie standardmäßig zum Teameigentümer.

Sie können die Teameigentümer für alle Teams anzeigen, wenn Sie einen Bericht für Teams erstellen und das Feld &quot;Eigentümername&quot;in Ihren Bericht aufnehmen. (Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
