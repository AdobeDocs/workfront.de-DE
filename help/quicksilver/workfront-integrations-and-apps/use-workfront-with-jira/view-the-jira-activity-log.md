---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira-Aktivitätsprotokoll anzeigen
description: Als  [!DNL Jira]  können Sie die Ausnahmen und Fehler, die bei der Synchronisierung oder Erstellung der Tickets zwischen/und [!DNL Adobe Workfront]  auftreten,  [!DNL Jira]  einem Aktivitätsprotokoll anzeigen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Anzeigen des [!UICONTROL [!DNL Jira] Aktivitätsprotokolls]

Als [!DNL Jira] können Sie die Ausnahmen und Fehler, die bei der Synchronisierung oder Erstellung der Tickets zwischen [!DNL Adobe Workfront] und [!DNL Jira] auftreten, in einem [!UICONTROL Aktivitätsprotokoll] anzeigen.

Im Aktivitätsprotokoll werden bis zu 500 Elemente angezeigt, wobei sie mit den neuesten aufgelistet werden.

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
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe [!DNL Workfront]-Lizenzen</a>*</td> 
   <td> <p>[!UICONTROL-Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu ermöglichen, anstatt vorhandene Konten zu verwenden, die an Benutzer angehängt sein könnten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] sein. Informationen zu [!DNL Workfront] finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

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
