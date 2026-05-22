---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projekte, die ich filtere, einschließlich unerwarteter Ergebnisse
description: Lesen Sie diesen Artikel, um eine Fehlerbehebung bei Projekten durchzuführen, die ich filtere, einschließlich unerwarteter Ergebnisse.
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 14b3bfaf16a4ab8749538b32100ce6363a3a9335
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 23%

---

# Filter „Projekte, an denen ich mitwirke“ enthält unerwartete Ergebnisse

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td>Beliebig</td>
  </tr>
  <tr>
   <td>Adobe Workfront-Lizenzen
   </td>
   <td><p>Standard</p>
   <p>Abo</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++


## Problem

Der Filter [!UICONTROL **Projekte, an denen**] mitarbeite) enthält Ergebnisse, die nicht erwartet werden, da ich diesen Projekten nicht zugewiesen oder zugeordnet bin.

## Lösung

Der Filter [!UICONTROL **Projekte, an denen**] mitarbeite) enthält Projekte, die den Benutzer in einem seiner Felder [!UICONTROL **Projektdetails**] enthalten, einschließlich leicht übersehener oder automatisch ausgefüllter Felder wie [!UICONTROL **Eingegeben von**] oder [!UICONTROL **Sponsor-ID**]. Um unerwünschte Ergebnisse zu entfernen, gibt es zwei mögliche Lösungen:

1. Markieren Sie [!UICONTROL **Projektdetails**] für jedes unerwartete Projekt, das im Filter enthalten ist, und entfernen Sie Ihren Namen aus allen Feldern.

   ODER

1. Verwenden Sie einen ähnlichen Filter, z. B. [!UICONTROL **Projekte in meinem Besitz**], der nur Projekte enthält, die Ihnen speziell zugewiesen wurden.

Weitere Informationen zur Verwendung von Filtern in [!DNL Workfront] finden Sie unter [Filterübersicht](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
