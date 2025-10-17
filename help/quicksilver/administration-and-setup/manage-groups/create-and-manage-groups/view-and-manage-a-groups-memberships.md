---
user-type: administrator
product-area: system-administration;user-management
keywords: Hinzufügen,Benutzer,Gruppe,Hinzufügen,Weitere,Zuweisen,Administrator,Entfernen,Benutzer,Ansicht,Rollen,Mitglieder,Export,Mitgliedschaft,Daten
navigation-topic: create-and-manage-groups
title: Anzeigen und Verwalten der Gruppenmitgliedschaften
description: Als Adobe Workfront-Administrator können Sie Mitglieder jeder Gruppe, die Sie verwalten, anzeigen, hinzufügen, entfernen, exportieren, aktivieren und deaktivieren. Sie können auch ihre Profile bearbeiten, Aktualisierungen zu ihren Profilen hinzufügen und sie als zusätzliche Gruppenadministratoren für die Gruppe zuweisen.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Anzeigen und Verwalten der Gruppenmitgliedschaften

Als Adobe Workfront-Administrator können Sie Mitglieder jeder Gruppe, die Sie verwalten, anzeigen, hinzufügen, entfernen, exportieren, aktivieren und deaktivieren. Sie können auch ihre Profile bearbeiten, Aktualisierungen zu ihren Profilen hinzufügen und sie als zusätzliche Gruppenadministratoren für die Gruppe zuweisen.

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen und Verwalten der Gruppenmitgliedschaften

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen**.

   In der angezeigten Liste können Workfront-Administratoren alle Gruppen und Untergruppen anzeigen. Gruppenadministratoren können nur die von ihnen verwalteten Gruppen und Untergruppen sehen.

1. Klicken Sie auf den Namen der Gruppe, die Sie bearbeiten möchten.
1. Führen Sie auf der angezeigten Seite **Gruppenmitglieder** im linken Menü einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Hinzufügen eines Benutzers zur Gruppe</td> 
      <td> 
       <ol> 
        <li>Klicken Sie auf <strong>Mitglieder hinzufügen</strong> <img src="assets/add-icon-plus-in-circle.png">, tippen Sie den Namen des Benutzers ein und wählen Sie ihn aus, wenn er angezeigt wird.</li>
        <li> <p>Wiederholen Sie diesen Vorgang für alle anderen Benutzer, die Sie hinzufügen möchten.</p> <p>Wenn Sie diesen Benutzer nicht hinzufügen möchten, können Sie rechts neben einem Namen auf das X klicken.</p> </li>
        <li>Klicken Sie <strong> Abschluss </strong>Fertig“.</li>
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entfernen eines Benutzers aus der Gruppe</td> 
      <td> 
       <ol> 
        <li>Wählen Sie einen oder mehrere Benutzernamen aus und klicken Sie dann auf <strong>Mitglied entfernen</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li> <p>Klicken <strong> in </strong> angezeigten Warnmeldung auf „Entfernen“.</p> <p>Sie können einen Benutzer suchen, den Sie aus der Liste entfernen möchten, indem Sie auf <strong>Personen und Gruppen in der Liste suchen</strong> seinen Namen in das Feld eingeben und dann auf den Namen klicken, wenn er angezeigt wird.</p> <p><b>HINWEIS</b>:  
          <ul> 
           <li>Wenn diese Gruppe die Hauptgruppe eines Benutzers ist, den Sie entfernen möchten, müssen Sie dem Profil des Benutzers zunächst eine andere Hauptgruppe zuweisen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Übersicht über Hauptgruppen</a> und <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils</a>.</li> 
           <li>Wenn die Gruppe nur einen Gruppenadministrator hat und Sie ihn oder sie aus der Gruppe entfernen müssen, müssen Sie der Gruppe zuerst einen anderen Gruppenadministrator zuweisen.</li> 
           <li>Ein Benutzer kann sowohl einzeln zu einer Untergruppe als auch zu der übergeordneten Gruppe gehören. Wenn Sie jemanden aus einer Untergruppe entfernen, bleibt er Teil der übergeordneten Gruppe. Wenn Sie sie aus der übergeordneten Gruppe entfernen, bleiben sie entsprechend Teil der Untergruppe. Wenn Sie nicht möchten, dass ein Benutzer Zugriff auf die übergeordnete Gruppe hat, müssen Sie den Benutzer sowohl aus den Untergruppen als auch aus der übergeordneten Gruppe entfernen, wenn sie an beiden Stellen einzeln aufgeführt sind.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bearbeiten der Profilinformationen von Benutzenden</td> 
      <td> 
       <ol> 
        <li>Wählen Sie einen oder mehrere Benutzernamen aus und klicken Sie dann auf <strong>Bearbeiten</strong> <img src="assets/edit-icon.png">.</li> 
        <li> <p>Ändern der Profilinformationen des Benutzers.</p> <p>Informationen zu den Änderungen, die Sie vornehmen können, finden <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> unter „Benutzerprofil bearbeiten</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzermitgliedschaftsdaten exportieren</td> 
      <td> 
       <ol> 
        <li>Wählen Sie einen oder mehrere Benutzernamen aus und klicken Sie dann auf <strong>Exportieren</strong> <img src="assets/export.png">.</li> 
        <li> <p>Exportieren Sie die Daten als durch PDF, Excel oder Tabulatoren getrennte Datei.</p> <p>Weitere Informationen zum Exportieren von Daten finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportieren von Daten</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenrollen der Mitglieder anzeigen und bearbeiten</td> 
      <td> <p>Die Spalte <strong>Gruppenrolle</strong> listet die Rolle jedes Mitglieds auf. Als Gruppenadministrator können Sie auf die Rolle eines Mitglieds doppelklicken, um diese zu ändern.</p> <p>Für Mitglieder der Gruppe, die keine Gruppenadministratoren sind, kann diese Spalte nicht bearbeitet werden.</p> <p>Gruppenadministratoren stehen immer oben auf der Liste.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kommentar an Gruppenmitglieder senden</td> 
      <td> 
       <ol> 
        <li>Wählen Sie mindestens ein Gruppenmitglied aus und klicken Sie dann in der Symbolleiste <strong>Aktualisierung an Benutzer </strong>).</li> 
        <li><p>Geben Sie den Kommentar ein, den Sie den Benutzern und dem Bereich Aktualisierungen ihrer Benutzerprofile senden möchten.</p>
        <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Senden von Direktnachrichten an andere Benutzer</a>.</p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivieren von Benutzenden in Workfront</td> 
      <td>Wählen Sie einen oder mehrere inaktive Benutzer aus und klicken Sie dann auf <strong>Benutzer aktivieren</strong>, um sie in Workfront zu aktivieren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deaktivieren von Benutzenden in Workfront</td> 
      <td>Wählen Sie einen oder mehrere aktive Benutzer aus und klicken Sie dann auf <strong>Benutzer deaktivieren</strong><img src="assets/deactivate-user.png">, um sie in Workfront zu deaktivieren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nach Spalte sortieren</td> 
      <td>Klicken Sie auf die Überschrift einer Spalte, um die Liste nach dem Inhalt dieser Spalte zu sortieren.</td> 
     </tr> 
    </tbody> 
   </table>
