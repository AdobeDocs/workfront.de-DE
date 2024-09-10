---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Anzeigen und Verwalten von Untergruppenmitgliedern
description: Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzer in den Untergruppen der Gruppe anzeigen und verwalten.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 63c2206905f4ebbc35cb162ae6e895b98b5d20eb
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Anzeigen und Verwalten von Untergruppenmitgliedern

Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzer in den Untergruppen der Gruppe anzeigen und verwalten.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

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
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsebene, die für den Zugriff auf <b>Bearbeiten</b> konfiguriert ist, wobei <b>Erstellen</b> und mindestens eine der beiden Optionen <b>Benutzeradministrator</b> unter <b>Optimieren Ihrer Einstellungen</b> <img src="assets/gear-icon-settings.png"> aktiviert sind. </p> <p>Wenn von diesen beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)</b> aktiviert ist, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mitglieder der Untergruppen unter einer Gruppe anzeigen und verwalten

{{step-1-to-setup}}

1. Klicken Sie auf **Gruppen**.

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Klicken Sie auf den Namen der Gruppe, deren Mitglieder Sie anzeigen oder verwalten möchten.
1. Klicken Sie im linken Bereich auf **Mitglieder der Untergruppe**.

   Dieses linke Bedienfeldelement ist nur verfügbar, wenn die Gruppe Untergruppen enthält.

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie ein Mitglied in der Liste aus und klicken Sie auf Bearbeiten ![](assets/edit-icon.png) , um das Benutzerprofil dieser Person zu ändern.

     Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) oder [Benutzerprofile stapelweise bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md) .

   * Wählen Sie eine beliebige Anzahl von Mitgliedern in der Liste aus und klicken Sie auf Aktualisieren ![](assets/comment-icon.png) , um ihren Benutzerprofilen einen Kommentar hinzuzufügen.

     Der Benutzer erhält eine In-App-Benachrichtigung sowie eine E-Mail-Benachrichtigung mit Ihrem Kommentar. Der Kommentar wird im Bereich Updates des Benutzerprofils angezeigt.

   * Wählen Sie eine beliebige Anzahl von Mitgliedern in der Liste aus und klicken Sie dann auf &quot;Deaktivieren&quot;![](assets/deactivate-user.png) oder &quot;Aktivieren&quot;![](assets/activate-user.png).

     Weitere Informationen finden Sie unter [Deaktivieren oder Reaktivieren eines Benutzers](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exportieren Sie ![](assets/export.png) die Liste der Mitglieder.
