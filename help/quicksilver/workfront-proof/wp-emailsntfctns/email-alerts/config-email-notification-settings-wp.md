---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Konfigurieren Sie E-Mail-Benachrichtigungseinstellungen in [!DNL Workfront Proof]
description: Von Workfront Proof generierte E-Mail-Benachrichtigungen informieren Mitwirkende über aktuelle Aktivitäten im Zusammenhang mit Korrekturabzügen, wie Kommentare, Antworten oder Entscheidungen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2065'
ht-degree: 0%

---

# Konfigurieren der E-Mail-Benachrichtigungseinstellungen in [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

E-Mail-Benachrichtigungen informieren Mitwirkende über aktuelle Aktivitäten bei Korrekturabzügen, wie Kommentare, Antworten oder Entscheidungen.

Sie können E-Mail-Benachrichtigungen für Prüfer in den folgenden Bereichen festlegen:

E-Mail-Benachrichtigungen für Validierungsverantwortliche können auf der Seite Neuer Korrekturabzug [!UICONTROL Neue Version] festgelegt und im Abschnitt [!UICONTROL Workflow] der Seite [!UICONTROL Korrekturabzugsdetails] verwaltet werden. Weitere Informationen finden Sie unter [Erstellen von Korrekturabzügen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* Die Seite Neuer Korrekturabzug
* Die [!UICONTROL Neue Version] Seite
* Der [!UICONTROL Workflow] der Seite [!UICONTROL Details des &#x200B;]&quot;.

Weitere Informationen finden Sie unter [Erstellen von Korrekturabzügen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Korrekturabzüge generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


Jeder Benutzer kann auch seine eigenen E-Mail-Warnhinweiseinstellungen festlegen, die automatisch angewendet werden, wenn ein Korrekturabzug für ihn freigegeben wird, wenn die Mitarbeiter ihre Voreinstellungen haben oder Kontoadministratoren ihre Empfehlungen zur Häufigkeit von Warnhinweisen haben. Dies kann als Standard-Korrekturabzug auf den Benutzerdetailseiten festgelegt werden.

Jeder Benutzer kann auch seine eigenen E-Mail-Warnhinweiseinstellungen festlegen, die automatisch angewendet werden, wenn ein Korrekturabzug für ihn freigegeben wird. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>Diese Einstellungen werden empfohlen, wenn Benutzende die Korrekturabzüge erstellen und diese Mitarbeiter hinzufügen. Es handelt sich jedoch nur um Vorschläge, die jederzeit während des Überprüfungsprozesses angepasst werden können und die Änderungen gelten für alle Aktivitäten, die nach der Änderung durchgeführt werden. Die Standardeinstellungen für den Korrekturabzug werden durch die Einstellungen auf der Korrekturabzugsebene überschrieben.

Benutzer mit [!UICONTROL Administrator] oder [!UICONTROL Abrechnungsadministrator]-Profilen können die Standardeinstellungen für Korrekturabzüge auch für andere Benutzer in ihrem Konto über die Kontoeinstellungen festlegen.

Weitere Informationen zu Profilen finden Sie unter [Korrekturabzugsberechtigungen in Profilen [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">Produkt</td> 
   <td>Workfront Proof eigenständig</td> 
  </tr> 
</table>

+++

## Standardeinstellungen für Korrekturabzüge in persönlichen Einstellungen konfigurieren (nur [!DNL Workfront Proof] Benutzer)

Sie können die Einstellungen für Korrekturabzüge konfigurieren, die Sie erstellen.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Klicken Sie oben rechts auf Ihr Profilbild und dann auf **[!UICONTROL Persönliche Einstellungen]**.

1. Klicken Sie auf die **[!UICONTROL Proofing-Standardeinstellungen]**.
1. Klicken Sie auf **[!UICONTROL Standardeinstellungen für E-Mail]** Benachrichtigungen, um sie zu erweitern.
1. Wählen Sie in der Dropdown-Liste rechts neben den beiden folgenden Einstellungen eine der in der folgenden Tabelle erläuterten Optionen aus.

   * **[!UICONTROL Standard-E-Mail]** Warnhinweis: Wirkt sich auf alle Korrekturabzüge aus, die für Sie freigegeben wurden. Diese Einstellung kann auf der Ebene des Korrekturabzugs überschrieben werden.
   * **[!UICONTROL Standard-E-Mail-Warnhinweis für neue Gast]** Reviewer: Betrifft Reviewer, die zuvor nicht als Kontakte in Ihrem Konto vorhanden waren.

   >[!NOTE]
   >
   >Wenn Sie keine der folgenden Optionen auswählen, sendet [!DNL Workfront Proof] Ihnen eine tägliche Zusammenfassung über die Aktivitäten bei Ihren Testsendungen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Alle Aktivitäten]</td> 
      <td>[!UICONTROL Workfront] sendet jedes Mal eine E-Mail an den Prüfer, wenn es eine Aktivität im Korrekturabzug gibt, z. B. einen neuen Kommentar, eine neue Antwort oder eine neue Entscheidung. <p>Dies ist eine hervorragende Option für die Person, die den Proofing-Prozess verwaltet, da sie die Aktivität direkt sehen kann. </p><p>Benutzende erhalten keine E-Mail-Benachrichtigung über ihre eigene Aktivität.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL antwortet auf meine Kommentare]</td> 
      <td>Eine E-Mail wird nur dann an den Prüfer gesendet, wenn jemand explizit auf seinen Kommentar antwortet (dies schließt die eigenen Antworten auf seine eigenen Kommentare aus). Das bedeutet, dass, wenn jemand auf dem Korrekturabzug einen neuen Kommentar abgibt, der Prüfer nicht benachrichtigt wird.<p>Diese Einstellung wird für Ihre Kunden auf dem Korrekturabzug empfohlen, damit sie nicht über andere Kommentare zu dem Korrekturabzug benachrichtigt werden und nur über Antworten auf ihre eigenen Kommentare.</p><p>Reviewer mit dieser E-Mail-Warnhinweiseinstellung werden zwar nicht über andere neue Kommentare benachrichtigt, sie können jedoch alle Kommentare zum Korrekturabzug in der Proofing-Anzeige anzeigen.</p><p>Weitere Informationen zu Kommentaren finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Kommentare zu Korrekturabzügen anzeigen und </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL -Entscheidungen]</td> 
      <td>[!DNL Workfront] Sendet nur dann eine E-Mail an den Validierungsverantwortlichen, wenn jemand eine Entscheidung trifft.<p>Dies kann für die Person nützlich sein, die den Genehmigungsprozess verwaltet (z. B. einen Projektmanager) und den Fortschritt beim Korrekturabzug überwachen muss, um zu sehen, welche Benutzer ihre Entscheidung getroffen haben.</p><p>Sie werden über Ihre eigene Entscheidung nur benachrichtigt, wenn Sie beim Senden Ihrer Entscheidung eine E-Mail-Bestätigungsoption auswählen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Endgültige Entscheidung]</td> 
      <td>[!DNL Workfront] Sendet eine E-Mail, wenn die letzte genehmigende Person für den Korrekturabzug ihre Entscheidung getroffen hat.<p>Dieser Warnhinweis wird häufig vom Designer verwendet, der normalerweise nicht an der eigentlichen Überprüfungsdiskussion teilnehmen muss. Wenn die endgültige Entscheidung getroffen wird, wird der Designer benachrichtigt und kann dann die erforderlichen Änderungen vornehmen.</p><p>Dieser Warnhinweis kann auch für einen Abteilungsleiter nützlich sein, der erst benachrichtigt werden muss, wenn der Überprüfungsprozess abgeschlossen ist.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Stündliche Zusammenfassung]</td> 
      <td>[!DNL Workfront] Sendet stündlich eine E-Mail mit einer Zusammenfassung aller Kommentare, Antworten und Entscheidungen, die in dieser Stunde stattgefunden haben, an den Prüfer.<p>Die E-Mail wird nur gesendet, wenn innerhalb der letzten Stunde eine andere Aktivität als die eigene stattgefunden hat. </p><p>Dieser Warnhinweis bietet eine gute Möglichkeit, einen Überblick über das Projekt zu erhalten.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein leitender Prüfer, der einen Überblick über das Projekt benötigt, aber nicht sofort über alle Aktivitäten im Korrekturabzug benachrichtigt werden muss.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tägliche Zusammenfassung]</td> 
      <td>[!DNL Workfront] Sendet eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen, die nur an Tagen aufgelistet sind, an denen außer Ihrer eigenen Aktivität eine andere Aktivität stattfindet.<p>Dieser Warnhinweis bietet eine gute Möglichkeit, eine Zusammenfassung des Projekts anzuzeigen, ohne im Laufe des Tages durch mehrere Updates überfordert zu werden.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Abteilungsleiter, der den Gesamtfortschritt des Projekts überwachen möchte.</p><p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Verwalten von Benachrichtigungen für Kommentare und Entscheidungen zu Korrekturabzügen</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Keine E-Mail]</td> 
      <td>[!DNL Workfront] sendet keine E-Mail-Warnungen.<br>Dies ist für Personen nützlich, die einem Korrekturabzug nur zu Referenzzwecken hinzugefügt werden und nicht über Änderungen benachrichtigt werden müssen.<p>Der Systemstandard ist [!UICONTROL Daily Summary] (auch als [!UICONTROL Not Set] bezeichnet). Wenn Sie oder Ihre Prüfer keine anderen Änderungen vornehmen, haben alle Ihre Korrekturabzüge diese Einstellung.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Ändern Sie Folgendes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL E-Mail-Bestätigung, wenn die Testsendungen fertig sind]</td> 
      <td>Geben Sie an, ob Sie beim Erstellen eines Korrekturabzugs eine [!UICONTROL Proof made]-E-Mail erhalten möchten. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">Die E-Mail [!UICONTROL Proof Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format der an mich gesendeten E-Mails] </td> 
      <td> <p>Wählen Sie zwischen E-Mails im HTML-Stil und Nur-Text-E-Mails. </p> <p><b>NOTIZ</b></p>
      <p>Die Standardeinstellungen für das Proofing werden von den Einstellungen auf der Ebene des Korrekturabzugs überschrieben. Wenn jedoch in den Einstellungen von [!UICONTROL Account] E-Mail-Benachrichtigungen zu Korrekturabzügen für das gesamte Konto deaktiviert sind, werden keine E-Mail-Warnungen an die Mitwirkenden gesendet, selbst wenn in Korrekturabzügen die Option [!UICONTROL Disabled email alert] nicht ausgewählt ist.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ändern **[!UICONTROL unter &quot;]**&quot; eine der folgenden Einstellungen:

   | Testversandvorlage | Beschreibung |
   |---|---|
   | **[!UICONTROL Vorlage für Korrekturabzug-Betreff]** | Wird auf den Seiten Neuer Korrekturabzug, Neue Version, Nachricht und Erinnerung angezeigt. Kann bearbeitet werden, bevor es gesendet wird. |
   | **[!UICONTROL Testversandnachrichtenvorlage]** | Wird auf den Seiten Neuer Korrekturabzug, Neue Version, Nachricht und Erinnerung angezeigt. Kann bearbeitet werden, bevor es gesendet wird. |

