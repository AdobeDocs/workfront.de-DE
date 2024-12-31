---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Lizenztyp für externe Benutzer fehlt in den Zugriffsebenen
description: Ich kann den Lizenztyp Externer Benutzer unter „Zugriffsebenen“ im Setup nicht mehr sehen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 1%

---

# Lizenztyp für externe Benutzer fehlt in den Zugriffsebenen

## Problem

Ich kann den Lizenztyp Externer Benutzer unter „Zugriffsebenen“ im Setup nicht mehr sehen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Voreinstellungen]**.

1. Stellen Sie im Abschnitt **[!UICONTROL Sicherheit]** sicher, dass die Option **[!UICONTROL Mit Personen ohne Workfront-Konto über deren E-Mail-Adresse zusammenarbeiten]** aktiviert ist.

   Wenn diese Option nicht aktiviert ist, wird der externe Benutzer nicht im Setup der Zugriffsebene angezeigt.
