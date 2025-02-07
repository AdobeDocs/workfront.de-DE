---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Einrichten [!DNL Adobe Workfront] für [!DNL Outlook]
description: Mit  [!DNL Adobe Workfront] [!DNL Outlook] Add-In können Sie die wichtigsten  [!DNL Workfront]  direkt in Outlook ausführen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Einrichten von [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

Mit dem Add-in [!DNL Adobe Workfront] [!DNL Outlook] können Sie die folgenden wichtigen [!DNL Workfront] direkt in Outlook ausführen:

* Vorhandenes Projekt, vorhandene Aufgabe oder vorhandenes Problem mit Informationen aus einer E-Mail aktualisieren. Weitere Informationen finden Sie unter [Vorhandenes Objekt aus einer E- [!DNL Outlook]  aktualisieren](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Erstellen Sie eine [!DNL Workfront] Anfrage basierend auf einer E-Mail in [!DNL Outlook]. Weitere Informationen finden Sie unter [Erstellen einer Adobe Workfront-Anfrage aus einer E [!DNL Outlook] Mail](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Fügen Sie eine E-Mail als Aufgabe in Ihrem Bereich [!UICONTROL Meine Arbeit] hinzu. Weitere Informationen finden Sie unter [Hinzufügen einer E [!DNL Outlook] Mail als Aufgabe zu Ihrer Auftragsliste](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Antworten auf Kommentare über das [!DNL Workfront]-Add-in für [!DNL Outlook]. Informationen zum Beantworten von Kommentaren aus Workfront für [!DNL Outlook] finden Sie unter [Beantworten eines Kommentars aus [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Aufgaben und Probleme von Grund auf neu erstellen oder aus vorhandenen E-Mails erstellen (mit Drag-and-Drop-Funktion). Weitere Informationen finden Sie unter [Hinzufügen einer E [!DNL Outlook] Mail zu einem Projekt als Aufgabe oder Problem](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Sie müssen das Add-In [!DNL Workfront] Ihrem [!DNL Outlook]-Konto hinzufügen, bevor Sie [!DNL Workfront for Outlook] verwenden können.

Wenn Sie das Add-In [!DNL Workfront] nicht mit Ihrem [!DNL Outlook]-Konto installieren können, wenden Sie sich an Ihren [!DNL Workfront], um sicherzustellen, dass [!DNL Outlook] Add-Ins für Ihr Unternehmen aktiviert sind.

Informationen zum Aktivieren der [!DNL Outlook]-Integration für Ihr Unternehmen finden Sie unter [Aktivieren [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neuer Plan: [!UICONTROL Standard]</p> 
   <p>Aktueller Plan:[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Ihr [!DNL Workfront] muss [!DNL Outlook for Office] mit [!DNL Workfront] aktivieren, bevor Sie diese Integration verwenden können.

## Systemanforderungen

Die folgenden Anwendungen sind verfügbar:

* **[!DNL Outlook]im Web:** Das Add-In &quot;[!DNL Workfront]&quot; ist verfügbar, wenn [!DNL Outlook] über einen Webbrowser auf einem Desktop- oder Mobilgerät verwendet wird. Diese Funktion ist auch bei Verwendung der [!DNL Outlook] Web App verfügbar.
* **[!DNL Outlook]Desktop-Programm** Das [!DNL Workfront]-Add-in ist verfügbar, wenn die [!DNL Windows]- und [!DNL Mac]-Desktop-Versionen von [!DNL Outlook] verwendet werden, die im [!DNL Office]-Paket enthalten sind.

Das [!DNL Workfront]-Add-in für [!DNL Outlook] wird in Umgebungen unterstützt, die die folgenden Anforderungen erfüllen:

* [Kundenanforderungen](#client-requirements-client-requirements)
* [Mail-Server-Anforderungen](#mail-server-requirements-mail-server-requirements)

### Kundenanforderungen {#client-requirements}

Workfront unterstützt die folgenden Versionen von [!DNL Outlook]:

* [!DNL Outlook 2013] oder höher auf [!DNL Windows]
* [!DNL Outlook 2016] oder höher auf [!DNL Windows]
* [!DNL Outlook] am [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] am [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] im Internet

Sie müssen über eine direkte Verbindung mit einem [!DNL Exchange Server] oder [!DNL Office 365] verbunden sein.

Beim Konfigurieren des Clients muss der Benutzer einen der folgenden Kontotypen auswählen:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] Wenn der Client für die Verbindung mit POP3 oder IMAP konfiguriert ist, wird das [!DNL Workfront]-Add-in nicht geladen.

### Mail-Server-Anforderungen {#mail-server-requirements}

Die E-Mail-Server-Anforderungen werden standardmäßig erfüllt, wenn Sie eine Verbindung zu [!DNL Office 365] oder [!DNL Outlook.com] herstellen. Wenn Sie jedoch mit einer On-Premise-Installation von [!DNL Exchange Server] verbunden sind, gelten die folgenden Anforderungen:

* Workfront unterstützt alle [!DNL Exchange On-Premise]
* [!DNL Exchange Web Services] (EWS) muss aktiviert und für das Internet zugänglich sein.
* Der Server muss über ein gültiges Authentifizierungszertifikat verfügen, damit der Server gültige Identitäts-Token ausgeben kann. Neue Installationen von [!DNL Exchange Server] enthalten ein standardmäßiges Authentifizierungszertifikat.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Um über den [[!DNL Office] Store](https://store.office.com/) auf das [!DNL Workfront]-Add-in zugreifen zu können, müssen Ihre Clientzugriffsserver mit [https://store.office.com kommunizieren ](https://store.office.com/).

Weitere Informationen zu unterstützten Umgebungen finden Sie auf der [[!DNL Microsoft Office 365] Startseite](https://products.office.com/en-us/office-365-home).

## Installieren des Add-Ins

Das Workfront-Add-In für Outlook erhalten Sie im [Microsoft Store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] für [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Klicken Sie [!DNL Outlook 365] oben in der Office 365 **[!UICONTROL Benutzeroberfläche auf das Symbol]** Add-Ins durchsuchen![ ](assets/outlook-add-in-26x26.png) und anschließend auf **[!UICONTROL Add-Ins verwalten]**.

1. Suchen Sie im Feld **[!UICONTROL Add-Ins suchen]** nach **[!DNL Workfront]** drücken Sie dann die [!UICONTROL Eingabetaste].

1. Klicken Sie **[!UICONTROL Hinzufügen]**.

### [!DNL Workfront] für [!DNL Outlook] im Web {#workfront-for-outlook-on-the-web}

1. Öffnen Sie [!DNL Microsoft Outlook] in einem Webbrowser.
1. Klicken Sie auf **[!UICONTROL Symbol ]Durchsuchen** Add-Ins![Durchsuchen-Add-Ins](assets/outlook-add-in-web-version-20x20.png).

   Informationen zum Auffinden des Symbols finden Sie unter [Verwenden von Add [!DNL Outlook] Ins im Web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) in der Dokumentation zu Microsoft.

1. Suchen Sie im Feld **[!UICONTROL Add-Ins suchen]** nach **[!DNL Workfront]** und drücken Sie dann die **[!UICONTROL Eingabetaste]**.

1. Wenn es in der Liste angezeigt wird, klicken Sie auf **Hinzufügen**.

### [!DNL Workfront for Outlook] unter [!UICONTROL Windows] oder [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Klicken Sie **[!UICONTROL Menüband auf]** Startseite **[!UICONTROL >]** Store“.

1. Suchen Sie nach **[!DNL Workfront]** im Feld **[!UICONTROL Suche]** und drücken Sie dann die **[!UICONTROL Eingabetaste]**.

1. Klicken Sie auf den Umschalter, um das **[!UICONTROL [!DNL Workfront]-Add-in zu aktivieren]**.

## Anmelden bei [!DNL Workfront] von [!DNL Outlook]

1. Wählen Sie [!DNL Outlook] eine E-Mail-Nachricht aus und klicken Sie dann in der E-Mail-Kopfzeile auf das Symbol **[!DNL Workfront]** .
1. Klicken Sie auf der Anmeldeseite auf **Bei Workfront anmelden**.
1. Befolgen Sie die Anweisungen, um sich mit OAuth 2.0 bei [!DNL Workfront] anzumelden. <!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* Wenn Sie aufgefordert werden, die Domain Ihres [!DNL Workfront] Kontos einzugeben, geben Sie sie in folgendem Format ein: *yourCompany&#39;sDomain.my.workfront.com*. Die Domain Ihres Unternehmens ist normalerweise der Name Ihres Unternehmens.

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
