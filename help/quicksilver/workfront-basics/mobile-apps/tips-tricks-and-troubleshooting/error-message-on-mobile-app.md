---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: "Fehlermeldung in der  [!DNL Adobe Workfront] Mobile App: 'Ihr Konto ist nicht für die API aktiviert.'"
description: "Fehlermeldung in der  [!DNL Adobe Workfront] Mobile App: 'Ihr Konto ist nicht für die API aktiviert.'"
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# Fehlermeldung bei der [!DNL Adobe Workfront] Mobile App: &quot;[!UICONTROL Ihr Konto ist nicht für die API aktiviert.]&quot;

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p> Alle</p> </td> 
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

Wenn Sie versuchen, sich bei der mobilen App [!DNL Adobe Workfront] anzumelden, erhalten Sie den folgenden Fehler: *[!UICONTROL Ihr Konto ist nicht für die API aktiviert. Teilen Sie Ihrem Systemadministrator mit, dass er Sie einrichten wird. Tut mir leid.]*

## Ursache

Ihr [!DNL Workfront] -Administrator hat den Zugriff auf Ihre [!DNL Workfront] -Umgebung von einem Mobilgerät aus nicht aktiviert.

## Lösung

1. Melden Sie sich bei der [!DNL Workfront] -Webanwendung als [!DNL Workfront] Administrator an.
1. Wechseln Sie zum Bereich **[!UICONTROL Setup]** .
1. Erweitern Sie das Menü **[!UICONTROL System]** und klicken Sie dann auf **[!UICONTROL Voreinstellungen]**.

1. Wählen Sie unter dem Abschnitt **[!UICONTROL Sicherheit]** die Option **[!UICONTROL Benutzer dürfen die Mobile Apps von [!DNL Workfront] verwenden und die Option [!DNL Workfront Outlook] Add-In]** , um sie zu aktivieren.

1. Klicken Sie auf **[!UICONTROL Speichern]**.\
   Alle Benutzer im System können jetzt von ihren mobilen Apps aus auf [!DNL Workfront] und von [!DNL Outlook] zugreifen.
