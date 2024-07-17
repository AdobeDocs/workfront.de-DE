---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Empfangen von [!DNL Adobe Workfront] Benachrichtigungen in  [!DNL Slack]
description: Empfangen von [!DNL Adobe Workfront] Benachrichtigungen in  [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---

# [!DNL Adobe Workfront] Benachrichtigungen in [!DNL Slack] empfangen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Nachdem Sie [!DNL Adobe Workfront for Slack] installiert haben, können Sie [!DNL Workfront] Benachrichtigungen in [!DNL Slack] erhalten.\
Weitere Informationen zum Installieren von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Sie können festlegen, dass eine bestimmte Anzahl von [!UICONTROL Benachrichtigungen], die in der Benachrichtigungsblase in der [!DNL Workfront] -Benutzeroberfläche angezeigt werden, auch in [!DNL Slack] bereitgestellt wird.

E-Mail-Benachrichtigungen funktionieren unabhängig von [!DNL Workfront] -Benachrichtigungen in der Benutzeroberfläche. Sie oder Ihr [!DNL Workfront] -Administrator können E-Mail-Benachrichtigungen deaktivieren, während Schnittstellenbenachrichtigungen in [!DNL Workfront] nicht deaktiviert werden können.\
Sie können jedoch [!DNL Workfront]-Benachrichtigungen deaktivieren, die Sie möglicherweise in [!DNL Slack] erhalten, wenn Sie sich nur auf diese Benachrichtigungen in der [!DNL Workfront] -Oberfläche konzentrieren möchten.

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

Bevor Sie [!DNL Workfront]-Benachrichtigungen in [!DNL Slack] erhalten können, müssen Sie

* Konfigurieren von [!DNL Workfront for Slack]\
   Anweisungen zum Konfigurieren von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## [!DNL Workfront]-Benachrichtigungen für [!DNL Slack] konfigurieren {#configure-workfront-notifications-for-slack}

1. (Bedingt) Nachdem [!DNL Workfront] zu Ihrer [!DNL Slack]-Instanz hinzugefügt wurde, melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an.\
   Informationen zum Anmelden bei [!DNL Workfront] von [!DNL Slack] finden Sie unter [Zugriff [!DNL Adobe Workfront] von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus einen der folgenden Befehle in das Meldungsfeld ein:

   `/workfront settings`

   Oder

   `/wf settings`

1. Alle Benachrichtigungen sind standardmäßig aktiviert.\
   Deaktivieren Sie eine der folgenden Benachrichtigungen:

   * [!UICONTROL Ich bin einer neuen Aufgabe oder einem neuen Problem zugewiesen]
   * [!UICONTROL Mein Team wird einer neuen Aufgabe oder einem neuen Problem zugewiesen]
   * [!UICONTROL Ich erhalte eine neue Genehmigungs- oder Zugriffsanfrage]
   * [!UICONTROL Jemand bezieht mich in eine gezielte Aktualisierung ein]
   * [!UICONTROL Jemand kommentiert einen Thread, in dem ich mich in] befinde
   * [!UICONTROL An einer Aufgabe, einem Problem oder einem Projekt, für das ich angemeldet bin, wird eine Aktualisierung vorgenommen.]
   * [!UICONTROL Jemand kommentiert eines meiner Arbeitselemente]
   * [!UICONTROL Jemand kommentiert meine Hilfeanfrage]

   Die Änderungen, die Sie an den Optionen für [!UICONTROL Benachrichtigungen] vornehmen, werden sofort wirksam.\
   Die Benachrichtigungen, die Sie aktiviert haben, werden im Kanal [!DNL Workfront] [!DNL Slack] bereitgestellt. Wenn Sie Benachrichtigungen hier deaktivieren, sind sie nur für [!DNL Slack] und nicht für die [!DNL Workfront] -Oberfläche deaktiviert. Sie erhalten sie weiterhin in der &quot;[!DNL Workfront]&quot;-Benachrichtigungsblase oben rechts in der Benutzeroberfläche.

## [!DNL Workfront] Benachrichtigungen von [!DNL Slack] verwalten

Sie können [!DNL Workfront]-Benachrichtigungen von [!DNL Slack] empfangen und darauf reagieren.

Sie können E-Mail-Benachrichtigungen für Benachrichtigungen deaktivieren, die Sie in [!DNL Slack] aktivieren, um sicherzustellen, dass Sie keine doppelten Benachrichtigungen erhalten.\
Informationen zum Konfigurieren Ihrer E-Mail-Benachrichtigungen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Die Aktivierung oder Deaktivierung von [!DNL Workfront] -Benachrichtigungen in [!DNL Slack] wirkt sich nicht auf die Benachrichtigungen aus, die Sie innerhalb der [!DNL Workfront] -Oberfläche erhalten.\
Benachrichtigungen innerhalb der [!DNL Workfront] -Oberfläche können nicht deaktiviert werden.

So verwalten Sie Ihre [!DNL Workfront]-Benachrichtigungen für [!DNL Slack]:

1. Melden Sie sich bei [!UICONTROL Slack] an.
1. Melden Sie sich bei [!DNL Workfront] von [!DNL Slack] an.\
   Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt &quot;Anmeldung bei [!DNL Workfront] von [!DNL Slack]&quot;unter [Zugriff [!DNL Adobe Workfront] von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Stellen Sie sicher, dass Ihre [!DNL Workfront] -Benachrichtigungen für [!DNL Slack] aktiviert sind.\
   Weitere Informationen dazu, welche [!DNL Workfront]-Benachrichtigungen so konfiguriert werden können, dass sie auch an [!DNL Slack] gesendet werden, finden Sie unter [Konfigurieren von [!DNL Workfront] Benachrichtigungen für  [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Gehen Sie zum Kanal **[!DNL Workfront]** , um Ihre [!DNL Workfront] -Benachrichtigungen zu finden.
1. (Bedingt und optional) Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Bearbeiten]** , um die Bearbeitung einer Aufgabe zu akzeptieren.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Antworten in[!DNL Workfront]]** , um auf einen Kommentar zu antworten, geben Sie Ihre Antwort ein und klicken Sie auf **[!UICONTROL Antworten]**.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]** , um eine Aufgabe, ein Problem oder ein Projekt zu genehmigen oder abzulehnen, für die die Genehmigung aussteht.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Genehmigen]**, **[!UICONTROL Änderungen]** oder **[!UICONTROL Ablehnen]** , um ein Dokument zu genehmigen, mit Änderungen zu genehmigen oder abzulehnen.

     Sie können auch mit dem Mauszeiger über die Miniaturansicht des Dokuments fahren und auf das Lupensymbol klicken, um eine größere Vorschau des Dokuments anzuzeigen, bevor Sie es genehmigen.\
      Nur die genehmigten Slack [Dateitypen](https://api.slack.com/types/file) können in der Vorschau angezeigt werden.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Grant]** oder **[!UICONTROL Ignore]** , um die Anforderung eines weiteren Zugriffs von einem anderen Benutzer zu erteilen oder zu ignorieren.\

     Sie erhalten eine Bestätigung, dass Ihre Aktion in [!DNL Workfront] abgeschlossen wurde, für jede Entscheidung, die Sie in Ihren Benachrichtigungen treffen.
