---
content-type: reference
navigation-topic: notifications
title: "Benachrichtigungen: Informationen über Projekte, deren Inhaber ich bin"
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die in einem Projekt durchgeführt werden, dessen Eigentümer Sie sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter Ändern Ihrer eigenen E-Mail-Benachrichtigungen.
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 1%

---

# Benachrichtigungen: Informationen zu Projekten, die ich besitze

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die in einem Projekt durchgeführt werden, dessen Eigentümer Sie sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>Ein Dokument wird zu einem Projekt hinzugefügt, dessen Eigentümer ich bin</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn ein Dokument zum Projekt hinzugefügt wird, es sei denn, der Benutzer, der das Dokument hinzugefügt hat, ist auch Projektinhaber.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet und das Dokument nicht privat ist.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Dokument hinzugefügt zu] &lt;Projektname&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Projektname<br>Projektname<br>Projektnummer<br>Name des Portfolios, der das Dokument hinzugefügt hat<br>Dokumentname<br>Hinzugefügt am Datum<br>Dokumentdetails (Format, Größe, Versionsnummer)<br><strong>[!UICONTROL Vorschau]</strong> und <strong>[!UICONTROL Download]</strong> Schaltflächen<br>*Projektname<br>*Projektnummer<br>}*Gesamtzahl der hinzugefügten Dokumente<br>*Dokumentname<br>*Name des Benutzers, der das Dokument hinzugefügt hat<br>*Datum des täglichen Digest<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Meilensteinaufgabe wird für ein Projekt abgeschlossen, dessen Eigentümer ich bin</strong> </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;Task Name&gt; unter &lt;Projektname&gt;</em></p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, wird im Betreff der E-Mail weiterhin "[!UICONTROL Complete]"angezeigt.</p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>}*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum des täglichen Digest </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Projekt, das in meinem Besitz ist, ist in Verzug geraten</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn das Projekt verspätet ist. Ein Projekt liegt hinter dem Zeitplan, wenn der Fortschrittsstatus "[!UICONTROL At Risk]", "[!UICONTROL Behind]"oder "[!UICONTROL Late]"lautet.</p> <p>Es empfiehlt sich, diese Benachrichtigung aktiv zu halten. </p> <p>Benutzer mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Project Progress Change]: &lt;Projektname&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Projektname<br>Projektname<br>Projektreferenz-Nummer<br>Projektfortschrittsstatus<br>Projekt [!UICONTROL Geplantes Startdatum]<br>Projekt [!UICONTROL Geplantes Abschlussdatum]<br>Projekt [!UICONTROL Voraussichtlicher Starttermin]<br>Projekt [!UICONTROL Projektergebnisdatum]<br>Projektanteil abgeschlossen<br>Projektstatus<br>Projektverantwortlicher 10}*Projektname<br>*Referenznummer des Projekts<br>*Projektfortschrittsstatus<br>*Datum des täglichen Digest<br><br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Problem wird einem Projekt in meinem Besitz hinzugefügt</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Problem hinzugefügt zu] &lt;Projektname&gt;</em></p> <p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Projektname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Portfolios, der das Problem hinzugefügt hat<br>Problemname<br>Problemtyp<br>Eingegebener Zeitpunkt<br>Problempriorität<br>Zugeordneter Name <br>Problemstatus<br>Primärer Kontakt<br>*Projektname<br>*Projektreferenz<br>*Gesamtzahl der dem Projekt hinzugefügten Probleme 13}*Problemname<br>*Name des Benutzers, der das Problem hinzugefügt hat<br>*Datum des täglichen Digest<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und Täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Aufgabe wird für ein Projekt abgeschlossen, dessen Eigentümer ich bin</strong> </p> <p>Der Projekteigentümer erhält eine Benachrichtigung, wenn eine Aufgabe in seinem Projekt abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;Task Name&gt; unter &lt;Projektname&gt;</em></p> <p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, wird im Betreff der E-Mail weiterhin "[!UICONTROL Complete]"angezeigt.</p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat <br>Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Siehe Weitere Informationen]</strong> Schaltfläche<br>*Projektname<br>*Projektreferenz-Nummer<br>*Gesamtzahl der abgeschlossenen Aufgaben <br>*Aufgabenname*12} Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum des täglichen Digest<br><br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Aufgabe in einem Projekt, dessen Eigentümer ich bin, wird von </strong> zurückgehalten </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn eine Aufgabe im Projekt hinter den Zeitplan zurückfällt. Eine Aufgabe liegt hinter dem Zeitplan, wenn der Fortschrittsstatus "[!UICONTROL At Risk]"oder "[!UICONTROL Behind]"oder "[!UICONTROL Late]"lautet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Task Progress Change]: &lt;Task Name&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Neuer Aufgabenfortschrittsstatus<br>Aufgabe [!UICONTROL Geplantes Startdatum]<br>Aufgabe [!UICONTROL Geplantes Abschlussdatum]<br>Aufgabe [!UICONTROL Voraussichtliches Startdatum]<br>Aufgabe [!UICONTROL Voraussichtliches Abschlussdatum]<br>Aufgabenprozentsatz abgeschlossen<br>Aufgabenstatus<br> 10}Eingegeben nach Name<br>*Projektname<br>*Projektnummer<br>*Gesamtanzahl der Aufgaben, die hinter der Planung liegen<br>*Aufgabenname<br>*Zugeordneter Name<br>*Datum des täglichen Digest<br> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Problem ist bei einem Projekt, dessen Eigentümer ich bin, abgeschlossen</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn ein Problem in seinem Projekt abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung. </p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;Name des Problems&gt; unter &lt;Projektname&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Problemstatus<br>Datum und Uhrzeit des Abschlusses des Problems<br>Vorheriger Problemstatus<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche <br>*Projektname<br>*Projektverweisnummer<br>*Gesamtzahl der abgeschlossenen Probleme<br> Problemname<br>*Name des Benutzers, der der Ausgabe zugewiesen ist<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein nicht zugewiesenes Problem wird zu einem Projekt hinzugefügt, dessen Eigentümer ich bin</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein nicht zugewiesenes Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Wer sollte diesem neuen Problem zugewiesen werden unter] &lt;Projektname&gt;?</em></p> <p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> Digest of Projects You Own &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Projektname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Portfolios, der das Problem hinzugefügt hat<br>Problemname<br>Problemtyp<br>Eingegebener Zeitpunkt<br>Problempriorität<br>Zugeordneter Name (leer)<br>Problemstatus<br>Primärer Kontakt<br>*Projektname<br>*Projektreferenz<br> Gesamtzahl der Probleme hinzugefügt 13}*Problemname<br>*Name des Benutzers, der das Problem hinzugefügt hat<br>*Datum des täglichen Digest<br><br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und Täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich bin als Eigentümer eines neuen Projekts festgelegt</strong> </p> <p>Wenn ein Benutzer als Eigentümer eines Projekts zugewiesen wird, erhält er eine E-Mail-Benachrichtigung.</p> <p>Wenn der Projekteigentümer derselbe Benutzer ist, der die Zuweisung vorgenommen hat, wird keine E-Mail-Benachrichtigung gesendet.</p> <p>Benutzer mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Schalten Sie das ein, weil ihnen etwas zugeordnet wird. </p> <p> Zuweisen von etwas, Teilen von etwas, Zugriff auf etwas.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Sie sind jetzt Projektinhaber von] &lt;Projektname&gt;</em></p> <p>Der folgende Text ist im Text der E-Mail-Benachrichtigung enthalten:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;Ihr Name&gt;,<br></em><em>&lt;Name des Benutzers, der Sie als Projektinhaber zugewiesen hat&gt; [!UICONTROL hat Sie zum Eigentümer von] &lt;Projektname&gt; gemacht. [!UICONTROL Als Projekteigentümer erhalten Sie möglicherweise zusätzliche E-Mail-Benachrichtigungen über die Projektaktivität, müssen die Stunden für das Projekt genehmigen oder an der Genehmigung der mit dem Projekt verbundenen Arbeit beteiligt sein. Das ist alles deins.]</em> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> <p> </p> </td> 
   <td> <p>Projektname<br>Projektname<br>Projektreferenz-Nummer<br>Projektabschlussdatum<br>*Projektname<br>*Projektnummer<br>*Datum des täglichen Digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Das Datum der Übertragung ändert sich für eine Aufgabe in einem meiner Projekte</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn sich das Veröffentlichungsdatum für eine Aufgabe im Projekt ändert, es sei denn, der Benutzer, der das Veröffentlichungsdatum geändert hat, ist auch Projektinhaber.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Datum für die Übermittlung für] &lt;Aufgabenname&gt; [!UICONTROL ist jetzt] &lt;Neues Veröffentlichungsdatum&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> Digest of Projects You Own &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Name des Benutzers, der das Veröffentlichungsdatum geändert hat<br>Neues Veröffentlichungsdatum<br>Aufgabe [!UICONTROL Geplantes Abschlussdatum]<br>Informationen darüber, wie sich diese Änderung auf die Projekt-Timeline auswirkt<br>Zugeordneter Name<br>Eingegebener Name<br>Projektinhaber<br><strong>[!UICONTROL Siehe Weitere Informationen]{1] 0} button<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtanzahl der Aufgaben, deren Veröffentlichungsdatum geändert wurde<br>*Aufgabenname<br>*Datum des täglichen Digest</strong><br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und [!UICONTROL Täglich]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Das Commitdatum ändert sich für ein Problem in einem meiner Projekte</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn sich das Veröffentlichungsdatum für ein Problem im Projekt ändert, es sei denn, der Benutzer, der das Veröffentlichungsdatum ändert, ist derselbe Benutzer wie der Projekteigentümer.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Datum für die Veröffentlichung für] &lt;Name des Problems&gt; [!UICONTROL ist jetzt] &lt;Neues Datum für die Zusage&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Benutzers, der das Veröffentlichungsdatum geändert hat<br>Neues Veröffentlichungsdatum<br>Geplantes Abschlussdatum des Problems<br>Zugeordneter Name<br>Eingegeben nach Name<br>Projektinhaber<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Projektnummer <br>*Gesamtzahl der Probleme, deren Veröffentlichungsdatum sich geändert hat<br>*Name des Problems<br>*Datum des täglichen Digest<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und [!UICONTROL Täglich]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
