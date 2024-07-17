---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installieren Sie [!DNL Adobe Workfront] für [!DNL Jira]
description: Sie können [!DNL Adobe Workfront] für [!DNL Jira] zur Integration Ihrer [!DNL Jira] und [!DNL Workfront] Systeme verwenden.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Installieren Sie [!DNL Adobe Workfront for Jira]

Sie können [!DNL Adobe Workfront for Jira] verwenden, um Ihre [!DNL Jira]- und [!DNL Workfront]-Systeme zu integrieren.

Nach der Installation des Add-ons können Sie Workflows definieren, die bei der Erstellung von [!DNL Workfront] Arbeitselementen automatisch [!DNL Jira] Probleme verursachen. Die Elemente in beiden Anwendungen werden verknüpft und einige ihrer Informationen können automatisch in beiden Systemen aktualisiert werden.

Alle Benutzer in [!DNL Workfront] und [!DNL Jira] können von dieser Integration profitieren. Sie benötigen nur eine Lizenz für das System, in dem sie am besten funktionieren, und nicht für beide Systeme.

Dieses Add-on ist für die Versionen [!UICONTROL Server] und [!UICONTROL OnDemand] (oder [!UICONTROL Cloud]) der Software [!DNL Jira] verfügbar. Dieses Add-on ist nicht für die [!DNL Data Center] -Version der [!DNL Jira] -Software verfügbar.

Eine Liste der von [!DNL Workfront for Jira] derzeit unterstützten [!DNL Jira] Versionen finden Sie unter [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) im Atlassian Marketplace.

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
   <td role="rowheader">Übersicht über Adobe [!DNL Workfront] -Lizenzen</td> 
   <td> 
   <p>Neu: Standard</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu widmen, anstatt vorhandene zu Benutzern gehörende Konten zu verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td><p>Sie müssen ein [!DNL Workfront] -Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Installieren Sie [!DNL Workfront] für [!DNL Jira]

Die Installation von [!DNL Workfront] für [!DNL Jira] OnDemand entspricht der Installation auf einer [!DNL Jira] Server-Instanz.

Sie müssen ein [!DNL Jira] -Administrator sein, um das [!DNL Workfront]-Add-on zu installieren.

Wenn Sie kein [!DNL Jira] -Administrator sind, können Sie nach dem [!DNL Workfront] -Add-on suchen und dessen Installation anfordern. Ihre Anfrage wird zur Genehmigung und Installation an den [!DNL Jira] -Administrator gesendet.

Weitere Informationen zum Anfordern eines Add-ons für die Installation in Ihrer [!DNL Jira]-Anwendung finden Sie unter [Verwalten von Benutzeranforderungen für Add-ons](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html).

So installieren Sie [!DNL Workfront for Jira]:

1. Melden Sie sich bei [!DNL Jira] als [!DNL Jira] -Administrator an.
1. Suchen Sie das Add-on **[!DNL Workfront for Jira]** im [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Klicken Sie auf **[!UICONTROL Jetzt herunterladen]** , um es zu installieren.

   Nach Abschluss der Installation können Sie sich von [!DNL Jira] bei [!DNL Workfront] anmelden und Ihre Integration konfigurieren.

   Weitere Informationen finden Sie unter [Adobe Workfront für Jira konfigurieren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Überlegungen zur Installation von [!DNL Jira Server]

>[!NOTE]
>
>Diese Anforderungen gelten nicht für die Version [!UICONTROL OnDemand] ([!UICONTROL Cloud]) der [!DNL Jira] -Software.

Obwohl die Installation des [!DNL Workfront]-Add-ons in den beiden [!DNL Jira] -Umgebungen ähnlich ist, müssen Sie beim Arbeiten mit einer [!DNL Jira Server] -Installation Folgendes beachten:

* Beim Konfigurieren des Add-ons in [!DNL Jira] ist die im Feld **[!DNL JIRA Base URL]** angegebene Adresse möglicherweise nicht dieselbe URL, die Sie für den Zugriff auf [!DNL Jira] auf Ihrem privaten Server verwenden. Die **[!DNL JIRA Base URL]** muss eine öffentlich zugängliche Adresse sein, die über NAT- oder Reverse-Proxy-Protokolle mit Ihrem privaten Server verbunden ist, sodass [!DNL Workfront] darauf zugreifen kann, um Anfragen an Ihren Server zu senden.

* Sie müssen die SSL-Verschlüsselung verwenden, um die Kommunikation zwischen [!DNL Jira] und [!DNL Workfront] zu sichern. Wenn Sie SSL aktivieren, müssen Sie über einen vollständigen SSL-Zertifikatstapel von einer Zertifizierungsstelle verfügen. Selbstsignierte Zertifikate werden nicht unterstützt.
* Sie müssen sicherstellen, dass der Zugriff auf die Domäne [!DNL jira.workfront.com] von Ihren Unternehmensservern aus erfolgt. Es dient als Middleware-Umgebung zwischen [!DNL Workfront] und [!DNL Jira] und ist erforderlich, damit das Add-on funktioniert.

  Sie müssen außerdem die folgenden statischen IP-Adressen zur Zulassungsliste in Ihrer Firewall für ausgehende und eingehende Verbindungen hinzufügen.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Weitere Informationen zum Konfigurieren Ihrer Firewall für eine optimale Funktionalität mit [!DNL Workfront] finden Sie unter [Konfigurieren Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
