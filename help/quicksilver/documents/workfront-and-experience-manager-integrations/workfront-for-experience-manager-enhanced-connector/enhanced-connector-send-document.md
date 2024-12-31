---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Senden eines Dokuments mit dem erweiterten Connector
description: Sie können Dokumente von Workfront an Experience Manager Assets senden. Dokumente, die von Workfront hochgeladen und an Experience Manager Assets gesendet wurden, werden weiterhin für den gesamten Dokumentspeicher gezählt. Assets, die über Experience Manager Assets verknüpft sind, werden nicht für den gesamten Speicher angerechnet.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# Senden eines Dokuments mit dem erweiterten Connector

Sie können Dokumente von Workfront an Experience Manager Assets senden. Dokumente, die von Workfront hochgeladen und an Experience Manager Assets gesendet wurden, werden weiterhin für den gesamten Dokumentspeicher gezählt. Assets, die über Experience Manager Assets verknüpft sind, werden nicht für den gesamten Speicher angerechnet.

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
   <td> <p>Anfrage oder höher</p> </td> 
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
   <td> <p>Zugriff auf Dokumente anzeigen oder höher</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Installieren Sie den erweiterten Connector von Workfront for Experience Manager.

## Senden eines Dokuments an Experience Manager Assets

Wenn ein(e) Benutzende(r) ein Dokument von Workfront an Experience Manager Assets sendet, werden zugeordnete Metadaten entlang des Dokuments übertragen. Falls konfiguriert, werden die Metadaten bei jeder Änderung kontinuierlich synchronisiert.

Senden eines Dokuments:

1. Wechseln Sie zum Bereich **Dokumente** in Workfront und wählen Sie das Dokument aus, das Sie senden möchten.
1. Klicken Sie **Senden an** und wählen Sie dann die Experience Manager Assets-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name ausgewählt werden, sodass Experience Manager Assets nicht explizit erwähnt wird.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Wählen Sie aus, wohin das Asset gesendet werden soll, und klicken Sie dann auf **Ordner auswählen**.
1. Wenn Sie das gewünschte Ziel gefunden haben, klicken Sie auf **Speichern**.

## Senden einer neuen Version an Experience Manager Assets

Sie können zu einem Dokument, das Sie zuvor in Workfront hochgeladen haben, eine neue Version hinzufügen. Weitere Informationen finden Sie unter [Hochladen einer neuen Version eines Dokuments](../../../documents/managing-documents/upload-new-document-version.md). Nachdem die neueste Version hochgeladen wurde, können Sie sie an Experience Manager Assets senden. Wenn sich ein zugeordnetes Feld in Workfront geändert hat, aktualisiert die neue Version beim Senden die Metadaten in Experience Manager Assets.

So senden Sie die neueste Version:

1. Navigieren Sie zum Bereich **Dokumente** in Workfront und suchen Sie das Dokument.
1. Klicken Sie **Senden an** und wählen Sie dann die Experience Manager Assets-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Für diese Integration kann ein beliebiger Name ausgewählt werden, sodass Experience Manager Assets nicht explizit erwähnt wird.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klicken Sie auf **Speichern**. Die neue Version wird am selben Speicherort wie die vorherige Version gespeichert.