## Ändern von E-Mail-Warnungen für einen Empfänger

Sie können E-Mail-Warnhinweise für einen bestimmten Empfänger in einer Batch-Aktion ändern.

1. Klicken Sie **[!UICONTROL linken Navigationsbereich auf]** Kontakte“.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü ![Mehr](assets/more-button-small.png) für den Empfänger und klicken Sie dann **[!UICONTROL Dropdown-Menü]** Mitgliederdetails anzeigen“.

1. Öffnen Sie den **[!UICONTROL Freigegebene Elemente]** Abschnitt.
1. Aktivieren Sie das Kontrollkästchen links neben jedem Element, für das Sie den E-Mail-Warnhinweis ändern möchten.
1. Klicken Sie **[!UICONTROL Mehr]** über der Liste der freigegebenen Elemente auf und klicken Sie dann **Dropdown-Menü auf** E-Mail-Warnhinweis ändern.

1. Ändern Sie den E-Mail-Warnhinweis und klicken Sie dann auf **[!UICONTROL Senden]**.

## Konfigurieren der Standardeinstellungen für Korrekturabzüge für Benutzende

Als [!DNL Workfront Proof] können Sie Standardeinstellungen für Korrekturabzüge für Benutzende in Ihrem Konto festlegen.

1. Klicken **[!UICONTROL oben]** Bildschirm auf „Kontoeinstellungen“.

