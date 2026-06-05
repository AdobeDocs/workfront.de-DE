---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS-Abmelde-URL funktioniert nicht
description: Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Adobe Admin Console integriert haben.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
TQID: https://experienceleague.adobe.com/RRaLL70JcSBcvoS6EUFuWj5Ejwljekt4QuQ3kXDx-44
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
source-wordcount: 250
ht-degree: 13%

---

# ADFS-Abmelde-URL funktioniert nicht

<!-- Audited: 1/2024 -->

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren galt nur für Organisationen, die noch nicht in die [!UICONTROL Adobe Admin Console integriert &#x200B;].
>
>Da nun alle Unternehmen in die Adobe Admin Console integriert wurden, wird dieser Artikel in naher Zukunft entfernt.
>
>Wenn Ihre Organisation das Onboarding für die [!UICONTROL Adobe Admin Console] durchgeführt hat, lesen Sie den Abschnitt [Unterschiede bei der plattformbasierten Administration ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problem

Bei Verwendung der ADFS-Abmelde-URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) erhalten Sie eine Nachrichtenseite mit dem Fehler: „Beim Zugriff auf die Website ist ein Problem aufgetreten. Versuchen Sie erneut, auf die Website zuzugreifen.“

Wenn das Problem weiterhin besteht, wenden Sie sich an den Administrator dieser Website und geben Sie die folgende Referenznummer an, um das Problem zu identifizieren: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] Package</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] License</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>  
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Lösung

1. Wechseln Sie auf Ihrem ADFS-Manager-Server zu **[!UICONTROL Vertrauensstellungen]** > **[!UICONTROL Vertrauensstellungen von vertrauenden Parteien]** > `<your party trust>`.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Endpunkte“ auf **[!UICONTROL Hinzufügen]**.

1. **[!UICONTROL Endpunkttyp]** = SAML-Abmeldung, Bindung = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Sie können eine Antwort-URL festlegen, wenn Sie sie auf eine andere Seite umleiten möchten. Wir empfehlen jedoch die ADFS-Website, da sie Sie warnt, dass Sie abgemeldet sind, aber Sie sollten dennoch Ihren Browser schließen.
