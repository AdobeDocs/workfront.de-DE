---
content-type: reference
navigation-topic: notifications
title: "Mitteilungen: Verschiedene Informationen"
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die an einem Projekt durchgeführt werden, das Sie sponsern.
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 8%

---

# Mitteilungen: Verschiedene Informationen

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die an einem Projekt durchgeführt werden, das Sie sponsern.

Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>Sie können tägliche Benachrichtigungen nicht aktivieren oder deaktivieren und erhalten keine täglichen Digest-E-Mails für die Ereignisse in dieser Kategorie. Sie können einzelne Instant-Benachrichtigungen für die [!UICONTROL Sonstiges] Kategorie.

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
   <td> <p><strong>Eine Nachricht wird an das [!UICONTROL Ankündigungszentrum] gesendet.</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, sobald eine neue Nachricht an das [!UICONTROL Ankündigungszentrum] gesendet wurde. </p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL [!DNL Adobe Workfront] Mitteilung]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> Gegenstand der Mitteilung<br>Text der in der Mitteilung enthaltenen Nachricht<br>Attached Document(s)<br>Name des Benutzers, der die Mitteilung gesendet hat<br>Datum und Uhrzeit des Versands der Mitteilung </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Aufgabenzuweisung wirkt sich auf einen meiner Mitarbeiter aus</strong> </p> <p>Wenn einer der Direktberichte eines Benutzers, der als Manager benannt wurde, einer neuen Aufgabe zugewiesen wird, erhält der Manager eine E-Mail über die Zuweisung. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Task Resource Assignment]: &lt;task name=""&gt;</em></p> </td> 
   <td>Projektname<br>Aufgabenname<br>Datum und Uhrzeit der Erstellung der Aufgabe<br>Name des Benutzers, der die Aufgabe erstellt hat<br>Zuweisungsnamen<br>Fälligkeitsdatum (Geplantes Abschlussdatum)<br>Aufgabenstatus<br></td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Nachdem Sie eine Anfrage zum Hochladen erhalten haben, wird die Anfrage storniert.</strong> </p> <p>Die Dokumentanforderung erhält eine E-Mail-Benachrichtigung, wenn eine Dokumentanforderung abgebrochen wird.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; die Dokumentanforderung abgebrochen hat. </em></p> <p>Der folgende Text ist im Text der E-Mail-Benachrichtigung enthalten:</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL braucht keine Informationen mehr zu der zuvor gestellten Anfrage hochzuladen. Wir wollten euch nur Bescheid geben.]</em> </p> </td> 
   <td>Name des Benutzers, der die Anforderung abgebrochen hat<br>Der Text der ursprünglichen Anforderung zum Hochladen von Dokumenten<br>Ein Banner "[!UICONTROL CANCELED]"über der ursprünglichen Dokumentanforderung<br>Datum und Uhrzeit der ursprünglichen Dokumentanforderung<br></td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Es wurde ein Fehler gefunden, der meine Aufmerksamkeit erfordert</strong> </p> <p>Der Benutzer, der auf einen Kommentar per E-Mail antwortet, erhält eine E-Mail-Benachrichtigung, wenn die Antwort nicht zugestellt werden kann.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Fehler bei der Verarbeitung von] &lt;subject of="" original="" message=""&gt;</em></p> <p>Informationen zur Verwendung von E-Mails zur Beantwortung von Kommentaren finden Sie unter .<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Änderung bei einer Problemzuweisung wirkt sich auf mein Team aus</strong> </p> <p>Der Manager eines einem Problem zugewiesenen Benutzers erhält eine E-Mail-Benachrichtigung, wenn dieser Benutzer aus einem Problem entfernt oder einem Problem zugewiesen wird. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Problemzuweisung: &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemverweisnummer<br>Name des Benutzers, der die Zuweisung vorgenommen hat<br>Problemtyp<br>Name des dem Problem zugewiesenen Benutzers<br>Ausgabedatum eingegeben<br>Problempriorität<br>Primärer Kontakt<br>Problem [!UICONTROL Geplantes Abschlussdatum]<br>Problemstatus<br><strong>[!UICONTROL Weitere Informationen]</strong> button</p> </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Einer meiner Mitarbeiter wird einem Projekt hinzugefügt</strong> </p> <p>Ein Manager erhält eine E-Mail-Benachrichtigung, wenn einem Projekt ein Benutzer hinzugefügt wird. Diese Benachrichtigung wird unabhängig vom Status des Projekts gesendet. </p> <p>Benutzer mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail ist: <em>Projektzuweisung: &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>Projektname<br>Portfolio Name<br>Referenz-Nummer des Projekts<br>Name des Benutzers, der die Person zum Projekt hinzugefügt hat<br>Name des Benutzers, der zum Projekt hinzugefügt wurde<br>Projekt [!UICONTROL Geplantes Startdatum]<br>Projekt [!UICONTROL Geplantes Abschlussdatum]<br>Projektanprozentsatz abgeschlossen<br>Namen anderer Personen im Projekt<br>Projektstatus<br>Projektinhaber<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br><br><br></p> </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand fügt ein Projekt einem Portfolio oder Programm zu, dessen Besitzer ich bin</strong> </p> <p>Das Portfolio und/oder der Programmeigentümer erhalten eine Benachrichtigung, wenn ein neues Projekt zu einem Portfolio oder Programm hinzugefügt wird.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Projekt hinzugefügt zu] &lt;portfolio name=""&gt;[Projekt-GUID]</em></p> </td> 
   <td> Portfolio Name<br>Referenz-Nummer des Projekts<br>Name des Benutzers, der das Projekt zum Portfolio/Programm hinzugefügt hat<br><br></td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand hat ein Objekt für mich freigegeben</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn Sie von einer Person zur Liste der Berechtigungen für ein Objekt hinzugefügt werden.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Zugriff gewährt]: &lt;object name=""&gt;</em></p> <p>Eine Benachrichtigung wird nur gesendet, wenn das Projekt den Status [!UICONTROL Aktuell] aufweist.</p> </td> 
   <td> Objektname<br>Übergeordneter Objektname<br>Objektverweisnummer<br>Originalzugriff auf das Objekt<br>Neuer Zugriff für das Objekt gewährt<br>Datum und Uhrzeit der Gewährung des Zugriffs <br>Name des Benutzers, der den Zugriff gewährt hat </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand hat ein Objekt für mein Team freigegeben</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn jemand Ihr Team zur Liste der Berechtigungen für ein Objekt hinzufügt.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Zugriff gewährt]: &lt;object name=""&gt; [ZugriffsregelGUID]</em></p> </td> 
   <td> Objektname<br>Übergeordneter Objektname<br>Objektverweisnummer<br>Alter Zugriff<br>Neuer Zugriff<br>Datum und Uhrzeit der Gewährung des Zugriffs<br>Name Ihres Teams<br>Name des Benutzers, der den Zugriff gewährt hat </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>An einer Aufgabe, einem Problem oder einem Projekt, für das ich angemeldet bin, wird eine Aktualisierung vorgenommen.</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn jemand einen Artikel kommentiert, für den Sie sich angemeldet haben.</p> <p>Betreff der Abonnement-E-Mail ist: <em>[!UICONTROL Es wurde ein Update am] &lt;object type=""&gt; Sie haben ein Abonnement für: &lt;object name=""&gt;</em></p> </td> 
   <td> Objektname<br> Objektverweisnummer<br> Name des Benutzers, der einen Kommentar zum abonnierten Element abgegeben hat<br> Datum, an dem Kommentar abgegeben wurde<br> Kommentar zum abonnierten Element hinzugefügt  </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
 </tbody> 
</table>
