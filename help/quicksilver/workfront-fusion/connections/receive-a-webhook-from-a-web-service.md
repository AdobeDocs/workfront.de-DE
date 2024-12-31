---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Empfangen eines Webhooks von einem Webservice
description: Wenn ein Webservice derzeit nicht als App in implementiert ist [!DNL Adobe Workfront Fusion] aber den Versand von Webhooks unterstützt, können Sie den Service mit dem benutzerdefinierten Webhook-Modul als sofortigen Trigger zu einem Szenario hinzufügen.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Empfangen eines Webhooks von einem Webservice

Wenn ein Webservice derzeit nicht als App in [!DNL Adobe Workfront Fusion] implementiert ist, aber den Versand von Webhooks unterstützt, können Sie den Service mit dem benutzerdefinierten Webhook-Modul als sofortigen Trigger zu einem Szenario hinzufügen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Webhook empfangen

1. Fügen Sie das **[!UICONTROL Webhooks] > [!UICONTROL Benutzerdefinierter Webhook]**-Modul zu Ihrem Szenario hinzu.
1. Klicken Sie auf **[!UICONTROL Hinzufügen]**, geben Sie einen **[!UICONTROL Webhook-Namen]** in das angezeigte Feld ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

1. Klicken Sie **[!UICONTROL Adresse in Zwischenablage kopieren]** und dann auf **[!UICONTROL OK]**.

1. Melden Sie sich beim -Webdienst an und führen Sie dort folgende Schritte aus:

   1. Erstellen Sie [!UICONTROL  Webhook ] Bereich „Einstellungen“ für den Webservice.
   1. Fügen Sie die in Schritt 3 in die Zwischenablage kopierte Adresse ein.
   1. Wählen Sie das Ereignis aus, durch das der Webhook Trigger wird.

1. Geben Sie im [!DNL Workfront Fusion] Szenario das Ereignis oder die Ereignisse an, für die Sie den Trigger des Moduls [!UICONTROL Benutzerdefinierter Webhook] erstellen möchten.
1. Führen Sie das Szenario aus.

   Trigger Wenn das Ereignis bzw. die Ereignisse eintreten, wird [!UICONTROL  Modul &quot;] Webhook“ ausgeführt und das Szenario wird ausgeführt.
