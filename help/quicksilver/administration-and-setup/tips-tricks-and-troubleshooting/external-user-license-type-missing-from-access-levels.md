---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Lizenztyp für externe Benutzer fehlt in den Zugriffsebenen
description: Ich kann den Lizenztyp Externer Benutzer unter „Zugriffsebenen“ im Setup nicht mehr sehen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
TQID: https://experienceleague.adobe.com/g65Yq7r0Hvr6ZyC2niVw4Dnbil37epPeoyfQVOWOiy8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 119
ht-degree: 24%

---

# Lizenztyp für externe Benutzer fehlt in den Zugriffsebenen

## Problem

Ich kann den Lizenztyp Externer Benutzer unter „Zugriffsebenen“ im Setup nicht mehr sehen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Lösung

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Voreinstellungen]**.

1. Stellen Sie im Abschnitt **[!UICONTROL Sicherheit]** sicher, dass die Option **[!UICONTROL Mit Personen ohne Workfront-Konto über deren E-Mail-Adresse zusammenarbeiten]** aktiviert ist.

   Wenn diese Option nicht aktiviert ist, wird der externe Benutzer nicht im Setup der Zugriffsebene angezeigt.
