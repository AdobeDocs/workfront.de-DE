---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Senden eines Dokuments mit dem erweiterten Connector
description: Sie können Dokumente von Workfront an Experience Manager Assets senden. Dokumente, die von Workfront hochgeladen und an Experience Manager Assets gesendet wurden, werden weiterhin mit Ihrem gesamten Dokumentenspeicher angerechnet. Von Experience Manager Assets verknüpfte Assets zählen nicht zum Gesamtspeicher.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# Senden eines Dokuments mit dem erweiterten Connector

Sie können Dokumente von Workfront an Experience Manager Assets senden. Dokumente, die von Workfront hochgeladen und an Experience Manager Assets gesendet wurden, werden weiterhin mit Ihrem gesamten Dokumentenspeicher angerechnet. Von Experience Manager Assets verknüpfte Assets zählen nicht zum Gesamtspeicher.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
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
   <td> <p>Zugriff oder höher auf Dokumente anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Installieren Sie den Connector Workfront for Experience Manager.

## Senden eines Dokuments an Experience Manager Assets

Wenn ein Benutzer ein Dokument von Workfront an Experience Manager Assets sendet, werden zugeordnete Metadaten entlang des Dokuments übertragen. Falls konfiguriert, werden die Metadaten bei jeder Änderung kontinuierlich synchronisiert.

So senden Sie ein Dokument:

1. Navigieren Sie zu **Dokumente** und wählen Sie das zu sendende Dokument aus.
1. Klicken **Senden an** und wählen Sie dann die Experience Manager Assets-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name gewählt werden. Daher wird Experience Manager Assets möglicherweise nicht speziell erwähnt.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Wählen Sie aus, wohin das Asset gehen soll, und klicken Sie auf **Ordner auswählen**.
1. Wenn Sie Ihr gewünschtes Ziel finden, klicken Sie auf **Speichern**.

## Neue Version an Experience Manager Assets senden

Sie können einem Dokument, das Sie zuvor in Workfront hochgeladen haben, eine neue Version hinzufügen. Weitere Informationen finden Sie unter [Eine neue Version eines Dokuments hochladen](../../../documents/managing-documents/upload-new-document-version.md). Nachdem die neueste Version hochgeladen wurde, können Sie sie an Experience Manager Assets senden. Wenn sich ein zugeordnetes Feld in Workfront geändert hat, aktualisiert die neue Version die Metadaten in Experience Manager Assets beim Senden.

So senden Sie die neueste Version:

1. Navigieren Sie zu **Dokumente** und suchen Sie nach dem Dokument.
1. Klicken **Senden an** und wählen Sie dann die Experience Manager Assets-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name gewählt werden. Daher wird Experience Manager Assets möglicherweise nicht speziell erwähnt.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klicken Sie auf **Speichern**. Die neue Version speichert am selben Speicherort wie die vorherige Version.
