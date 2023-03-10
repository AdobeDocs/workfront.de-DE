---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: E-Mail-Benachrichtigungseinstellungen konfigurieren in [!DNL Workfront Proof]
description: E-Mail-Benachrichtigungen informieren die Mitwirkenden über die letzten Aktivitäten bei Testsendungen, wie Kommentare, Antworten und Entscheidungen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1998'
ht-degree: 0%

---

# E-Mail-Benachrichtigungseinstellungen konfigurieren in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

E-Mail-Benachrichtigungen informieren die Mitwirkenden über die letzten Aktivitäten bei Testsendungen, wie Kommentare, Antworten und Entscheidungen.

E-Mail-Benachrichtigungen für Validierungsverantwortliche können auf der Seite Neuer Testversand eingestellt werden. [!UICONTROL Neue Version] und in der [!UICONTROL Workflow] Abschnitt [!UICONTROL Testversanddetails] Seite. Weitere Informationen finden Sie unter [Testsendungen generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Testsendungen generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Testsendungen generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Jeder Benutzer kann auch seine eigenen E-Mail-Warneinstellungen festlegen, die automatisch angewendet werden, wenn ein Testversand für ihn freigegeben wird. Wenn die Mitwirkenden ihre Voreinstellungen haben oder Kontoadministratoren ihre Empfehlungen zur Häufigkeit der Warnhinweise erhalten. Dies kann auf den Detailseiten der Benutzer als Testversand-Standard festgelegt werden.

>[!NOTE]
>
>Diese Einstellungen werden vorgeschlagen, wenn Benutzer die Testsendungen erstellen und diese Mitwirkenden hinzufügen. Diese Vorschläge sind jedoch nur Vorschläge, sodass sie jederzeit während des Überprüfungsprozesses angepasst werden können und die Änderungen für alle Aktivitäten gelten, die nach der Änderung durchgeführt werden. Die Standardeinstellungen für Testsendungen werden von den Einstellungen auf Testversandebene überschrieben.

Benutzer mit [!UICONTROL Administrator] oder [!UICONTROL Rechnungsadministrator] -Profile können auch die Testversand-Standardeinstellungen für andere Benutzer in ihrem Konto in den Kontoeinstellungen festlegen.

Weitere Informationen zu Profilen finden Sie unter [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Konfigurieren Sie die standardmäßigen Testsendungen in den persönlichen Einstellungen ([!DNL Workfront Proof] nur Benutzer)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [E-Mail-Warnungen für einen Empfänger ändern](#change-email-alerts-for-a-recipient)
* [Konfigurieren der Standardwerte für den Testversand eines Benutzers](#configure-proof-defaults-for-a-user)

## Konfigurieren Sie die standardmäßigen Testsendungen in den persönlichen Einstellungen ([!DNL Workfront Proof] nur Benutzer)

Sie können Testversand-Einstellungen für von Ihnen erstellte Testsendungen konfigurieren.

Informationen zu den Testversandeinstellungen finden Sie unter [!DNL Workfront] Administrator oder [!DNL Workfront Proof] -Administrator kann konfigurieren, siehe .

1. Klicken **[!UICONTROL Einstellungen]** > **[!UICONTROL Persönliche Einstellungen]**.

1. Klicken Sie auf **[!UICONTROL Standardeinstellungen für die Prüfung]** Registerkarte.
1. Klicken **[!UICONTROL Standard-E-Mail-Benachrichtigungseinstellungen]** um sie zu erweitern.
1. Wählen Sie in der Dropdown-Liste rechts neben den beiden folgenden Einstellungen eine der Optionen aus, die in der unten stehenden Tabelle beschrieben sind.

   * **[!UICONTROL Standard-E-Mail-Warnhinweis]**: Betrifft alle für Sie freigegebenen Testsendungen. Diese Einstellung kann auf der Testversandebene überschrieben werden.
   * **[!UICONTROL Standard-E-Mail-Warnung für neue Gastreviewer]**: Betrifft Validierer, die zuvor nicht als Kontakte in Ihrem Konto vorhanden waren.

   >[!NOTE]
   >
   >Wenn Sie keine der folgenden Optionen auswählen, [!DNL Workfront Proof] sendet Ihnen eine tägliche Zusammenfassung der Aktivitäten Ihrer Testsendungen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Alle Aktivitäten]</td> 
      <td>[!UICONTROL Workfront] sendet eine E-Mail an den Validierer jedes Mal, wenn eine Aktivität auf dem Testversand ausgeführt wird, z. B. wenn ein neuer Kommentar, eine neue Antwort oder eine neue Entscheidung eingeht. <p>Dies ist eine großartige Option für die Person, die den Testversand verwaltet, da sie die Aktivität so sehen kann, wie sie ausgeführt wird. </p><p>Benutzer erhalten keine E-Mail-Warnung zu ihrer eigenen Aktivität.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Antworten auf meine Kommentare]</td> 
      <td>Eine E-Mail wird nur dann an den Validierer gesendet, wenn jemand explizit auf seinen Kommentar antwortet (dabei werden eigene Antworten auf eigene Kommentare ausgeschlossen). Das bedeutet, dass der Validierer nicht benachrichtigt wird, wenn jemand, der den Testversand durchführt, einen neuen Kommentar abgibt.<p>Diese Einstellung wird Ihren Kunden empfohlen, den Testversand durchzuführen, damit sie über keine weiteren Kommentare zum Testversand informiert und nur über Antworten auf ihre eigenen Kommentare informiert werden.</p><p>validierungsverantwortliche Benutzer mit dieser E-Mail-Warnungseinstellung werden zwar nicht über andere neue Kommentare benachrichtigt, können aber dennoch alle Kommentare zum Testversand im Testversand-Viewer anzeigen.</p><p>Weitere Informationen zu Kommentaren finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Kommentare zum Testversand anzeigen und beantworten</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Entscheidungen]</td> 
      <td>[!DNL Workfront] sendet eine E-Mail nur dann an den Validierer, wenn jemand eine Entscheidung trifft.<p>Dies kann für die Person nützlich sein, die den Validierungsprozess verwaltet (z. B. einen Projektmanager), und muss den Fortschritt des Testversands überwachen und sehen, welche Benutzer ihre Entscheidung getroffen haben.</p><p>Sie werden nicht über Ihre eigene Entscheidung informiert, es sei denn, Sie wählen beim Senden Ihrer Entscheidung eine E-Mail-Bestätigungsoption aus.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Endbeschluss]</td> 
      <td>[!DNL Workfront] sendet eine E-Mail, wenn der letzte Validierer des Testversands seine Entscheidung getroffen hat.<p>Dieser Warnhinweis wird häufig vom Designer verwendet, der normalerweise nicht an der eigentlichen Reviewdiskussion teilnehmen muss. Wenn die endgültige Entscheidung getroffen wird, wird der Designer benachrichtigt und kann dann alle notwendigen Änderungen vornehmen.</p><p>Dieser Warnhinweis kann auch für einen Abteilungsleiter nützlich sein, der nur benachrichtigt werden muss, wenn der Überprüfungsprozess abgeschlossen ist.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Stündliche Zusammenfassung]</td> 
      <td>[!DNL Workfront] sendet stündlich eine E-Mail mit einer Zusammenfassung aller Kommentare, Antworten und Entscheidungen, die in der entsprechenden Stunde getroffen wurden.<p>Die E-Mail wird nur gesendet, wenn neben Ihrer eigenen Aktivität innerhalb der letzten Stunde stattgefunden hat. </p><p>Mit diesem Warnhinweis können Sie einen Überblick über das Projekt erhalten.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Senior Reviewer, der einen Überblick über das Projekt benötigt, aber nicht sofort über alle Aktivitäten auf dem Testversand benachrichtigt werden muss.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tägliche Zusammenfassung]</td> 
      <td>[!DNL Workfront] sendet eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen, die nur an Tagen aufgelistet sind, an denen neben Ihrer eigenen Aktivität Aktivitäten vorhanden sind.<p>Mit diesem Warnhinweis können Sie eine Zusammenfassung des Projekts anzeigen, ohne über den gesamten Tag hinweg durch mehrere Aktualisierungen überlastet zu sein.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Abteilungsleiter, der den Gesamtfortschritt des Projekts überwachen möchte.</p><p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Benachrichtigungen für Testversandkommentare und -entscheidungen verwalten</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Keine E-Mail]</td> 
      <td>[!DNL Workfront] sendet keine E-Mail-Warnungen.<br>Dies ist für eine Person nützlich, die einem Testversand nur zu Referenzzwecken hinzugefügt wird und nicht über Änderungen benachrichtigt werden muss.<p>Der Systemstandard lautet [!UICONTROL Daily summary] (auch als [!UICONTROL Not Set] bezeichnet). Wenn Sie oder Ihre Validierer keine anderen Änderungen vornehmen, haben alle Testsendungen diese Einstellung.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Ändern Sie Folgendes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL E-Mail-Bestätigung, wenn Testsendungen abgeschlossen sind]</td> 
      <td>Geben Sie an, ob Sie beim Erstellen eines Testversands eine [!UICONTROL Testversand]-E-Mail erhalten möchten. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">Die [!UICONTROL Testversand-Made-E-Mail</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Format der an mich gesendeten E-Mails]</strong> </td> 
      <td> <p>Wählen Sie zwischen HTML formatierten E-Mails und Nur Text-E-Mails. </p> <p>Hinweis:  Die Standardeinstellungen für die Prüfung werden von den Einstellungen auf der Testversandebene überschrieben. Wenn jedoch in den Einstellungen für [!UICONTROL Konto] die E-Mail-Benachrichtigungen zum Testversand für das gesamte Konto deaktiviert sind, werden keine E-Mail-Warnungen an die Mitwirkenden gesendet, selbst wenn in Testsendungen der Warnhinweis für deaktivierte E-Mails nicht ausgewählt wurde.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. under **[!UICONTROL Nachrichteneinstellungen]**&#x200B;ändern Sie einen der folgenden Parameter:

   | **[!UICONTROL Vorlage für Testversand-Betreff]** | Wird auf der Seite Neuer Testversand , Neue Version , Nachrichtenseite und Remind angezeigt. Kann bearbeitet werden, bevor es gesendet wird. |
   |---|---|
   | **[!UICONTROL Vorlage für Testnachrichten]** | Wird auf der Seite Neuer Testversand , Neue Version , Nachrichten und Erinnerung angezeigt. Kann bearbeitet werden, bevor es gesendet wird. |

   {style=&quot;table-layout:auto&quot;}

