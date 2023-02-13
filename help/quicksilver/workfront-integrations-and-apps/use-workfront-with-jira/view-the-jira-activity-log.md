---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira-Aktivitätsprotokoll anzeigen
description: Als [!DNL Jira] Administrator können Sie die Ausnahmen und Fehler anzeigen, die während der Synchronisation oder Erstellung der Tickets zwischen [!DNL Adobe Workfront] und [!DNL Jira] in einem Aktivitätsprotokoll.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Anzeigen der [!UICONTROL [!DNL Jira] Aktivitätsprotokoll]

Als [!DNL Jira] Administrator können Sie die Ausnahmen und Fehler anzeigen, die während der Synchronisation oder Erstellung der Tickets zwischen [!DNL Adobe Workfront] und [!DNL Jira] in einer [!UICONTROL Aktivitätsprotokoll].

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
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] Plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Lizenzübersicht</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in der [!DNL Jira] und [!DNL Workfront] , um dieser Integration zu widmen, anstatt vorhandene zu verwenden, die möglicherweise mit Benutzern verbunden sind.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Bevor Sie Elemente verknüpfen können zwischen [!DNL Workfront] und [!DNL Jira], müssen Sie

* Installieren [!DNL Workfront for Jira]

   Anweisungen zur Installation [!DNL Workfront for Jira], siehe [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Zugriff auf [!UICONTROL [!DNL Jira] Aktivitätsprotokoll]:

1. Melden Sie sich bei Jira als Systemadministrator an.
1. Klicken **[!UICONTROL Einstellungen]** im Hauptteil [!DNL Jira] Menü.
1. Klicken **[!UICONTROL Add-ons]**, dann **[!UICONTROL Verwalten von Add-ons]**.

1. Erweitern Sie die **[!DNL Workfront]** -Add-on.
1. Klicken **[!UICONTROL Konfigurieren]**.
1. Anmelden bei [!DNL Workfront] als Systemadministrator.
1. Wählen Sie die **[!UICONTROL Aktivitätsprotokoll]** Registerkarte.

   Zeigen Sie Informationen zu Ausnahmen und Fehlern an, die während der Erstellung von Elementen oder der Synchronisierung von Feldern zwischen den beiden Anwendungen aufgetreten sind.

   Das Protokoll enthält die folgenden Felder:

   * Datum des Vorkommens
   * Der Name des Benutzers in Jira
   * Nummer der Jira-Ausgabe
   * Eine kurze Beschreibung des aufgetretenen Fehlers.
