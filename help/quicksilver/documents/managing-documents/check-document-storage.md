---
product-area: documents
navigation-topic: manage-documents
title: Überprüfen der Speicherbeschränkungen für Dokumente
description: Als Adobe Workfront-Administrator können Sie die Nutzung und das Kontingent des Dokumentenspeichers auf der Seite Kundeninformationen einsehen. Wie Speicher aussieht, hängt davon ab, ob Ihr Unternehmen ältere Workfront-Speicher oder Adobe Enterprise-Speicher verwendet.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7b6d24d6a5b7fd052a3e7c97034e920e771022a6
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 8%

---

# Überprüfen der Speicherbeschränkungen für Dokumente

{{highlighted-preview}}

Es gibt zwar keine Einschränkungen hinsichtlich der Typen und Größen einzelner Dateien, die Benutzerinnen und Benutzer in Ihre Workfront-Instanz hochladen können, Ihr Workfront-Plan umfasst jedoch ein Gesamtspeicherkontingent. Als Workfront-Administrator überwachen Sie die Nutzung und das Kontingent über den Bereich „Setup“ auf der Seite „Kundeninformationen“.

Wie Speicher aussieht, hängt davon ab, ob Ihr Unternehmen ältere Workfront-Speicher oder Adobe Enterprise-Speicher verwendet:

* Wenn Sie Legacy-Workfront-Speicher verwenden, lesen Sie [Legacy-Workfront-Speicher](#legacy-workfront-storage) in diesem Artikel.
* Wenn Sie Adobe Enterprise Storage verwenden, lesen Sie [Adobe Enterprise Storage](#adobe-enterprise-storage) in diesem Artikel.

  Weitere Informationen zu Massenspeicher für Unternehmen finden Sie unter [Übersicht über Speicher für Unternehmen in Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront-Plan</td> 
   <td> <p>Jedes Workfront-Paket zum Verwalten von Dokumenten unter Verwendung des alten Speichers</p>
      <p>Beliebiges Workflow-Paket zum Verwalten von Dokumenten mit Adobe Enterprise Storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Legacy Workfront-Speicher

Wenn Ihr Unternehmen Legacy-Workfront-Speicher verwendet, wird auf der Seite „Kundeninformationen“ ein einziges Speicherkontingent für Dokumente angezeigt, die direkt in Workfront hochgeladen werden.

So überprüfen Sie den alten Workfront-Dokumentspeicher:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Kundeninformationen**.
1. Suchen Sie im Abschnitt **Grundlegende Informationen** nach **Speicherkontingent**. Hier können Sie anzeigen, wie viel Speicher Sie derzeit verwenden, sowie die Gesamtmenge des Speichers, den Ihr Workfront-Plan beinhaltet.

Das Speicherkontingent wird täglich aktualisiert, um die aktuellste Anzahl anzuzeigen.

>[!NOTE]
>
>Diese Beschränkung gilt nicht für Dokumente, die Sie von einem anderen Drittanbieter (SharePoint, Google Drive, Webdam, Box, Dropbox oder einem anderen Anbieter von Dokumenten-Asset-Management) mit Workfront verknüpfen.

<div class="preview">

## Adobe Enterprise-Speicher

<!--
If your organization uses Adobe enterprise storage, your storage quota is reported as a single pooled allocation that combines storage provisioned through your V2 Workfront SKU and any storage provisioned through a Frame.io Enterprise SKU or add-on. There's no hard cap on storage usage; users can continue uploading documents even when usage exceeds your quota.

Beginning with the May 2026 release, you can view your pooled storage quota and a usage breakdown on the Customer Info page.

-->

### Anzeigen der Speichernutzung in Kundeninformationen

So überprüfen Sie den Adobe Enterprise-Dokumentenspeicher:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Kundeninformationen**.
1. Gehen Sie zum Abschnitt **Speicherübersicht**.
1. Überprüfen Sie Ihre Verwendung. Die Speicherübersicht zeigt Ihr Speicherkontingent im Pool und unterteilt die Nutzung in:

   * Ältere Workfront-Projekte und Speicherprojekte für Adobe Enterprise werden in der blauen Leiste angezeigt.
   * Einzelne Projekte werden in der grünen Leiste angezeigt. Diese Projekte sind unabhängig von Workfront und nur verfügbar, wenn Sie über eine Frame.io Enterprise-Lizenz verfügen.


![Nutzung von Adobe Enterprise-Speicher in Kundeninformationen](assets/storage-usage.png)

Die Nutzungsdaten werden regelmäßig aktualisiert, sodass Sie eine aktuelle Zählung sehen.

### E-Mail-Benachrichtigungen für Administratoren

Wenn die Nutzung 75 %, 90 % oder 100 % Ihres Speicherkontingents überschreitet, sendet Workfront eine E-Mail-Benachrichtigung an Systemadministratoren.

</div>