## E-Mail-Warnungen für einen Empfänger ändern

Sie können E-Mail-Warnungen für einen bestimmten Empfänger in einer Batch-Aktion ändern.

1. Klicken **[!UICONTROL Kontakte]** im linken Navigationsbereich.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü (drei Punkte) für den Empfänger und klicken Sie auf **[!UICONTROL Mitgliederdetails anzeigen]** im Dropdown-Menü.

1. Öffnen Sie die **[!UICONTROL Freigegebene Elemente]** Abschnitt.
1. Aktivieren Sie das Kontrollkästchen links neben jedem Element, für das Sie den E-Mail-Warnhinweis ändern möchten.
1. Klicken **[!UICONTROL Mehr]** über der Liste der freigegebenen Elemente und klicken Sie dann auf **[!UICONTROL E-Mail-Warnhinweis ändern]** im Dropdown-Menü.

1. Ändern Sie den E-Mail-Warnhinweis und klicken Sie auf **[!UICONTROL Einsenden]**.

## Konfigurieren der Standardwerte für den Testversand eines Benutzers

Wenn Sie [!DNL Workfront Proof] -Administrator können Sie für Benutzer in Ihrem Konto Testversandstandards festlegen.

1. Klicken **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]**.

1. Öffnen Sie die **[!UICONTROL Benutzer]** Registerkarte.
1. Öffnen Sie die **[!UICONTROL Mehr]** Menü rechts neben dem Namen des Benutzers. ![More_button_small.png](assets/more-button-small.png)

