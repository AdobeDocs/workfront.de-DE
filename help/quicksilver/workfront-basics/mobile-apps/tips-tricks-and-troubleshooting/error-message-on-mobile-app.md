---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: 'Fehlermeldung in der Mobile  [!DNL Adobe Workfront] : ''Ihr Konto ist nicht API-fähig.'''
description: 'Fehlermeldung in der Mobile  [!DNL Adobe Workfront] : ''Ihr Konto ist nicht API-fähig.'''
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# Fehlermeldung in der [!DNL Adobe Workfront] Mobile App: &quot;[!UICONTROL Ihr Konto ist nicht API-fähig.]&quot;

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] Lizenz</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Systemadministrator] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

Beim Versuch, sich bei der [!DNL Adobe Workfront] Mobile App anzumelden, wird die folgende Fehlermeldung angezeigt: *[!UICONTROL Ihr Konto ist nicht API-aktiviert. Teilen Sie dies Ihrem Systemadministrator mit, damit er Sie einrichten kann. Tut mir leid.]*

## Ursache

Ihr [!DNL Workfront] hat den Zugriff auf Ihre [!DNL Workfront]-Umgebung von einem Mobilgerät aus nicht aktiviert.

## Lösung

1. Melden Sie sich bei der [!DNL Workfront]-Web-Anwendung als [!DNL Workfront] an.
1. Navigieren Sie zum Bereich **[!UICONTROL Setup]**.
1. Erweitern Sie das **[!UICONTROL System]**-Menü und klicken Sie auf **[!UICONTROL Voreinstellungen]**.

1. Wählen Sie **[!UICONTROL Abschnitt]** die Option **[!UICONTROL Benutzer dürfen die mobilen Anwendungen von [!DNL Workfront] und das [!DNL Workfront Outlook]-Add-In verwenden]** aus, um sie zu aktivieren.

1. Klicken Sie auf **[!UICONTROL Speichern]**.\
   Alle Benutzer im System können jetzt über ihre Mobile Apps und über [!DNL Outlook] auf [!DNL Workfront] zugreifen.
