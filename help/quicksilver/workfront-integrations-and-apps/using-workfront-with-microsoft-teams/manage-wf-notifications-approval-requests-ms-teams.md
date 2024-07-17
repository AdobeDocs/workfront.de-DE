---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Verwalten von [!DNL Adobe Workfront] Benachrichtigungen in [!DNL Microsoft] Teams
description: Sie können von  [!DNL Adobe Workfront]  Benachrichtigungen zu Elementen erhalten, die Sie genehmigen müssen, zu Zuweisungen, zu Kommentaren und Änderungen an Elementen, mit denen Sie verknüpft sind.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 0%

---

# Verwalten von [!DNL Adobe Workfront] Benachrichtigungen in [!DNL Microsoft Teams]

>[!NOTE]
>
>Die Adobe Workfront für Microsoft Teams-Integration wird derzeit nur für das klassische Microsoft Teams-Erlebnis unterstützt.

Sie können von [!DNL Adobe Workfront] Benachrichtigungen zu Elementen erhalten, die Sie genehmigen müssen, zu erteilten Zuweisungen oder zu Kommentaren und Änderungen an Elementen, mit denen Sie verknüpft sind.

Diese Benachrichtigungen enthalten [!DNL Workfront] Aktionen, die Sie innerhalb von [!DNL Microsoft Teams] ausführen können, ohne von [!DNL Microsoft Teams] weg zu navigieren, um sie durchzuführen.

>[!NOTE]
>
>[!DNL Microsoft Teams] unterstützt [!DNL Internet Explorer] nicht mehr. Um den [!DNL Adobe Workfront for Microsoft Teams integration] zu verwenden, müssen Sie einen anderen Webbrowser als [!DNL Internet Explorer] verwenden.


## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen für den Empfang von [!DNL Workfront]-Benachrichtigungen in [!DNL Microsoft Teams]

Sie können [!DNL Workfront]-Benachrichtigungen in [!DNL Microsoft Teams] erhalten, wenn die folgenden Bedingungen erfüllt sind:

