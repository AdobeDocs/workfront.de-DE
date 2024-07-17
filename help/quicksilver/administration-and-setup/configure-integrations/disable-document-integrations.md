---
title: Dokumentintegrationen deaktivieren
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Als [!DNL anAdobe] [!DNL Workfront] -Administrator können Sie die Verbindung zwischen Workfront und einem der Dokumentenanbieter eines Drittanbieters deaktivieren.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Dokumentintegrationen deaktivieren

Als [!DNL Adobe] [!DNL Workfront] -Administrator können Sie die Verbindung zwischen [!DNL Workfront] und einem der Dokumentenanbieter eines Drittanbieters deaktivieren.

Wenn Sie die Verbindung zwischen [!DNL Workfront] und einem Dokumentanbieter deaktivieren, werden die Links zu den Dokumenten in [!DNL Workfront] nicht mehr angezeigt. Benutzer können die verknüpften Dokumente nicht mehr sehen, sie können keine Änderungen an den Dokumenten über die &quot;[!DNL Workfront]&quot;-Links vornehmen und sie können diesem Anbieter keine weiteren Dokumente hinzufügen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen zu [!DNL Workfront] -Administratoren finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Cloud-Provider-Integrationen deaktivieren

So deaktivieren Sie Dokumentintegrationen für [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Melden Sie sich bei [!DNL Workfront] als [!DNL Workfront] -Administrator an.
1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **[!UICONTROL Dokumente]** > **[!UICONTROL Cloud-Anbieter]**.

1. Deaktivieren Sie einen der Cloud-Anbieter, von denen Sie die Verbindung mit [!DNL Workfront] trennen möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Benutzer können keine Verbindung zu dem spezifischen Cloud-Anbieter herstellen, den Sie deaktiviert haben, und sie können keine Dokumente von diesem Cloud-Anbieter mehr mit Workfront verknüpfen.

## Die [!DNL SharePoint]-Integration deaktivieren

1. Melden Sie sich bei [!DNL Workfront] als [!DNL Workfront] -Administrator an.
1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Erweitern Sie **[!UICONTROL Dokumente]** und klicken Sie dann auf **[!UICONTROL [!DNL SharePoint]Integration]**.
1. Wählen Sie die [!DNL SharePoint] -Integration aus, die Sie deaktivieren möchten.
1. Klicken Sie auf **[!UICONTROL Deaktivieren]**.\
   Benutzer können keine Verbindung zur deaktivierten [!DNL SharePoint]-Site herstellen und sie können Dokumente nicht mehr von [!DNL SharePoint] zu [!DNL Workfront] verknüpfen.

## Deaktivieren benutzerdefinierter Integrationen

1. Melden Sie sich bei [!DNL Workfront] als Administrator an.
1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **[!UICONTROL Dokumente]** > **[!UICONTROL Benutzerdefinierte Integration]**.
1. Wählen Sie die benutzerdefinierte Integration aus, die Sie deaktivieren möchten.
1. Klicken Sie auf **[!UICONTROL Deaktivieren]**.

   Benutzer können keine Verbindung zu dem von Ihnen deaktivierten Dokumentanbieter von Drittanbietern herstellen und können keine Dokumente von diesem Cloud-Anbieter mehr mit [!DNL Workfront] verknüpfen.
