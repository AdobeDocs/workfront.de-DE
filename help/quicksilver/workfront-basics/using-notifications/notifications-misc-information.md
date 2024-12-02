---
content-type: reference
navigation-topic: notifications
title: 'Mitteilungen: Verschiedene Informationen'
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die an einem Projekt durchgeführt werden, das Sie sponsern.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 298b74c2d228a76c02d34470fa8298028605cab4
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# Mitteilungen: Verschiedene Informationen

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die an einem Projekt durchgeführt werden, das Sie sponsern.

Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Sie können tägliche Benachrichtigungen nicht aktivieren oder deaktivieren und erhalten keine täglichen Digest-E-Mails für die Ereignisse in dieser Kategorie. Sie können einzelne Instant-Benachrichtigungen für die Kategorie [!UICONTROL Verschiedenes] aktivieren oder deaktivieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th> <p>Einbezogene Felder </p> <p> *Nur tägliche Digest-Felder</p> </th> 
   <th>Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Eine Nachricht wird an das [!UICONTROL Ankündigungszentrum]</strong> gesendet </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, sobald eine neue Nachricht an das [!UICONTROL Ankündigungszentrum] gesendet wurde. </p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL [!DNL Adobe Workfront] Mitteilung]: &lt;Betreff der Mitteilung&gt;</em></p> </td> 
   <td> Betreff der Mitteilung<br>Text der Nachricht, die in der Mitteilung enthalten ist<br>Angehängte Dokument(e)<br>Name des Benutzers, der die Mitteilung gesendet hat<br>Datum und Uhrzeit des Versands der Mitteilung </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Änderung der Aufgabenzuweisung wirkt sich auf eine meiner Personen aus</strong> </p> <p>Wenn einer der Direktberichte eines Benutzers, der als Manager benannt wurde, einer neuen Aufgabe zugewiesen wird, erhält der Manager eine E-Mail über die Zuweisung. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Task Resource Assignment]: &lt;Task Name&gt;</em></p> </td> 
   <td>Projektname<br>Aufgabenname<br>Datum und Uhrzeit der Erstellung der Aufgabe<br>Name des Benutzers, der die Aufgabe erstellt hat<br>Zuweisungsnamen<br>Fälligkeitsdatum (Geplantes Abschlussdatum)<br>Aufgabenstatus<br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Nach Erhalt einer Dokument-Upload-Anfrage wird die Anfrage abgebrochen</strong> </p> <p>Die Dokumentanforderung erhält eine E-Mail-Benachrichtigung, wenn eine Dokumentanforderung abgebrochen wird.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>&lt;Name des Benutzers, der die Anforderung abgebrochen hat&gt; die Dokumentanforderung abgebrochen hat. </em></p> <p>Der folgende Text ist im Text der E-Mail-Benachrichtigung enthalten:</p> <p><em>[!UICONTROL Hi] &lt;Ihr Name&gt;, <br><br>&lt;Name des Benutzers, der die Anfrage abgebrochen hat&gt;[!UICONTROL braucht keine Informationen mehr zu der Anfrage hochzuladen, die Sie zuvor erhalten haben. Wir wollten Ihnen nur Bescheid geben.]</em> </p> </td> 
   <td>Name des Benutzers, der die Anforderung abgebrochen hat<br>Der Text der ursprünglichen Anforderung zum Hochladen von Dokumenten<br>Ein Banner "[!UICONTROL CANCELED]"über der ursprünglichen Anforderung für das Dokument<br>Datum und Uhrzeit der ursprünglichen Anforderung für das Dokument<br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Es wurde ein Fehler gefunden, der meine Aufmerksamkeit erfordert</strong> </p> <p>Der Benutzer, der auf einen Kommentar per E-Mail antwortet, erhält eine E-Mail-Benachrichtigung, wenn die Antwort nicht zugestellt werden kann.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Failed to Process on] &lt;subject of original message&gt;</em></p> <p>Informationen zur Verwendung von E-Mail zur Beantwortung von Kommentaren finden Sie unter <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">Antworten auf E-Mail-Benachrichtigungen </a>.</p> </td>
   <td> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Änderung bei der Zuweisung von Problemen betrifft eine meiner Personen</strong> </p> <p>Der Manager eines einem Problem zugewiesenen Benutzers erhält eine E-Mail-Benachrichtigung, wenn dieser Benutzer aus einem Problem entfernt oder einem Problem zugewiesen wird. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>Problemzuweisung: &lt;Problemname&gt;</em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Benutzers, der die Zuweisung vorgenommen hat<br>Problemtyp<br>Name des dem Problem zugewiesenen Benutzers<br>Bereitstellungsdatum eingegeben<br>Problempriorität<br>Primärer Kontakt<br>Problem [!UICONTROL Geplantes Abschlussdatum]<br>Problemstatus<br><strong>[!UICONTROL Siehe Weitere Informationen] 11}-Schaltfläche</strong></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Einer meiner Personen wird einem Projekt hinzugefügt</strong> </p> <p>Ein Manager erhält eine E-Mail-Benachrichtigung, wenn einem Projekt ein Benutzer hinzugefügt wird. Diese Benachrichtigung wird unabhängig vom Status des Projekts gesendet. </p> <p>Benutzer mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail ist: <em>Projektzuweisung: &lt;Benutzername&gt;[&lt;Projekt-GUID&gt;_ &lt;Benutzer-GUID&gt;]</em></p> </td> 
   <td> <p>Projektname<br>Projektname<br>Projektreferenz-Nummer<br>Name des Portfolios, der die Person zum Projekt hinzugefügt hat<br>Name des Benutzers, der zum Projekt hinzugefügt wurde<br>Projekt [!UICONTROL Geplantes Startdatum]<br>Projekt [!UICONTROL Geplantes Abschlussdatum]<br>Projektanteil abgeschlossen<br>Namen anderer Benutzer im Projekt<br>Projektstatus<br>Projektverantwortlicher <br><strong>[!UICONTROL Weitere Informationen]</strong>-Schaltfläche<br><br><br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand fügt einem Portfolio oder Programm, das ich besitze, ein Projekt hinzu</strong> </p> <p>Das Portfolio und/oder der Programmeigentümer erhalten eine Benachrichtigung, wenn ein neues Projekt zu einem Portfolio oder Programm hinzugefügt wird.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Project added to] &lt;Portfolio Name&gt;[Project GUID]</em></p> </td> 
   <td> Projektname<br>Projektnummer<br>Name des Portfolios, der das Projekt zum Portfolio/Programm hinzugefügt hat<br><br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand teilt ein Objekt mit mir</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn Sie von einer Person zur Liste der Berechtigungen für ein Objekt hinzugefügt werden.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Access Granted]: &lt;Object Name&gt;</em></p> <p>Eine Benachrichtigung wird nur gesendet, wenn das Projekt den Status [!UICONTROL Aktuell] aufweist.</p> </td> 
   <td> Objektname<br>Übergeordneter Objektname<br>Objektreferenz-Nummer<br>Originalzugriff auf das Objekt<br>Neuer Zugriff für das Objekt<br>Datum und Uhrzeit der Gewährung des Zugriffs <br>Name des Benutzers, der den Zugriff gewährt hat </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand teilt ein Objekt mit meiner Mannschaft</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn jemand Ihr Team zur Liste der Berechtigungen für ein Objekt hinzufügt.</p> <p>Betreff der E-Mail mit der sofortigen Benachrichtigung ist: <em>[!UICONTROL Access Granted]: &lt;Object Name&gt; [Access Rule GUID]</em></p> </td> 
   <td> Objektname<br>Übergeordneter Objektname<br>Objektreferenz-Nummer<br>Alter Zugriff<br>Neuer Zugriff<br>Datum und Uhrzeit der Gewährung des Zugriffs<br>Name Ihres Teams<br>Name des Benutzers, der den Zugriff gewährt hat </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>An einer Aufgabe, einem Problem oder einem Projekt, für das ich angemeldet bin, wird eine Aktualisierung vorgenommen.</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn jemand einen Artikel kommentiert, für den Sie sich angemeldet haben.</p> <p>Betreff der Abonnement-E-Mail ist: <em>[!UICONTROL Es wurde eine Aktualisierung an dem von Ihnen abonnierten &lt;Objekttyp&gt; vorgenommen: &lt;Objektname&gt;</em></p> </td> 
   <td> Objektname<br> Objektreferenz-Nummer<br> Name des Benutzers, der einen Kommentar zum abonnierten Element abgegeben hat<br> Datumskommentar <br> Kommentar zum abonnierten Element hinzugefügt  </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
