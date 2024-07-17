---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Erstellen von Aufgaben und Problemen über Slack
description: Nachdem Sie [!DNL Adobe Workfront] für das Slack installiert und konfiguriert haben, können Sie Aufgaben und Probleme von Slack erstellen und sie mit Projekten in Workfront verknüpfen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Erstellen von Aufgaben und Problemen aus [!DNL Slack]

Nachdem Sie [!DNL Adobe Workfront for Slack] installiert und konfiguriert haben, können Sie Aufgaben und Probleme aus [!DNL Slack] erstellen und sie mit Projekten in [!DNL Workfront] verknüpfen.

Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit [!DNL Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Sie müssen Zugriff haben, um Aufgaben und Probleme in Ihrer Zugriffsebene erstellen zu können, und Sie müssen über [!UICONTROL Contribute] -Berechtigungen für das Projekt verfügen, mit dem Sie sie verknüpfen.

Weitere Informationen zu Zugriffsebenen finden Sie unter [Übersicht über Zugriffsebenen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Weitere Informationen zu Berechtigungen für Objekte finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.\

## Voraussetzungen

Bevor Sie Aufgaben und Probleme mit [!DNL Slack] erstellen können, müssen Sie

* [!DNL Workfront] für Slack konfigurieren\
   Anweisungen zum Konfigurieren von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Erstellen von Aufgaben aus [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz an und melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an.\
   Weitere Informationen zum Anmelden bei Workfront von [!DNL Slack] finden Sie im Abschnitt &quot;Anmeldung bei [!DNL Workfront] von [!DNL Slack]&quot;unter [Zugriff [!DNL Adobe Workfront] von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus den folgenden Befehl in das Meldungsfeld ein:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden. Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.
   >  
   >Der Aufgabenname muss so eingegeben werden, wie er in der Benutzeroberfläche von [!DNL Workfront] angezeigt wird, ohne Klammern oder Anführungszeichen.

1. (Optional) Beginnen Sie mit der Eingabe des Namens eines Projekts, mit dem Sie die neue Aufgabe verknüpfen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird.\
   Sie erhalten eine Bestätigung, die angibt, dass die Aufgabe zum ausgewählten Projekt hinzugefügt wurde.
1. (Optional) Klicken Sie in der Bestätigungsnachricht auf den Namen der Aufgabe, um sie in [!DNL Workfront] auf einer neuen Registerkarte des Browsers zu öffnen.

## Erstellen von Problemen aus [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz an und melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an.\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt &quot;Anmeldung bei [!DNL Workfront] von [!DNL Slack]&quot;unter [Zugriff [!DNL Adobe Workfront]  von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus den folgenden Befehl in das Meldungsfeld ein:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden. Sie können Ihren Befehl mit &quot;/wf&quot;anstelle von &quot;/workfront&quot;starten. \
   >Der Name des Problems muss so eingegeben werden, wie er in der Benutzeroberfläche von [!DNL Workfront] angezeigt wird, ohne Klammern oder Anführungszeichen.

1. (Optional) Geben Sie den Namen eines Projekts ein, mit dem Sie das neue Problem verknüpfen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird.\
   Sie erhalten eine Bestätigung, dass das Problem zum ausgewählten Projekt hinzugefügt wurde.
1. (Optional) Klicken Sie in der Bestätigungsnachricht auf den Namen des Problems, um es in [!DNL Workfront] auf einer neuen Browser-Registerkarte zu öffnen.
