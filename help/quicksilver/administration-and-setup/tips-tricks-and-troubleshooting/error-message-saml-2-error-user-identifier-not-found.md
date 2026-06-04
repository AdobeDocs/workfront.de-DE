---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: SAML 2.0 Fehler: Benutzerkennung nicht gefunden'
description: Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
TQID: https://experienceleague.adobe.com/H7-Y9pZ-w4K3iEkJTVeHrx1cJJYXHiIMIvO3VoGYq9g
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 16%

---

# Fehlermeldung: SAML 2.0 Fehler: Benutzerkennung nicht gefunden

## Problem

Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Wenn Sie eine erfolgreiche Testverbindung herstellen und weiterhin Probleme auftreten, kann es sein, dass falsche Attributzuordnungen oder Probleme mit den Federation IDs vorliegen. Wenden Sie sich bei Fragen an den Support.

## Ursache:

Behauptungen auf dem ADFS-Server sind falsch.

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

Stellen Sie auf dem ADFS-Server sicher, dass ein Anspruch für die Namens-ID besteht:

1. Klicken Sie unter Windows auf **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Wählen **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauensstellungen der vertrauenden]** im linken Bereich aus.

1. Klicken Sie mit der rechten Maustaste auf die Vertrauensstellung der vertrauenden Seite in Bezug auf Adobe Workfront und wählen Sie **[!UICONTROL Anspruchsregeln bearbeiten]**.
1. Überprüfen Sie, ob der Anspruch über **[!UICONTROL Typ des ausgehenden Anspruchs]** von **[!UICONTROL Name ID]** verfügt.

![1.png](assets/1-350x287.png)