1. Öffnen Sie die Registerkarte **[!UICONTROL Benutzer]**.
1. Öffnen Sie das Menü **[!UICONTROL Mehr]** ![Mehr_button_small.](assets/more-button-small.png) rechts neben dem Namen des Benutzers.

1. Klicken Sie **[!UICONTROL Dropdown-Menü auf]** Benutzerdetails anzeigen“.
1. Klicken Sie unter **[!UICONTROL Einstellungen]** auf **[!UICONTROL Standardmäßige E-Mail-Warnhinweiseinstellungen]**, um sie zu erweitern.

1. Wählen Sie in der Dropdown-Liste rechts neben den beiden folgenden Einstellungen eine der in der folgenden Tabelle erläuterten Optionen aus:

   * **[!UICONTROL Standard-E-Mail]** Warnhinweis: Wirkt sich auf alle Korrekturabzüge aus, die für Sie freigegeben wurden. Diese Einstellung kann auf der Ebene des Korrekturabzugs überschrieben werden.
   * **[!UICONTROL Standard-E-Mail-Warnhinweis für neue Gast]** Reviewer: Betrifft Reviewer, die zuvor nicht als Kontakte in Ihrem Konto vorhanden waren.

   >[!NOTE]
   >
   >Wenn Sie für einen Benutzer keine der folgenden Optionen auswählen, sendet [!DNL Workfront Proof] Benutzern eine tägliche Zusammenfassung über die Aktivitäten bei ihren Korrekturabzügen.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Alle Aktivitäten]</td>
      <td>[!DNL Workfront] sendet jedes Mal eine E-Mail an den Prüfer, wenn eine Aktivität im Korrekturabzug vorhanden ist, z. B. ein neuer Kommentar, eine neue Antwort oder eine neue Entscheidung. <p>Dies ist eine hervorragende Option für die Person, die den Proofing-Prozess verwaltet, da sie die Aktivität direkt sehen kann. </p><p>Benutzende erhalten keine E-Mail-Benachrichtigung über ihre eigene Aktivität.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL antwortet auf meine Kommentare]</td>
      <td>Eine E-Mail wird nur dann an den Prüfer gesendet, wenn jemand explizit auf seinen Kommentar antwortet (dies schließt die eigenen Antworten auf seine eigenen Kommentare aus). Das bedeutet, dass, wenn jemand auf dem Korrekturabzug einen neuen Kommentar abgibt, der Prüfer nicht benachrichtigt wird.<p>Diese Einstellung wird für Ihre Kunden auf dem Korrekturabzug empfohlen, damit sie nicht über andere Kommentare zu dem Korrekturabzug benachrichtigt werden und nur über Antworten auf ihre eigenen Kommentare.</p><p>Reviewer mit dieser E-Mail-Warnhinweiseinstellung werden zwar nicht über andere neue Kommentare benachrichtigt, sie können jedoch alle Kommentare zum Korrekturabzug in der Proofing-Anzeige anzeigen.</p><p>Weitere Informationen zu Kommentaren finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Kommentare zu Korrekturabzügen anzeigen und </a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL -Entscheidungen]</td>
      <td>[!DNL Workfront] Sendet nur dann eine E-Mail an den Validierungsverantwortlichen, wenn jemand eine Entscheidung trifft.<p>Dies kann für die Person nützlich sein, die den Genehmigungsprozess verwaltet (z. B. einen Projektmanager) und den Fortschritt beim Korrekturabzug überwachen muss, um zu sehen, welche Benutzer ihre Entscheidung getroffen haben.</p><p>Sie werden über Ihre eigene Entscheidung nur benachrichtigt, wenn Sie beim Senden Ihrer Entscheidung eine E-Mail-Bestätigungsoption auswählen.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Endgültige Entscheidung]</td>
      <td>[!DNL Workfront] Sendet eine E-Mail, wenn die letzte genehmigende Person für den Korrekturabzug ihre Entscheidung getroffen hat.<p>Dieser Warnhinweis wird häufig vom Designer verwendet, der normalerweise nicht an der eigentlichen Überprüfungsdiskussion teilnehmen muss. Wenn die endgültige Entscheidung getroffen wird, wird der Designer benachrichtigt und kann dann die erforderlichen Änderungen vornehmen.</p><p>Dieser Warnhinweis kann auch für einen Abteilungsleiter nützlich sein, der erst benachrichtigt werden muss, wenn der Überprüfungsprozess abgeschlossen ist.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Stündliche Zusammenfassung]</td>
      <td>[!DNL Workfront] Sendet stündlich eine E-Mail mit einer Zusammenfassung aller Kommentare, Antworten und Entscheidungen, die in dieser Stunde stattgefunden haben, an den Prüfer.<p>Die E-Mail wird nur gesendet, wenn innerhalb der letzten Stunde eine andere Aktivität als die eigene stattgefunden hat. </p><p>Dieser Warnhinweis bietet eine gute Möglichkeit, einen Überblick über das Projekt zu erhalten.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein leitender Prüfer, der einen Überblick über das Projekt benötigt, aber nicht sofort über alle Aktivitäten im Korrekturabzug benachrichtigt werden muss.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Tägliche Zusammenfassung]</td>
      <td>[!DNL Workfront] Sendet eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen, die nur an Tagen aufgelistet sind, an denen außer Ihrer eigenen Aktivität eine andere Aktivität stattfindet.<p>Dieser Warnhinweis bietet eine gute Möglichkeit, eine Zusammenfassung des Projekts anzuzeigen, ohne im Laufe des Tages durch mehrere Updates überfordert zu werden.</p><p>Ein Anwendungsbeispiel für diese Zusammenfassung ist ein Abteilungsleiter, der den Gesamtfortschritt des Projekts überwachen möchte.</p><p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Verwalten von Benachrichtigungen für Kommentare und Entscheidungen zu Korrekturabzügen</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL Keine E-Mail]</td>
      <td>[!DNL Workfront] sendet keine E-Mail-Warnungen.<br>Dies ist für Personen nützlich, die einem Korrekturabzug nur zu Referenzzwecken hinzugefügt werden und nicht über Änderungen benachrichtigt werden müssen.<p>Der Systemstandard ist [!UICONTROL Daily Summary] (auch als [!UICONTROL Not Set] bezeichnet). Wenn Sie oder Ihre Prüfer keine anderen Änderungen vornehmen, haben alle Ihre Korrekturabzüge diese Einstellung.</p></td>
     </tr>
    </tbody>
   </table>

1. Ändern Sie in den **[!UICONTROL Standardeinstellungen für E-Mail]** Warnhinweise) einen der folgenden Schritte:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL E-Mail-Bestätigung, wenn die Testsendungen fertig sind]</td> 
      <td>Geben Sie an, ob Sie beim Erstellen eines Korrekturabzugs eine [!UICONTROL Proof made]-E-Mail erhalten möchten. Weitere Informationen finden Sie unter <a href="https://support.workfront.com/hc/en-us/article">Die E-Mail mit dem [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format der an mich gesendeten E-Mails] </td> 
      <td> <p>Wählen Sie zwischen E-Mails im HTML-Stil und Nur-Text-E-Mails. </p> <p><b>NOTIZ</b></p> <p>Die Standardeinstellungen für das Proofing werden von den Einstellungen auf der Ebene des Korrekturabzugs überschrieben. Wenn jedoch in den Einstellungen von [!UICONTROL Account] E-Mail-Benachrichtigungen zu Korrekturabzügen für das gesamte Konto deaktiviert sind, werden keine E-Mail-Warnungen an die Mitwirkenden gesendet, selbst wenn in Korrekturabzügen die Option [!UICONTROL Disabled email alert] nicht ausgewählt ist.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
