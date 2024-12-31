---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Entfernen einer externen Seite aus einem Dashboard
description: Sie können eine externe Seite aus einem Dashboard entfernen, wenn sie nicht mehr benötigt wird.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Entfernen einer externen Seite aus einem Dashboard

Sie können eine externe Seite aus einem Dashboard entfernen, wenn sie nicht mehr benötigt wird.

Sie können eine externe Seite jedoch nicht löschen, nachdem sie in Adobe Workfront erstellt wurde. Eine externe Seite kann nur mithilfe der API gelöscht werden. Weitere Informationen zur Workfront-API finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md). Informationen zum Erstellen externer Seiten finden Sie unter [Externe Web-Seite in ein Dashboard einbetten](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Verwalten von Berechtigungen für das Dashboard</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Entfernen einer externen Seite aus einem Dashboard

1. Klicken Sie auf das **Hauptmenü**-Symbol ![](assets/main-menu-icon.png) und dann auf **Dashboards**.
1. Wählen Sie das Dashboard aus, aus dem Sie die externe Seite entfernen möchten, und klicken Sie dann auf **Bearbeiten** ![](assets/edit-icon.png).

   ![Wählen Sie das Symbol Bearbeiten aus.](assets/nwe-editdashboard2021-350x188.png)

1. Suchen Sie rechts im Bildschirm die externe Seite, die Sie entfernen möchten, und klicken Sie auf das Symbol **Löschen** ![](assets/delete.png).

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Klicken Sie **Speichern + Schließen** in der linken unteren Ecke.

   Dadurch wird die externe Seite aus dem ausgewählten Dashboard entfernt. Die externe Seite verbleibt in Workfront und kann über einen Bericht aufgerufen werden. Weitere Informationen finden Sie im Abschnitt „Anzeigen externer Seiten in einem Bericht“ im Artikel [Einbetten einer externen Web-Seite in ein Dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
