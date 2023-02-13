---
title: Verknüpfen von Assets und Ordnern mit dem erweiterten Connector
description: Sie können ein Asset oder einen Ordner aus Experience Manager Assets mit einem beliebigen Workfront-Objekt verknüpfen, das Dokumente unterstützt.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Verknüpfen von Assets und Ordnern mit dem erweiterten Connector

Sie können ein Asset oder einen Ordner aus Experience Manager Assets mit einem beliebigen Workfront-Objekt verknüpfen, das Dokumente unterstützt. Von Experience Manager Assets gesendete Assets werden nicht auf Ihren gesamten Dokumentenspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Experience Manager Assets gesendet werden, zählen zum Gesamtspeicher.

## Zugriffsanforderungen

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
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf ein Dokument oder höher anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Workfront für Experience Manager-Connector installieren

## Verknüpfen eines Assets mit Experience Manager Assets

Sie können ein Asset von Experience Manager Assets mit Workfront verknüpfen. Sobald das Asset verknüpft ist, können Sie

* [Testen eines verknüpften Assets für Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Eine neue Version eines Dokuments hochladen](../../../documents/managing-documents/upload-new-document-version.md)

So verknüpfen Sie ein Asset mit Experience Manager Assets:

1. Navigieren Sie zu **Dokumente** Bereich in Workfront, in dem Sie das Dokument hinzufügen möchten.
1. Klicken **Neu hinzufügen** und wählen Sie dann die Experience Manager Assets-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name gewählt werden. Daher wird Experience Manager Assets möglicherweise nicht speziell erwähnt.

1. Wählen Sie die gewünschten Assets aus.

   ![](assets/select-an-asset.png)

1. Klicken **Link**.

## Ordner aus Experience Manager Assets verknüpfen

Berechtigungen zum Anzeigen einzelner Assets innerhalb eines Ordners hängen von den Experience Manager Assets-Berechtigungen ab.

So verknüpfen Sie einen Ordner mit Experience Manager Assets:

1. Navigieren Sie zu **Dokumente** Bereich in Workfront, in dem Sie das Dokument hinzufügen möchten.
1. Klicken **Neu hinzufügen** und wählen Sie dann die Experience Manager Assets-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name gewählt werden. Daher wird Experience Manager Assets möglicherweise nicht speziell erwähnt.

1. Wählen Sie die gewünschten Ordner aus.

   ![](assets/select-a-folder.png)

1. Klicken **Link**.

## Neue Version von Experience Manager Assets verknüpfen

Sie können ein neues Asset aus Experience Manager Assets ziehen und es einem vorhandenen Asset als neue Version in Workfront hinzufügen. Wenn das Dokument bereits verknüpft ist und eine neue Version in Experience Manager Assets hinzugefügt wird, wird die neue Version automatisch in Workfront angezeigt.

>[!TIP]
>
>Sie können alle Versionen eines Assets anzeigen, wenn Sie **Dokumentdetails** > **Versionen**.

So verknüpfen Sie eine neue Version von Experience Manager Assets:

1. Navigieren Sie zu **Dokumente** Bereich in Workfront, in dem Sie das Dokument hinzufügen möchten.
1. Wählen Sie das Asset aus, das Sie durch eine neue Version ersetzen möchten. Sie können keine neue Version eines Assets in einem verknüpften Ordner erstellen.
1. Klicken **Neu hinzufügen** und wählen Sie dann die Experience Manager Assets-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name gewählt werden. Daher wird Experience Manager Assets möglicherweise nicht speziell erwähnt.

1. Wählen Sie das gewünschte Asset aus.

   ![](assets/select-an-asset.png)

1. Klicken **Link**.
