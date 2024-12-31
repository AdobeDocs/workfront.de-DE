---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projekte, die ich filtere, einschließlich unerwarteter Ergebnisse
description: Lesen Sie diesen Artikel, um eine Fehlerbehebung bei Projekten durchzuführen, die ich filtere, einschließlich unerwarteter Ergebnisse.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# Projekte, an denen ich arbeite, enthalten unerwartete Ergebnisse

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] Lizenz</strong></td> 
   <td> <p>[!UICONTROL-Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Systemadministrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

Der Filter [!UICONTROL **Projekte, an denen**] mitarbeite) enthält Ergebnisse, die nicht erwartet werden, da ich diesen Projekten nicht zugewiesen oder zugeordnet bin.

## Lösung

Der Filter [!UICONTROL **Projekte, an denen**] mitarbeite) enthält Projekte, die den Benutzer in einem seiner Felder [!UICONTROL **Projektdetails**] enthalten, einschließlich leicht übersehener oder automatisch ausgefüllter Felder wie [!UICONTROL **Eingegeben von**] oder [!UICONTROL **Sponsor-ID**]. Um unerwünschte Ergebnisse zu entfernen, gibt es zwei mögliche Lösungen:

1. Markieren Sie [!UICONTROL **Projektdetails**] für jedes unerwartete Projekt, das im Filter enthalten ist, und entfernen Sie Ihren Namen aus allen Feldern.

   ODER

1. Verwenden Sie einen ähnlichen Filter, z. B. [!UICONTROL **Projekte in meinem Besitz**], der nur Projekte enthält, die Ihnen speziell zugewiesen wurden.

Weitere Informationen zur Verwendung von Filtern in [!DNL Workfront] finden Sie unter [Filterübersicht](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
