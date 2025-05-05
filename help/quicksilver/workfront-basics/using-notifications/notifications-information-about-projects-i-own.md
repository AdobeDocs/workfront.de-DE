---
content-type: reference
navigation-topic: notifications
title: 'Benachrichtigungen: Informationen zu Projekten in meinem Besitz'
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die in einem von Ihnen verwalteten Projekt stattfinden. Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter Ändern Ihrer eigenen E-Mail-Benachrichtigungen .
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 1%

---

# Benachrichtigungen: Informationen zu Projekten in meinem Besitz

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die in einem von Ihnen verwalteten Projekt stattfinden. Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>Ein Dokument wird einem Projekt in meinem Besitz hinzugefügt</strong> </p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn ein Dokument zum Projekt hinzugefügt wird, es sei denn, der Benutzer, der das Dokument hinzugefügt hat, ist auch der Projektbesitzer.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] und das Dokument nicht Privat ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Dokument hinzugefügt zu] &lt;Projektname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> Projektname<br>Portfolio-Name<br>Projekt-Referenznummer<br>Name des Benutzers, der das Dokument hinzugefügt hat<br>Dokumentname<br>Am Datum hinzugefügt<br>Dokumentdetails (Format, Größe, Versionsnummer)<br><strong>[!UICONTROL -Vorschau]</strong> und <strong>[!UICONTROL -Download]</strong> Schaltflächen<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der hinzugefügten Dokumente<br>*Dokumentname<br>*Name des Benutzers, der das Dokument hinzugefügt hat<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Meilensteinaufgabe wurde in einem Projekt abgeschlossen, dessen Besitzer ich bin</strong> </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] oder [!UICONTROL Planning] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Complete]: &lt;Aufgabenname&gt; auf &lt;Projektname&gt;</em></p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, wird im Betreff der E-Mail weiterhin "[!UICONTROL Complete]" angezeigt.</p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenznummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>-Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Projekt, das in meinem Besitz ist, ist in Verzug geraten</strong> </p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn das Projekt in Verzug ist. Ein Projekt ist in Verzug, wenn der Fortschrittsstatus "[!UICONTROL At Risk], "[!UICONTROL Behind]" oder "[!UICONTROL Late]" ist.</p> <p>Es empfiehlt sich, diese Benachrichtigung aktiv zu halten. </p> <p>Benutzende mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Projektfortschrittsänderung]: &lt;Projektname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> <p>Projektname<br>Portfolio-Name<br>Projekt-Referenznummer<br>Projektfortschrittsstatus<br>Projekt [!UICONTROL Geplantes Startdatum]<br>Projekt [!UICONTROL Geplantes Abschlussdatum]<br>Projekt [!UICONTROL Geplantes Startdatum]<br>Projekt [!UICONTROL Geplantes Abschlussdatum]<br>Projekt-Prozentsatz abgeschlossen<br>Projektstatus<br>Projektinhaber<br>*Projektname<br>*Projekt-Referenznummer<br>*Projektfortschrittsstatus<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Problem wird einem Projekt in meinem Besitz hinzugefügt</strong> </p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn ein Problem zum Projekt hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] oder [!UICONTROL Planning] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Problem hinzugefügt zu] &lt;Projektname&gt;</em></p> <p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> <p>Projektname<br>Portfolio-Name<br>Problem-Referenznummer<br>Name des Benutzers, der das Problem hinzugefügt hat<br>Problem-Name<br>Problem-Typ<br>Eingegebenes Datum<br>Problem-Priorität<br>Dem Namen zugewiesen<br>Problemstatus<br>Primärer Kontakt<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der dem Projekt hinzugefügten Probleme<br>*Problem-Name<br>*Name des Benutzers, der das Problem hinzugefügt hat<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Aufgabe wurde in einem Projekt abgeschlossen, dessen Besitzer ich bin</strong> </p> <p>Der Projektbesitzer erhält eine Benachrichtigung, wenn eine Aufgabe für sein Projekt abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Complete]: &lt;Aufgabenname&gt; auf &lt;Projektname&gt;</em></p> <p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, wird im Betreff der E-Mail weiterhin "[!UICONTROL Complete]" angezeigt.</p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenznummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat <br>Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der Aufgaben, die <br> abgeschlossen wurden*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum des täglichen Digest<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Aufgabe aus einem Projekt, dessen Besitzer ich bin, wird erstellt</strong> </p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn eine Aufgabe für das Projekt in Verzug gerät. Eine Aufgabe ist in Verzug, wenn der Fortschrittsstatus "[!UICONTROL At Risk]", "[!UICONTROL Behind]" oder "[!UICONTROL Late]" ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Änderung des Aufgabenstatus]: &lt;Aufgabenname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Referenznummer der Aufgabe<br>Neuer Aufgabenstatus<br>Aufgabe [!UICONTROL Geplantes Startdatum]<br>Aufgabe [!UICONTROL Geplantes Abschlussdatum]<br>Aufgabe [!UICONTROL Geplantes Startdatum]<br>Aufgabe [!UICONTROL Projiziertes Abschlussdatum]<br>Aufgabenprozentsatz<br>Aufgabenstatus<br>Zugeordneter Name<br>Eingegeben nach Name<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der Aufgaben, die sich in Verzug befinden<br> <br>*Aufgabenname<br>*Tag des täglichen Digest </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Problem wurde in einem Projekt abgeschlossen, dessen Besitzer ich bin</strong> </p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn ein Problem in seinem Projekt abgeschlossen wurde.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] oder [!UICONTROL Planning] ist.</p> <p>Benutzende mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung. </p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Complete]: &lt;Issue Name&gt; am &lt;Project Name&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Anfragenstatus<br>Datum und Uhrzeit, zu der das Problem abgeschlossen wurde<br>Vorheriger Anfragenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche <br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der abgeschlossenen Probleme<br>*Anfragename<br>*Name des Benutzers, der dem Problem zugewiesen wurde<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Einem Projekt in meinem Besitz wird eine nicht zugewiesene Anfrage hinzugefügt</strong> </p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn ein nicht zugewiesenes Problem zum Projekt hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] oder [!UICONTROL Planning] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Wer soll diesem neuen Problem zugewiesen werden bei] &lt;Projektname&gt;?</em></p> <p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Digest of Projects You Own &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> <p>Projektname<br>Portfolio-Name<br>Problem-Referenznummer<br>Name des Benutzers, der das Problem hinzugefügt hat<br>Problem-Name<br>Problem-Typ<br>Eingegebenes Datum<br>Problem-Priorität<br>Dem Namen zugewiesen (leer)<br>Problemstatus<br>Primärer Kontakt<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der hinzugefügten Probleme<br>*Problem-Name<br>*Name des Benutzers, der das Problem hinzugefügt hat<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich bin der Besitzer eines neuen Projekts</strong> </p> <p>Wenn ein Benutzer als Eigentümer eines Projekts zugewiesen wird, erhält dieser Benutzer eine E-Mail-Benachrichtigung.</p> <p>Wenn es sich beim Projektbesitzer um denselben Benutzer handelt, der den Arbeitsauftrag erteilt hat, wird keine E-Mail-Benachrichtigung gesendet.</p> <p>Benutzende mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Schalten Sie das an, weil sie etwas zugewiesen werden. </p> <p> Etwas zuweisen, etwas teilen, Zugriff für etwas erhalten.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Sie sind jetzt der Projektbesitzer von] &lt;Projektname&gt;</em></p> <p>Der folgende Text ist im Textkörper der E-Mail-Benachrichtigung enthalten:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;Ihr Name&gt;,<br></em><em>&lt;Name des Benutzers, der Sie als Projektbesitzer zugewiesen hat&gt; [!UICONTROL hat Sie zum Besitzer von] &lt;Projektname&gt; gemacht. [!UICONTROL Als Projektbesitzer erhalten Sie möglicherweise zusätzliche E-Mail-Benachrichtigungen über Projektaktivitäten, werden Sie aufgefordert, Projektstunden zu genehmigen, oder werden Sie an der Genehmigung projektbezogener Arbeiten beteiligt. Es gehört alles dir.]</em> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> <p> </p> </td> 
   <td> <p>Projektname<br>Portfolio-Name<br>Projekt-Referenznummer<br>Projekt-Abschlussdatum<br>*Projektname<br>*Projekt-Referenznummer<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Das Commit-Datum ändert sich für eine Aufgabe in einem meiner Projekte</strong> </p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn sich das Commit-Datum für eine Aufgabe im Projekt ändert, es sei denn, der Benutzer, der das Commit-Datum geändert hat, ist auch der Projektbesitzer.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Commit-Datum für] &lt;Aufgabenname&gt; [!UICONTROL ist jetzt] &lt;Neues Commit-Datum&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Digest of Projects You Own &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> <p>Aufgabenname<br>Projektname<br>Vorgangs-Referenznummer<br>Name des Benutzers, der das Commit-Datum geändert hat<br>Neues Commit-Datum<br>Aufgabe [!UICONTROL Geplantes Abschlussdatum]<br>Informationen darüber, wie sich diese Änderung auf die Projekt-Zeitleiste auswirkt<br>Dem Namen zugewiesen<br>Nach Name eingegeben<br>Projekteigentümer<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>Schaltfläche<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der Aufgaben, deren Commit-Datum geändert wurde<br>*Aufgabenname<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Das Commit-Datum ändert sich für ein Problem in einem meiner Projekte</strong> </p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn sich das Commit-Datum für ein Problem im Projekt ändert, es sei denn, der Benutzer, der das Commit-Datum ändert, ist derselbe Benutzer wie der Projektbesitzer.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Commit-Datum für] &lt;Problemname&gt; [!UICONTROL ist jetzt] &lt;Neues Commit-Datum&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects You Own] &lt;Date of Daily Digest&gt; </em></p> </td> 
   <td> <p>Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der das Commit-Datum geändert hat<br>Neues Commit-Datum<br>Geplantes Abschlussdatum für die Anfrage<br>Zugeordneter Name<br>Von Name eingegeben<br>Projektinhaber<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>-Schaltfläche<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der Anfragen, deren Commit-Datum geändert wurde<br>*Anfragename<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
