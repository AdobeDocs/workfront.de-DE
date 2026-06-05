---
title: Verknüpfen von Assets und Ordnern mit dem erweiterten Connector
description: Sie können ein Asset oder einen Ordner aus Experience Manager Assets mit jedem Workfront-Objekt verknüpfen, das Dokumente unterstützt.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
TQID: https://experienceleague.adobe.com/e7Lmt14iKZNJpq3MirbKST-KjdZJODNbG9pbmvZveeU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 519
ht-degree: 13%

---

# Verknüpfen von Assets und Ordnern mit dem erweiterten Connector

Sie können ein Asset oder einen Ordner aus Experience Manager Assets mit jedem Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Experience Manager Assets gesendet werden, werden nicht für den gesamten Dokumentenspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Experience Manager Assets gesendet wurden, zählen beim Gesamtspeicher.


>[!NOTE]
>
>Excel-Dateien, die über den erweiterten Connector verknüpft sind, können in Workfront nicht in der Vorschau angezeigt werden. Sie müssen die Datei herunterladen, um darauf zugreifen zu können.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf ein Dokument anzeigen oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>


Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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

   ![Asset auswählen](assets/select-an-asset.png)

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

   ![Ordner auswählen](assets/select-a-folder.png)

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

   ![Asset auswählen](assets/select-an-asset.png)

1. Klicken Sie auf **Link**.
