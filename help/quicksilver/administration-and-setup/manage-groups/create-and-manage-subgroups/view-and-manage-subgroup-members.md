---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Anzeigen und Verwalten von Untergruppenmitgliedern
description: Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzer in den Untergruppen der Gruppe anzeigen und verwalten.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Anzeigen und Verwalten von Untergruppenmitgliedern

Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzer in den Untergruppen der Gruppe anzeigen und verwalten.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Benutzer bearbeiten, wobei die Option "Benutzeradministrator (Alle Benutzer)"ausgewählt ist</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Mitglieder der Untergruppen unter einer Gruppe anzeigen und verwalten

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Gruppen**.

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Klicken Sie auf den Namen der Gruppe, deren Mitglieder Sie anzeigen oder verwalten möchten.
1. Klicken Sie im linken Bereich auf **Untergruppenmitglieder**.

   Dieses linke Bedienfeldelement ist nur verfügbar, wenn die Gruppe Untergruppen enthält.

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie ein Mitglied in der Liste aus und klicken Sie auf Bearbeiten ![](assets/edit-icon.png) , um das Benutzerprofil dieser Person zu ändern.

      Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) oder [Massenbearbeitung von Benutzerprofilen](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Wählen Sie eine beliebige Anzahl von Mitgliedern in der Liste aus und klicken Sie auf Aktualisieren ![](assets/comment-icon.png) , um ihren Benutzerprofilen einen Kommentar hinzuzufügen.

      Der Benutzer erhält eine In-App-Benachrichtigung sowie eine E-Mail-Benachrichtigung mit Ihrem Kommentar. Der Kommentar wird im Bereich Updates des Benutzerprofils angezeigt.

   * Wählen Sie eine beliebige Anzahl von Mitgliedern in der Liste aus und klicken Sie dann auf &quot;Deaktivieren&quot; ![](assets/deactivate-user.png) oder aktivieren ![](assets/activate-user.png).

      Weitere Informationen finden Sie unter [Benutzer deaktivieren oder reaktivieren](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Export ![](assets/export.png) die Liste der Mitglieder.