* Ein Teaminhaber hat [!DNL Workfront for Microsoft Teams] für Ihr Team installiert und konfiguriert.
* Sie sind von [!DNL Microsoft Teams] bei [!DNL Workfront] angemeldet.
* Sie haben Instant-Benachrichtigungen in [!DNL Workfront] aktiviert. Informationen zum Aktivieren von Sofortbenachrichtigungen finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Informationen zum Installieren von [!DNL Workfront for Microsoft Teams] und Anmelden bei [!DNL Workfront from Microsoft Teams] finden Sie unter [Installieren [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Verwalten von [!DNL Workfront] Benachrichtigungen in [!DNL Microsoft Teams]

Wenn die [!DNL Workfront for Microsoft Teams] -App installiert ist, wird in [!DNL Microsoft Teams] für jedes Mitglied dieses Teams ein [!DNL Workfront] Chat-Kanal erstellt. Wenn eine bestimmte Aktion in [!DNL Workfront] ausgeführt wird, können Sie die Einstellungen so konfigurieren, dass [!DNL Workfront for Microsoft Teams] Benachrichtigungen über diese Aktion im Chat-Kanal [!DNL Workfront] von [!DNL Microsoft Teams] erhält.

Beachten Sie beim Arbeiten mit [!DNL Workfront] -Benachrichtigungen von [!DNL Microsoft Teams] Folgendes:

* Sie können nicht alle, sondern nur eine ausgewählte Anzahl von [!DNL Workfront] Benachrichtigungen in [!DNL Microsoft Teams] empfangen.
* Alle Benachrichtigungen, die Sie von [!DNL Workfront] erhalten, werden im Bot-Chat-Kanal [!DNL Workfront] angezeigt.

  Informationen zum Installieren des Bot-Kanals [!DNL Workfront] finden Sie im Artikel [Installieren [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) im Abschnitt [Anmelden bei [!DNL Workfront] von [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) .

* Zwischen dem Zeitpunkt, zu dem eine Aktualisierung in [!DNL Workfront] vorgenommen wird, und dem Zeitpunkt, zu dem Sie die Benachrichtigung in [!DNL Microsoft Teams] erhalten, kann es bis zu einer 5-minütigen Verzögerung geben.
* Für jede [!DNL Microsoft Teams] -Benachrichtigung erhalten Sie auch eine E-Mail-Benachrichtigung.

So verwalten Sie die [!DNL Workfront]-Benachrichtigungen, die Sie in [!DNL Microsoft Teams] empfangen können:

1. Klicken Sie in der linken Navigationsleiste in [!DNL Microsoft Teams] auf das Symbol **[!UICONTROL Mehr hinzugefügt]** (drei Punkte) für Apps .

1. Klicken Sie in der angezeigten Liste auf [!DNL Workfront] .
1. Wählen Sie die Registerkarte **[!UICONTROL Einstellungen]**.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Deaktivieren Sie alle Benachrichtigungen, die Sie nicht erhalten möchten. Sie können Benachrichtigungsgruppen aktivieren oder deaktivieren, z. B. Informationen oder Validierungsbenachrichtigungen, oder Sie können Benachrichtigungen einzeln verwalten.

   Alle Benachrichtigungen sind standardmäßig aktiviert.

   Die Benachrichtigungseinstellungen für [!DNL Workfront for Microsoft] Teams werden automatisch gespeichert.

   >[!NOTE]
   >
   >Den standardmäßig verfügbaren Benachrichtigungen können keine weiteren Benachrichtigungen hinzugefügt werden.

## Antwort auf [!DNL Workfront] Benachrichtigungen und Genehmigungsanfragen in [!DNL Microsoft Teams]

1. Melden Sie sich bei [!DNL Workfront] von [!DNL Microsoft Teams] an.\
   Informationen zur Anmeldung bei [!DNL Workfront] finden Sie unter [Installieren [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Wechseln Sie zum Bereich **[!UICONTROL Chat]** und klicken Sie auf den Bot-Kanal **[!DNL Workfront]** .\
   Dieser Kanal ist für Ihren persönlichen Chat mit dem [!DNL Workfront]-Bot. Hier werden alle [!DNL Workfront] -Benachrichtigungen angezeigt.
1. Je nach Art der Benachrichtigung, die Sie erhalten, gehen Sie zum entsprechenden Abschnitt:

   * [Validierungsbenachrichtigungen](#approval-notifications-approval-notifications)
   * [Zuweisungsbenachrichtigungen](#assignment-notifications-assignment-notifications)
   * [Kommentar-Benachrichtigungen](#comment-notifications-comment-notifications)
   * [Benachrichtigungen aktualisieren](#update-notifications-update-notifications)
   * [Datumsänderungsbenachrichtigungen](#date-change-notifications-date-change-notifications)

### Validierungsbenachrichtigungen {#approval-notifications}

Sie erhalten Validierungsbenachrichtigungen, wenn Sie zur Validierung eines Objekts wie einer Aufgabe, eines Zeitplans oder eines Testversands aufgefordert werden. Sie können die Benachrichtigung dennoch kommentieren. In der Validierungsbenachrichtigung können Sie jedoch die folgenden Aktionen ausführen:

* **[!UICONTROL Genehmigen]**: Klicken Sie auf , um das Element zu genehmigen.
* **[!UICONTROL Ändern]**: Klicken Sie auf , um das Element mit Änderungen zu genehmigen.
* **[!UICONTROL Ablehnen]**: Klicken Sie auf , um das Element abzulehnen.
* **[!UICONTROL Kommentar]**: Klicken Sie auf , um einen Kommentar abzugeben. Ihr Kommentar erscheint auch in [!DNL Workfront] als Aktualisierung des Objekts, um das es bei der Benachrichtigung geht.
* **[!UICONTROL Gehe zu Testversand]**: Klicken Sie auf , um den Testversand zu öffnen. Sie können dann direkt im Testversand eine Entscheidung treffen. Weitere Informationen finden Sie unter [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Nachdem Sie eine Validierungsentscheidung getroffen haben, können Sie sie nicht mehr in der Benachrichtigung ändern.

#### In bestimmten Validierungsbenachrichtigungen verfügbare Aktionen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL Ablehnen]</th> 
   <th> <p>[!UICONTROL Änderung]</p> </th> 
   <th> <p>[!UICONTROL Gehe zu Testversand] </p> </th> 
   <th>[!UICONTROL Kommentar]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Sie müssen ein Projekt genehmigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sie müssen eine Aufgabe validieren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sie müssen ein Problem genehmigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sie müssen ein Dokument genehmigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sie müssen den Zugriff auf ein Objekt genehmigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sie müssen ein Timesheet genehmigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand möchte, dass Sie diesen Beweis genehmigen</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihr Timesheet wird abgelehnt.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihr Timesheet wird erneut geöffnet</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eine von Ihnen angeforderte Dokumentgenehmigungsanforderung wurde genehmigt</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eine angeforderte Dokumentgenehmigungsanforderung wird mit Änderungen genehmigt</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eine von Ihnen angeforderte Dokumentgenehmigungsanforderung wird abgelehnt</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihr Timesheet wurde genehmigt</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Zuweisungsbenachrichtigungen {#assignment-notifications}

Sie erhalten Zuweisungsbenachrichtigungen, wenn Sie oder ein Team, in dem Sie sich befinden, in Workfront einer Aufgabe oder einem Problem zugewiesen sind. In der Zuweisungsbenachrichtigung können Sie die folgenden Aktionen durchführen:

* **[!UICONTROL Bearbeiten]**: Wählen Sie diese Option aus, um das Element zu bearbeiten. Es wird kurz eine Benachrichtigung angezeigt, um zu bestätigen, dass ein neues Element zu Ihrer Arbeitsliste hinzugefügt wurde.
* **[!UICONTROL Anzeigen in[!DNL Workfront]]**: Wählen Sie diese Option aus, um das zugewiesene Problem oder die zugewiesene Aufgabe in Workfront anzuzeigen, wodurch eine neue Registerkarte geöffnet wird.
* **[!UICONTROL Start]**: Klicken Sie auf , um mit der Arbeit an dem Element zu beginnen. Es wird kurz eine Benachrichtigung angezeigt, um zu bestätigen, dass ein neues Element zu Ihrer Arbeitsliste hinzugefügt wurde.
* **[!UICONTROL Kommentar]**: Klicken Sie auf , um einen Kommentar zum Element abzugeben. Ihr Kommentar wird auch im Aktualisierungsstream des Elements in Workfront angezeigt.
* **[!UICONTROL Status]**: Klicken Sie auf und wählen Sie dann im Dropdownmenü den neuen Status für das Arbeitselement aus.

#### Aktionen, die für spezifische Zuweisungsbenachrichtigungen verfügbar sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Kommentar]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Sie sind einer Aufgabe zugewiesen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sie haben ein Problem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Team, dem Sie zugewiesen sind, erhält eine Arbeitsanforderung für eine Aufgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Team, dem Sie zugewiesen sind, erhält eine Arbeitsanforderung für ein Problem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Kommentar-Benachrichtigungen {#comment-notifications}

Sie erhalten eine Benachrichtigung, wenn jemand zu einem Artikel kommentiert, mit dem Sie verknüpft sind, oder Sie in eine Aktualisierung einbezieht. In der Benachrichtigung können Sie die folgenden Aktionen ausführen:

* **Reply**: Klicken Sie auf , um auf den Kommentar oder [!UICONTROL update] zu antworten. Ihre Antwort wird auch im Aktualisierungsstream angezeigt, wo der Kommentar in Workfront angezeigt wird.
* **[!UICONTROL In Workfront anzeigen]**: Wählen Sie diese Option aus, um den Kommentar und das Element in Workfront anzuzeigen, das auf einer neuen Registerkarte geöffnet wird.
* **[!UICONTROL Status]**: Klicken Sie auf und wählen Sie dann einen neuen Status für das Arbeitselement aus, um das es bei dem Kommentar oder der Aktualisierung geht.

#### Maßnahmen für spezifische Kommunikationsbenachrichtigungen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th>[!UICONTROL Antwort]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Auf Ihrer Anfrage wird ein Kommentar veröffentlicht</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eine Antwort auf Ihre Arbeitsanforderung wird veröffentlicht</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand kommentiert einen Thread, in dem Sie sich befinden</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand kommentiert eines Ihrer Arbeitselemente</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand kommentiert ein von Ihnen genehmigtes Timesheet</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Kommentar wird auf Ihrer Benutzerprofilseite hinzugefügt oder durch Massenbearbeitung mehrerer Benutzer</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zu einem Ihrer Updates wird ein Kommentar hinzugefügt</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Kommentar wird auf Ihrem Zeitblatt hinzugefügt</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Benachrichtigungen aktualisieren {#update-notifications}

Sie erhalten eine Informationsbenachrichtigung, wenn ein Artikel aktualisiert wird, mit dem Sie verknüpft sind. Sie müssen jedoch keine Maßnahmen für das Element ergreifen. In der Benachrichtigung können Sie die folgenden Aktionen ausführen:

* **[!UICONTROL Antwort]**: Klicken Sie auf , um auf die [!UICONTROL Aktualisierung] zu antworten. Ihre Antwort wird auch im Aktualisierungsstream des Elements in Workfront angezeigt.
* **In Workfront anzeigen**: Wählen Sie diese Option aus, um den Kommentar und das Element in Workfront anzuzeigen, das auf einer neuen Registerkarte geöffnet wird.
* **[!UICONTROL Status]**: Klicken Sie auf und wählen Sie dann den neuen Status für das Element aus dem Dropdownmenü aus.

#### Verfügbare Aktionen für spezifische Informationsbenachrichtigungen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th>[!UICONTROL Antwort]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">An einer Aufgabe, einem Problem oder einem Projekt, für die Sie angemeldet sind, wird eine Aktualisierung vorgenommen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand nimmt Sie an einer direkten Aktualisierung auf</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand bezieht Ihr Team in ein [!UICONTROL direktes Update] ein</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Datumsänderungsbenachrichtigungen {#date-change-notifications}

Sie erhalten eine Benachrichtigung über eine Datumsänderung, wenn sich das Datum für ein Arbeitselement ändert, dem Sie zugewiesen sind. Ab der Benachrichtigung über die Änderung des Datums können Sie die folgenden Aktionen durchführen.

* **[!UICONTROL Kommentar]**: Klicken Sie auf , um einen Kommentar zum Element abzugeben. Ihr Kommentar wird auch im Aktualisierungsstream des Elements in Workfront angezeigt.
* **[!UICONTROL Status]**: Klicken Sie auf und wählen Sie dann im Dropdownmenü den neuen Status für das Arbeitselement aus.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th> <p>[!UICONTROL Kommentar]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Das Fälligkeitsdatum ändert sich bei einer Aufgabe, der Sie zugewiesen sind</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
