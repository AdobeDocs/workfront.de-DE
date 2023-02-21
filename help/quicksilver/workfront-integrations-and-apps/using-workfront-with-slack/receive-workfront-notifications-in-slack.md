---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Empfangen [!DNL Adobe Workfront] Benachrichtigungen in [!DNL Slack]
description: Empfangen [!DNL Adobe Workfront] Benachrichtigungen in [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 6%

---

# Empfangen [!DNL Adobe Workfront] Benachrichtigungen in [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Nach der Installation [!DNL Adobe Workfront for Slack]können Sie [!DNL Workfront] Benachrichtigungen in [!DNL Slack].\
Informationen zur Installation [!DNL Workfront for Slack], siehe [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Sie können eine bestimmte Anzahl von [!UICONTROL Benachrichtigungen] die in der Benachrichtigungsblase im [!DNL Workfront] -Schnittstelle, die auch in bereitgestellt werden soll [!DNL Slack].

E-Mail-Benachrichtigungen funktionieren unabhängig von [!DNL Workfront] Schnittstellenbenachrichtigungen. Sie oder Ihr [!DNL Workfront] -Administrator kann E-Mail-Benachrichtigungen deaktivieren, während Schnittstellenbenachrichtigungen in [!DNL Workfront].\
Sie können jedoch [!DNL Workfront] Benachrichtigungen, die Sie möglicherweise erhalten in [!DNL Slack], wenn Sie sich nur innerhalb der [!DNL Workfront] -Schnittstelle.

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

Bevor Sie [!DNL Workfront] Benachrichtigungen in [!DNL Slack], müssen Sie

* Konfigurieren [!DNL Workfront for Slack]\
   Anweisungen zum Konfigurieren von [!DNL Workfront for Slack], siehe [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Konfigurieren [!DNL Workfront] Benachrichtigungen für [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Bedingt) Nach [!DNL Workfront] wurde zu Ihrem [!DNL Slack] -Instanz, anmelden [!DNL Workfront] von [!DNL Slack].\
   Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack], siehe [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus einen der folgenden Befehle in das Meldungsfeld ein:

   `/workfront settings`

   Oder

   `/wf settings`

1. Alle Benachrichtigungen sind standardmäßig aktiviert.\
   Deaktivieren Sie eine der folgenden Benachrichtigungen:

   * [!UICONTROL Ich habe eine neue Aufgabe oder ein neues Problem.]
   * [!UICONTROL Mein Team wird einer neuen Aufgabe oder einem neuen Problem zugewiesen]
   * [!UICONTROL Ich erhalte eine neue Genehmigungs- oder Zugriffsanfrage]
   * [!UICONTROL Jemand hat mich in die direkte Aktualisierung einbezogen]
   * [!UICONTROL Jemand hat einen Thread kommentiert, an dem ich teilnehme]
   * [!UICONTROL Für eine Aufgabe, ein Problem oder ein Projekt wird ein Update durchgeführt.]
   * [!UICONTROL Jemand kommentiert eines meiner Arbeitselemente]
   * [!UICONTROL Jemand kommentiert meinen Hilfeantrag]

   Die Änderungen, die Sie an den [!UICONTROL Benachrichtigungen] werden sofort wirksam.\
   Die Benachrichtigungen, die Sie aktiviert haben, werden im Abschnitt [!DNL Workfront] [!DNL Slack] -Kanal. Wenn Sie Benachrichtigungen hier deaktivieren, werden sie nur für [!DNL Slack]und nicht für die [!DNL Workfront] -Schnittstelle. Sie erhalten sie weiterhin im [!DNL Workfront] Benachrichtigungen werden oben rechts in der Benutzeroberfläche angezeigt.

## Verwalten [!DNL Workfront] Benachrichtigungen von [!DNL Slack]

Sie können empfangen und beantworten [!DNL Workfront] Benachrichtigungen von [!DNL Slack].

Sie können E-Mail-Benachrichtigungen für Benachrichtigungen deaktivieren, die Sie in [!DNL Slack], um sicherzustellen, dass Sie keine doppelten Benachrichtigungen erhalten.\
Informationen zur Konfiguration Ihrer E-Mail-Benachrichtigungen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Aktivieren oder Deaktivieren [!DNL Workfront] Benachrichtigungen in [!DNL Slack] wirkt sich nicht auf die Benachrichtigungen aus, die Sie innerhalb der [!DNL Workfront] -Schnittstelle.\
Benachrichtigungen innerhalb der [!DNL Workfront] -Schnittstelle kann nicht deaktiviert werden.

So verwalten Sie [!DNL Workfront] Benachrichtigungen für [!DNL Slack]:

1. Anmelden bei [!UICONTROL Slack].
1. Anmelden bei [!DNL Workfront] von [!DNL Slack].\
   Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack], siehe &quot;Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; Abschnitt in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Stellen Sie sicher, dass [!DNL Workfront] Benachrichtigungen für [!DNL Slack] aktiviert sind.\
   Weitere Informationen darüber, [!DNL Workfront] Benachrichtigungen können so konfiguriert werden, dass sie auch an [!DNL Slack], siehe [Konfigurieren [!DNL Workfront] Benachrichtigungen für [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Navigieren Sie zu **[!DNL Workfront]** Kanal zum Auffinden Ihrer [!DNL Workfront] Benachrichtigungen.
1. (Bedingt und optional) Führen Sie einen der folgenden Schritte aus:

   * Klicken **[!UICONTROL Arbeiten daran]** , um zu akzeptieren, an einer Aufgabe zu arbeiten.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Antwort in[!DNL Workfront]]** Um auf einen Kommentar zu antworten, geben Sie Ihre Antwort ein und klicken Sie auf **[!UICONTROL Antwort]**.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]** , um Aufgaben, Probleme oder Projekte zu genehmigen oder abzulehnen, die noch nicht genehmigt wurden.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Genehmigen]**, **[!UICONTROL Änderungen]** oder **[!UICONTROL Ablehnen]**, um ein Dokument zu genehmigen, mit Änderungen zu genehmigen oder abzulehnen.

      Sie können auch mit dem Mauszeiger über die Miniaturansicht des Dokuments fahren und auf das Lupensymbol klicken, um eine größere Vorschau des Dokuments anzuzeigen, bevor Sie es genehmigen.\
      Nur der genehmigte Slack [Dateitypen](https://api.slack.com/types/file) kann in der Vorschau angezeigt werden.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Förderung]** oder **[!UICONTROL Ignorieren]** , um die Anforderung eines weiteren Zugriffs von einem anderen Benutzer zu erteilen oder zu ignorieren.\

      Sie erhalten eine Bestätigung, dass Ihre Aktion in [!DNL Workfront]für jede Entscheidung, die Sie in Ihren Benachrichtigungen treffen.
