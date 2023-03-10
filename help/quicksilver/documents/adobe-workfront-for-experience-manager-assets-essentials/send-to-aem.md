---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Senden eines Dokuments an Experience Manager Assets oder Assets Essentials
description: Sie können Dokumente von Workfront an Experience Manager Assets oder Assets Essentials senden. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden weiterhin mit Ihrem gesamten Dokumentenspeicher angerechnet. Von Assets Essentials verknüpfte Assets zählen nicht zum Gesamtspeicher.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 6bedca2f3394fadc6d6ffbb34654fd1f0194a5d6
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Senden eines Dokuments an Experience Manager Assets oder Assets Essentials


Sie können Dokumente von Workfront an Experience Manager Assets oder Assets Essentials senden. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden weiterhin mit Ihrem gesamten Dokumentenspeicher angerechnet. Von Assets Essentials verknüpfte Assets zählen nicht zum Gesamtspeicher.

Metadatenfelder werden zuerst zugeordnet, wenn Sie ein Asset von Workfront an Experience Manager Assets oder Assets Essentials senden. Alle Metadaten, die für die Zuordnung zu übergeordneten Objekten konfiguriert wurden, werden ebenfalls gesendet. Weitere Informationen zum Konfigurieren der Metadaten-Zuordnung finden Sie unter [Konfigurieren der as a Cloud Service Integration von Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Integration von Experience Manager Assets Essentials konfigurieren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Beispiel** Wenn Sie ein Asset zum ersten Mal senden, das an eine Aufgabe angehängt ist, werden die Aufgabenmetadaten Experience Manager Assets oder Assets Essentials sowie alle zugeordneten Metadaten von übergeordneten Objekten wie einem Projekt, Portfolio und Programm zugeordnet.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-Abo</a>*</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>*</td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über Experience Manager as a Cloud Service oder Assets Essentials verfügen und dem Produkt als Benutzer in der Admin Console hinzugefügt werden.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff oder höher auf Dokumente anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der as a Cloud Service Integration von Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Integration von Experience Manager Assets Essentials konfigurieren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Senden eines Dokuments aus Workfront

Wenn ein Benutzer ein Dokument aus Workfront an Experience Manager Assets oder Assets Essentials sendet, werden zugeordnete Metadaten entlang des Dokuments übertragen. Nachdem das Dokument gesendet wurde, werden Änderungen an den Metadaten des Dokuments in Workfront nicht in Assets oder Assets Essentials übernommen. Wenn ein zugeordnetes Feld in Workfront geändert wird, müssen Sie eine neue Dokumentversion mit den aktualisierten Metadaten an Assets oder Assets Essentials senden. Informationen zum Einrichten oder Bearbeiten von Metadaten finden Sie unter [Konfigurieren der as a Cloud Service Integration von Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Integration von Experience Manager Assets Essentials konfigurieren](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

So senden Sie ein Dokument:

1. Navigieren Sie zu **Dokumente** und wählen Sie das zu sendende Dokument aus.
1. Klicken **Senden an** und wählen Sie dann die vom Administrator eingerichtete Experience Manager-Integration aus.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration wählen, sodass Assets oder Assets Essentials nicht ausdrücklich erwähnt werden.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Wählen Sie aus, wohin das Asset gehen soll, und klicken Sie auf **Ordner auswählen**.
1. Wenn Sie Ihr gewünschtes Ziel finden, klicken Sie auf **Speichern**.

## Neue Version senden

Sie können einem Dokument, das Sie zuvor in Workfront hochgeladen haben, eine neue Version hinzufügen. Weitere Informationen finden Sie unter [Eine neue Version eines Dokuments hochladen](../../documents/managing-documents/upload-new-document-version.md). Nachdem die neueste Version hochgeladen wurde, können Sie sie an Assets Essentials senden. Wenn sich ein zugeordnetes Feld in Workfront geändert hat, aktualisiert die neue Version die Metadaten in Assets Essentials beim Senden.

>[!IMPORTANT]
>
>Bevor Sie eine neue Version in Workfront hochladen, wird empfohlen, die Datei umzubenennen. Wenn Sie eine neue Version mit exakt demselben Dateinamen wie eine frühere Version hochladen, kann nur die neueste Version von Workfront heruntergeladen werden. Alle Versionen können unabhängig vom Dateinamen von Experience Manager Assets oder Assets Essentials heruntergeladen werden.

So senden Sie die neueste Version:

1. Navigieren Sie zu **Dokumente** und suchen Sie nach dem Dokument.
1. Auswählen **Senden an** und wählen Sie dann die vom Administrator eingerichtete Experience Manager-Integration aus.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration wählen, sodass Assets oder Assets Essentials nicht ausdrücklich erwähnt werden.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klicken Sie auf **Speichern**. Die neue Version speichert am selben Speicherort wie die vorherige Version.
