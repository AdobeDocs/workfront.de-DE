---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Verwalten von Benachrichtigungen für Korrekturabzugskommentare und Entscheidungen
description: Wenn Sie an einem Korrekturabzug arbeiten, egal ob Sie Adobe Workfront-Benutzer oder externer Mitarbeiter sind, können Sie angeben, welche E-Mail-Benachrichtigungen Sie zu Kommentaren und Entscheidungen bezüglich des Korrekturabzugs erhalten möchten. Weitere Informationen finden Sie unter Kommentare und Entscheidungen zu Korrekturabzügen - Überblick.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 385f4a6663cacfdcf519bf5699fc1840c2cb2adc
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 2%

---

# Verwalten von Benachrichtigungen für Korrekturabzugskommentare und Entscheidungen

<!-- Audited: 4/2025 -->

Wenn Sie an einem Korrekturabzug arbeiten, egal ob Sie Adobe Workfront-Benutzer oder externer Mitarbeiter sind, können Sie angeben, welche E-Mail-Benachrichtigungen Sie zu Kommentaren und Entscheidungen bezüglich des Korrekturabzugs erhalten möchten. Weitere Informationen finden Sie unter [Benachrichtigungen für Korrekturabzugskommentare und Entscheidungen - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Diese Benachrichtigungen unterscheiden sich von den E-Mail-Warnhinweisen, die Sie zum Testversandfluss zwischen den Validierungsverantwortlichen erhalten können, sowie von den E-Mail-Warnhinweiseinstellungen, die Sie in Workfront konfigurieren können.

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
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rolle des Korrekturabzugs </td> 
   <td>Prüfer, Prüfer und genehmigende Person, Autor, Moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verwalten von Benachrichtigungen für Korrekturabzugskommentare und Entscheidungen

1. Öffnen Sie den Korrekturabzug, für den Sie Benachrichtigungen konfigurieren möchten.
1. Wenn die linke Symbolleiste nicht angezeigt wird, klicken Sie auf **Menü** in der linken oberen Ecke der Web-Korrekturabzugsanzeige.

   ![menu_icon_in_proofing_viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Klicken Sie in der linken Symbolleiste auf das Symbol **Einstellungen** (![_icon.png](assets/settings-icon.png) .

1. Wählen **im Abschnitt E-Mail-Benachrichtigungen senden über** Benachrichtigungseinstellung für diesen Korrekturabzug aus.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle Aktivitäten</td> 
      <td>Der Validierungsverantwortliche erhält jedes Mal eine E-Mail, wenn es eine Aktivität im Korrekturabzug gibt, z. B. einen neuen Kommentar, eine neue Antwort oder eine neue Entscheidung.<br><p>Diese Einstellung wird der Person, die den Proofing-Prozess verwaltet, empfohlen, da sie die Aktivität direkt sehen kann. Benutzende erhalten keine E-Mail-Benachrichtigung über ihre eigene Aktivität (z. B. Kommentare, Antworten oder Entscheidungen).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Antworten auf meine Kommentare</td> 
      <td>Eine E-Mail wird nur dann an den Prüfer gesendet, wenn jemand direkt auf seinen Kommentar antwortet (wobei die Antworten auf seine eigenen Kommentare ausgeschlossen werden).<p>Diese Einstellung wird Ihren Kunden empfohlen, damit sie nur über Antworten auf ihre eigenen Kommentare benachrichtigt werden und nicht über andere Kommentare zu dem Korrekturabzug. Sie können jedoch weiterhin alle Kommentare in der Korrekturabzugsansicht anzeigen.</p>
      <p>Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Kommentare zu Korrekturabzügen anzeigen und beantworten</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidungen</td> 
      <td>Eine E-Mail wird nur dann an den Validierungsverantwortlichen gesendet, wenn jemand eine Entscheidung trifft.<br><p>Dieser E-Mail-Warnhinweis kann für die Person, die den Genehmigungsprozess verwaltet, nützlich sein, da die Person, die den Genehmigungsprozess verwaltet, den Fortschritt des Korrekturabzugs überwachen und sehen kann, welche Benutzenden ihre Entscheidung getroffen haben.<br></p><p>Sie werden über Ihre eigene Entscheidung nur benachrichtigt, wenn Sie beim Senden Ihrer Entscheidung eine E-Mail-Bestätigungsoption auswählen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Finale Entscheidung</td> 
      <td>Eine E-Mail wird gesendet, wenn die endgültige Entscheidung über den Korrekturabzug getroffen wird.<br><p>Dieser Warnhinweis wird häufig vom Designer verwendet, da er nicht an der eigentlichen Überprüfungsdiskussion teilnehmen muss. Wenn die endgültige Entscheidung getroffen wird, wird der Designer benachrichtigt und kann dann die erforderlichen Änderungen vornehmen.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Stündliche Zusammenfassung</td> 
      <td>Der Validierungsverantwortliche erhält stündlich eine E-Mail mit einer Zusammenfassung aller Kommentare, Antworten und Entscheidungen, die in der letzten Stunde vorgenommen wurden.<br><p>Die E-Mail wird nur gesendet, wenn innerhalb der letzten Stunde eine andere Aktivität als die eigene stattgefunden hat. Wenn keine Aktivität von anderen Benutzern vorhanden ist, wird keine E-Mail gesendet.<br></p><p>Dieser Warnhinweis bietet eine gute Möglichkeit, um einen Überblick über das Projekt zu erhalten, während es ausgeführt wird.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tägliche Zusammenfassung</td> 
      <td>(Standardeinstellung): Täglich wird eine E-Mail mit allen Kommentaren, Antworten und Entscheidungen gesendet. Dieser Versand erfolgt nur an Tagen, an denen neben der eigenen Aktivität auch eine andere Aktivität stattfindet.<br><p>Dieser Warnhinweis bietet eine gute Möglichkeit, eine Zusammenfassung des Projekts anzuzeigen, ohne im Laufe des Tages durch mehrere Updates überfordert zu werden.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Keine E-Mail</td> 
      <td>Keine E-Mail-Warnungen gesendet.<br><p>Diese Einstellung ist für Personen nützlich, die einem Korrekturabzug nur zu Referenzzwecken hinzugefügt werden und nicht über Änderungen benachrichtigt werden müssen.</p><p>Hinweis: <p>Mit dieser Option werden nur E-Mail-Warnungen zu Korrekturabzugskommentaren und -entscheidungen deaktiviert. Die E-Mail-Warnungen, die Sie über den Fluss eines Korrekturabzugs erhalten können, wie z. B. die E-Mail Neuer Korrekturabzug oder Später Korrekturabzug , werden nicht deaktiviert. Weitere Informationen finden Sie in den folgenden Artikeln: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Neue Korrekturabzugs-E-Mail</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">Die neue E-Mail-Version</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-Mail zu verspätetem Korrekturabzug</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">Die E-Mail mit dem Korrekturabzug</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
