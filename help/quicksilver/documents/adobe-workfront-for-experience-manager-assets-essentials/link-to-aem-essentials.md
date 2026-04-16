---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verknüpfen von Assets und Ordnern aus Experience Manager Assets Essentials
description: Sie können ein Asset oder einen Ordner aus Experience Manager Assets Essentials mit jedem Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt. Assets, die von Assets Essentials gesendet wurden, werden nicht für den gesamten Dokumentspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden für den gesamten Speicher gezählt.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a9dfc5c7838668bd3007c157a4e1a53ab4bd86f5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 12%

---

# Verknüpfen von Assets und Ordnern aus Experience Manager Assets Essentials

Sie können ein Asset oder einen Ordner aus Experience Manager Assets Essentials mit jedem Adobe Workfront-Objekt verknüpfen, das Dokumente unterstützt.

Informationen zum Verknüpfen von Assets und Ordnern aus Experience Manager Assets mithilfe von Content Advisor finden Sie [Verknüpfen von Assets und Ordnern mit Content Advisor auf Basis von Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> 
   <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>Sie müssen über Experience Manager as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-Berechtigungen</td> 
    <td>Sie müssen Schreibzugriff auf den Ordner haben.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Ansichtszugriff oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen:

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [ der Experience Manager Assets Essentials-Integration ](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Verknüpfen von Assets aus Experience Manager Assets Essentials

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Wählen Sie **Neu hinzufügen** und dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und darf daher Experience Manager Assets Essentials nicht explizit erwähnen.

1. Wählen Sie die gewünschten Assets.

   ![Asset auswählen](assets/select-an-asset.png)

1. Klicken Sie auf **Auswählen**.

## Verknüpfen einer neuen Version von Experience Manager Assets Essentials

Sie können ein neues Asset aus Experience Manager Assets Essentials abrufen und es einem vorhandenen Asset als neue Version hinzufügen. Wenn das Dokument bereits verknüpft ist und in Experience Manager Assets Essentials eine neue Version hinzugefügt wird, wird die neue Version automatisch in Workfront angezeigt.

Verknüpfen einer neuen Version:

1. Wechseln Sie zum **Dokumente** in Workfront, wo Sie das Dokument hinzufügen möchten.
1. Wählen Sie das Asset aus, das Sie durch eine neue Version ersetzen möchten. Sie können keine neue Version eines Assets in einem verknüpften Ordner erstellen.
1. Wählen Sie **Neu hinzufügen** > **Version** und wählen Sie dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Experience Manager Assets Essentials möglicherweise nicht explizit erwähnt wird.

1. Wählen Sie das Asset aus, das Sie verknüpfen möchten.

1. Klicken Sie auf **Auswählen**.

## Verknüpfen von Ordnern aus Experience Manager Assets Essentials

Die Berechtigungen zum Anzeigen einzelner Assets innerhalb eines Ordners basieren auf Experience Manager Assets Essentials-Berechtigungen.

1. Wechseln Sie zum **Dokumente** in Workfront, in dem Sie den Ordner ablegen möchten.
1. Wählen Sie **Neu hinzufügen** und dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Experience Manager Assets Essentials möglicherweise nicht explizit erwähnt wird.

1. Wählen Sie die gewünschten Ordner.

   ![Ordner auswählen](assets/select-a-folder.png)

1. Klicken Sie auf **Auswählen**.

## Zu beachten

* Die Funktion „Inhaltsratgeber“ ist für Assets Essentials nicht verfügbar. Informationen zum Verknüpfen von Assets und Ordnern mit Content Advisor finden Sie unter [Verknüpfen von Assets und Ordnern mit Content Advisor auf Basis von Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

* Assets, die von Assets Essentials gesendet wurden, werden nicht für den gesamten Dokumentspeicher in Workfront angerechnet. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden für den gesamten Speicher gezählt.

* Metadatenfelder werden zuerst zugeordnet, wenn Sie ein Asset von Workfront an Experience Manager Assets Essentials senden. Wenn Ihr Workfront-Administrator die Synchronisierung von Objektmetadaten aktiviert hat, bleiben die Felder auf dem neuesten Stand, wenn sie in einer der Anwendungen geändert werden.
