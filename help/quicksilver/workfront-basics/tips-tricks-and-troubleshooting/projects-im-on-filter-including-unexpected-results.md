---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projekte, die ich filtere, einschließlich unerwarteter Ergebnisse
description: Lesen Sie diesen Artikel, um eine Fehlerbehebung bei Projekten durchzuführen, die ich filtere, einschließlich unerwarteter Ergebnisse.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 3%

---

# Projekte, an denen ich arbeite, enthalten unerwartete Ergebnisse

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Prime oder Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront-Lizenzen
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## Problem

Der Filter [!UICONTROL **Projekte, an denen**] mitarbeite) enthält Ergebnisse, die nicht erwartet werden, da ich diesen Projekten nicht zugewiesen oder zugeordnet bin.

## Lösung

Der Filter [!UICONTROL **Projekte, an denen**] mitarbeite) enthält Projekte, die den Benutzer in einem seiner Felder [!UICONTROL **Projektdetails**] enthalten, einschließlich leicht übersehener oder automatisch ausgefüllter Felder wie [!UICONTROL **Eingegeben von**] oder [!UICONTROL **Sponsor-ID**]. Um unerwünschte Ergebnisse zu entfernen, gibt es zwei mögliche Lösungen:

1. Markieren Sie [!UICONTROL **Projektdetails**] für jedes unerwartete Projekt, das im Filter enthalten ist, und entfernen Sie Ihren Namen aus allen Feldern.

   ODER

1. Verwenden Sie einen ähnlichen Filter, z. B. [!UICONTROL **Projekte in meinem Besitz**], der nur Projekte enthält, die Ihnen speziell zugewiesen wurden.

Weitere Informationen zur Verwendung von Filtern in [!DNL Workfront] finden Sie unter [Filterübersicht](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
