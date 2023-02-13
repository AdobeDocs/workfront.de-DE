---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Webhook von einem Webdienst empfangen
description: Wenn ein Webdienst derzeit nicht als App in implementiert ist [!DNL Adobe Workfront Fusion], unterstützt jedoch das Senden von Webhooks, können Sie den Dienst einem Szenario mit dem benutzerdefinierten Webhook-Modul als Instant Trigger hinzufügen.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Webhook von einem Webdienst empfangen

Wenn ein Webdienst derzeit nicht als App in implementiert ist [!DNL Adobe Workfront Fusion], unterstützt jedoch das Senden von Webhooks, können Sie den Dienst einem Szenario mit dem benutzerdefinierten Webhook-Modul als Instant Trigger hinzufügen.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Webhook empfangen

1. Fügen Sie die **[!UICONTROL Webhooks] >[!UICONTROL Benutzerspezifischer Webhook]** -Modul zu Ihrem Szenario hinzu.
1. Klicken **[!UICONTROL Hinzufügen]**, geben Sie einen **[!UICONTROL Webhook-Name]** in dem angezeigten Feld klicken Sie auf **[!UICONTROL Speichern]**.

1. Klicken **[!UICONTROL Adresse in Zwischenablage kopieren]** Klicken Sie auf **[!UICONTROL OK]**.

1. Melden Sie sich beim Webdienst an und führen Sie dort die folgenden Schritte aus:

   1. Im [!UICONTROL Einstellungen] Erstellen Sie einen Webhook für den Webdienst.
   1. Fügen Sie die Adresse ein, die Sie in Schritt 3 in die Zwischenablage kopiert haben.
   1. Wählen Sie das Ereignis aus, das den Webhook Trigger.

1. Im [!DNL Workfront Fusion] -Szenario festzulegen, geben Sie das Ereignis oder die Ereignisse an, auf die Sie den Trigger [!UICONTROL Benutzerspezifischer Webhook] -Modul.
1. Führen Sie das Szenario aus.

   Wenn das Ereignis oder die Ereignisse eintreten, wird die [!UICONTROL Benutzerspezifischer Webhook] -Trigger und das -Szenario ausgeführt.
