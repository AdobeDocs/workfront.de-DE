---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Ändern der interaktiven Auflösung von Korrekturabzügen im Proofing Viewer
description: Sie können eine Vorschau davon anzeigen, wie ein interaktiver Korrekturabzug auf verschiedenen Geräten aussieht, sodass Sie sehen können, wie Inhalte basierend auf verschiedenen Auflösungen angezeigt werden und wie sie reagieren.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 1%

---

# Ändern der interaktiven Auflösung von Korrekturabzügen im Proofing Viewer

Sie können eine Vorschau davon anzeigen, wie ein interaktiver Korrekturabzug auf verschiedenen Geräten aussieht, sodass Sie sehen können, wie Inhalte basierend auf verschiedenen Auflösungen angezeigt werden und wie sie reagieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Auswählen oder Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Geräte- und Auflösungsansichten im Desktop Proofing Viewer im Vergleich zum Web Proofing Viewer

Ihr Adobe Workfront-Administrator hat Ihr System so konfiguriert, dass Sie interaktive Inhalte entweder im Desktop Proofing Viewer oder, als gebündelte Inhalte in einer ZIP-Datei, im Web Proofing Viewer überprüfen können:

* Im Desktop Proofing Viewer können Sie sehen, wie Inhalte sowohl in verschiedenen Auflösungen als auch auf verschiedenen Geräten angezeigt und reagiert werden. Wenn ein Reviewer ein bestimmtes Gerät angibt, wird der Inhalt mit den Benutzeroberflächenspezifikationen für das Gerät wie auf dem Gerät angezeigt. Beispielsweise kann eine rote Schaltfläche auf einer Smartphone-Marke bei einer anderen Marke blau sein.

* Im Web Proofing Viewer können Sie interaktive Inhalte so anzeigen, wie sie in den Auflösungen für die verschiedenen Geräte angezeigt werden. Der Web Proofing Viewer emuliert den Inhalt jedoch nicht mithilfe von Schnittstellenspezifikationen auf diesen Geräten, z. B. Schaltflächenfarbe.

  >[!NOTE]
  >
  >Ihr Workfront-Administrator kann benutzerdefinierte Geräte für Benutzende in Ihrer Organisation konfigurieren, wie unter [Konfigurieren von benutzerdefinierten Geräten für Korrekturabzüge](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#configure-custom-devices-for-proofs) im Artikel [Konfigurieren der Korrekturabzugseinstellungen für Ihre Organisation](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) beschrieben.

## Anzeigen eines Korrekturabzugs mit einem vordefinierten Gerät oder einer vordefinierten Auflösungseinstellung

1. Navigieren Sie zur Dokumentliste, die den Korrekturabzug enthält, den Sie öffnen möchten.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf **Korrekturabzug öffnen**.
1. Klicken **unten in** Mitte der Proofing-Anzeige auf „Responsiv“.

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. Klicken Sie im Desktop Proofing Viewer in der angezeigten Liste der Geräte und Lösungen auf das gewünschte Gerät.

   Oder

   Klicken Sie im Web Proofing Viewer in der angezeigten Liste der Auflösungen auf die gewünschte Auflösung.

   Informationen zu den Unterschieden zwischen diesen beiden Viewern finden Sie unter [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer - Übersicht](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   Der interaktive Korrekturabzug wird in der ausgewählten Auflösung gerendert.

## Korrekturabzug mit einer benutzerdefinierten Auflösungseinstellung anzeigen

1. Navigieren Sie zur Dokumentliste, die den Korrekturabzug enthält, den Sie öffnen möchten.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf **Korrekturabzug öffnen**.
1. Klicken **unten in** Mitte der Proofing Viewer auf „Responsiv“.
1. Geben Sie eine benutzerdefinierte **responsive**-Auflösung ein.

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   Oder

   Bewegen Sie den Mauszeiger über Ihren interaktiven Inhalt und ziehen Sie den blauen Rahmen auf die untere rechte Ecke oder die rechte oder untere Kante, um die gewünschte Auflösung zu erhalten.

   ![Drag_blue_edges_for_resolution.png](assets/drag-blue-edges-for-resolution-350x251.png)

   Die benutzerdefinierte Auflösung wird an den folgenden Stellen angezeigt:

   * Im Bedienfeld **Auflösung** unten in der Mitte des Viewers.\
     ![screen_shot_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * In allen Kommentaren fügen Prüfer zum Korrekturabzug hinzu. Jeder Kommentar enthält die Bildschirmauflösung, die beim Erstellen des Kommentars durch den Reviewer ausgewählt wurde.
