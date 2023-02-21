---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Erstellen von Aufgaben und Problemen aus Slack
description: 'Nach der Installation und Konfiguration [!DNL Adobe Workfront] Slack: Sie können Aufgaben und Probleme aus Slack erstellen und sie mit Projekten in Workfront verknüpfen.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Erstellen von Aufgaben und Problemen aus [!DNL Slack]

Nach der Installation und Konfiguration [!DNL Adobe Workfront for Slack], können Sie Aufgaben und Probleme erstellen aus [!DNL Slack] und verknüpfen sie mit Projekten in [!DNL Workfront].

Weitere Informationen zur Konfiguration [!DNL Workfront] mit [!DNL Slack], siehe [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Sie müssen Zugriff auf die Erstellung von Aufgaben und Problemen in Ihrer Zugriffsebene haben und über [!UICONTROL Beitragen] Berechtigungen für das Projekt, mit dem Sie sie verknüpfen.

Weitere Informationen zu Zugriffsebenen finden Sie unter [Übersicht über Zugriffsebenen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Weitere Informationen zu Berechtigungen für Objekte finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] Plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] administrator.\

## Voraussetzungen

Bevor Sie Aufgaben und Probleme aus erstellen können, [!DNL Slack], müssen Sie

* Konfigurieren [!DNL Workfront] für Slack\
   Anweisungen zum Konfigurieren von [!DNL Workfront for Slack], siehe [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Erstellen von Aufgaben aus [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz und melden Sie sich bei [!DNL Workfront] von [!DNL Slack].\
   Weitere Informationen zur Anmeldung bei Workfront von [!DNL Slack], siehe &quot;Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; Abschnitt in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus den folgenden Befehl in das Meldungsfeld ein:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden. Sie können Ihren Befehl mit `/wf` anstelle von `/workfront`.
   >  
   >Der Aufgabenname muss so eingegeben werden, wie er im [!DNL Workfront] -Schnittstelle ohne Klammern oder Anführungszeichen.

1. (Optional) Beginnen Sie mit der Eingabe des Namens eines Projekts, mit dem Sie die neue Aufgabe verknüpfen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird.\
   Sie erhalten eine Bestätigung, die angibt, dass die Aufgabe zum ausgewählten Projekt hinzugefügt wurde.
1. (Optional) Klicken Sie in der Bestätigungsnachricht auf den Namen der Aufgabe, um sie in [!DNL Workfront]in einer neuen Browser-Registerkarte.

## Erstellen von Problemen aus [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz und melden Sie sich bei [!DNL Workfront] von [!DNL Slack].\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack], siehe &quot;Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; Abschnitt in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus den folgenden Befehl in das Meldungsfeld ein:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden. Sie können Ihren Befehl mit &quot;/wf&quot;anstelle von &quot;/workfront&quot;starten. \
   >Der Problemname muss so eingegeben werden, wie er im [!DNL Workfront] -Schnittstelle ohne Klammern oder Anführungszeichen.

1. (Optional) Beginnen Sie mit der Eingabe des Namens eines Projekts, mit dem Sie das neue Problem verknüpfen möchten, und wählen Sie es aus, wenn es in der Liste angezeigt wird.\
   Sie erhalten eine Bestätigung, dass das Problem zum ausgewählten Projekt hinzugefügt wurde.
1. (Optional) Klicken Sie in der Bestätigungsnachricht auf den Namen des Problems, um es in [!DNL Workfront]in einer neuen Browser-Registerkarte.
