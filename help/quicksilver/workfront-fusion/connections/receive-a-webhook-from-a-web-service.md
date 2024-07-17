---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Webhook von einem Webdienst empfangen
description: Wenn ein Webdienst derzeit nicht als App in  [!DNL Adobe Workfront Fusion] implementiert ist, aber das Senden von Webhooks unterstützt wird, können Sie den Dienst mit dem benutzerdefinierten Webhook-Modul als Instant Trigger zu einem Szenario hinzufügen.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Webhook von einem Webdienst empfangen

Wenn ein Webdienst derzeit nicht als App in [!DNL Adobe Workfront Fusion] implementiert ist, aber das Senden von Webhooks unterstützt wird, können Sie den Dienst mit dem benutzerdefinierten Webhook-Modul als Instant Trigger zu einem Szenario hinzufügen.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Webhook empfangen

1. Fügen Sie Ihrem Szenario das Modul **[!UICONTROL Webhooks] >[!UICONTROL Benutzerspezifischer Webhook]** hinzu.
1. Klicken Sie auf **[!UICONTROL Hinzufügen]**, geben Sie einen **[!UICONTROL Webhook-Namen]** in das angezeigte Feld ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

1. Klicken Sie auf **[!UICONTROL Adresse in Zwischenablage kopieren]** und dann auf **[!UICONTROL OK]**.

1. Melden Sie sich beim Webdienst an und führen Sie dort die folgenden Schritte aus:

   1. Erstellen Sie im Bereich [!UICONTROL Einstellungen] für den Webdienst einen Webhook.
   1. Fügen Sie die Adresse ein, die Sie in Schritt 3 in die Zwischenablage kopiert haben.
   1. Wählen Sie das Ereignis aus, das den Webhook Trigger.

1. Geben Sie im Szenario [!DNL Workfront Fusion] das Ereignis oder die Ereignisse an, die auf das Modul [!UICONTROL Benutzerspezifischer Webhook] Trigger werden sollen.
1. Führen Sie das Szenario aus.

   Wenn das Ereignis oder die Ereignisse eintreten, wird der [!UICONTROL Benutzerspezifische Webhook] -Trigger ausgeführt und das Szenario wird ausgeführt.
