---
product-area: workfront-integrations
keywords: Google,DOC,Dokument,Blatt,Folie
navigation-topic: workfront-for-g-suite
title: Verwalten  [!DNL Adobe Workfront]  Benachrichtigungsdetails aus Google Workspace
description: Wenn Sie in Google Workspace eine von Adobe gesendete Benachrichtigungs [!DNL Workfront] E-Mail öffnen, können Sie die zugehörigen Arbeitsaufgabendetails anzeigen und antworten, ohne Ihren Posteingang zu verlassen. Wenn Aktionen verfügbar sind, z. B. die Genehmigung einer Anfrage, können Sie diese Aktionen direkt über Workfront für Google Workspace durchführen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 1%

---

# Verwalten von [!DNL Adobe Workfront]-Benachrichtigungsdetails über [!DNL Google Workspace]

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieser Umstellung werden die folgenden Funktionen von Workfront für Google Workspace nach dem 28. **2026 nicht mehr verfügbar**:
>
>* Zugriff auf Google Workspace-Funktionen in Workfront
>
>* Anzeigen und Verwalten von Workfront-Aufgaben über Gmail oder das Site-Panel des Google-Kalenders
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Google Workspace zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Google Workspace finden Sie unter [Gmail-](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) und [Google-](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Wenn Sie [!DNL Google Workspace] eine von [!DNL Adobe Workfront] gesendete Benachrichtigungs-E-Mail öffnen, können Sie die zugehörigen Arbeitsaufgabendetails anzeigen und antworten, ohne Ihren [!UICONTROL Posteingang“ &#x200B;]. Wenn Aktionen verfügbar sind, z. B. die Genehmigung einer Anfrage, können Sie diese Aktionen direkt über [!DNL Workfront for Google Workspace] ausführen.

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] unterstützt fast alle Arten von E-Mail-Benachrichtigungen, die Sie von [!DNL Workfront] erhalten können (etwa 120 verschiedene Arten). [!UICONTROL Daily Digest] E-Mails, die von [!DNL Workfront] gesendet werden, werden nicht in [!DNL Workfront for Google Workspace] angezeigt. Informationen zu den [!DNL Workfront] E-Mail-Benachrichtigungstypen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p><p>Arbeit oder höher</p>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie Benachrichtigungsdetails aus [!DNL Google Workspace] verwalten können, müssen Sie Folgendes tun

* Installieren von [!DNL Workfront for Google Workspace]\
   Anweisungen finden Sie unter [Installieren [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Verwalten von [!DNL Adobe Workfront]-Benachrichtigungsdetails über [!DNL Google Workspace]

1. Wenn das [!DNL Workfront for Google Workspace] nicht angezeigt wird, klicken Sie auf das [!DNL Workfront]-Symbol ![Workfront](assets/wf-lion-icon.png) in der Seitenleiste [!DNL Google Workspace] Add-ons ganz rechts auf der Seite.
1. Öffnen Sie [!DNL Google Workspace] eine E-Mail mit einer [!DNL Workfront].
1. Klicken Sie **[!UICONTROL Alle Updates anzeigen]**, wenn es oben im Bedienfeld angezeigt wird.
1. Klicken Sie auf **[!UICONTROL Details]**.
1. Klicken Sie auf eine der verfügbaren Optionen.

   Die angezeigten Optionen beziehen sich möglicherweise auf den Typ der von Ihnen geöffneten E-Mail-Benachrichtigung. Wenn Sie beispielsweise in einer E-Mail aufgefordert werden, eine Aufgabe zu genehmigen, werden **[!UICONTROL Genehmigen]** und **[!UICONTROL Ablehnen]** anstelle von Optionen wie **[!UICONTROL Bearbeiten]** oder **[!UICONTROL Fertig]**:

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
      <td><strong>[!UICONTROL genehmigen]</strong>, <strong>[!UICONTROL ablehnen]</strong>, <strong>[!UICONTROL gewähren]</strong> Zugriff darauf, <strong>[!UICONTROL Ignorieren]</strong> eine Zugriffsanforderung <strong>[!UICONTROL bearbeiten]</strong> oder auf eine Option klicken, um anzugeben, dass Sie <strong>[!UICONTROL fertig]</strong> damit sind</td> 
     </tr> 
     <tr> 
      <td>Projekt</td> 
      <td><strong>[!UICONTROL genehmigen]</strong>, <strong>[!UICONTROL ablehnen]</strong>, <strong>[!UICONTROL gewähren]</strong> Zugriff darauf, oder <strong>[!UICONTROL ignorieren]</strong> eine Zugriffsanforderung</td> 
     </tr> 
     <tr> 
      <td>Dokument</td> 
      <td><strong>[!UICONTROL genehmigen]</strong>, <strong>[!UICONTROL ablehnen]</strong>, <strong>[!UICONTROL gewähren]</strong> Zugriff darauf, oder <strong>[!UICONTROL ignorieren]</strong> eine Zugriffsanforderung</td> 
     </tr> 
     <tr> 
      <td>Update </td> 
      <td> <p>Zeigen Sie einen beliebigen Teil der gesamten Aktualisierungsliste für das Element an, damit Sie über den Kontext verfügen, in dem Sie[!UICONTROL Post]<strong> neues Update oder eine </strong>[!UICONTROL Reply]<strong> müssen</strong>. Sie können auf <strong>[!UICONTROL Notify]</strong> klicken, um bestimmte Benutzer über Ihre Antwort zu informieren. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Antwort auf eine [!DNL Adobe Workfront] Update-Benachrichtigung von [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Genehmigungsanforderung</td> 
      <td><strong>[!UICONTROL Approve]</strong> oder <strong>[!UICONTROL Reject]</strong> sie (Sie können Ihre Meinung ändern, indem Sie auf die andere Option klicken), laden Sie sie herunter, zeigen Sie ihren Besitzer an oder zeigen Sie die Referenznummer an</td> 
     </tr> 
     <tr> 
      <td>Änderung des Status eines Projekts</td> 
      <td> Zeigt alle aktuellen Informationen über das Projekt an, einschließlich benutzerdefinierter Formulare. </td> 
     </tr> 
    </tbody> 
   </table>
