---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projekte, die ich filtern möchte, einschließlich unerwarteter Ergebnisse
description: Lesen Sie diesen Artikel, um Probleme mit dem Filter Projekte zu beheben, die mit unerwarteten Ergebnissen verbunden sind.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# Projekte, bei denen es sich um Filter handelt, enthalten unerwartete Ergebnisse

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] Lizenz</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Systemadministrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

Der Filter &quot;[!UICONTROL **Projekte, die ich verwende&quot;**] enthält Ergebnisse, die ich nicht erwarten würde, da ich diesen Projekten nicht zugewiesen oder damit verbunden bin.

## Lösung

Der Filter &quot;[!UICONTROL **Projekte, die ich verwende&quot;**] enthält Projekte, die den Benutzer in einem seiner Felder [!UICONTROL **Projektdetails**] enthalten, einschließlich einfach verpasster oder automatisch ausgefüllter Felder wie [!UICONTROL **Eingestiegen von**] oder [!UICONTROL **Sponsor-ID**]. Um unerwünschte Ergebnisse zu entfernen, gibt es zwei mögliche Lösungen:

1. Überprüfen Sie die [!UICONTROL **Projektdetails**] für jedes unerwartete Projekt, das vom Filter enthalten ist, und entfernen Sie Ihren Namen aus allen Feldern.

   ODER

1. Versuchen Sie, einen ähnlichen Filter zu verwenden, z. B. [!UICONTROL **Projekte, die ich besitze**], der nur Projekte enthält, die Ihnen speziell zugewiesen sind.

Weitere Informationen zur Verwendung von Filtern in [!DNL Workfront] finden Sie unter [Übersicht über Filter](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
