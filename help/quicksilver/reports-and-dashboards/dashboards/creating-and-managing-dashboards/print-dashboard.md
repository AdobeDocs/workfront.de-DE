---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Drucken eines Dashboards
description: Sie können ein Dashboard drucken oder in eine PDF-Datei exportieren. Zum Drucken eines Dashboards benötigen Sie die Berechtigung zum Anzeigen.
author: Courtney
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/N5pjtNW6Oy3Nk5L3-MlrdorX-icIvEWm4w0wOJj8N3A
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 460
ht-degree: 11%

---

# Drucken eines Dashboards

<!-- Audited: 1/2025 -->

Sie können ein Dashboard drucken oder in eine PDF-Datei exportieren. Zum Drucken eines Dashboards benötigen Sie die Berechtigung zum Anzeigen.

>[!NOTE]
>
>Diese Funktion ist nur für die Verwendung mit der standardmäßigen Dashboard-Ansicht vorgesehen. Sie ist nicht für Dashboards verfügbar, die in den Bereich Projekte eingebettet oder als benutzerdefinierte Registerkarten festgelegt sind.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Work oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für das Dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Das Dashboard muss erstellt werden, bevor Sie es drucken können.

Informationen zum Erstellen von Dashboards finden Sie unter [Erstellen eines Dashboards](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Informationen, welche Informationen beim Drucken eines Dashboards gedruckt werden

Beim Drucken oder Speichern eines Dashboards als PDF-Datei werden einige Informationen aus dem Dashboard, wie sie in der Adobe Workfront-Web-Anwendung angezeigt werden, möglicherweise nicht in der gedruckten oder exportierten Datei angezeigt.

* [Was wird angezeigt?](#what-is-displayed)
* [Was wird nicht angezeigt?](#what-is-not-displayed)

### Was wird angezeigt? {#what-is-displayed}

Die folgenden Informationen sind in der gedruckten oder exportierten Dashboard-Datei enthalten:

* Dashboard-Titel
* Berichtstitel
* Zeitstempel der letzten Berichterstellung
* Alle Objekte im Dashboard, einschließlich Listenansichten, externen Web-Seiten, Berichten und Kalendern
* Das Logo Ihres Unternehmens, wenn es von Ihrem Workfront-Administrator in Ihrer globalen Navigationsleiste angepasst wurde. Weitere Informationen zum Branding der Workfront-Site finden Sie unter [Branding Ihrer Adobe Workfront-Instanz](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Was wird nicht angezeigt? {#what-is-not-displayed}

Die folgenden Informationen sind nicht in der gedruckten oder exportierten Dashboard-Datei enthalten:

* Die Workfront-Navigationsleiste
* Alle anderen Formatierungen, die für Workfront spezifisch sind
* Je nach Größe der Berichte und der Anzahl und Breite der einzelnen Spalten kann der Export und das Drucken eines Dashboards dazu führen, dass einige Spalten abgeschnitten werden.

## Drucken eines Dashboards

1. Wechseln Sie zum Dashboard, das Sie drucken möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie **Dashboard-Aktionen** > **Druckvorschau**

   * Drücken Sie **Strg+P** (unter Windows) oder **Befehl+P** (unter Mac)

     >[!IMPORTANT]
     >
     >* Keine dieser Optionen ist verfügbar, wenn das Dashboard in eine benutzerdefinierte Registerkarte eingebettet ist. Informationen zum Erstellen benutzerdefinierter Registerkarten finden Sie unter [Erstellen benutzerdefinierter Registerkarten oder Abschnitte](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
     >* Die Option „Tastaturbefehl“ ist bei der Verwendung des Internet Explorer-Browsers nicht verfügbar.

1. Wählen Sie im Feld **Ziel** aus den verschiedenen verfügbaren Druckoptionen.\
   Die Druckoptionen variieren je nach verwendetem Browser und Browser-Version.

1. (Optional) Speichern Sie das Dashboard als PDF-Datei und klicken Sie dann auf **Speichern** um die PDF zu speichern.\
   Informationen zum Speichern des Dashboards als PDF-Datei finden Sie unter [Dashboard exportieren](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Klicken Sie **Drucken**.
