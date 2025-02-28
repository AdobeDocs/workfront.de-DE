---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verknüpfen von Assets und Ordnern aus Experience Manager Assets oder Assets Essentials
description: Sie können ein Asset oder einen Ordner aus Experience Manager Assets oder Assets Essentials mit jedem Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Assets Essentials gesendet wurden, werden nicht für den gesamten Dokumentspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden für den gesamten Speicher gezählt.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Verknüpfen von Assets und Ordnern aus Experience Manager Assets oder Assets Essentials

Sie können ein Asset oder einen Ordner aus Experience Manager Assets oder Assets Essentials mit jedem Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Assets Essentials gesendet wurden, werden nicht für den gesamten Dokumentspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden für den gesamten Speicher gezählt.

Metadatenfelder werden zuerst zugeordnet, wenn Sie ein Asset von Workfront an Experience Manager Assets oder Assets Essentials senden. Wenn Ihr Workfront-Administrator die Synchronisierung von Objektmetadaten aktiviert hat, bleiben die Felder auf dem neuesten Stand, wenn sie in einer der Anwendungen geändert werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>Anfrage oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über Experience Manager as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-Berechtigungen</td> 
    <td>Sie müssen Schreibzugriff auf den Ordner haben.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Ansichtszugriff oder höher</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Verknüpfen von Assets aus Experience Manager Assets oder Assets Essentials

Sie können ein Asset aus Experience Manager Assets oder Assets Essentials mit Workfront verknüpfen. Sobald das Asset verknüpft ist, können Sie Folgendes tun

* [Testen eines verknüpften Assets für Experience Manager Assets oder Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Hochladen einer neuen Version eines Dokuments](../../documents/managing-documents/upload-new-document-version.md)

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Wählen Sie **Neu hinzufügen** und dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und darf daher Assets oder Assets Essentials nicht explizit erwähnen.

1. Wählen Sie die gewünschten Assets.

   ![Asset auswählen](assets/select-an-asset.png)

1. Klicken Sie **Auswählen**.

## Verknüpfen von Ordnern aus Experience Manager Assets oder Assets Essentials

Die Berechtigungen zum Anzeigen einzelner Assets innerhalb eines Ordners basieren auf Experience Manager Assets- oder Assets Essentials-Berechtigungen.

1. Wechseln Sie zum **Dokumente** in Workfront, in dem Sie den Ordner ablegen möchten.
1. Wählen Sie **Neu hinzufügen** und dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und erwähnt daher möglicherweise nicht speziell Assets oder Assets Essentials.

1. Wählen Sie die gewünschten Ordner.

   ![Ordner auswählen](assets/select-a-folder.png)

1. Klicken Sie **Auswählen**.

## Verknüpfen einer neuen Version aus Experience Manager Assets oder Assets Essentials

Sie können ein neues Asset aus Assets Essentials abrufen und es einem vorhandenen Asset als neue Version hinzufügen. Wenn das Dokument bereits verknüpft ist und in Assets Essentials eine neue Version hinzugefügt wurde, wird die neue Version automatisch in Workfront angezeigt.

So verknüpfen Sie eine neue Version von Assets Essentials:

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Wählen Sie das Asset aus, das Sie durch eine neue Version ersetzen möchten. Sie können keine neue Version eines Assets in einem verknüpften Ordner erstellen.
1. Wählen Sie **Neu hinzufügen** > **Version** und wählen Sie dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und erwähnt daher möglicherweise nicht speziell Assets oder Assets Essentials.

1. Wählen Sie das gewünschte Asset aus.

   ![Asset auswählen](assets/select-an-asset.png)

1. Klicken Sie **Auswählen**.

>[!TIP]
>
>Sie können alle Versionen eines Assets anzeigen, indem Sie zu **Dokumentdetails** > **Versionen** gehen.
