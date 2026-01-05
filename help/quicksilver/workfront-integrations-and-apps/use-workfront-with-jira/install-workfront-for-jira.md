---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installieren [!DNL Adobe Workfront] für [!DNL Jira]
description: Sie können  [!DNL Adobe Workfront] -for [!DNL Jira]  verwenden, um Ihre  [!DNL Jira] - [!DNL Workfront]  zu integrieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 3%

---

# Installieren von [!DNL Adobe Workfront for Jira]

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses wird die Integration von Workfront für Jira nach dem 28. **2026 nicht mehr**.
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Jira zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Jira finden Sie unter [Jira-Softwaremodule](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Sie können [!DNL Adobe Workfront for Jira] verwenden, um Ihre [!DNL Jira]- und [!DNL Workfront] zu integrieren.

Nach der Installation des Add-ons können Sie Workflows definieren, die beim Erstellen von [!DNL Jira] automatisch [!DNL Workfront] Probleme verursachen. Die Elemente in beiden Anwendungen werden verknüpft, und einige ihrer Informationen können in beiden Systemen automatisch aktualisiert werden.

Von dieser Integration können alle Anwender in [!DNL Workfront] und [!DNL Jira] profitieren. Sie benötigen lediglich eine Lizenz für das System, in dem sie am meisten arbeiten, und nicht für beide Systeme.

Dieses Add-on ist für die Versionen [!UICONTROL Server] und [!UICONTROL OnDemand] (oder [!UICONTROL Cloud]) [!DNL Jira] Software verfügbar. Dieses Add-on ist für die [!DNL Data Center] Version [!DNL Jira] Software nicht verfügbar.

Eine Liste der [!DNL Jira] Versionen, die [!DNL Workfront for Jira] derzeit unterstützt, finden Sie unter [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) im Atlassian Marketplace.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira-Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in Jira und Workfront zu erstellen, um diese Integration zu ermöglichen, anstatt vorhandene Konten zu verwenden, die an Benutzende angehängt sein könnten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++## Installieren von [!DNL Workfront] für [!DNL Jira]

Die Installation von [!DNL Workfront] für [!DNL Jira] OnDemand entspricht der Installation auf einer [!DNL Jira] Server-Instanz.

Sie müssen [!DNL Jira] sein, um das [!DNL Workfront]-Add-on zu installieren.

Wenn Sie kein [!DNL Jira] sind, können Sie nach dem [!DNL Workfront]-Add-on suchen und dessen Installation anfordern. Ihre Anforderung wird zur Genehmigung und Installation an den [!DNL Jira]-Administrator gesendet.

Weitere Informationen zum Anfordern eines Add-ons zur Installation in Ihrem [!DNL Jira]-Programm finden Sie unter [Verwalten von Benutzeranfragen für Add-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

So installieren Sie [!DNL Workfront for Jira]:

1. Melden Sie sich bei [!DNL Jira] als [!DNL Jira] an.
1. Suchen Sie das **[!DNL Workfront for Jira]**-Add-on in der [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Klicken Sie **[!UICONTROL Jetzt abrufen]**, um es zu installieren.

   Nach Abschluss der Installation können Sie sich von [!DNL Workfront] aus bei [!DNL Jira] anmelden und Ihre Integration konfigurieren.

   Weitere Informationen finden Sie unter [Konfigurieren von Adobe Workfront für Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Überlegungen zu einer [!DNL Jira Server] Installation

>[!NOTE]
>
>Diese Anforderungen gelten nicht für die [!UICONTROL OnDemand]-Version ([!UICONTROL Cloud]) [!DNL Jira] Software.

Obwohl die Installation des [!DNL Workfront]-Add-ons in den beiden [!DNL Jira] Umgebungen ähnlich ist, müssen Sie bei der Arbeit mit einer [!DNL Jira Server] Folgendes berücksichtigen:

* Beim Konfigurieren des Add-ons in [!DNL Jira] ist die im Feld **[!DNL JIRA Base URL]** angegebene Adresse möglicherweise nicht die URL, die Sie für den Zugriff auf [!DNL Jira] auf Ihrem privaten Server verwenden. Der **[!DNL JIRA Base URL]** muss eine öffentlich zugängliche Adresse sein, die über NAT- oder Reverse-Proxy-Protokolle mit Ihrem privaten Server verbunden ist, damit [!DNL Workfront] darauf zugreifen können, um Anfragen an Ihren Server zu stellen.

* Sie müssen eine SSL-Verschlüsselung verwenden, um die Kommunikation zwischen [!DNL Jira] und [!DNL Workfront] zu sichern. Wenn Sie SSL aktivieren, müssen Sie über einen vollständigen SSL-Zertifikatstapel von einer Zertifizierungsstelle verfügen. Wir unterstützen keine selbstsignierten Zertifikate.
* Sie müssen sicherstellen, dass die [!DNL jira.workfront.com] Domain von Ihren Unternehmensservern aus zugänglich ist. Es dient als Middleware-Umgebung zwischen [!DNL Workfront] und [!DNL Jira] und ist für den Betrieb des Add-ons erforderlich.

  Außerdem müssen Sie die folgenden statischen IP-Adressen zur -Zulassungsliste Ihrer Firewall für ausgehende und eingehende Verbindungen hinzufügen.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Weitere Informationen zum Konfigurieren der Firewall für eine optimale Funktionalität mit [!DNL Workfront] finden Sie unter [Konfigurieren der Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
