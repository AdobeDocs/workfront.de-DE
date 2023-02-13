---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Erstellen eines Ordners, der mit Experience Manager Assets oder Assets Essentials verknüpft ist
description: Sie können in Workfront einen Ordner erstellen, der mit Experience Manager Assets oder Assets Essentials verknüpft ist.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Erstellen eines Ordners, der mit Experience Manager Assets oder Assets Essentials verknüpft ist

Sie können in Workfront einen Ordner erstellen, der mit Experience Manager Assets oder Assets Essentials verknüpft ist. Da der Ordner verknüpft ist, werden alle dem Ordner hinzugefügten Assets automatisch sowohl in Workfront als auch in Experience Manager angezeigt. Sie müssen das Asset nicht manuell senden, wenn es sich in einem verknüpften Ordner befindet.


## Zugriffsanforderungen

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
   <td>Sie müssen über Experience Manager Assets as a Cloud Service oder Assets Essentials verfügen und dem Produkt als Benutzer hinzugefügt werden.
   </td>
  </tr>
  <tr>
   <td><strong>Berechtigungen für Experience Manager</strong>
   </td>
   <td>Sie müssen über Schreibzugriff auf den Zielordner in der Experience Manager-Integration verfügen.
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen auf Zugriffsebene</strong>
   </td>
   <td>Sie müssen Workfront-Administrator sein. Informationen zu Workfront-Administratoren finden Sie unter <strong>Gewähren eines vollen Administratorzugriffs</strong>.
   </td>
  </tr>
</table>


*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.


## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der as a Cloud Service Integration von Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Integration von Experience Manager Assets Essentials konfigurieren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Verknüpften Ordner erstellen

Der verknüpfte Ordner wird an dem Speicherort erstellt, der vom Workfront-Administrator beim Einrichten der Integration angegeben wird. Jede Integration kann nur einen Ordnerspeicherort für verknüpfte Ordner haben.

Der Name des verknüpften Ordners wird automatisch basierend auf dem Portfolio, dem Programm und dem zugehörigen Projekt erstellt und kann nicht geändert werden. Wenn das Projekt nicht mit einem Portfolio oder Programm verknüpft ist, zeigt der verknüpfte Ordner den Projektnamen und das Erstellungsdatum an.

So erstellen Sie einen verknüpften Ordner:



1. Wechseln Sie zu dem Projekt, in dem Sie den Ordner ablegen möchten.
1. Auswählen **Neu hinzufügen** und gehen Sie dann zur Experience Manager-Integration, die Ihr Administrator eingerichtet hat.
   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration wählen, sodass Experience Manager Assets oder Assets Essentials möglicherweise nicht speziell erwähnt werden.

1. Auswählen **Verknüpften Ordner erstellen**. Das System erstellt automatisch einen Ordner in Experience Manager basierend auf dem Speicherort, der beim Einrichten der Integration angegeben wurde.
   ![Erstellen eines verknüpften Ordners](assets/linked-folder.png)