1. Klicken **[!UICONTROL Anzeigen von Benutzerdetails]** im Dropdown-Menü.
1. under **[!UICONTROL Einstellungen]** klicken **[!UICONTROL Standard-E-Mail-Warnhinweiseinstellungen]** um sie zu erweitern.

1. Wählen Sie in der Dropdown-Liste rechts neben den beiden folgenden Einstellungen eine der Optionen aus, die in der folgenden Tabelle beschrieben sind:

   * **[!UICONTROL Standard-E-Mail-Warnhinweis]**: Betrifft alle für Sie freigegebenen Testsendungen. Diese Einstellung kann auf der Testversandebene überschrieben werden.
   * **[!UICONTROL Standard-E-Mail-Warnung für neue Gastreviewer]**: Betrifft Validierer, die zuvor nicht als Kontakte in Ihrem Konto vorhanden waren.

   >[!NOTE]
   >
   >Wenn Sie keine der folgenden Optionen für einen Benutzer auswählen, [!DNL Workfront Proof] sendet Benutzern eine tägliche Zusammenfassung der Aktivitäten auf ihren Testsendungen.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Alle Aktivitäten]</td>
      <td>[!DNL Workfront] sendet eine E-Mail an den Validierer, sobald eine Aktivität im Testversand vorhanden ist, z. B. einen neuen Kommentar, eine Antwort oder eine neue Entscheidung. <p>Dies ist eine großartige Option für die Person, die den Testversand verwaltet, da sie die Aktivität so sehen kann, wie sie ausgeführt wird. </p><p>Benutzer erhalten keine E-Mail-Warnung zu ihrer eigenen Aktivität.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Antworten auf meine Kommentare]</td>
      <td>Eine E-Mail wird nur dann an den Validierer gesendet, wenn jemand explizit auf seinen Kommentar antwortet (dabei werden eigene Antworten auf eigene Kommentare ausgeschlossen). Das bedeutet, dass der Validierer nicht benachrichtigt wird, wenn jemand, der den Testversand durchführt, einen neuen Kommentar abgibt.<p>Diese Einstellung wird Ihren Kunden empfohlen, den Testversand durchzuführen, damit sie über keine weiteren Kommentare zum Testversand informiert und nur über Antworten auf ihre eigenen Kommentare informiert werden.</p><p>validierungsverantwortliche Benutzer mit dieser E-Mail-Warnungseinstellung werden zwar nicht über andere neue Kommentare benachrichtigt, können aber dennoch alle Kommentare zum Testversand im Testversand-Viewer anzeigen.</p><p>Weitere Informationen zu Kommentaren finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Kommentare zum Testversand anzeigen und beantworten</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Entscheidungen]</td>
      <td>[!DNL Workfront] sendet eine E-Mail nur dann an den Validierer, wenn jemand eine Entscheidung trifft.<p>Dies kann für die Person nützlich sein, die den Validierungsprozess verwaltet (z. B. einen Projektmanager), und muss den Fortschritt des Testversands überwachen und sehen, welche Benutzer ihre Entscheidung getroffen haben.</p><p>Sie werden nicht über Ihre eigene Entscheidung informiert, es sei denn, Sie wählen beim Senden Ihrer Entscheidung eine E-Mail-Bestätigungsoption aus.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Endbeschluss]</td>
      <td>[!DNL Workfront] sendet eine E-Mail, wenn der letzte Validierer des Testversands seine Entscheidung getroffen hat.<p>Dieser Warnhinweis wird häufig vom Designer verwendet, der normalerweise nicht an der eigentlichen Reviewdiskussion teilnehmen muss. Wenn die endgültige Entscheidung getroffen wird, wird der Designer benachrichtigt und kann dann alle notwendigen Änderungen vornehmen.</p><p>Dieser Warnhinweis kann auch für einen Abteilungsleiter nützlich sein, der nur benachrichtigt werden muss, wenn der Überprüfungsprozess abgeschlossen ist.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Stündliche Zusammenfassung]</td>
      <td>[!DNL Workfront] sendet stündlich eine E-Mail mit einer Zusammenfassung aller Kommentare, Antworten und Entscheidungen, die in der entsprechenden Stunde getroffen wurden.<p>Die E-Mail wird nur gesendet, wenn neben Ihrer eigenen Aktivität innerhalb der letzten Stunde stattgefunden hat. </p><p>Mit diesem Warnhinweis können Sie einen Überblick über das Projekt erhalten.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Senior Reviewer, der einen Überblick über das Projekt benötigt, aber nicht sofort über alle Aktivitäten auf dem Testversand benachrichtigt werden muss.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Tägliche Zusammenfassung]</td>
      <td>[!DNL Workfront] sendet eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen, die nur an Tagen aufgelistet sind, an denen neben Ihrer eigenen Aktivität Aktivitäten vorhanden sind.<p>Mit diesem Warnhinweis können Sie eine Zusammenfassung des Projekts anzeigen, ohne über den gesamten Tag hinweg durch mehrere Aktualisierungen überlastet zu sein.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Abteilungsleiter, der den Gesamtfortschritt des Projekts überwachen möchte.</p><p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Benachrichtigungen für Testversandkommentare und -entscheidungen verwalten</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL Keine E-Mail]</td>
      <td>[!DNL Workfront] sendet keine E-Mail-Warnungen.<br>Dies ist für eine Person nützlich, die einem Testversand nur zu Referenzzwecken hinzugefügt wird und nicht über Änderungen benachrichtigt werden muss.<p>Der Systemstandard lautet [!UICONTROL Daily summary] (auch als [!UICONTROL Not Set] bezeichnet). Wenn Sie oder Ihre Validierer keine anderen Änderungen vornehmen, haben alle Testsendungen diese Einstellung.</p></td>
     </tr>
    </tbody>
   </table>

1. In der **[!UICONTROL Standard-E-Mail-Warnhinweiseinstellungen]**&#x200B;ändern Sie einen der folgenden Parameter:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL E-Mail-Bestätigung, wenn Testsendungen abgeschlossen sind]</td> 
      <td>Geben Sie an, ob Sie beim Erstellen eines Testversands eine [!UICONTROL Testversand]-E-Mail erhalten möchten. Weitere Informationen finden Sie unter <a href="https://support.workfront.com/hc/en-us/article">Die E-Mail zum [!UICONTROL Testversand].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Format der an mich gesendeten E-Mails]</strong> </td> 
      <td> <p>Wählen Sie zwischen HTML formatierten E-Mails und Nur Text-E-Mails. </p> <p>Hinweis:  Die Standardeinstellungen für die Prüfung werden von den Einstellungen auf der Testversandebene überschrieben. Wenn jedoch in den Einstellungen für [!UICONTROL Konto] die E-Mail-Benachrichtigungen zum Testversand für das gesamte Konto deaktiviert sind, werden keine E-Mail-Warnungen an die Mitwirkenden gesendet, selbst wenn in Testsendungen der Warnhinweis für deaktivierte E-Mails nicht ausgewählt wurde.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
