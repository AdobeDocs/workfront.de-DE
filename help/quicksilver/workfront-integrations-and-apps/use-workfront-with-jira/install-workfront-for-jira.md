---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installieren [!DNL Adobe Workfront] für [!DNL Jira]
description: Sie können  [!DNL Adobe Workfront] -for [!DNL Jira]  verwenden, um Ihre  [!DNL Jira] - [!DNL Workfront]  zu integrieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Installieren von [!DNL Adobe Workfront for Jira]

Sie können [!DNL Adobe Workfront for Jira] verwenden, um Ihre [!DNL Jira]- und [!DNL Workfront] zu integrieren.

Nach der Installation des Add-ons können Sie Workflows definieren, die beim Erstellen von [!DNL Workfront] automatisch [!DNL Jira] Probleme verursachen. Die Elemente in beiden Anwendungen werden verknüpft, und einige ihrer Informationen können in beiden Systemen automatisch aktualisiert werden.

Von dieser Integration können alle Anwender in [!DNL Workfront] und [!DNL Jira] profitieren. Sie benötigen lediglich eine Lizenz für das System, in dem sie am meisten arbeiten, und nicht für beide Systeme.

Dieses Add-on ist für die Versionen [!UICONTROL Server] und [!UICONTROL OnDemand] (oder [!UICONTROL Cloud]) [!DNL Jira] Software verfügbar. Dieses Add-on ist für die [!DNL Data Center] Version [!DNL Jira] Software nicht verfügbar.

Eine Liste der [!DNL Jira] Versionen, die [!DNL Workfront for Jira] derzeit unterstützt, finden Sie unter [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) im Atlassian Marketplace.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> 
   <p>Neu: Beliebig</p>
   <p>Aktuell: [!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] - Übersicht</td> 
   <td> 
   <p>Neu: Standard</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu ermöglichen, anstatt vorhandene Konten zu verwenden, die an Benutzer angehängt sein könnten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td><p>Sie müssen [!DNL Workfront] sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Installieren von [!DNL Workfront] für [!DNL Jira]

Die Installation von [!DNL Workfront] für [!DNL Jira] OnDemand entspricht der Installation auf einer [!DNL Jira] Server-Instanz.

Sie müssen [!DNL Jira] sein, um das [!DNL Workfront]-Add-on zu installieren.

Wenn Sie kein [!DNL Jira] sind, können Sie nach dem [!DNL Workfront]-Add-on suchen und dessen Installation anfordern. Ihre Anforderung wird zur Genehmigung und Installation an den [!DNL Jira]-Administrator gesendet.

Weitere Informationen zum Anfordern eines Add-ons zur Installation in Ihrem [!DNL Jira]-Programm finden Sie unter [Verwalten von Benutzeranfragen für Add-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

So installieren Sie [!DNL Workfront for Jira]:

1. Melden Sie sich bei [!DNL Jira] als [!DNL Jira] an.
1. Suchen Sie das **[!DNL Workfront for Jira]**-Add-on in der [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Klicken Sie **[!UICONTROL Jetzt abrufen]**, um es zu installieren.

   Nach Abschluss der Installation können Sie sich von [!DNL Jira] aus bei [!DNL Workfront] anmelden und Ihre Integration konfigurieren.

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
