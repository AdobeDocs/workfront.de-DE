---
product-area: documents
navigation-topic: manage-documents
title: Überprüfen der Speicherbeschränkungen für Dokumente
description: Als Adobe Workfront-Administrator können Sie die Nutzung und das Kontingent des Dokumentenspeichers auf der Seite Kundeninformationen einsehen. Wie die Speicherung aussieht, hängt davon ab, ob Ihr Unternehmen alten Workfront-Speicher oder Adobe-Cloud-Speicher verwendet.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/vOjgBLxX5rFIGHBCHB2a6Q3Bs3KE5x-opXUMvANjI1E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 09dff59503604894e61f2a62af7ae1c2e8a39068
workflow-type: tm+mt
source-wordcount: 491
ht-degree: 9%

---

# Überprüfen der Speicherbeschränkungen für Dokumente

Es gibt zwar keine Einschränkungen hinsichtlich der Typen und Größen einzelner Dateien, die Benutzerinnen und Benutzer in Ihre Workfront-Instanz hochladen können, Ihr Workfront-Plan umfasst jedoch ein Gesamtspeicherkontingent. Als Workfront-Administrator überwachen Sie die Nutzung und das Kontingent über den Bereich „Setup“ auf der Seite „Kundeninformationen“.

Wie die Speicherung aussieht, hängt davon ab, ob Ihr Unternehmen alten Workfront-Speicher oder Adobe-Cloud-Speicher verwendet:

* Wenn Sie Legacy-Workfront-Speicher verwenden, lesen Sie [Legacy-Workfront-Speicher](#legacy-workfront-storage) in diesem Artikel.
* Wenn Sie Adobe Cloud-Speicher verwenden, lesen Sie [Adobe Cloud-Speicher](#adobe-cloud-storage) in diesem Artikel.

  Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront-Plan</td> 
   <td> <p>Jedes Workfront-Paket zum Verwalten von Dokumenten unter Verwendung des alten Speichers</p>
      <p>Beliebiges Workflow-Paket zum Verwalten von Dokumenten mit dem Adobe Cloud-Speicher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Legacy-Workfront-Speicher

Wenn Ihr Unternehmen Legacy-Workfront-Speicher verwendet, wird auf der Seite „Kundeninformationen“ ein einziges Speicherkontingent für Dokumente angezeigt, die direkt in Workfront hochgeladen werden.

So überprüfen Sie den alten Workfront-Dokumentspeicher:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Kundeninformationen**.
1. Suchen Sie im Abschnitt **Grundlegende Informationen** nach **Speicherkontingent**. Hier können Sie anzeigen, wie viel Speicher Sie derzeit verwenden, sowie die Gesamtmenge des Speichers, den Ihr Workfront-Plan beinhaltet.

Das Speicherkontingent wird täglich aktualisiert, um die aktuellste Anzahl anzuzeigen.

>[!NOTE]
>
>Diese Beschränkung gilt nicht für Dokumente, die Sie von einem anderen Drittanbieter (SharePoint, Google Drive, Webdam, Box, Dropbox oder einem anderen Anbieter von Dokumenten-Asset-Management) mit Workfront verknüpfen.

## Cloud-Speicherplatz von Adobe


Wenn Ihr Unternehmen Adobe-Cloud-Speicher verwendet, wird Ihr Speicherkontingent als eine einzige gepoolte Zuordnung gemeldet, die Speicher, der über Ihre Workfront-Lizenz bereitgestellt wird, und Speicher, der über ein Frame.io Enterprise-Add-on bereitgestellt wird, kombiniert. Es gibt keine feste Begrenzung der Speichernutzung. Benutzer können weiterhin Dokumente hochladen, selbst wenn die Nutzung Ihr Kontingent überschreitet.

### Anzeigen der Speichernutzung in Kundeninformationen

So überprüfen Sie den Adobe Cloud-Speicher auf Dokumente:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **System** > **Kundeninformationen**.
1. Gehen Sie zum Abschnitt **Speicherübersicht**.
1. Überprüfen Sie Ihre Verwendung. Die Speicherübersicht zeigt Ihr Speicherkontingent im Pool und unterteilt die Nutzung in:

   * Ältere Workfront-Projekte und Adobe Cloud-Speicher-Projekte werden in der blauen Leiste angezeigt.
   * Einzelne Projekte werden in der grünen Leiste angezeigt. Diese Projekte sind unabhängig von Workfront und nur verfügbar, wenn Sie über eine Frame.io Enterprise-Lizenz verfügen.


![Nutzung des Adobe Cloud-Speichers in Kundeninformationen](assets/storage-usage.png)

Die Nutzungsdaten werden regelmäßig aktualisiert, sodass Sie eine aktuelle Zählung sehen.

### E-Mail-Benachrichtigungen für Administratoren

Wenn die Nutzung 75 %, 90 % oder 100 % Ihres Speicherkontingents überschreitet, sendet Workfront eine E-Mail-Benachrichtigung an Systemadministratoren.
