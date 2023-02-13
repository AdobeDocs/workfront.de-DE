---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: '"Fehlermeldung auf der [!DNL Adobe Workfront] Mobile App: "Ihr Konto ist nicht für die API aktiviert."'
description: '"Fehlermeldung auf der [!DNL Adobe Workfront] Mobile App: "Ihr Konto ist nicht für die API aktiviert."'
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# Fehlermeldung auf [!DNL Adobe Workfront] Mobile App: &quot;[!UICONTROL Ihr Konto ist nicht für die API aktiviert.]&quot;

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
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Systemadministrator] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

Beim Versuch, sich bei der [!DNL Adobe Workfront] Mobile App erhalten Sie den folgenden Fehler: *[!UICONTROL Ihr Konto ist nicht für die API aktiviert. Teilen Sie Ihrem Systemadministrator mit, dass er Sie einrichten wird. Entschuldige das!]*

## Ursache

Ihre [!DNL Workfront] Administrator hat die [!DNL Workfront] -Umgebung, auf die von einem Mobilgerät aus zugegriffen werden soll.

## Lösung

1. Melden Sie sich bei der [!DNL Workfront] Webanwendung als [!DNL Workfront] Administrator.
1. Navigieren Sie zu **[!UICONTROL Einrichtung]** Bereich.
1. Erweitern Sie die **[!UICONTROL System]** Menü und klicken Sie auf **[!UICONTROL Voreinstellungen]**.

1. Unter dem **[!UICONTROL Sicherheit]** auswählen, wählen Sie die **[!UICONTROL Verwendung von [!DNL Workfront]der mobilen Anwendungen und [!DNL Workfront Outlook] Add-In]** aktivieren.

1. Klicken Sie auf **[!UICONTROL Speichern]**.\
   Alle Benutzer im System können jetzt auf [!DNL Workfront] von ihren mobilen Apps und von [!DNL Outlook].
