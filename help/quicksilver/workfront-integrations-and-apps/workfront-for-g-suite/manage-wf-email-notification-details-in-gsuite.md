---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Verwalten von [!DNL Adobe Workfront] Benachrichtigungsdetails über Google Workspace
description: Wenn Sie in Google Workspace eine Benachrichtigungs-E-Mail öffnen, die Adobe [!DNL Workfront] gesendet wurde, können Sie die zugehörigen Arbeitselementdetails anzeigen und antworten, ohne den Posteingang verlassen zu müssen. Wenn Aktionen verfügbar sind, z. B. die Genehmigung einer Anforderung, können Sie diese direkt über Workfront für Google Workspace durchführen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# [!DNL Adobe Workfront] Benachrichtigungsdetails von [!DNL Google Workspace] verwalten

>[!NOTE]
>
>Die neueste Version des Adobe Workfront-Plug-ins für Google wurde am 26. Juni 2023 veröffentlicht.

Wenn Sie in [!DNL Google Workspace] eine Benachrichtigungs-E-Mail öffnen, die [!DNL Adobe Workfront] gesendet wurde, können Sie die zugehörigen Arbeitselementdetails anzeigen und antworten, ohne Ihren [!UICONTROL Posteingang] zu verlassen. Wenn Aktionen verfügbar sind, wie z. B. das Genehmigen einer Anfrage, können Sie diese Aktionen direkt über [!DNL Workfront for Google Workspace] ausführen.

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] unterstützt fast alle Arten von E-Mail-Benachrichtigungen, die Sie von [!DNL Workfront] empfangen können (etwa 120 verschiedene Typen). [!UICONTROL Tägliche Digest] -E-Mails, die von [!DNL Workfront] gesendet werden, werden nicht in [!DNL Workfront for Google Workspace] angezeigt. Informationen zu den [!DNL Workfront] E-Mail-Benachrichtigungstypen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie Benachrichtigungsdetails über [!DNL Google Workspace] verwalten können, müssen Sie

* Installieren Sie [!DNL Workfront for Google Workspace]\
   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## [!DNL Adobe Workfront] Benachrichtigungsdetails von [!DNL Google Workspace] verwalten

1. Wenn das Bedienfeld [!DNL Workfront for Google Workspace] nicht angezeigt wird, klicken Sie in der Seitenleiste [!DNL Google Workspace] für Add-ons ganz rechts auf der Seite auf das Symbol [!DNL Workfront] ![](assets/wf-lion-icon.png) .
1. Öffnen Sie in [!DNL Google Workspace] eine [!DNL Workfront] Benachrichtigungs-E-Mail.
1. Klicken Sie auf &quot;**[!UICONTROL Alle Aktualisierungen anzeigen&quot;]**&quot;, wenn sie oben im Bedienfeld angezeigt werden.
1. Klicken Sie auf **[!UICONTROL Details]**.
1. Klicken Sie auf eine beliebige verfügbare Option.

   Die angezeigten Optionen beziehen sich auf den Typ der von Ihnen geöffneten E-Mail-Benachrichtigung. Wenn es sich beispielsweise um eine E-Mail-Benachrichtigung handelt, in der Sie aufgefordert werden, eine Aufgabe zu genehmigen, sehen Sie &quot;**[!UICONTROL Genehmigen]**&quot;und &quot;**[!UICONTROL Ablehnen]**&quot;anstelle von Optionen wie &quot;**[!UICONTROL Bearbeiten&quot;]** oder &quot;**[!UICONTROL Fertig]**&quot;:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Art der E-Mail-Benachrichtigung</th> 
      <th>Aktion</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Aufgabe oder Problem</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, <strong>[!UICONTROL Ignore]</strong> eine Zugriffsanfrage, <strong>[!UICONTROL Work on it]</strong> oder klicken Sie auf eine Option, um anzugeben, dass Sie {10 sind.}[!UICONTROL Fertig]</strong> damit<strong></td> 
     </tr> 
     <tr> 
      <td>Projekt</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, oder <strong>[!UICONTROL Ignore]</strong> eine Zugriffsanfrage</td> 
     </tr> 
     <tr> 
      <td>Dokument</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, oder <strong>[!UICONTROL Ignore]</strong> eine Zugriffsanfrage</td> 
     </tr> 
     <tr> 
      <td>Aktualisieren </td> 
      <td> <p>Zeigen Sie einen beliebigen Teil der gesamten Liste der Updates für das Element an, damit Sie den Kontext haben, den Sie benötigen, um <strong>[!UICONTROL Post]</strong> ein neues Update oder eine <strong>[!UICONTROL Antwort]</strong> zu erhalten. Sie können auf <strong>[!UICONTROL Notify]</strong> klicken, um bestimmte Benutzer über Ihre Antwort zu informieren. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Antworten auf eine [!DNL Adobe Workfront] Update-Benachrichtigung von [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Validierungsanfrage</td> 
      <td><strong>[!UICONTROL Genehmigen]</strong> oder <strong>[!UICONTROL Ablehnen]</strong> Sie es (Sie können Ihre Meinung ändern, indem Sie auf die andere Option klicken), laden Sie es herunter, sehen Sie sich den Eigentümer an oder zeigen Sie seine Referenznummer an.</td> 
     </tr> 
     <tr> 
      <td>Änderung des Projektstatus</td> 
      <td> Zeigen Sie alle aktuellen Informationen zum Projekt an, einschließlich aller benutzerdefinierten Formulare. </td> 
     </tr> 
    </tbody> 
   </table>
