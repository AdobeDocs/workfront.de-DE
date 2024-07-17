---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verknüpfen von Assets und Ordnern mit Experience Manager Assets oder Assets Essentials
description: Sie können ein Asset oder einen Ordner aus Experience Manager Assets oder Assets Essentials mit einem beliebigen Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Assets Essentials gesendet werden, zählt nicht für Ihren gesamten Dokumentenspeicher in Workfront. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet werden, zählen zur Gesamtspeicherung.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Verknüpfen von Assets und Ordnern mit Experience Manager Assets oder Assets Essentials

Sie können ein Asset oder einen Ordner aus Experience Manager Assets oder Assets Essentials mit einem beliebigen Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Assets Essentials gesendet werden, zählt nicht für Ihren gesamten Dokumentenspeicher in Workfront. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet werden, zählen zur Gesamtspeicherung.

Metadatenfelder werden zuerst zugeordnet, wenn Sie ein Asset von Workfront an Experience Manager Assets oder Assets Essentials senden. Wenn Ihr Workfront-Administrator die Synchronisierung von Objektmetadaten aktiviert hat, bleiben die Felder immer auf dem neuesten Stand, wenn sie in beiden Anwendungen geändert werden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über Experience Manager as a Cloud Service oder Assets Essentials verfügen und dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-Berechtigungen</td> 
    <td>Sie müssen Schreibzugriff auf den Ordner haben.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff anzeigen oder höher</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Verknüpfen eines Assets aus Experience Manager Assets oder Assets Essentials

Sie können ein Asset aus Experience Manager Assets oder Assets Essentials mit Workfront verknüpfen. Sobald das Asset verknüpft ist, können Sie

* [Testen eines verknüpften Assets für Experience Manager Assets oder Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Eine neue Version eines Dokuments hochladen](../../documents/managing-documents/upload-new-document-version.md)

1. Wechseln Sie zum Bereich **Dokumente** in Workfront, in dem Sie das Dokument hinzufügen möchten.
1. Wählen Sie **Neu hinzufügen** und dann die vom Administrator eingerichtete Experience Manager-Integration aus.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration wählen, sodass Assets oder Assets Essentials möglicherweise nicht speziell erwähnt werden.

1. Wählen Sie die gewünschten Assets aus.

   ![](assets/select-an-asset.png)

1. Klicken Sie auf **Select**.

## Ordner aus Experience Manager Assets oder Assets Essentials verknüpfen

Berechtigungen zum Anzeigen einzelner Assets innerhalb eines Ordners erfordern Experience Manager Assets- oder Assets Essentials-Berechtigungen.

1. Wechseln Sie in Workfront zum Bereich **Dokumente** , in dem Sie den Ordner ablegen möchten.
1. Wählen Sie **Neu hinzufügen** und dann die vom Administrator eingerichtete Experience Manager-Integration aus.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration wählen, sodass Assets oder Assets Essentials möglicherweise nicht speziell erwähnt werden.

1. Wählen Sie die gewünschten Ordner aus.

   ![](assets/select-a-folder.png)

1. Klicken Sie auf **Select**.

## Neue Version von Experience Manager Assets oder Assets Essentials verknüpfen

Sie können ein neues Asset aus Assets Essentials ziehen und es einem vorhandenen Asset als neue Version hinzufügen. Wenn das Dokument bereits verknüpft ist und eine neue Version in Assets Essentials hinzugefügt wird, wird die neue Version automatisch in Workfront angezeigt.

So verknüpfen Sie eine neue Version aus Assets Essentials:

1. Wechseln Sie zum Bereich **Dokumente** in Workfront, in dem Sie das Dokument hinzufügen möchten.
1. Wählen Sie das Asset aus, das Sie durch eine neue Version ersetzen möchten. Sie können keine neue Version eines Assets in einem verknüpften Ordner erstellen.
1. Wählen Sie **Neu hinzufügen** > **Version** und wählen Sie dann die vom Administrator eingerichtete Experience Manager-Integration aus.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration wählen, sodass Assets oder Assets Essentials möglicherweise nicht speziell erwähnt werden.

1. Wählen Sie das gewünschte Asset aus.

   ![](assets/select-an-asset.png)

1. Klicken Sie auf **Select**.

>[!TIP]
>
>Sie können alle Versionen eines Assets anzeigen, wenn Sie zu **Dokumentdetails** > **Versionen** navigieren.
