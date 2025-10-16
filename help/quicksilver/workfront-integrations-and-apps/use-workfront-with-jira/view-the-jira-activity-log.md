---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira-Aktivitätsprotokoll anzeigen
description: Als  [!DNL Jira]  können Sie die Ausnahmen und Fehler, die bei der Synchronisierung oder Erstellung der Tickets zwischen/und [!DNL Adobe Workfront]  auftreten,  [!DNL Jira]  einem Aktivitätsprotokoll anzeigen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 1%

---

# Anzeigen des [!UICONTROL [!DNL Jira] Aktivitätsprotokolls]

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses wird die Integration von Workfront für Jira nach dem 28. **2026 nicht mehr**.
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Jira zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Jira finden Sie unter [Jira-Softwaremodule](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

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

Als [!DNL Jira] können Sie die Ausnahmen und Fehler, die bei der Synchronisierung oder Erstellung der Tickets zwischen [!DNL Adobe Workfront] und [!DNL Jira] auftreten, in einem [!UICONTROL Aktivitätsprotokoll] anzeigen.

Im Aktivitätsprotokoll werden bis zu 500 Elemente angezeigt, wobei sie mit den neuesten aufgelistet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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

+++

## Voraussetzungen

Bevor Sie Elemente zwischen [!DNL Workfront] und [!DNL Jira] verknüpfen können, müssen Sie

* Installieren von [!DNL Workfront for Jira]

  Anweisungen zur Installation von [!DNL Workfront for Jira] finden Sie unter [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Greifen Sie auf das [!UICONTROL [!DNL Jira] Aktivitätsprotokoll zu]:

1. Melden Sie sich bei Jira als Systemadministrator an.
1. Klicken Sie **[!UICONTROL Hauptmenü auf]** Einstellungen[!DNL Jira].
1. Klicken Sie **[!UICONTROL Add-ons]** und dann **[!UICONTROL Add-ons verwalten]**.

1. Erweitern Sie das Add-on **[!DNL Workfront]** .
1. Klicken Sie **[!UICONTROL Konfigurieren]**.
1. Melden Sie sich bei [!DNL Workfront] als Systemadministrator an.
1. Wählen Sie die **[!UICONTROL Aktivitätsprotokoll]** aus.

   Zeigt Informationen zu Ausnahmen und Fehlern an, die bei der Erstellung von Elementen oder der Synchronisierung von Feldern zwischen den beiden Anwendungen aufgetreten sind.

   Das Protokoll enthält die folgenden Felder:

   * Datum des Ereignisses
   * Der Name des Benutzers in Jira
   * Jira Problemnummer
   * Eine kurze Beschreibung des aufgetretenen Fehlers.
