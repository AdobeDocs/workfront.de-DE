---
user-type: administrator
product-area: system-administration;user-management
keywords: add,users,group,add,another,assign,administrator,remove,user,view,rollen,members,export,membership,data
navigation-topic: create-and-manage-groups
title: Anzeigen und Verwalten von Gruppenmitgliedschaften
description: Als Adobe Workfront-Administrator können Sie Mitglieder jeder von Ihnen verwalteten Gruppe anzeigen, hinzufügen, entfernen, exportieren, aktivieren und deaktivieren. Sie können auch ihre Profile bearbeiten, ihren Profilen Aktualisierungen hinzufügen und sie als zusätzliche Gruppenadministratoren für die Gruppe zuweisen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 1%

---

# Gruppenmitgliedschaften anzeigen und verwalten

Als Adobe Workfront-Administrator können Sie Mitglieder jeder von Ihnen verwalteten Gruppe anzeigen, hinzufügen, entfernen, exportieren, aktivieren und deaktivieren. Sie können auch ihre Profile bearbeiten, ihren Profilen Aktualisierungen hinzufügen und sie als zusätzliche Gruppenadministratoren für die Gruppe zuweisen.

Wenn es Gruppen über Ihrer Gruppe gibt, können ihre Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

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
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gruppenmitgliedschaften anzeigen und verwalten

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen**.

   In der angezeigten Liste können Workfront-Administratoren alle Gruppen und Untergruppen anzeigen. Gruppenadministratoren können nur die Gruppen und Untergruppen sehen, die sie verwalten.

1. Klicken Sie auf den Namen der Gruppe, die Sie bearbeiten möchten.
1. Führen Sie auf der angezeigten Seite, während im linken Menü **Gruppenmitglieder** ausgewählt ist, einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Einen Benutzer zur Gruppe hinzufügen</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Klicken Sie auf <strong>Mitglieder hinzufügen</strong> <img src="assets/add-icon-plus-in-circle.png">, geben Sie den Namen des Benutzers ein und wählen Sie ihn aus, wenn er angezeigt wird.</li> 
        <li value="2"> <p>Wiederholen Sie diesen Vorgang für alle anderen Benutzer, die Sie hinzufügen möchten.</p> <p>Sie können auf das X rechts neben einem Namen klicken, wenn Sie diesen Benutzer nicht hinzufügen möchten.</p> </li> 
        <li value="3">Klicken Sie auf <strong>Fertig</strong> , wenn Sie fertig sind.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einen Benutzer aus der Gruppe entfernen</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Wählen Sie einen oder mehrere Benutzernamen aus und klicken Sie dann auf <strong>Mitglied entfernen</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Klicken Sie in der angezeigten Warnmeldung auf <strong>Entfernen</strong> .</p> <p>Sie können einen Benutzer finden, den Sie aus der Liste entfernen möchten, indem Sie auf <strong>Personen und Gruppen in der Liste durchsuchen</strong> klicken, den Namen in das Feld eingeben und dann auf den Namen klicken, wenn er angezeigt wird.</p> <p><b>NOTE</b>:  
          <ul> 
           <li>Wenn es sich bei dieser Gruppe um die Home Group für einen Benutzer handelt, den Sie entfernen möchten, müssen Sie zunächst eine andere Home Group im Profil des Benutzers zuweisen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Übersicht über die Home-Gruppen</a> und <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a>.</li> 
           <li>Wenn die Gruppe nur einen Gruppenadministrator hat und Sie ihn oder sie aus der Gruppe entfernen müssen, müssen Sie zuerst einen weiteren Gruppenadministrator der Gruppe zuweisen.</li> 
           <li>Ein Benutzer kann einzeln zu einer Untergruppe sowie zur übergeordneten Gruppe gehören. Wenn Sie eine Person aus einer Untergruppe entfernen, bleiben sie Teil der übergeordneten Gruppe. Wenn Sie sie aus der übergeordneten Gruppe entfernen, bleiben sie ebenfalls Teil der Untergruppe. Wenn Sie nicht möchten, dass einem Benutzer der Zugriff für die übergeordnete Gruppe gestattet wird, müssen Sie den Benutzer sowohl aus den Untergruppen als auch aus der übergeordneten Gruppe entfernen, wenn er an beiden Stellen einzeln aufgeführt wird.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Profilinformationen eines Benutzers bearbeiten</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Wählen Sie einen oder mehrere Benutzernamen aus und klicken Sie dann auf <strong>Bearbeiten</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Ändern Sie die Profilinformationen des Benutzers.</p> <p>Informationen zu den Änderungen, die Sie vornehmen können, finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Profil eines Benutzers bearbeiten</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportieren von Daten zur Benutzermitgliedschaft</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Wählen Sie einen oder mehrere Benutzernamen aus und klicken Sie dann auf <strong>Export</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exportieren Sie die Daten als PDF-, Excel- oder tabulatorgetrennte Datei.</p> <p>Weitere Informationen zum Exportieren von Daten finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Daten exportieren</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anzeigen und Bearbeiten von Gruppenrollen von Mitgliedern</td> 
      <td> <p>Die Spalte <strong>Gruppenrolle</strong> enthält die Rolle jedes Mitglieds. Als Gruppenadministrator können Sie auf die Rolle eines Mitglieds doppelklicken, um sie zu ändern.</p> <p>Für Gruppenmitglieder, die keine Gruppenadministratoren sind, kann diese Spalte nicht bearbeitet werden.</p> <p>Gruppenadministratoren stehen immer oben in der Liste.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Senden eines Kommentars an Gruppenmitglieder</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Wählen Sie einen oder mehrere Benutzernamen aus und klicken Sie dann auf <strong>Aktualisieren</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">Geben Sie den Kommentar ein.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer in Workfront aktivieren</td> 
      <td>Wählen Sie einen oder mehrere inaktive Benutzer aus und klicken Sie dann auf <strong>Benutzer aktivieren</strong> , um sie in Workfront zu aktivieren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzer in Workfront deaktivieren</td> 
      <td>Wählen Sie einen oder mehrere aktive Benutzer aus und klicken Sie dann auf <strong>Benutzer deaktivieren</strong><img src="assets/deactivate-user.png"> , um sie in Workfront zu deaktivieren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nach Spalte sortieren</td> 
      <td>Klicken Sie auf die Spaltenüberschrift, um die Liste nach dem Inhalt der Spalte zu sortieren.</td> 
     </tr> 
    </tbody> 
   </table>
