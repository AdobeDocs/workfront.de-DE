---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Untergruppenmitglieder anzeigen und verwalten
description: Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzenden in den Untergruppen der Gruppe anzeigen und verwalten.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
TQID: https://experienceleague.adobe.com/BbyES980TEgJEigbZQuvzncLvGc1FlM09muH-t4zq44
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 384
ht-degree: 9%

---

# Anzeigen und Verwalten von Untergruppenmitgliedern

Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzenden in den Untergruppen der Gruppe anzeigen und verwalten.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
       <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-settings.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Anzeigen und Verwalten von Mitgliedern der Untergruppen unter einer Gruppe

{{step-1-to-setup}}

1. Klicken Sie **Gruppen**.

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, für die Sie Untergruppenmitglieder anzeigen oder verwalten möchten.
1. Klicken Sie im linken Bedienfeld auf **Untergruppenmitglieder**.

   Dieses Element im linken Bedienfeld ist nur verfügbar, wenn die Gruppe Untergruppen hat.

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie ein Mitglied aus der Liste aus und klicken Sie dann auf ![Bearbeiten](assets/edit-icon.png), um das Benutzerprofil dieser Person zu ändern.

     Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) oder [Benutzerprofile stapelweise bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Wählen Sie eine beliebige Anzahl von Untergruppenmitgliedern in der Liste aus und klicken Sie dann auf **Aktualisierung an Benutzer senden**, um ihren Benutzerprofilen einen Kommentar hinzuzufügen.

     Der oder die Benutzenden erhalten eine In-App-Benachrichtigung sowie eine E-Mail-Benachrichtigung mit Ihrem Kommentar. Der Kommentar wird im Bereich Aktualisierungen im Benutzerprofil angezeigt.

     Weitere Informationen finden Sie unter [Senden von Direktnachrichten an andere Benutzer](/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md).

   * Wählen Sie eine beliebige Anzahl von Mitgliedern in der Liste aus und klicken Sie dann auf Deaktivieren ![Benutzer deaktivieren](assets/deactivate-user.png) oder Aktivieren ![Benutzer aktivieren](assets/activate-user.png).

     Weitere Informationen finden Sie unter [Deaktivieren oder Reaktivieren eines Benutzers](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Export ![Export](assets/export.png) die Mitgliederliste.
