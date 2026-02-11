---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Verwalten  [!DNL Adobe Workfront]  Benachrichtigungen in [!DNL Microsoft] Teams
description: Sie können Benachrichtigungen von  [!DNL Adobe Workfront]  erhalten, die Sie genehmigen müssen, Zuweisungen, die Ihnen erteilt wurden, oder Kommentare und Änderungen an Elementen, mit denen Sie verknüpft sind.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 7720d51864428e6d7cf493f88bbee13b5203774b
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 5%

---

# Verwalten von [!DNL Adobe Workfront]-Benachrichtigungen in [!DNL Microsoft Teams]

>[!IMPORTANT]
>
>Da [Microsoft auf den neuen Teams-Client umstellt](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) ist der Classic Teams-Client nach dem 1. Juli 2025 nicht mehr verfügbar. Um Microsoft Teams und integrierte Apps wie Workfront weiterhin verwenden zu können, müssen Kunden vor diesem Datum zum neuen Teams-Client wechseln.
>
>Die aktualisierte Workfront-Integration ist jetzt verfügbar und vollständig mit der neuen Team-Erfahrung kompatibel. In den meisten Fällen wird Workfront automatisch angezeigt, sobald Benutzende den Wechsel vollzogen haben. Ist dies nicht der Fall, kann die Integration manuell über die Microsoft Teams App Store installiert werden. Informationen zum Installieren oder Überprüfen der Workfront-Integration im neuen Team-Client finden Sie unter [Installieren [!DNL Adobe Workfront]  für Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

Sie können Benachrichtigungen von [!DNL Adobe Workfront] über Elemente erhalten, die Sie genehmigen müssen, Zuweisungen, die Ihnen erteilt wurden, oder Kommentare und Änderungen an Elementen, mit denen Sie verknüpft sind.

Diese Benachrichtigungen enthalten [!DNL Workfront] Aktionen, die Sie in [!DNL Microsoft Teams] ausführen können, ohne die [!DNL Microsoft Teams] zu verlassen.

>[!NOTE]
>
>[!DNL Microsoft Teams] unterstützt [!DNL Internet Explorer] nicht mehr. Um die [!DNL Adobe Workfront for Microsoft Teams integration] verwenden zu können, müssen Sie einen anderen Webbrowser als [!DNL Internet Explorer] verwenden.




## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <td> <p>Standard</p>
   <p>Work oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen für den Empfang von [!DNL Workfront]-Benachrichtigungen in [!DNL Microsoft Teams]

Sie können [!DNL Workfront] Benachrichtigungen in [!DNL Microsoft Teams] erhalten, wenn die folgenden Bedingungen erfüllt sind:

* Ein Teambesitzer hat [!DNL Workfront for Microsoft Teams] für Ihr Team installiert und konfiguriert.
* Sie sind von [!DNL Workfront] aus bei [!DNL Microsoft Teams] angemeldet.
* Sie haben sofortige Benachrichtigungen in [!DNL Workfront] aktiviert. Informationen zur Aktivierung sofortiger Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Informationen zur Installation von [!DNL Workfront for Microsoft Teams] und zur Anmeldung bei [!DNL Workfront from Microsoft Teams] finden Sie unter [Installieren [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Verwalten von [!DNL Workfront]-Benachrichtigungen in [!DNL Microsoft Teams]

Wenn die [!DNL Workfront for Microsoft Teams]-App installiert ist, wird [!DNL Workfront] für jedes Mitglied dieses Teams ein [!DNL Microsoft Teams]-Chat-Kanal erstellt. Wenn eine bestimmte Aktion in [!DNL Workfront] ausgeführt wird, können Sie die Einstellungen für [!DNL Workfront for Microsoft Teams] so konfigurieren, dass sie Benachrichtigungen über diese Aktion im [!DNL Workfront] Chat-Kanal von [!DNL Microsoft Teams] erhalten.

Beachten Sie beim Arbeiten mit [!DNL Workfront]-Benachrichtigungen von [!DNL Microsoft Teams] Folgendes:

* Sie können nicht alle, sondern nur eine bestimmte Anzahl [!DNL Workfront] Benachrichtigungen in [!DNL Microsoft Teams] erhalten.
* Alle Benachrichtigungen, die Sie von [!DNL Workfront] erhalten, werden im [!DNL Workfront] Bot-Chat-Kanal angezeigt.

  Informationen zur Installation des [!DNL Workfront]-Bot-Kanals finden Sie im Abschnitt [Anmelden bei [!DNL Workfront] von [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) im Artikel [Installieren [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

* Zwischen dem Zeitpunkt, zu dem eine Aktualisierung in [!DNL Workfront] vorgenommen wird, und dem Zeitpunkt, zu dem Sie die Benachrichtigung in [!DNL Microsoft Teams] erhalten, kann es bis zu 5 Minuten dauern.
* Für jede [!DNL Microsoft Teams] erhalten Sie auch eine E-Mail-Benachrichtigung.

So verwalten Sie die [!DNL Workfront], die Sie in [!DNL Microsoft Teams] erhalten können:

1. Klicken Sie in der linken Navigationsleiste in **[!UICONTROL auf das Symbol]** Mehr hinzugefügt[!DNL Microsoft Teams] (drei Punkte) Apps .

1. Klicken Sie in der angezeigten Liste auf [!DNL Workfront] .
1. Wählen Sie die Registerkarte **[!UICONTROL Einstellungen]**.

   Registerkarte ![MS Teams-Einstellungen](assets/ms-teams-settings-tab-350x552.png)

1. Deaktivieren Sie alle Benachrichtigungen, die Sie nicht erhalten möchten. Sie können Benachrichtigungsgruppen (z. B. Informationen oder Genehmigungsbenachrichtigungen) aktivieren oder deaktivieren oder Benachrichtigungen einzeln verwalten.

   Alle Benachrichtigungen sind standardmäßig aktiviert.

   Die Benachrichtigungseinstellungen für [!DNL Workfront for Microsoft] Teams werden automatisch gespeichert.

   >[!NOTE]
   >
   >Sie können den standardmäßig verfügbaren Benachrichtigungen keine weiteren Benachrichtigungen hinzufügen.

## Antworten auf [!DNL Workfront] Benachrichtigungen und Genehmigungsanfragen in [!DNL Microsoft Teams]

1. Melden Sie sich von [!DNL Workfront] aus bei [!DNL Microsoft Teams] an.\
   Informationen zur Anmeldung bei [!DNL Workfront] finden Sie unter [Installieren [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Wechseln Sie zum Bereich **[!UICONTROL Chat]** und klicken Sie auf den **[!DNL Workfront]** Bot-Kanal.\
   Dieser Kanal ist für Ihren persönlichen Chat mit dem [!DNL Workfront] Bot. Hier werden alle [!DNL Workfront]-Benachrichtigungen angezeigt.
1. Je nachdem, welchen Benachrichtigungstyp Sie erhalten, fahren Sie mit dem entsprechenden Abschnitt fort:

   * [Validierungsbenachrichtigungen](#approval-notifications-approval-notifications)
   * [Zuweisungsbenachrichtigungen](#assignment-notifications-assignment-notifications)
   * [Benachrichtigungen kommentieren](#comment-notifications-comment-notifications)
   * [Benachrichtigungen aktualisieren](#update-notifications-update-notifications)
   * [Benachrichtigungen bei Datumsänderungen](#date-change-notifications-date-change-notifications)

### Validierungsbenachrichtigungen {#approval-notifications}

Sie erhalten Genehmigungsbenachrichtigungen, wenn Sie aufgefordert werden, ein Objekt zu genehmigen, z. B. eine Aufgabe, eine Arbeitszeittabelle oder einen Korrekturabzug. Sie können die Benachrichtigung jedoch weiterhin kommentieren. In der Validierungsbenachrichtigung können Sie die folgenden Aktionen ausführen:

* **[!UICONTROL Genehmigen]**: Klicken, um das Element zu genehmigen.
* **[!UICONTROL Ändern]**: Klicken Sie, um das Element mit den Änderungen zu genehmigen.
* **[!UICONTROL Ablehnen]**: Klicken, um das Element abzulehnen.
* **[!UICONTROL Kommentar]**: Klicken, um einen Kommentar abzugeben. Ihr Kommentar wird auch in [!DNL Workfront] als Aktualisierung des -Objekts angezeigt, um das es in der Benachrichtigung geht.
* **[!UICONTROL Zum Korrekturabzug gehen]**: Klicken Sie darauf, um den Korrekturabzug zu öffnen. Sie können dann eine Entscheidung direkt im Testversand treffen. Weitere Informationen finden Sie unter [Festlegen einer Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Nachdem Sie eine Genehmigungsentscheidung getroffen haben, können Sie sie in der Benachrichtigung nicht mehr ändern.

#### Für spezifische Genehmigungsbenachrichtigungen verfügbare Aktionen:

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
   <th>[!UICONTROL genehmigen]</th> 
   <th>[!UICONTROL Reject]</th> 
   <th> <p>[!UICONTROL ändern]</p> </th> 
   <th> <p>[!UICONTROL Zum Korrekturabzug wechseln] </p> </th> 
   <th>[!UICONTROL-Kommentar]</th> 
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
   <td role="rowheader">Aufgabe muss genehmigt werden</td> 
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
   <td role="rowheader">Zugriff auf ein Objekt muss genehmigt werden</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sie müssen eine Arbeitszeittabelle genehmigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand möchte, dass Sie diesen Korrekturabzug genehmigen</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihre Arbeitszeittabelle wurde abgelehnt</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihre Arbeitszeittabelle wird wieder geöffnet</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eine von Ihnen angeforderte Dokumentgenehmigungsanfrage wird genehmigt*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eine von Ihnen angeforderte Dokumentgenehmigungsanfrage wird mit Änderungen genehmigt*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Eine von Ihnen angeforderte Dokumentgenehmigungsanfrage wird abgelehnt*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihre Arbeitszeittabelle wurde genehmigt</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Diese Benachrichtigungen beziehen sich auf Genehmigungen älterer Dokumente. Einheitliche Dokumentengenehmigungsbenachrichtigungen werden derzeit in [!DNL Microsoft Teams] nicht unterstützt. Weitere Informationen zu den verschiedenen Genehmigungssystemen in Workfront finden Sie unter [Verfügbare Funktionen für Dokumentgenehmigungen](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md).

### Zuweisungsbenachrichtigungen {#assignment-notifications}

Sie erhalten Zuweisungsbenachrichtigungen, wenn Sie oder ein Team, dem Sie angehören, einer Aufgabe oder einem Problem in Workfront zugewiesen sind. In der Zuweisungsbenachrichtigung können Sie die folgenden Aktionen ausführen:

* **[!UICONTROL Bearbeiten]**: Wählen Sie diese Option aus, um die Arbeit am Element zu übernehmen. Es wird kurz eine Benachrichtigung angezeigt, die bestätigt, dass ein neues Element zu Ihrer Auftragsliste hinzugefügt wurde.
* **[!UICONTROL In[!DNL Workfront]]** anzeigen: Wählen Sie diese Option aus, um das zugewiesene Problem oder die zugewiesene Aufgabe in Workfront anzuzeigen. Dadurch wird eine neue Registerkarte geöffnet.
* **[!UICONTROL Starten]**: Klicken Sie, um mit der Bearbeitung des Elements zu beginnen. Es wird kurz eine Benachrichtigung angezeigt, die bestätigt, dass ein neues Element zu Ihrer Auftragsliste hinzugefügt wurde.
* **[!UICONTROL Kommentar]**: Klicken Sie, um einen Kommentar zu dem Element abzugeben. Ihr Kommentar wird auch im Aktualisierungsverlauf des Elements in Workfront angezeigt.
* **[!UICONTROL Status]**: Klicken Sie auf und wählen Sie dann im Dropdown-Menü den neuen Status für das Arbeitselement aus.

#### Für bestimmte Zuweisungsbenachrichtigungen verfügbare Aktionen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL-Kommentar]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Sie wurden einer Aufgabe zugewiesen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sie wurden einem Problem zugewiesen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Team, dem Sie zugewiesen sind, erhält einen Arbeitsauftrag für eine Aufgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Team, dem Sie zugewiesen sind, erhält einen Arbeitsauftrag für ein Problem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Benachrichtigungen kommentieren {#comment-notifications}

Sie erhalten eine Benachrichtigung, wenn jemand einen Kommentar zu einem Element abgibt, mit dem Sie verknüpft sind, oder Sie in eine Aktualisierung einbezieht. Von der Kommunikationsbenachrichtigung aus können Sie die folgenden Aktionen ausführen:

* **Reply**: Klicken, um auf den Kommentar zu antworten oder [!UICONTROL aktualisieren]. Ihre Antwort wird auch im Aktualisierungsverlauf angezeigt, in dem der Kommentar in Workfront erscheint.
* **[!UICONTROL In Workfront anzeigen]**: Wählen Sie diese Option aus, um den Kommentar und das Element in Workfront anzuzeigen, die in einer neuen Registerkarte geöffnet sind.
* **[!UICONTROL Status]**: Klicken Sie auf und wählen Sie dann einen neuen Status für das Arbeitselement aus, um das es bei dem Kommentar oder der Aktualisierung geht.

#### Für bestimmte Kommunikationsbenachrichtigungen verfügbare Aktionen:

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
   <td role="rowheader">Ein Kommentar zu Ihrer Anfrage wird veröffentlicht</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Auf Ihren Arbeitsauftrag wird eine Antwort veröffentlicht</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand kommentiert einen Thread, in dem Sie sich befinden</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand kommentiert ein Arbeitselement</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand kommentiert eine von Ihnen genehmigte Arbeitszeittabelle</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Kommentar wird auf Ihrer Benutzerprofilseite oder durch Massenbearbeitung mehrerer Benutzer hinzugefügt</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Kommentar wird zu einer Ihrer Aktualisierungen hinzugefügt</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Kommentar wird zu Ihrer Arbeitszeittabelle hinzugefügt</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Benachrichtigungen aktualisieren {#update-notifications}

Sie erhalten eine Informationsbenachrichtigung, wenn ein Element, mit dem Sie verknüpft sind, aktualisiert wird, müssen jedoch keine Maßnahmen für das Element ergreifen. In der Informationsbenachrichtigung können Sie die folgenden Aktionen ausführen:

* **[!UICONTROL Antwort]**: Klicken Sie, um auf die [!UICONTROL Aktualisierung] zu antworten. Ihre Antwort wird auch im Aktualisierungsverlauf des Elements in Workfront angezeigt.
* **In Workfront anzeigen**: Wählen Sie diese Option aus, um den Kommentar und das Element in Workfront anzuzeigen, die in einer neuen Registerkarte geöffnet sind.
* **[!UICONTROL Status]**: Klicken Sie auf und wählen Sie dann im Dropdown-Menü den neuen Status für das Element aus.

#### Für spezifische Informationsbenachrichtigungen verfügbare Aktionen:

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
   <td role="rowheader">An einer Aufgabe, einem Problem oder Projekt, die bzw. das Sie abonniert haben, wird ein Update vorgenommen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand schließt Sie in eine direkte Aktualisierung ein</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jemand schließt Ihr Team in ein [!UICONTROL Directed Update] ein</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Benachrichtigungen bei Datumsänderungen {#date-change-notifications}

Sie erhalten eine Benachrichtigung über eine Datumsänderung, wenn sich das Datum für ein Arbeitselement ändert, dem Sie zugewiesen sind. Mit der Benachrichtigung zur Datumsänderung können Sie die folgenden Aktionen ausführen.

* **[!UICONTROL Kommentar]**: Klicken Sie, um einen Kommentar zu dem Element abzugeben. Ihr Kommentar wird auch im Aktualisierungsverlauf des Elements in Workfront angezeigt.
* **[!UICONTROL Status]**: Klicken Sie auf und wählen Sie dann im Dropdown-Menü den neuen Status für das Arbeitselement aus.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th> <p>[!UICONTROL-Kommentar]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Die Fälligkeitsdatumsänderungen für eine Aufgabe, der Sie zugewiesen sind</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
