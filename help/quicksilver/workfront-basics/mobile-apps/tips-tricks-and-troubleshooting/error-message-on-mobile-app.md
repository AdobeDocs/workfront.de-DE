---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: 'Fehlermeldung in der [!DNL Adobe Workfront] Mobile App: ''Ihr Konto ist nicht API-fähig.'''
description: 'Fehlermeldung in der [!DNL Adobe Workfront] Mobile App: ''Ihr Konto ist nicht API-fähig.'''
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
TQID: 'https://experienceleague.adobe.com/t-ANxgXpzPBSM8cGUipyAIczqSEUJGXTthbaVP5dh2E'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 15%
---
# Fehlermeldung in der [!DNL Adobe Workfront] Mobile App: &quot;[!UICONTROL Ihr Konto ist nicht API-fähig.]&quot;

## Zugriffsanforderungen

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] License</strong></td> 
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

1. Wählen Sie **[!UICONTROL Abschnitt]** die Option **[!UICONTROL Benutzer dürfen die mobilen Anwendungen von [!DNL Workfront] verwenden]** aus, um sie zu aktivieren.

1. Klicken Sie auf **[!UICONTROL Speichern]**.\
   Alle Benutzer im System können jetzt über ihre Mobile Apps auf [!DNL Workfront] zugreifen.
