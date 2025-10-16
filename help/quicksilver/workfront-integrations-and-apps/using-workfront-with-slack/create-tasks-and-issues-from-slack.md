---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Erstellen von Aufgaben und Problemen aus Slack
description: Nach der Installation und Konfiguration  [!DNL Adobe Workfront]  Slack können Sie Aufgaben und Probleme aus Slack erstellen und sie mit Projekten in Workfront verknüpfen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Erstellen von Aufgaben und Problemen aus [!DNL Slack]

Nachdem Sie [!DNL Adobe Workfront for Slack] installiert und konfiguriert haben, können Sie Aufgaben und Probleme aus [!DNL Slack] erstellen und sie mit Projekten in [!DNL Workfront] verknüpfen.

Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit [!DNL Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Sie müssen Zugriff haben, um Aufgaben und Probleme in Ihrer Zugriffsebene zu erstellen, und Sie müssen [!UICONTROL Beitragen] für das Projekt haben, mit dem Sie sie verknüpfen.

Weitere Informationen zu Zugriffsebenen finden Sie unter [Zugriffsebenen - Übersicht](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Weitere Informationen zu Berechtigungen für Objekte finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Beliebig</p>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie Aufgaben und Probleme aus [!DNL Slack] erstellen können, müssen Sie

* Konfigurieren von [!DNL Workfront] für Slack\
   Anweisungen zum Konfigurieren von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Erstellen von Aufgaben aus [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack]-Instanz an und melden Sie sich von [!DNL Workfront] aus bei [!DNL Slack] an.\
   Weitere Informationen zur Anmeldung bei Workfront von [!DNL Slack] aus finden Sie im Abschnitt „Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal den folgenden Befehl in das Feld Nachricht ein:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden. Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.
   >  
   >Der Aufgabenname muss so eingegeben werden, wie er in der [!DNL Workfront] ohne Klammern oder Anführungszeichen angezeigt wird.

1. (Optional) Geben Sie den Namen eines Projekts ein, mit dem Sie die neue Aufgabe verknüpfen möchten, und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.\
   Sie erhalten eine Bestätigung, dass die Aufgabe zum ausgewählten Projekt hinzugefügt wurde.
1. (Optional) Klicken Sie auf den Namen der Aufgabe in der Bestätigungsnachricht, um sie in [!DNL Workfront] auf einer neuen Browser-Registerkarte zu öffnen.

## Anfragen aus [!DNL Slack] erstellen

1. Melden Sie sich bei Ihrer [!DNL Slack]-Instanz an und melden Sie sich von [!DNL Workfront] aus bei [!DNL Slack] an.\
   Weitere Informationen zum Anmelden bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt „Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal den folgenden Befehl in das Feld Nachricht ein:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden. Sie können Ihren Befehl mit &quot;/wf“ anstelle von &quot;/workfront“ starten. \
   >Der Problemname muss so eingegeben werden, wie er in der [!DNL Workfront]-Oberfläche ohne Klammern oder Anführungszeichen angezeigt wird.

1. (Optional) Geben Sie den Namen eines Projekts ein, mit dem Sie das neue Problem verknüpfen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird.\
   Sie erhalten eine Bestätigung, dass das Problem dem ausgewählten Projekt hinzugefügt wurde.
1. (Optional) Klicken Sie auf den Namen des Problems in der Bestätigungsnachricht, um es in [!DNL Workfront] auf einer neuen Browser-Registerkarte zu öffnen.
