---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Entfernen einer externen Seite aus einem Dashboard
description: Sie können eine externe Seite aus einem Dashboard entfernen, wenn sie nicht mehr benötigt wird.
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 1%

---

# Entfernen einer externen Seite aus einem Dashboard

<!-- Audited: 1/2025 -->

Sie können eine externe Seite aus einem Dashboard entfernen, wenn sie nicht mehr benötigt wird.

Sie können eine externe Seite jedoch nicht löschen, nachdem sie in Adobe Workfront erstellt wurde. Eine externe Seite kann nur mithilfe der API gelöscht werden. Weitere Informationen zur Workfront-API finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md). Informationen zum Erstellen externer Seiten finden Sie unter [Externe Web-Seite in ein Dashboard einbetten](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entfernen einer externen Seite aus einem Dashboard

1. Wechseln Sie zum Dashboard, das die externe Seite enthält, die Sie löschen möchten.

1. Klicken Sie **Dashboard-Aktionen** und dann auf **Bearbeiten**.

   ![Dashboard bearbeiten](assets/unshimmed-edit-dashboard.png)

1. Suchen Sie rechts im Bildschirm die externe Seite, die Sie entfernen möchten, und klicken Sie auf das Symbol **Löschen** ![Löschen](assets/delete.png).

   ![Symbol „Externe Seite löschen“ im Dashboard](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. Klicken Sie **Speichern + Schließen** in der linken unteren Ecke.

   Dadurch wird die externe Seite aus dem ausgewählten Dashboard entfernt. Die externe Seite verbleibt in Workfront und kann über einen Bericht aufgerufen werden. Weitere Informationen finden Sie im Abschnitt „Anzeigen externer Seiten in einem Bericht“ im Artikel [Einbetten einer externen Web-Seite in ein Dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).
