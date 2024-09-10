---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Externer Lizenztyp Fehlt von Zugriffsebenen
description: Der Lizenztyp für externe Benutzer wird unter Zugriffsebenen in der Einrichtung nicht mehr angezeigt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 1%

---

# Externer Lizenztyp fehlt in den Zugriffsebenen

## Problem

Der Lizenztyp für externe Benutzer wird unter Zugriffsebenen in der Einrichtung nicht mehr angezeigt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

1. Navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Voreinstellungen]**.

1. Stellen Sie im Abschnitt **[!UICONTROL Sicherheit]** sicher, dass die Option **[!UICONTROL Mit Personen ohne Workfront-Konten zusammenarbeiten, indem Sie deren E-Mail-Adresse verwenden]** aktiviert ist.

   Wenn diese Option nicht aktiviert ist, wird der externe Benutzer nicht in der Einrichtung der Zugriffsebene angezeigt.
