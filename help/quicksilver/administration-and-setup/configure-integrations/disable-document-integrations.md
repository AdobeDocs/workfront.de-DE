---
title: Dokumentintegrationen deaktivieren
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: As [!DNL anAdobe] [!DNL Workfront] -Administrator können Sie die Verbindung zwischen Workfront und einem der Dokumentenanbieter eines Drittanbieters deaktivieren.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 1%

---

# Dokumentintegrationen deaktivieren

Als [!DNL Adobe] [!DNL Workfront] Administrator, können Sie die Verbindung zwischen [!DNL Workfront] und einem der Dokumentenanbieter eines Drittanbieters.

Wenn Sie die Verbindung zwischen [!DNL Workfront] und einem Dokumentanbieter, werden die Links zu den Dokumenten von [!DNL Workfront]. Benutzer können die verknüpften Dokumente nicht mehr sehen, sie können keine Änderungen an den Dokumenten über die [!DNL Workfront] Links hinzufügen, und sie können diesem Provider keine weiteren Dokumente hinzufügen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Cloud-Provider-Integrationen deaktivieren

So deaktivieren Sie Dokumentintegrationen für [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Anmelden bei [!DNL Workfront] as a [!DNL Workfront] Administrator.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Dokumente]** > **[!UICONTROL Cloud-Anbieter]**.

1. Deaktivieren Sie alle Cloud-Anbieter, von denen Sie die Verbindung trennen möchten. [!DNL Workfront].
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Benutzer können keine Verbindung zu dem von Ihnen deaktivierten Cloud-Anbieter herstellen und können keine Dokumente von diesem Cloud-Anbieter mehr mit Workfront verknüpfen.

## Deaktivieren Sie die [!DNL SharePoint] Integration

1. Anmelden bei [!DNL Workfront] as a [!DNL Workfront] Administrator.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Erweitern **[!UICONTROL Dokumente]** Klicken Sie auf **[!UICONTROL [!DNL SharePoint]Integration]**.
1. Wählen Sie die [!DNL SharePoint] Integration, die Sie deaktivieren möchten.
1. Klicken **[!UICONTROL Deaktivieren]**.\
   Benutzer können keine Verbindung zum [!DNL SharePoint] Site, die Sie deaktiviert haben, und sie können Dokumente nicht mehr verknüpfen von [!DNL SharePoint] nach [!DNL Workfront].

## Deaktivieren benutzerdefinierter Integrationen

1. Anmelden bei [!DNL Workfront] als Administrator.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Dokumente]** > **[!UICONTROL Benutzerdefinierte Integration]**.
1. Wählen Sie die benutzerdefinierte Integration aus, die Sie deaktivieren möchten.
1. Klicken **[!UICONTROL Deaktivieren]**.

   Benutzer können keine Verbindung zu dem von Ihnen deaktivierten Dokumentanbieter von Drittanbietern herstellen und können keine Dokumente von diesem Cloud-Anbieter mehr mit [!DNL Workfront].
