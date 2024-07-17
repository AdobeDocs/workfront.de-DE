---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Ändern der interaktiven Testversandauflösung im Testversand-Viewer
description: Sie können eine Vorschau eines interaktiven Testversands auf verschiedenen Geräten anzeigen, um zu sehen, wie Inhalte basierend auf verschiedenen Auflösungen angezeigt und darauf reagiert werden.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: d4fa663e22daf25fec77be79a452eb207857bdda
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 1%

---

# Ändern der interaktiven Testversandauflösung im Testversand-Viewer

Sie können eine Vorschau eines interaktiven Testversands auf verschiedenen Geräten anzeigen, um zu sehen, wie Inhalte basierend auf verschiedenen Auflösungen angezeigt und darauf reagiert werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Wählen Sie oder Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Geräte- und Auflösungsansichten im Desktop Proofing Viewer im Vergleich zum Web Proofing Viewer

Ihr Adobe Workfront-Administrator hat Ihr System so konfiguriert, dass Sie interaktive Inhalte entweder im Desktop Proofing Viewer oder, als gebündelte Inhalte in einer ZIP-Datei, im Web Proofing Viewer überprüfen:

* Im Desktop Proofing Viewer können Sie anzeigen, wie Inhalte sowohl in verschiedenen Auflösungen als auch auf verschiedenen Geräten angezeigt und darauf reagiert werden. Wenn ein Validierer ein bestimmtes Gerät angibt, wird der Inhalt so angezeigt, wie er auf diesem Gerät mit den Benutzeroberflächenspezifikationen für das Gerät wäre. Beispielsweise kann eine rote Schaltfläche auf einer Smartphone-Marke auf einer anderen Marke blau sein.

* Im Web Proofing Viewer können Sie interaktive Inhalte so anzeigen, wie sie in den Auflösungen für die verschiedenen Geräte angezeigt werden. Der Web Proofing Viewer emuliert den Inhalt jedoch nicht mithilfe von Benutzeroberflächenspezifikationen auf diesen Geräten, wie z. B. Schaltflächenfarbe.

  >[!NOTE]
  >
  >Ihr Workfront-Administrator kann benutzerdefinierte Geräte für Benutzer in Ihrem Unternehmen konfigurieren, wie unter [Konfigurieren benutzerdefinierter Geräte für Testsendungen](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#configure-custom-devices-for-proofs) im Artikel [Konfigurieren der Testversandeinstellungen für Ihr Unternehmen](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) beschrieben.

## Anzeigen eines Testversands mit einer vordefinierten Geräte- oder Auflösungseinstellung

1. Gehen Sie zur Dokumentliste, die den Testversand enthält, den Sie öffnen möchten.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie auf **Testversand öffnen**.
1. Klicken Sie unten im Testversand-Viewer auf **Responsiv** .

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. Klicken Sie im Desktop Proofing Viewer in der Liste der angezeigten Geräte und Auflösungen auf das gewünschte Gerät.

   Oder

   Klicken Sie im Web Proofing Viewer in der Liste der angezeigten Auflösungen auf die gewünschte Auflösung.

   Informationen dazu, wie sich diese beiden Viewer unterscheiden, finden Sie unter [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer - Übersicht](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   Der interaktive Testversand wird in der von Ihnen ausgewählten Auflösung gerendert.

## Anzeigen eines Testversands mit einer benutzerdefinierten Auflösungseinstellung

1. Gehen Sie zur Dokumentliste, die den Testversand enthält, den Sie öffnen möchten.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie auf **Testversand öffnen**.
1. Klicken Sie unten im Proofing-Viewer auf **Responsive**.
1. Geben Sie eine benutzerdefinierte **Responsive** Auflösung ein.

   ![Typ_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   Oder

   Bewegen Sie den Mauszeiger über Ihren interaktiven Inhalt und ziehen Sie den blauen Rahmen unten rechts oder rechts oder unten auf die gewünschte Auflösung.

   ![Drag_blue_edge_for_resolution.png](assets/drag-blue-edges-for-resolution-350x251.png)

   Die benutzerdefinierte Auflösung wird an den folgenden Stellen angezeigt:

   * Im Bedienfeld **Auflösung** in der unteren Mitte des Viewers.\
     ![Screenshot_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * In allen Kommentaren fügen Überprüfer zum Testversand hinzu. Jeder Kommentar enthält die Bildschirmauflösung, die beim Erstellen des Kommentars durch den Validierer ausgewählt wurde.
