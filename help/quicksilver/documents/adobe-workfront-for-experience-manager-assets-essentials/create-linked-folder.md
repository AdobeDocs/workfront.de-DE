---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Erstellen eines Ordners, der mit Experience Manager Assets oder Assets Essentials verknüpft ist
description: In Workfront können Sie einen Ordner erstellen, der mit Experience Manager Assets oder Assets Essentials verknüpft ist.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 84760d5fe301bd0a44879490fb030bd29821bd41
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Erstellen eines Ordners, der mit Experience Manager Assets oder Assets Essentials verknüpft ist

In Workfront können Sie einen Ordner erstellen, der mit Experience Manager Assets oder Assets Essentials verknüpft ist. Da der Ordner verknüpft ist, wird jedes zum Ordner hinzugefügte Asset automatisch sowohl in Workfront als auch in Experience Manager angezeigt. Sie müssen das Asset nicht manuell senden, wenn es sich in einem verknüpften Ordner befindet.

Wenn ein Asset aus einem verknüpften Ordner innerhalb von Experience Manager Assets oder Assets Essentials gelöscht oder verschoben wird, behält Workfront eine Kopie des Assets im Bereich Projekt > Dokumente bei.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>Adobe Workfront-Plan*</strong>
   </td>
   <td>Beliebig
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenzen*</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td>Sie müssen über Experience Manager Assets as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzerin bzw. Benutzer hinzugefügt werden.
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager-Berechtigungen</strong>
   </td>
   <td>Sie müssen über Schreibzugriff auf den Zielordner in der Experience Manager-Integration verfügen.
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen der Zugriffsebene</strong>
   </td>
   <td>Sie müssen ein Workfront-Administrator sein, um eine Experience Manager-Integration zu konfigurieren. Nach der Konfiguration können Benutzer mit Planlizenz verknüpfte Ordner für einzelne Projekte einrichten.
   </td>
  </tr>
</table>


*Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Verknüpften Ordner erstellen

Der verknüpfte Ordner wird an dem Speicherort erstellt, der vom Workfront-Administrator bei der Einrichtung der Integration angegeben wurde. Jede Integration kann nur einen Ordnerspeicherort für verknüpfte Ordner haben.

Der Name des verknüpften Ordners wird automatisch auf Grundlage des Portfolios, des Programms und des zugehörigen Projekts erstellt und kann nicht geändert werden. Wenn das Projekt keinem Portfolio oder Programm zugeordnet ist, zeigt der verknüpfte Ordner den Projektnamen und das Erstellungsdatum an.

So erstellen Sie einen verknüpften Ordner:

1. Wechseln Sie zu dem Projekt, in dem Sie den Ordner haben möchten.
1. Wählen Sie **Neu hinzufügen** und navigieren Sie dann zur Experience Manager-Integration, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen, sodass Experience Manager Assets oder Assets Essentials möglicherweise nicht explizit erwähnt werden.

1. Wählen Sie **Verknüpften Ordner erstellen** aus. Das System erstellt automatisch einen Ordner im Experience Manager basierend auf dem Speicherort, der beim Einrichten der Integration angegeben wurde.
   ![Verknüpften Ordner erstellen](assets/linked-folder.png)
