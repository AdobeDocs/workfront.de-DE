---
title: Verknüpfen von Assets und Ordnern mit dem erweiterten Connector
description: Sie können ein Asset oder einen Ordner aus Experience Manager Assets mit jedem Workfront-Objekt verknüpfen, das Dokumente unterstützt.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: dd8718b00a310bee6caa13db7644b86174b476f4
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---


# Verknüpfen von Assets und Ordnern mit dem erweiterten Connector

Sie können ein Asset oder einen Ordner aus Experience Manager Assets mit jedem Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Experience Manager Assets gesendet werden, werden nicht für den gesamten Dokumentenspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Experience Manager Assets gesendet wurden, zählen beim Gesamtspeicher.


>[!NOTE]
>
>Excel-Dateien, die über den erweiterten Connector verknüpft sind, können in Workfront nicht in der Vorschau angezeigt werden. Sie müssen die Datei herunterladen, um darauf zugreifen zu können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktuell: Anforderung oder höher</p> 
   oder
   <p>Neu: Mitwirkender oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf ein Dokument anzeigen oder höher</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.
+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Installieren des erweiterten Connectors für Workfront for Experience Manager

## Verknüpfen von Assets aus Experience Manager Assets

Sie können ein Asset von Experience Manager Assets mit Workfront verknüpfen. Sobald das Asset verknüpft ist, können Sie Folgendes tun

* [Testen eines verknüpften Assets für Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Hochladen einer neuen Version eines Dokuments](../../../documents/managing-documents/upload-new-document-version.md)

So verknüpfen Sie ein Asset mit Experience Manager Assets:

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Klicken Sie **Neu hinzufügen** und wählen Sie dann die von Ihrem Administrator eingerichtete Experience Manager Assets-Integration aus.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name ausgewählt werden, sodass Experience Manager Assets nicht explizit erwähnt wird.

1. Wählen Sie die gewünschten Assets.

   ![](assets/select-an-asset.png)

1. Klicken Sie auf **Link**.

## Verknüpfen von Ordnern aus Experience Manager Assets

Berechtigungen zum Anzeigen einzelner Assets innerhalb eines Ordners sind von Experience Manager Assets-Berechtigungen abhängig.

So verknüpfen Sie einen Ordner mit Experience Manager Assets:

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Klicken Sie **Neu hinzufügen** und wählen Sie dann die von Ihrem Administrator eingerichtete Experience Manager Assets-Integration aus.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name ausgewählt werden, sodass Experience Manager Assets nicht explizit erwähnt wird.

1. Wählen Sie die gewünschten Ordner.

   ![](assets/select-a-folder.png)

1. Klicken Sie auf **Link**.

## Verknüpfen einer neuen Version aus Experience Manager Assets

Sie können ein neues Asset aus Experience Manager Assets abrufen und es einem vorhandenen Asset als neue Version in Workfront hinzufügen. Wenn das Dokument bereits verknüpft ist und in Experience Manager Assets eine neue Version hinzugefügt wurde, wird die neue Version automatisch in Workfront angezeigt.

>[!TIP]
>
>Sie können alle Versionen eines Assets anzeigen, indem Sie zu **Dokumentdetails** > **Versionen** gehen.

So verknüpfen Sie eine neue Version aus Experience Manager Assets:

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Wählen Sie das Asset aus, das Sie durch eine neue Version ersetzen möchten. Sie können keine neue Version eines Assets in einem verknüpften Ordner erstellen.
1. Klicken Sie **Neu hinzufügen** und wählen Sie dann die von Ihrem Administrator eingerichtete Experience Manager Assets-Integration aus.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name ausgewählt werden, sodass Experience Manager Assets nicht explizit erwähnt wird.

1. Wählen Sie das gewünschte Asset aus.

   ![](assets/select-an-asset.png)

1. Klicken Sie auf **Link**.
