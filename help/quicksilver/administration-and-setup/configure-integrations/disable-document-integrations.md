---
title: Dokumentintegrationen deaktivieren
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Als  [!DNL anAdobe] [!DNL Workfront] können Sie die Verbindung zwischen Workfront und den Dokumentanbietern von Drittanbietern deaktivieren.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
TQID: https://experienceleague.adobe.com/3tfxxth82eJEjEmdVD3AJFxl6B1m3EVKMQP9Gy4LC24
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 279
ht-degree: 13%

---

# Deaktivieren von Dokumentintegrationen

Als [!DNL Adobe] [!DNL Workfront] können Sie die Verbindung zwischen [!DNL Workfront] und den Dokumentanbietern von Drittanbietern deaktivieren.

Wenn Sie die Verbindung zwischen [!DNL Workfront] und einem Dokumentanbieter deaktivieren, verschwinden die Links zu den Dokumenten aus der [!DNL Workfront]. Benutzer können die verknüpften Dokumente nicht mehr sehen, sie können keine Änderungen an den Dokumenten über die [!DNL Workfront] Links vornehmen und sie können diesem Anbieter keine weiteren Dokumente hinzufügen.

## Zugriffsanforderungen

+++Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Prime oder Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-Lizenzen
   </td>
   <td><p>Standard</p>
   <p>Abo</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Cloud-Provider-Integrationen deaktivieren

So deaktivieren Sie Dokumentintegrationen für [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Melden Sie sich bei [!DNL Workfront] als [!DNL Workfront] an.

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Dokumente]** > **[!UICONTROL Cloud-Anbieter]**.

1. Heben Sie die Auswahl eines der Cloud-Anbieter auf, von denen Sie [!DNL Workfront] trennen möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Benutzende können keine Verbindung zu dem spezifischen Cloud-Anbieter herstellen, den Sie deaktiviert haben, und sie können keine Dokumente mehr von diesem Cloud-Anbieter mit Workfront verknüpfen.

## [!DNL SharePoint] deaktivieren

1. Melden Sie sich bei [!DNL Workfront] als [!DNL Workfront] an.

{{step-1-to-setup}}

1. Erweitern Sie **[!UICONTROL Dokumente]** und klicken Sie dann auf **[!UICONTROL [!DNL SharePoint]Integration]**.
1. Wählen Sie die [!DNL SharePoint] Integration aus, die Sie deaktivieren möchten.
1. Klicken Sie **[!UICONTROL Deaktivieren]**.\
   Benutzende können keine Verbindung zur [!DNL SharePoint]-Site herstellen, die Sie deaktiviert haben, und sie können keine Dokumente mehr von [!DNL SharePoint] zu [!DNL Workfront] verknüpfen.

## Benutzerdefinierte Integrationen deaktivieren

1. Melden Sie sich bei [!DNL Workfront] als Admin an.

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Dokumente]** > **[!UICONTROL Benutzerdefinierte Integration]**.
1. Wählen Sie die benutzerdefinierte Integration aus, die Sie deaktivieren möchten.
1. Klicken Sie **[!UICONTROL Deaktivieren]**.

   Benutzende können keine Verbindung zu dem von Ihnen deaktivierten Drittanbieter von Dokumenten herstellen und sie können keine Dokumente mehr von diesem Cloud-Anbieter mit [!DNL Workfront] verknüpfen.
