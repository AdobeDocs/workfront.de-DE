---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: ' [!DNL Adobe Workfront] für  [!DNL Outlook] einrichten'
description: Mit dem Add-in [!DNL Adobe Workfront] [!DNL Outlook] können Sie die Schlüssel [!DNL Workfront] aufgaben direkt in Outlook ausführen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Einrichten von [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

Mit dem Add-In [!DNL Adobe Workfront] [!DNL Outlook] können Sie die folgenden wichtigen [!DNL Workfront] Aufgaben direkt in Outlook ausführen:

* Aktualisieren eines vorhandenen Projekts, einer Aufgabe oder eines Problems mit Informationen aus einer E-Mail Weitere Informationen finden Sie unter [Aktualisieren eines vorhandenen Objekts von einer  [!DNL Outlook] E-Mail](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Erstellen Sie eine [!DNL Workfront] -Anfrage basierend auf einer E-Mail in [!DNL Outlook]. Weitere Informationen finden Sie unter [Erstellen einer Adobe Workfront-Anforderung aus einer  [!DNL Outlook] E-Mail](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Fügen Sie eine E-Mail als Aufgabe in Ihrem Bereich [!UICONTROL Meine Arbeit] hinzu. Weitere Informationen finden Sie unter [Hinzufügen einer [!DNL Outlook] E-Mail als Aufgabe zur Arbeitsliste](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Antworten Sie über das Add-in [!DNL Workfront] für [!DNL Outlook] auf Kommentare. Weitere Informationen zur Beantwortung von Kommentaren von Workfront für [!DNL Outlook] finden Sie unter [Antworten auf einen Kommentar von  [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Erstellen Sie Aufgaben und Probleme von Grund auf neu oder erstellen Sie sie aus vorhandenen E-Mails (mithilfe der Drag &amp; Drop-Funktion). Weitere Informationen finden Sie unter [Hinzufügen einer [!DNL Outlook] E-Mail zu einem Projekt als Aufgabe oder Problem](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Sie müssen das [!DNL Workfront]-Add-In zu Ihrem [!DNL Outlook]-Konto hinzufügen, bevor Sie [!DNL Workfront for Outlook] verwenden können.

Wenn Sie das [!DNL Workfront]-Add-In nicht mit Ihrem [!DNL Outlook]-Konto installieren können, wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um sicherzustellen, dass [!DNL Outlook] Add-Ins für Ihre Organisation aktiviert sind.

Informationen zum Aktivieren der [!DNL Outlook]-Integration für Ihr Unternehmen finden Sie unter [Aktivieren [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neuer Plan: [!UICONTROL Standard]</p> 
   <p>Aktueller Plan:[!UICONTROL Arbeit], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Ihr [!DNL Workfront] -Administrator muss [!DNL Outlook for Office] mit [!DNL Workfront] aktivieren, bevor Sie diese Integration verwenden können.

## Systemanforderungen

Die folgenden Anwendungen sind verfügbar:

* **[!DNL Outlook]im Web:** Das [!DNL Workfront]-Add-in ist verfügbar, wenn Sie [!DNL Outlook] über einen Webbrowser auf einem Desktop- oder Mobilgerät verwenden. Diese Funktion ist auch bei Verwendung der [!DNL Outlook]-Webanwendung verfügbar.
* **[!DNL Outlook]Desktop-Anwendung:** Das [!DNL Workfront] Add-In ist verfügbar, wenn die im Paket [!DNL Office] enthaltenen [!DNL Windows] - und [!DNL Mac] -Desktop-Versionen von [!DNL Outlook] verwendet werden.

Das [!DNL Workfront]-Add-in für [!DNL Outlook] wird in Umgebungen unterstützt, die die folgenden Anforderungen erfüllen:

* [Kundenanforderungen](#client-requirements-client-requirements)
* [Mail-Server-Anforderungen](#mail-server-requirements-mail-server-requirements)

### Kundenanforderungen {#client-requirements}

Workfront unterstützt die folgenden Versionen von [!DNL Outlook]:

* [!DNL Outlook 2013] oder höher am [!DNL Windows]
*[!DNL  Outlook 2016] oder höher am [!DNL Windows]
* [!DNL Outlook] auf [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] auf [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] im Internet

Sie müssen über eine direkte Verbindung mit einem [!DNL Exchange Server] oder einem [!DNL Office 365] verbunden sein.

Beim Konfigurieren des Clients muss der Benutzer einen der folgenden Kontotypen auswählen:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] &#x200B;**&#x200B;** &#x200B; Wenn der Client für die Verbindung mit POP3 oder IMAP konfiguriert ist, wird das [!DNL Workfront]-Add-In nicht geladen.

### Mail-Server-Anforderungen {#mail-server-requirements}

Die Anforderungen an den Mailserver werden standardmäßig erfüllt, wenn Sie eine Verbindung zu [!DNL Office 365] oder [!DNL Outlook.com] herstellen. Wenn Sie jedoch mit einer On-Premise-Installation von [!DNL Exchange Server] verbunden sind, gelten folgende Anforderungen:

* Workfront unterstützt alle [!DNL Exchange On-Premise] -Server
* [!DNL Exchange Web Services] (EWS) muss aktiviert sein und für das Internet verfügbar gemacht werden.
* Der Server muss über ein gültiges Authentifizierungszertifikat verfügen, damit der Server gültige Identitäts-Token ausgibt. Neue Installationen von [!DNL Exchange Server] enthalten ein standardmäßiges Authentifizierungszertifikat.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Um über den [[!DNL Office] Store](https://store.office.com/) auf das [!DNL Workfront] -Add-In zugreifen zu können, müssen Ihre Client-Zugriffsserver mit [https://store.office.com](https://store.office.com/) kommunizieren können.

Weitere Informationen zu unterstützten Umgebungen finden Sie auf der [[!DNL Microsoft Office 365] Startseite](https://products.office.com/en-us/office-365-home).

## Installieren des Add-Ins

Sie können das Workfront-Add-in für Outlook vom [Microsoft-Store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview) abrufen.

### [!DNL Workfront] für [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Klicken Sie in [!DNL Outlook 365] oben in der Office 365-Benutzeroberfläche auf das Symbol **[!UICONTROL Add-Ins durchsuchen]** ![](assets/outlook-add-in-26x26.png) und klicken Sie dann auf **[!UICONTROL Add-Ins verwalten]**.

1. Suchen Sie im Feld **[!UICONTROL Add-Ins durchsuchen]** nach **[!DNL Workfront]** und drücken Sie dann die Taste [!UICONTROL Enter].

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.

### [!DNL Workfront] für [!DNL Outlook] im Web {#workfront-for-outlook-on-the-web}

1. Öffnen Sie [!DNL Microsoft Outlook] in einem Webbrowser.
1. Klicken Sie auf das Symbol **[!UICONTROL Add-Ins durchsuchen]** ![](assets/outlook-add-in-web-version-20x20.png).

   Informationen zum Suchen des Symbols finden Sie unter [Verwenden von Add-Ins in [!DNL Outlook] im Web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) in der Microsoft-Dokumentation.

1. Suchen Sie im Feld **[!UICONTROL Add-Ins durchsuchen]** nach **[!DNL Workfront]** und drücken Sie dann die **[!UICONTROL Eingabetaste]**.

1. Wenn es in der Liste angezeigt wird, klicken Sie auf **Hinzufügen**.

### [!DNL Workfront for Outlook] bei [!UICONTROL Windows] oder [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Klicken Sie auf **[!UICONTROL Home]** > **[!UICONTROL Store]** auf dem Band.

1. Suchen Sie im Feld **[!UICONTROL Suche]** nach **[!DNL Workfront]** und drücken Sie dann die **[!UICONTROL Eingabetaste]**.

1. Klicken Sie auf den Umschalter, um das **[!UICONTROL [!DNL Workfront]Add-in]** zu aktivieren.

## Anmelden bei [!DNL Workfront] von [!DNL Outlook]

1. Wählen Sie in [!DNL Outlook] eine E-Mail-Nachricht aus und klicken Sie dann auf das Symbol **[!DNL Workfront]** im E-Mail-Header.
1. Befolgen Sie die Anweisungen zum Anmelden bei [!DNL Workfront] mithilfe von Enhanced Authentication, OAuth 2.0 oder Ihrer SAML-URL (Security Assertion Markup Language).

   Bevor sich Benutzer mit SAML beim [!DNL Workfront] -Add-in anmelden können, muss ein [!DNL Workfront] -Administrator zunächst [!DNL Office 365] -Add-Ins aktivieren, um sich mit einer SAML 2.0-Lösung zu authentifizieren. Weitere Informationen finden Sie im Abschnitt [Konfigurieren von [!DNL Adobe Workfront] mit SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) im Artikel [Konfigurieren von [!DNL Adobe Workfront] mit SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Wenn Sie aufgefordert werden, die Domäne Ihres [!DNL Workfront]-Kontos einzugeben, geben Sie es in folgendem Format ein: *sDomain.my.workfront.com* Ihres Unternehmens. Die Domäne Ihres Unternehmens ist normalerweise der Name Ihres Unternehmens.
   >* Die erweiterte Authentifizierung ist erst verfügbar, wenn ein [!DNL Workfront] -Administrator sie für diese Integration aktiviert hat.

