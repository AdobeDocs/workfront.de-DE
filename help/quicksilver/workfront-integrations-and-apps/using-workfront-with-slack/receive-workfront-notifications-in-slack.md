---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Empfangen  [!DNL Adobe Workfront]  Benachrichtigungen in [!DNL Slack]
description: Empfangen  [!DNL Adobe Workfront]  Benachrichtigungen in [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

# [!DNL Adobe Workfront]-Benachrichtigungen in [!DNL Slack] empfangen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Nach der Installation von [!DNL Adobe Workfront for Slack] können Sie [!DNL Workfront] Benachrichtigungen in [!DNL Slack] erhalten.\
Informationen zur Installation von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Sie können festlegen, dass eine bestimmte Anzahl [!UICONTROL Benachrichtigungen], die in der Benachrichtigungsblase in der [!DNL Workfront] angezeigt werden, auch in [!DNL Slack] zugestellt wird.

E-Mail-Benachrichtigungen funktionieren unabhängig von Benachrichtigungen in der [!DNL Workfront]. Sie oder Ihr [!DNL Workfront] können E-Mail-Benachrichtigungen deaktivieren, während Benachrichtigungen über die Benutzeroberfläche in [!DNL Workfront] nicht deaktiviert werden können.\
Sie können jedoch [!DNL Workfront] Benachrichtigungen deaktivieren, die Sie möglicherweise in [!DNL Slack] erhalten, wenn Sie sich nur auf diese Benachrichtigungen innerhalb der [!DNL Workfront] konzentrieren möchten.

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

Bevor Sie [!DNL Workfront]-Benachrichtigungen in [!DNL Slack] erhalten können, müssen Sie

* Konfigurieren von [!DNL Workfront for Slack]\
   Anweisungen zum Konfigurieren von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Konfigurieren von [!DNL Workfront]-Benachrichtigungen für [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Bedingt) Nachdem [!DNL Workfront] zu Ihrer [!DNL Slack]-Instanz hinzugefügt wurde, melden Sie sich von [!DNL Workfront] aus bei [!DNL Slack] an.\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie unter [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal einen der folgenden Befehle in das Feld Nachricht ein:

   `/workfront settings`

   Oder

   `/wf settings`

1. Alle Benachrichtigungen sind standardmäßig aktiviert.\
   Deaktivieren Sie eine der folgenden Benachrichtigungen:

   * [!UICONTROL Ich wurde einer neuen Aufgabe oder einem neuen Problem zugewiesen]
   * [!UICONTROL Mein Team wurde einer neuen Aufgabe oder einem neuen Problem zugewiesen]
   * [!UICONTROL Ich erhalte eine neue Genehmigungs- oder Zugriffsanfrage]
   * [!UICONTROL Jemand bezieht mich in eine gezielte Aktualisierung ein]
   * [!UICONTROL Jemand kommentiert einen Thread, an dem ich teilnehme]
   * [!UICONTROL An einer Aufgabe, einem Problem oder Projekt, die bzw. das ich abonniert habe, wird eine Aktualisierung vorgenommen]
   * [!UICONTROL Jemand kommentiert eines meiner Arbeitselemente]
   * [!UICONTROL Jemand kommentiert meine Hilfeanfrage]

   Die Änderungen, die Sie an den [!UICONTROL Benachrichtigungen]-Optionen vornehmen, werden sofort wirksam.\
   Die von Ihnen aktivierten Benachrichtigungen werden im [!DNL Workfront] [!DNL Slack] Kanal zugestellt. Wenn Sie hier Benachrichtigungen deaktivieren, werden sie nur für [!DNL Slack] deaktiviert, nicht aber für die [!DNL Workfront]. Sie erhalten sie weiterhin in der [!DNL Workfront] Benachrichtigungsblase oben rechts in der Benutzeroberfläche.

## Verwalten von [!DNL Workfront]-Benachrichtigungen von [!DNL Slack]

Sie können [!DNL Workfront] Benachrichtigungen von [!DNL Slack] empfangen und darauf reagieren.

Sie können E-Mail-Benachrichtigungen für Benachrichtigungen deaktivieren, die Sie in [!DNL Slack] aktivieren, um sicherzustellen, dass Sie keine doppelten Benachrichtigungen erhalten.\
Informationen zum Konfigurieren Ihrer E-Mail-Benachrichtigungen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Das Aktivieren oder Deaktivieren [!DNL Workfront] Benachrichtigungen in [!DNL Slack] hat keine Auswirkungen auf die Benachrichtigungen, die Sie in der [!DNL Workfront] erhalten.\
Benachrichtigungen in der [!DNL Workfront] können nicht deaktiviert werden.

So verwalten Sie [!DNL Workfront]-Benachrichtigungen für [!DNL Slack]:

1. Anmelden bei [!UICONTROL Slack].
1. Melden Sie sich von [!DNL Workfront] aus bei [!DNL Slack] an.\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt „Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Stellen Sie sicher, dass Ihre [!DNL Workfront] Benachrichtigungen für [!DNL Slack] aktiviert sind.\
   Weitere Informationen dazu, welche [!DNL Workfront] Benachrichtigungen konfiguriert werden können, um auch an [!DNL Slack] gesendet zu werden, finden Sie unter [Konfigurieren von  [!DNL Workfront]  für [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Gehen Sie zum **[!DNL Workfront]** Kanal, um Ihre [!DNL Workfront] Benachrichtigungen zu finden.
1. (Bedingt und optional) Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Bearbeiten]**, um eine Aufgabe anzunehmen.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Antworten in[!DNL Workfront]]**, um auf einen Kommentar zu antworten, geben Sie Ihre Antwort ein und klicken Sie auf **[!UICONTROL Antworten]**.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]** um eine Aufgabe, ein Problem oder ein Projekt, für die bzw. das Ihre Genehmigung noch aussteht, zu genehmigen oder abzulehnen.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Genehmigen]**, **&#x200B;**&#x200B;oder **[!UICONTROL Ablehnen]**, um ein Dokument zu genehmigen, mit Änderungen zu genehmigen oder abzulehnen.

     Sie können auch mit dem Mauszeiger über die Miniaturansicht des Dokuments fahren und auf das Lupensymbol klicken, um eine größere Vorschau des Dokuments anzuzeigen, bevor Sie es genehmigen.\
      Nur die genehmigten Slack [Dateitypen](https://api.slack.com/types/file) können in der Vorschau angezeigt werden.

   * (Bedingt und optional) Klicken Sie auf **[!UICONTROL Gewähren]** oder **[!UICONTROL Ignorieren]**, um einem anderen Benutzer die Anforderung für weiteren Zugriff zu gewähren oder zu ignorieren.\

     Sie erhalten für jede Entscheidung, die Sie in Ihren Benachrichtigungen treffen, eine Bestätigung, dass Ihre Aktion in [!DNL Workfront] abgeschlossen wurde.
