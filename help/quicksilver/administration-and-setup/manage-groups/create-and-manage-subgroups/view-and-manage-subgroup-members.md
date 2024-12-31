---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Untergruppenmitglieder anzeigen und verwalten
description: Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzenden in den Untergruppen der Gruppe anzeigen und verwalten.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 63c2206905f4ebbc35cb162ae6e895b98b5d20eb
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Untergruppenmitglieder anzeigen und verwalten

Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzenden in den Untergruppen der Gruppe anzeigen und verwalten.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

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
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-settings.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen und Verwalten von Mitgliedern der Untergruppen unter einer Gruppe

{{step-1-to-setup}}

1. Klicken Sie **Gruppen**.

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, für die Sie Untergruppenmitglieder anzeigen oder verwalten möchten.
1. Klicken Sie im linken Bedienfeld auf **Untergruppenmitglieder**.

   Dieses Element im linken Bedienfeld ist nur verfügbar, wenn die Gruppe Untergruppen hat.

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie ein Mitglied in der Liste aus und klicken Sie dann auf ![](assets/edit-icon.png) bearbeiten , um das Benutzerprofil dieser Person zu ändern.

     Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) oder [Benutzerprofile stapelweise bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Wählen Sie eine beliebige Anzahl von Mitgliedern in der Liste aus und klicken Sie dann auf ![](assets/comment-icon.png) aktualisieren , um ihren Benutzerprofilen einen Kommentar hinzuzufügen.

     Der oder die Benutzenden erhalten eine In-App-Benachrichtigung sowie eine E-Mail-Benachrichtigung mit Ihrem Kommentar. Der Kommentar wird im Bereich Aktualisierungen im Benutzerprofil angezeigt.

   * Wählen Sie eine beliebige Anzahl von Mitgliedern in der Liste aus und klicken Sie dann auf ![](assets/deactivate-user.png) deaktivieren oder ![](assets/activate-user.png) aktivieren .

     Weitere Informationen finden Sie unter [Deaktivieren oder Reaktivieren eines Benutzers](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exportieren Sie ![](assets/export.png) die Mitgliederliste.
