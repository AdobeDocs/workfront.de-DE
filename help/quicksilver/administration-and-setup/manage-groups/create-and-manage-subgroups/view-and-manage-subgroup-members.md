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
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Anzeigen und Verwalten von Untergruppenmitgliedern

Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie alle Benutzer in den Untergruppen der Gruppe anzeigen und verwalten.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Benutzer bearbeiten, wobei die Option "Benutzeradministrator (Alle Benutzer)"ausgewählt ist</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

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
