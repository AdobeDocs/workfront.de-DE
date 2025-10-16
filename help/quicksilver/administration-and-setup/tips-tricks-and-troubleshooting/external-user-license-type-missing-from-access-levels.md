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
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 4%

---

# Lizenztyp für externe Benutzer fehlt in den Zugriffsebenen

## Problem

Ich kann den Lizenztyp Externer Benutzer unter „Zugriffsebenen“ im Setup nicht mehr sehen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Voreinstellungen]**.

1. Stellen Sie im Abschnitt **[!UICONTROL Sicherheit]** sicher, dass die Option **[!UICONTROL Mit Personen ohne Workfront-Konto über deren E-Mail-Adresse zusammenarbeiten]** aktiviert ist.

   Wenn diese Option nicht aktiviert ist, wird der externe Benutzer nicht im Setup der Zugriffsebene angezeigt.
