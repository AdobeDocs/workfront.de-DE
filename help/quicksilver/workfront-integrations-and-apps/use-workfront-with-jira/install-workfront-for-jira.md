---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installieren [!DNL Adobe Workfront] für [!DNL Jira]
description: Sie können [!DNL Adobe Workfront] für [!DNL Jira] zur Integration Ihrer [!DNL Jira] und [!DNL Workfront] Systeme.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Installieren [!DNL Adobe Workfront for Jira]

Sie können [!DNL Adobe Workfront for Jira] zur Integration Ihrer [!DNL Jira] und [!DNL Workfront] Systeme.

Nach der Installation des Add-ons können Sie Workflows definieren, die [!DNL Jira] automatisch Probleme bei [!DNL Workfront] Arbeitselemente werden erstellt. Die Elemente in beiden Anwendungen werden verknüpft und einige ihrer Informationen können automatisch in beiden Systemen aktualisiert werden.

Alle Benutzer in [!DNL Workfront] und [!DNL Jira] kann von dieser Integration profitieren. Sie benötigen nur eine Lizenz für das System, in dem sie am besten funktionieren, und nicht für beide Systeme.

Dieses Add-on ist für das [!UICONTROL Server] und [!UICONTROL OnDemand] (oder [!UICONTROL Cloud]) Versionen von [!DNL Jira] Software. Dieses Add-on steht nicht für die [!DNL Data Center] Version von [!DNL Jira] Software.

Für eine Liste von [!DNL Jira] Versionen [!DNL Workfront for Jira] unterstützt derzeit, siehe [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) im Atlassian Marketplace.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td role="rowheader">Adobe [!DNL Workfront] Lizenzübersicht</td> 
   <td> 
   <p>Neu: Standard</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in der [!DNL Jira] und [!DNL Workfront] , um dieser Integration zu widmen, anstatt vorhandene zu verwenden, die möglicherweise mit Benutzern verbunden sind.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td><p>Sie müssen [!DNL Workfront] Administrator.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Installieren [!DNL Workfront] für [!DNL Jira]

Installieren [!DNL Workfront] für [!DNL Jira] OnDemand ist mit der Installation auf einer [!DNL Jira] Serverinstanz.

Sie müssen [!DNL Jira] Administrator zum Installieren der [!DNL Workfront] -Add-on.

Wenn Sie keine [!DNL Jira] Administrator können Sie nach der [!DNL Workfront] -Add-on hinzufügen und die Installation anfordern. Ihre Anfrage wird an die [!DNL Jira] Administrator für Genehmigung und Installation.

Weitere Informationen zum Anfordern eines Add-ons zur Installation auf Ihrem [!DNL Jira] -Anwendung, siehe [Verwalten von Benutzeranforderungen für Add-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Installieren [!DNL Workfront for Jira]:

1. Anmelden bei [!DNL Jira] as a [!DNL Jira] Administrator.
1. Suchen Sie die **[!DNL Workfront for Jira]** -Add-on im [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Klicks **[!UICONTROL Jetzt downloaden]** um es zu installieren.

   Nach Abschluss der Installation können Sie sich bei [!DNL Workfront] von [!DNL Jira] und konfigurieren Sie Ihre Integration.

   Weitere Informationen finden Sie unter [Adobe Workfront für Jira konfigurieren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Überlegungen zu einer [!DNL Jira Server] Installation

>[!NOTE]
>
>Diese Anforderungen gelten nicht für die [!UICONTROL OnDemand] ([!UICONTROL Cloud]) Version von [!DNL Jira] Software.

Obwohl die [!DNL Workfront] Add-on in den beiden [!DNL Jira] -Umgebungen ähneln, müssen Sie beim Arbeiten mit einer [!DNL Jira Server] Installation:

* Beim Konfigurieren des Add-ons in [!DNL Jira], die in der **[!DNL JIRA Base URL]** darf nicht mit der URL übereinstimmen, auf die Sie zugreifen [!DNL Jira] auf Ihrem privaten Server. Die **[!DNL JIRA Base URL]** muss eine öffentlich zugängliche Adresse sein, die über NAT- oder Reverse-Proxy-Protokolle mit Ihrem privaten Server verbunden ist. [!DNL Workfront] kann darauf zugreifen, um Anfragen an Ihren Server zu senden.

* Sie müssen die SSL-Verschlüsselung verwenden, um die Kommunikation zwischen [!DNL Jira] und [!DNL Workfront]. Wenn Sie SSL aktivieren, müssen Sie über einen vollständigen SSL-Zertifikatstapel von einer Zertifizierungsstelle verfügen. Selbstsignierte Zertifikate werden nicht unterstützt.
* Sie müssen sicherstellen, dass [!DNL jira.workfront.com] auf die Domäne von Ihren Unternehmensservern aus zugegriffen werden kann. Es dient als Middleware-Umgebung zwischen [!DNL Workfront] und [!DNL Jira] und ist erforderlich, damit das Add-on funktioniert.

  Sie müssen außerdem die folgenden statischen IP-Adressen zur Zulassungsliste in Ihrer Firewall für ausgehende und eingehende Verbindungen hinzufügen.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Weitere Informationen zum Konfigurieren der Firewall für optimale Funktionalität finden Sie unter [!DNL Workfront], siehe [Konfigurieren der Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
