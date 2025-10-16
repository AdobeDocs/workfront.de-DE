---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Senden eines Dokuments an Experience Manager Assets oder Assets Essentials
description: Sie können Dokumente von Workfront an Experience Manager Assets oder Assets Essentials senden. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden weiterhin für den gesamten Dokumentspeicher gezählt. Assets, das über Assets Essentials verknüpft ist, wird nicht für den gesamten Speicher angerechnet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '868'
ht-degree: 0%

---

# Senden eines Dokuments an Experience Manager Assets oder Assets Essentials

Sie können Dokumente von Workfront an Experience Manager Assets oder Assets Essentials senden. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden weiterhin für den gesamten Dokumentspeicher gezählt. Assets, das über Assets Essentials verknüpft ist, wird nicht für den gesamten Speicher angerechnet.

Für Assets, die über diese Integration an Experience Manager gesendet werden, gilt eine Größenbeschränkung von **5 GB**.

In der Vorschau-Umgebung sind für Assets, die über diese Integration an Experience Manager gesendet werden, Größenbeschränkungen von **30 GB** vorgesehen.

Metadatenfelder werden zuerst zugeordnet, wenn Sie ein Asset von Workfront an Experience Manager Assets oder Assets Essentials senden. Alle Metadaten, die für die Zuordnung übergeordneter Objekte konfiguriert wurden, werden ebenfalls gesendet. Weitere Informationen zum Konfigurieren der Metadatenzuordnung finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Beispiel** Wenn Sie zum ersten Mal ein an eine Aufgabe angehängtes Asset senden, werden die Aufgabenmetadaten Experience Manager Assets oder Assets Essentials sowie alle zugeordneten Metadaten aus übergeordneten Objekten wie einem Projekt, einem Portfolio und einem Programm zugeordnet.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <p>Mitwirkender oder höher</p> 
   <p>Anfrage oder höher</p> </td> 
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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Ansichtszugriff oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Senden eines Dokuments aus Workfront

Wenn ein(e) Benutzende(r) ein Dokument von Workfront an Experience Manager Assets oder Assets Essentials sendet, werden zugeordnete Metadaten entlang des Dokuments übertragen. Nachdem das Dokument gesendet wurde, werden Änderungen an den Metadaten des Dokuments in Workfront nicht in Assets oder Assets Essentials übernommen. Wenn ein zugeordnetes Feld in Workfront geändert wird, müssen Sie eine neue Version des Dokuments mit den aktualisierten Metadaten an Assets oder Assets Essentials senden. Informationen zum Einrichten oder Bearbeiten von Metadaten finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Senden eines Dokuments:

1. Wechseln Sie zum Bereich **Dokumente** in Workfront und wählen Sie das Dokument aus, das Sie senden möchten.
1. Klicken Sie **Senden an** und wählen Sie dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und darf daher Assets oder Assets Essentials nicht explizit erwähnen.

   ![Senden an](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Wählen Sie aus, wohin das Asset gesendet werden soll, und klicken Sie dann auf **Ordner auswählen**.
1. Wenn Sie das gewünschte Ziel gefunden haben, klicken Sie auf **Speichern**.

## Neue Version senden

Sie können zu einem Dokument, das Sie zuvor in Workfront hochgeladen haben, eine neue Version hinzufügen. Weitere Informationen finden Sie unter [Hochladen einer neuen Version eines Dokuments](../../documents/managing-documents/upload-new-document-version.md). Nachdem die neueste Version hochgeladen wurde, können Sie sie an Assets Essentials senden. Wenn sich ein zugeordnetes Feld in Workfront geändert hat, aktualisiert die neue Version beim Senden die Metadaten in Assets Essentials.

>[!IMPORTANT]
>
>Bevor Sie eine neue Version in Workfront hochladen, empfehlen wir, die Datei umzubenennen. Wenn Sie eine neue Version mit genau demselben Dateinamen wie eine frühere Version hochladen, kann nur die neueste Version von Workfront heruntergeladen werden. Alle Versionen können unabhängig vom Dateinamen von Experience Manager Assets oder Assets Essentials heruntergeladen werden.

So senden Sie die neueste Version:

1. Navigieren Sie zum Bereich **Dokumente** in Workfront und suchen Sie das Dokument.
1. Wählen Sie **Senden an** und dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und erwähnt daher möglicherweise nicht speziell Assets oder Assets Essentials.

   ![Senden an](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klicken Sie auf **Speichern**. Die neue Version wird am selben Speicherort wie die vorherige Version gespeichert.

## Verschieben eines Dokuments in einen verknüpften Ordner in Experience Manager Assets

>[!NOTE]
>
>Diese Funktion ist nur für Experience Manager Assets as a Cloud Service verfügbar. Es ist nicht für Experience Manager Assets Essentials verfügbar.

Sie können ein Dokument in einen verknüpften Ordner in Experience Manager Assets verschieben, wenn sich sowohl das Dokument als auch der verknüpfte Ordner in derselben Dokumentliste befinden (z. B. der Dokumentbereich eines Projekts).

1. Suchen Sie das Dokument, das Sie verschieben möchten.
1. Ziehen Sie das Dokument per Drag-and-Drop auf den verknüpften Experience Manager Assets-Ordner, in den Sie es verschieben möchten.

Die Dokumentoptionen sind nicht verfügbar, während das Dokument verschoben wird. Nachdem das Dokument in Experience Manager Assets verschoben wurde, ist in der Dokumentliste in Workfront nicht mehr sichtbar.

>[!NOTE]
>
> Alle Aktionen oder Bearbeitungen, die Sie am Dokument vornehmen, während es verschoben wird, werden nicht im Dokument in Experience Manager Assets angezeigt und gehen daher verloren.

