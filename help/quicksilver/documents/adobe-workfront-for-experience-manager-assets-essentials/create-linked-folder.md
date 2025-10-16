---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Erstellen eines mit Experience Manager Assets oder Assets Essentials verknüpften Ordners
description: Sie können in Workfront einen Ordner erstellen, der mit Experience Manager Assets oder Assets Essentials verknüpft ist.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Erstellen eines mit Experience Manager Assets oder Assets Essentials verknüpften Ordners

Sie können in Workfront einen Ordner erstellen, der mit Experience Manager Assets oder Assets Essentials verknüpft ist. Da der Ordner verknüpft ist, wird jedes zum Ordner hinzugefügte Asset automatisch sowohl in Workfront als auch in Experience Manager angezeigt. Sie müssen das Asset nicht manuell senden, wenn es sich in einem verknüpften Ordner befindet.

Wenn ein Asset aus einem verknüpften Ordner innerhalb von Experience Manager Assets oder Assets Essentials gelöscht oder verschoben wird, behält Workfront eine Kopie des Assets im Bereich Projekt > Dokumente bei.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table>
  <tr>
   <td><strong>Adobe Workfront-Paket</strong>
   </td>
   <td>Beliebig
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenzen</strong>
   </td>
   <td>
   <p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
  <tr>
   <td><strong>Zusätzliche Produkte</strong>
   </td>
   <td>Sie müssen über Experience Manager Assets as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzer hinzugefügt werden.
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
   <td>Sie müssen ein Workfront-Administrator sein, um eine Experience Manager-Integration konfigurieren zu können. Nach der Konfiguration können Benutzer mit Planlizenz verknüpfte Ordner für einzelne Projekte einrichten.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Verknüpften Ordner erstellen

Der verknüpfte Ordner wird an dem Speicherort erstellt, der vom Workfront-Administrator bei der Einrichtung der Integration angegeben wurde. Jede Integration kann nur einen Ordnerspeicherort für verknüpfte Ordner haben.

Der Name des verknüpften Ordners wird automatisch auf der Basis von Portfolio, Programm und dem zugehörigen Projekt erstellt und kann nicht geändert werden. Wenn das Projekt nicht mit einer Portfolio oder einem Programm verknüpft ist, zeigt der verknüpfte Ordner den Projektnamen und das Erstellungsdatum an.

>[!NOTE]
>
>Sie können kein neues Dokument oder keine neue Korrekturabzugsversion innerhalb eines verknüpften Ordners erstellen.


So erstellen Sie einen verknüpften Ordner:

1. Wechseln Sie zu dem Projekt, in dem Sie den Ordner haben möchten.
1. Wählen Sie **Neu hinzufügen** und navigieren Sie dann zur Experience Manager-Integration, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und erwähnt daher möglicherweise nicht speziell Experience Manager Assets oder Assets Essentials.

1. Wählen Sie **Verknüpften Ordner erstellen** aus. Das System erstellt automatisch einen Ordner in Experience Manager basierend auf dem Speicherort, der beim Einrichten der Integration angegeben wurde.
   ![Verknüpften Ordner erstellen](assets/linked-folder.png)
