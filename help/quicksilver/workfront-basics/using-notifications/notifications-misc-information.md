---
content-type: reference
navigation-topic: notifications
title: 'Benachrichtigungen: Verschiedene Informationen'
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten in einem Projekt, das Sie als Sponsor unterstützen.
author: Courtney
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# Benachrichtigungen: Verschiedene Informationen

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten in einem Projekt, das Sie als Sponsor unterstützen.

Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Sie können keine täglichen Benachrichtigungen aktivieren oder deaktivieren und Sie erhalten auch keine täglichen Auswahl-E-Mails für die Ereignisse in dieser Kategorie. Sie können einzelne Sofortbenachrichtigungen für die Kategorie [!UICONTROL Verschiedenes] aktivieren oder deaktivieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th> <p>Enthaltene Felder </p> <p> *Nur Tägliche Digest-Felder</p> </th> 
   <th>Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Eine Nachricht wird an das [!UICONTROL Announcement Center] gesendet</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn eine neue Nachricht an das [!UICONTROL Announcement Center] gesendet wurde. </p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL [!DNL Adobe Workfront] Ankündigung]: &lt;Betreff der Ankündigung&gt;</em></p> </td> 
   <td> Betreff der Ankündigung<br>Text der Nachricht in den Ankündigungsbeilagen<br><br> DokumentenName des Benutzers, der die Ankündigung gesendet hat<br> Datum und Uhrzeit, an dem die Ankündigung gesendet wurde </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Aufgabenzuweisungsänderung wirkt sich auf mein Team aus</strong> </p> <p>Wenn einer der Direktberichte eines als Manager bestimmten Benutzers einer neuen Aufgabe zugewiesen wird, erhält der Manager eine E-Mail über die Zuweisung. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Task Resource Assignment]: &lt;Aufgabenname&gt;</em></p> </td> 
   <td>Projektname<br>Aufgabenname<br>Datum und Uhrzeit der Erstellung der Aufgabe<br>Name des Benutzers, der die <br> erstellt hat<br>Fälligkeitsdatum (Geplantes Abschlussdatum)<br>Aufgabenstatus<br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Nach Erhalt einer Dokumentuploadanfrage wird die Anfrage abgebrochen</strong> </p> <p>Der angeforderte Dokumentverantwortliche erhält eine E-Mail-Benachrichtigung, wenn eine Dokumentanforderung abgebrochen wird.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>&lt;Name des Benutzers, der die Anforderung storniert hat&gt; hat die Dokumentanforderung storniert. </em></p> <p>Der folgende Text ist im Textkörper der E-Mail-Benachrichtigung enthalten:</p> <p><em>[!UICONTROL Hi] &lt;Ihr Name&gt;, <br><br>&lt;Name des Benutzers, der die Anfrage storniert hat&gt;[!UICONTROL braucht nicht länger irgendetwas hochzuladen, was die Anfrage betrifft, die Sie zuvor erhalten haben. Wir wollten Ihnen nur Bescheid geben.]</em> </p> </td> 
   <td>Name des Benutzers, der die Anfrage storniert hat<br>Der Text der Anfrage zum ursprünglichen Dokument-Upload<br>Ein "[!UICONTROL CANCELLED]"-Banner über der Anfrage zum ursprünglichen Dokument<br>Datum und Uhrzeit der Anfrage zum ursprünglichen Dokument<br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Es wurde ein Fehler gefunden, der meine Aufmerksamkeit erfordert</strong> </p> <p>Der Benutzer, der auf einen Kommentar per E-Mail antwortet, erhält eine E-Mail-Benachrichtigung, wenn die Antwort nicht zugestellt werden kann.</p> <p>Der Betreff der Sofort-Benachrichtigungs-E-Mail ist: <em>[!UICONTROL konnte nicht verarbeitet werden am] &lt;Betreff der ursprünglichen Nachricht&gt;</em></p> <p>Informationen zur Verwendung von E-Mail zum Antworten auf Kommentare finden Sie unter <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Antworten auf E-Mail-Benachrichtigungen</a>.</p> </td>
   <td> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Änderung bei einer Problemzuweisung wirkt sich auf mein Team aus</strong> </p> <p>Der Manager eines Benutzers, der einem Problem zugewiesen wurde, erhält eine E-Mail-Benachrichtigung, wenn dieser Benutzer aus einem Problem entfernt oder einem Problem zugewiesen wurde. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Problemzuweisung: &lt;Problemname&gt;</em></p> </td> 
   <td> <p>Problemname<br> Projektname<br>Problem-Referenznummer<br>Name des Benutzers, der die Zuweisung vorgenommen hat<br>Problemtyp<br>Name des Benutzers, der dem Problem zugewiesen wurde<br>Problemdatum eingegeben<br>Problempriorität<br>Primärer Kontakt<br>Problem [!UICONTROL Geplantes Abschlussdatum]<br>Problemstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Einer meiner Mitarbeiter wird einem Projekt hinzugefügt</strong> </p> <p>Ein Manager erhält eine E-Mail-Benachrichtigung, wenn einer seiner Benutzer zu einem Projekt hinzugefügt wird. Diese Benachrichtigung wird unabhängig vom Status des Projekts gesendet. </p> <p>Benutzende mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der E-Mail lautet: <em>Projektzuweisung: &lt;Benutzername&gt;[&lt;Projekt-GUID&gt;_ &lt;Benutzer-GUID&gt;]</em></p> </td> 
   <td> <p>Projektname<br>Portfolio-Name<br>Projekt-Referenznummer<br>Name des Benutzers, der die Person zum Projekt hinzugefügt hat<br>Name des Benutzers, der zum Projekt hinzugefügt wurde<br>Projekt [!UICONTROL Geplantes Startdatum]<br>Projekt [!UICONTROL Geplantes Abschlussdatum]<br>Projekt Prozent abgeschlossen<br>Namen anderer auf Projekt<br>Projektstatus<br>Projektinhaber<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br><br><br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand fügt ein Projekt einem Portfolio oder Programm hinzu, dessen Besitzer ich bin</strong> </p> <p>Das Portfolio und/oder der Programmbesitzer erhalten eine Benachrichtigung, wenn ein neues Projekt zu einem Portfolio oder Programm hinzugefügt wird.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Projekt hinzugefügt zu] &lt;Portfolio-Name&gt;[Projekt-GUID]</em></p> </td> 
   <td> Portfolio Name<br>Project Reference Number<br>Name des Benutzers, der das Projekt zum Portfolio/Programm hinzugefügt hat<br><br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand hat ein Objekt für mich freigegeben</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn Sie jemand zur [!UICONTROL Sharing]-Liste mit Berechtigungen für ein Objekt hinzufügt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Zugriff erteilt]: &lt;Objektname&gt;</em></p> <p>Eine Benachrichtigung wird nur gesendet, wenn sich das Projekt im Status [!UICONTROL Aktuell] befindet.</p> </td> 
   <td> Objektname<br>übergeordneter Objektname<br>Objektreferenznummer<br>Originalzugriff auf das Objekt<br>Neuer Zugriff gewährt für das Objekt<br>Datum und Uhrzeit, an dem der Zugriff gewährt wurde<br>Name des Benutzers, der den Zugriff gewährt hat </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand hat ein Objekt für mein Team freigegeben</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn jemand Ihr Team zur Freigabeliste für ein Objekt hinzufügt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Zugriff erteilt]: &lt;Objektname&gt; [Zugriffsregel-GUID]</em></p> </td> 
   <td> Objektname<br>übergeordneter Objektname<br>Objektreferenz-Nummer<br>Alter Zugriff<br>Neuer Zugriff<br> Datum und Uhrzeit der Zugriffsgewährung<br>Name Ihres Teams<br>Name des Benutzers, der den Zugriff gewährt hat </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>An einer Aufgabe, einem Problem oder einem Projekt, die bzw. das ich abonniert habe, wird eine Aktualisierung vorgenommen</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn jemand einen Kommentar zu einem Element abonniert, für das Sie angemeldet sind.</p> <p>Der Betreff der Abonnement-E-Mail ist: <em>[!UICONTROL Ein Update wurde für den] &lt;Objekttyp&gt; durchgeführt, den Sie abonniert haben: &lt;Objektname&gt;</em></p> </td> 
   <td> Objektname<br> Objektreferenz-Nummer<br> Name des Benutzers, der einen Kommentar zum abonnierten Element abgegeben hat<br> Date comment was made<br> Comment added to the subscribed item  </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
