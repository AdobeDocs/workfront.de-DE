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
source-git-commit: e25be455e16beee813e612b983bca1302f129e6f
workflow-type: tm+mt
source-wordcount: '438'
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

Wenn Ihr Unternehmen Adobe Enterprise Storage verwendet, wird in den Kundeninformationen eine Speicherübersicht angezeigt, die die Nutzung in verschiedene Abschnitte für Legacy-Workfront-Speicher, Adobe Enterprise Storage und Frame.io unterteilt. Workfront wendet auch eine Soft Cap auf Uploads an, wenn die Nutzung Ihr Kontingent überschreitet, sodass Benutzer weiterhin Dokumente hochladen können.

### Anzeigen der Speichernutzung in Kundeninformationen

So überprüfen Sie den Adobe Enterprise-Dokumentenspeicher:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Kundeninformationen**.
1. Gehen Sie zum Abschnitt **Speicherübersicht**.
1. Anzeigen der Nutzung von Adobe Enterprise-Speicher.
   <!--Both Workfront and Frame.io usage are broken down separately, but roll up to the total usage for Adobe enterprise storage.-->

![Nutzung von Adobe Enterprise-Speicher in Kundeninformationen](assets/storage-usage.png)

Die Nutzungsdaten werden regelmäßig aktualisiert, sodass Sie eine aktuelle Zählung sehen.

### E-Mail-Benachrichtigungen für Administratoren

Wenn die Nutzung 75 %, 85 % oder 100 % Ihres Speicherkontingents überschreitet, sendet Workfront eine E-Mail-Benachrichtigung an Systemadministratoren.

</div>