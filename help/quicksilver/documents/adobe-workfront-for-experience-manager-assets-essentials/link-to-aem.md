---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verknüpfen von Assets und Ordnern aus Experience Manager Assets oder Assets Essentials
description: Sie können ein Asset oder einen Ordner aus Experience Manager Assets oder Assets Essentials mit jedem Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Assets Essentials versandt werden, werden nicht auf den gesamten Dokumentenspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden für den Gesamtspeicher mitgezählt.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Verknüpfen von Assets und Ordnern aus Experience Manager Assets oder Assets Essentials

Sie können ein Asset oder einen Ordner aus Experience Manager Assets oder Assets Essentials mit jedem Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Assets Essentials versandt werden, werden nicht auf den gesamten Dokumentenspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden für den Gesamtspeicher mitgezählt.

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
   <td>Sie müssen über Experience Manager-as a Cloud Service oder Assets Essentialss verfügen und dem Produkt als Benutzerin bzw. Benutzer in der Admin Console hinzugefügt werden.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Berechtigungen für Experience Manager</td> 
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
1. Klicken Sie **Neu hinzufügen** und wählen Sie dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Assets oder Assets Essentials möglicherweise nicht explizit erwähnt werden.

1. Wählen Sie die gewünschten Assets.

   ![](assets/select-an-asset.png)

1. Klicken Sie **Auswählen**.

## Verknüpfen von Ordnern aus Experience Manager Assets oder Assets Essentials

Die Berechtigungen zum Anzeigen einzelner Assets in einem Ordner hängen von den Berechtigungen von Experience Manager Assets oder Assets Essentials ab.

1. Wechseln Sie zum **Dokumente** in Workfront, in dem Sie den Ordner ablegen möchten.
1. Klicken Sie **Neu hinzufügen** und wählen Sie dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Assets oder Assets Essentials möglicherweise nicht explizit erwähnt werden.

1. Wählen Sie die gewünschten Ordner.

   ![](assets/select-a-folder.png)

1. Klicken Sie **Auswählen**.

## Verknüpfen neuer Versionen von Experience Manager Assets oder Assets Essentials

Sie können ein neues Asset aus den Assets Essentials abrufen und es als neue Version einem vorhandenen Asset hinzufügen. Wenn das Dokument bereits verknüpft ist und eine neue Version in Assets Essentials hinzugefügt wurde, wird die neue Version automatisch in Workfront angezeigt.

So verknüpfen Sie eine neue Version aus Assets Essentials:

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Wählen Sie das Asset aus, das Sie durch eine neue Version ersetzen möchten. Sie können keine neue Version eines Assets in einem verknüpften Ordner erstellen.
1. Wählen Sie **Neu hinzufügen** > **Version** und wählen Sie dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Assets oder Assets Essentials möglicherweise nicht explizit erwähnt werden.

1. Wählen Sie das gewünschte Asset aus.

   ![](assets/select-an-asset.png)

1. Klicken Sie **Auswählen**.

>[!TIP]
>
>Sie können alle Versionen eines Assets anzeigen, indem Sie zu **Dokumentdetails** > **Versionen** gehen.
