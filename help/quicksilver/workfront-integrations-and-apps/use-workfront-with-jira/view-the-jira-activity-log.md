---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira-Aktivitätsprotokoll anzeigen
description: Als [!DNL Jira] Administrator können Sie die Ausnahmen und Fehler anzeigen, die während der Synchronisierung oder Erstellung der Tickets zwischen [!DNL Adobe Workfront] und [!DNL Jira] in einem Aktivitätsprotokoll auftreten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Anzeigen des [!UICONTROL [!DNL Jira] Aktivitätsprotokolls]

Als [!DNL Jira] -Administrator können Sie die Ausnahmen und Fehler anzeigen, die während der Synchronisation oder Erstellung der Tickets zwischen [!DNL Adobe Workfront] und [!DNL Jira] in einem [!UICONTROL Aktivitätsprotokoll] auftreten.

Sie können bis zu 500 Elemente im Aktivitätsprotokoll anzeigen. Diese werden beginnend mit den letzten aufgelistet.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Lizenzübersicht</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu widmen, anstatt vorhandene zu Benutzern gehörende Konten zu verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen zu [!DNL Workfront] -Administratoren finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für einen Benutzer</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie Elemente zwischen [!DNL Workfront] und [!DNL Jira] verknüpfen können, müssen Sie

* Installieren Sie [!DNL Workfront for Jira]

  Anweisungen zum Installieren von [!DNL Workfront for Jira] finden Sie unter [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Greifen Sie auf das [!UICONTROL [!DNL Jira] Aktivitätsprotokoll] zu:

1. Melden Sie sich bei Jira als Systemadministrator an.
1. Klicken Sie im Hauptmenü von [!DNL Jira] auf **[!UICONTROL Einstellungen]** .
1. Klicken Sie auf **[!UICONTROL Add-ons]** und dann auf **[!UICONTROL Add-ons verwalten]**.

1. Erweitern Sie das Add-on **[!DNL Workfront]** .
1. Klicken Sie auf **[!UICONTROL Konfigurieren]**.
1. Melden Sie sich bei [!DNL Workfront] als Systemadministrator an.
1. Wählen Sie die Registerkarte **[!UICONTROL Aktivitätsprotokoll]** aus.

   Zeigen Sie Informationen zu Ausnahmen und Fehlern an, die während der Erstellung von Elementen oder der Synchronisierung von Feldern zwischen den beiden Anwendungen aufgetreten sind.

   Das Protokoll enthält die folgenden Felder:

   * Datum des Vorkommens
   * Der Name des Benutzers in Jira
   * Jira-Ausgabe Nr.
   * Eine kurze Beschreibung des aufgetretenen Fehlers.
