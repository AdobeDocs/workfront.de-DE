---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Externe Seite aus einem Dashboard entfernen
description: Sie können eine externe Seite aus einem Dashboard entfernen, wenn sie nicht mehr benötigt wird.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Externe Seite aus einem Dashboard entfernen

Sie können eine externe Seite aus einem Dashboard entfernen, wenn sie nicht mehr benötigt wird.

Eine externe Seite kann jedoch nicht gelöscht werden, nachdem sie in Adobe Workfront erstellt wurde. Sie können eine externe Seite nur mithilfe der API löschen. Informationen zur Workfront-API finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md). Informationen zum Erstellen externer Seiten finden Sie unter [Einbetten einer externen Webseite in ein Dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

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
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für das Dashboard verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Externe Seite aus einem Dashboard entfernen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png)Klicken Sie auf **Dashboards**.
1. Wählen Sie das Dashboard aus, aus dem Sie die externe Seite entfernen möchten, und klicken Sie dann auf **Bearbeiten** ![](assets/edit-icon.png).

   ![Wählen Sie das Symbol Bearbeiten aus.](assets/nwe-editdashboard2021-350x188.png)

1. Suchen Sie rechts im Bildschirm nach der zu entfernenden externen Seite und klicken Sie auf die Schaltfläche **Löschen** icon ![](assets/delete.png).

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Klicken **Speichern und schließen** in der linken unteren Ecke.

   Dadurch wird die externe Seite aus dem ausgewählten Dashboard entfernt. Die externe Seite bleibt in Workfront und kann über einen Bericht aufgerufen werden. Weitere Informationen finden Sie im Abschnitt &quot;Anzeigen externer Seiten in einem Bericht&quot;im Artikel [Einbetten einer externen Webseite in ein Dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
