---
title: Erstellen eines Teams aus dem Einrichtungsbereich
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Als Adobe Workfront-Administrator können Sie im Bereich "Einrichtung"ein Team erstellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 6409f8fa5072413444545d2d3a80935dc6e04b4c
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 4%

---

# Erstellen eines Teams im Bereich &quot;Einrichtung&quot;

Als Adobe Workfront-Administrator können Sie im Bereich &quot;Einrichtung&quot;ein Team erstellen. Weitere Informationen zu Teams finden Sie unter [Übersicht über Teams](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Ein Gruppenadministrator kann ein Team für eine Gruppe erstellen, die er verwaltet, und zwar über den Bereich Einrichtung . Weitere Informationen finden Sie unter [Erstellen und Ändern von Teams einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Ein Benutzer mit einer Standard- oder Planlizenz kann auch ein Team aus dem Bereich Teams erstellen. Weitere Informationen finden Sie unter [Team erstellen](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

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

## Team erstellen

{{step-1-to-setup}}

1. Klicken Sie auf **Teams** und dann auf **Neues Team**.

1. Geben Sie im angezeigten Feld **Neues Team** die folgenden Informationen an:

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
      <td> <p>Wenn Sie das Team mit einer Gruppe verknüpfen möchten, geben Sie den Namen der Gruppe ein und wählen Sie den Namen aus, wenn er angezeigt wird.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe mit dem Team verknüpfen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol "<img src="assets/info-icon.png">" klicken, das neben der Gruppe angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> <p><b>HINWEIS</b>: Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied zu sein. Gruppenadministratoren können im Hauptmenü den Bereich Teams aufrufen und auf den Pfeil "Switch Teams"<img src="assets/switch-team-icon.png" alt="Symbol &quot;Team wechseln&quot;"> klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
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
      <td>Wählen Sie den Status aus, den Sie für Elemente festlegen möchten, wenn Sie auf die Schaltfläche Fertig klicken.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Team erstellen**.

## Team-Eigentümer

Wenn Sie ein Team erstellen, werden Sie standardmäßig zum Teameigentümer.

Sie können die Teameigentümer für alle Teams anzeigen, wenn Sie einen Bericht für Teams erstellen und das Feld &quot;Eigentümername&quot;in Ihren Bericht aufnehmen. (Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
