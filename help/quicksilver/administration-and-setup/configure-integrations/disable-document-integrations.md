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
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 2%

---

# Dokumentintegrationen deaktivieren

Als [!DNL Adobe] [!DNL Workfront] können Sie die Verbindung zwischen [!DNL Workfront] und den Dokumentanbietern von Drittanbietern deaktivieren.

Wenn Sie die Verbindung zwischen [!DNL Workfront] und einem Dokumentanbieter deaktivieren, verschwinden die Links zu den Dokumenten aus der [!DNL Workfront]. Benutzer können die verknüpften Dokumente nicht mehr sehen, sie können keine Änderungen an den Dokumenten über die [!DNL Workfront] Links vornehmen und sie können diesem Anbieter keine weiteren Dokumente hinzufügen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
