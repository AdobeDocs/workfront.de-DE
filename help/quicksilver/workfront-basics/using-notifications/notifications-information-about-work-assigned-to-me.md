---
content-type: reference
navigation-topic: notifications
title: "Benachrichtigungen: Informationen über die mir zugewiesenen Aufgaben"
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die mit einem Ihnen zugewiesenen Arbeitselement stattfinden.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 1%

---

# Benachrichtigungen: Informationen über die mir zugewiesenen Aufgaben

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die mit einem Ihnen zugewiesenen Arbeitselement stattfinden.

Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Ein Vorgänger einer Aufgabe, die meinem Team zugewiesen wurde, ist abgeschlossen</strong> </p> <p>Das zugewiesene Team erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben abgeschlossen ist. </p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>Abgeschlossen: &lt;Aufgabenname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Name der Vorgänger-Aufgabe <br>Vorläufer-Aufgabenprojekt<br>Vorläufer-Aufgabenreferenz Nummer<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit, zu der der Vorgänger abgeschlossen wurde<br>Vorheriger Status der Vorgängeraufgabe<br><strong>Siehe Schaltfläche Weitere Informationen</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br> Gesamtzahl der abgeschlossenen Vorgänger<br>*Task Name<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum des täglichen Digest </p> </td> 
   <td><strong>Täglich</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Wenn eine Aufgabe abgeschlossen ist, die primär zugewiesenen Benutzer aller abhängigen Aufgaben per E-Mail benachrichtigen</strong> </p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben abgeschlossen ist. </p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;Task Name&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Name der Vorgänger-Aufgabe <br>Vorgänger-Aufgabenprojekt<br>Vorgänger-Aufgabenreferenz Nummer<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit, zu der der Vorgänger abgeschlossen wurde<br>Vorheriger Status der Vorgängeraufgabe<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche<br>*Projektname<br> Projektnummer<br>*Gesamtzahl der abgeschlossenen Vorgänger<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>Eine Aufgabe, die ich abgeschlossen habe, wird genehmigt oder abgelehnt</strong> </p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe genehmigt oder abgelehnt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;Task Name&gt; unter &lt;Projektname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Name des Benutzers, der die Genehmigung erteilt hat<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit der Genehmigung oder Ablehnung der Aufgabe<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br>*Gesamtzahl der genehmigten oder abgelehnten Aufgaben<br><br>*Name des Benutzers, der die Aufgabe genehmigt oder abgelehnt hat<br>*Genehmigungsentscheidung ([!UICONTROL Genehmigt]/ [!UICONTROL Abgelehnt])<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Eine Aufgabe, der ich zugewiesen bin, ist abgeschlossen</strong> </p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;Task Name&gt; unter &lt;Projektname&gt;</em></p> <p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, wird im Betreff der E-Mail weiterhin "Complete"angezeigt.</p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Weitere Informationen]</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers Aufgabe<br>*Datum des täglichen Digest<br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Alle Vorgänger einer Aufgabe, die meinem Team zugewiesen ist, sind abgeschlossen</strong> </p> <p>Das zugewiesene Team erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben als abgeschlossen markiert wurde.</p> <p>Benutzer mit der Lizenz "Review"oder "Anforderer"erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>Aufgabe abgeschlossen: &lt;Name&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Arbeitstitel zugewiesen an Sie &lt;Datum des täglichen Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Task Project<br>Task Reference Number<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit des Abschlusses des Vorgängers<br>Vorheriger Status der Vorgängeraufgabe<br><strong>Siehe Mehr Details</strong> button<br>*Projektname<br>*Projektnummer<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum des täglichen Digest </td>
   <td><strong>Instant</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Alle Vorgänger meiner Aufgaben sind abgeschlossen</strong> </p> <p>Der Aufgabenverantwortliche erhält für jeden abgeschlossenen Vorgänger eine E-Mail-Benachrichtigung.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;Task Name&gt;</em><br></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Aufgabenprojekt<br>Aufgabenreferenz-Nummer<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit des Abschlusses des Vorgängers<br>Vorheriger Status der Vorgängeraufgabe<br><strong>[!UICONTROL Siehe Weitere Informationen]</strong> button<br>*Projektname<br>*Projektnummer<br> Gesamtzahl Aufgaben abgeschlossen<br>*Task Name<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum des täglichen Digest </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Ein von mir gelöstes Problem wird genehmigt oder abgelehnt</strong> </p> <p>Der Verantwortliche eines Problems erhält eine E-Mail-Benachrichtigung, wenn eine Genehmigungsentscheidung getroffen (genehmigt oder abgelehnt) wird.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit der sofortigen Benachrichtigung ist: <em>Problem ausstehend Genehmigung: &lt;Geplantes Startdatum&gt; &lt;Referenznummer des Problems&gt; - &lt;Name des Problems&gt; in &lt;Projektname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Arbeitstitel zugewiesen an Sie &lt;Datum des täglichen Digest&gt; </em></p> </td> 
   <td> Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Benutzers, der das Problem genehmigt oder abgelehnt hat<br>Genehmigungsentscheidung (genehmigt oder abgelehnt)<br>Problemstatus<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>[!UICONTROL Siehe Mehr Details]</strong> Schaltfläche<br>*Projektname<br>*Projektverweisnummer<br>*Gesamtzahl der genehmigten oder abgelehnten Probleme 11}*Problemname<br>*Name des Benutzers, der das Problem genehmigt oder abgelehnt hat<br>*Genehmigungsentscheidung (genehmigt oder abgelehnt)<br>*Datum des täglichen Digest<br><br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Ein Problem, dem ich zugewiesen bin, ist abgeschlossen</strong> </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>Abgeschlossen: &lt;Name des Problems&gt; unter &lt;Projektname&gt;</em></p> <p><em> Der Betreff der täglichen Digest-Benachrichtigung lautet: Digest of Work Assigned to You &lt;Datum der täglichen Digest&gt; </em> </p> </td> 
   <td> Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Neuer Problemstatus<br>Datum und Uhrzeit, zu dem das Problem abgeschlossen wurde<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br>*Gesamtzahl der abgeschlossenen Probleme<br>*Problemname 12}*Name des Benutzers, der das Problem abgeschlossen hat<br>*Datum des täglichen Digest<br><br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dokumente werden bei Anforderungen, denen ich zugewiesen bin, hochgeladen oder geändert.</strong> </p> <p>Der Problemverantwortliche erhält eine E-Mail-Benachrichtigung, wenn Dokumente hochgeladen werden oder Dokumentdetails zu einem von ihm hinzugefügten Problem geändert werden.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn der Benutzer, der das Problem ausgelöst hat, der Problemverantwortliche ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet und das Projekt als Warteschlange für Hilfeanfragen eingerichtet ist (wie in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Anforderungswarteschlange erstellen</a> beschrieben).</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Dokument hinzugefügt zu] &lt;Anforderungsname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> <p>Anforderungsname<br>Projektname (Name der Anforderungswarteschlange)<br>Referenznummer des Dokuments <br>Name des Benutzers, der das Dokument hochgeladen hat<br>Dokumentname <br>Hinzugefügt am Datum<br>Dokumentdetails (Format, Größe, Versionsnummer)<br>Dokumentminiatur<br><strong>[!UICONTROL Vorschau]</strong> und <strong>[!UICONTROL Download]</strong> Schaltflächen Projektname<br>*Projektnummer<br>*Gesamtanzahl der hochgeladenen oder geänderten Dokumente<br>*Dokumentname<br>*Objektname<br>*Name des Benutzers, der das Dokument hochgeladen hat<br>*Datum des täglichen Digest<br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Den zugewiesenen Benutzer per E-Mail benachrichtigen, wenn sich das geplante Abschlussdatum der Aufgabe ändert</strong> </p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich das geplante Abschlussdatum der Aufgabe ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Aufgabenverantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus etwas Anderes als die [!UICONTROL Planung] ist.</p> <p>Was persönliche Aufgaben betrifft, so wird keine Benachrichtigung gesendet.</p> <p> Benutzer mit der Lizenz "Review"oder "Anforderer"erhalten keine Benachrichtigung. </p> <p> Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Fälligkeitsdatum wurde geändert.]</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Neues Fälligkeitsdatum ([!UICONTROL Planes Abschlussdatum])<br>Datum und Uhrzeit der Änderung des Fälligkeitsdatums<br>Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Projektname<br>*Projektnummer<br>*Gesamtanzahl der Aufgaben, bei denen das Fälligkeitsdatum geändert wurde<br> Aufgabenname}*Neues geplantes Abschlussdatum<br>*Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Datum des täglichen Digest<br> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und Täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Das Fälligkeitsdatum ändert sich in Bezug auf ein Problem, dem ich zugewiesen bin.</strong> </p> <p>Der Problemverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich das geplante [!UICONTROL Abschlussdatum] ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Verantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus etwas Anderes als die [!UICONTROL Planung] ist.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Fälligkeitsdatum wurde geändert]</em></p> <p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Zusammenfassung&gt;</em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Bezugsnummer des Problems<br>Neues Fälligkeitsdatum ([!UICONTROL Plantes Abschlussdatum])<br>Datum und Uhrzeit der Änderung des Fälligkeitsdatums<br>Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Projektname<br>*Referenznummer des Projekts<br>*Gesamtzahl der Probleme, bei denen das Fälligkeitsdatum geändert wurde ([!UICONTROL Geplantes Abschlussdatum])<br>*Name des Problems<br>*Neu [!UICONTROL Geplantes Abschlussdatum]<br>*Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Datum des täglichen Digest<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und Täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Der Status ändert sich bei einer Aufgabe, der ich zugewiesen bin, für </strong> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich der Status der Aufgabe ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Verantwortliche.</p> <p>Hinweis: Diese Benachrichtigung wird nicht gesendet, wenn sich der Aufgabenstatus zu Ende ändert. Für abgeschlossene Aufgaben wird eine separate Benachrichtigung verwendet. Siehe <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Eine Aufgabe, der ich zugewiesen bin, ist abgeschlossen</a> oben.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der E-Mail mit der sofortigen Benachrichtigung lautet: <em>&lt;Aufgabenname&gt; von &lt;Projektname&gt; ist &lt;neuer Status&gt;</em></p> <p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Name des Benutzers, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit der Statusänderung<br>Vorschaustatus<br><strong>[!UICONTROL Weitere Informationen]</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br>*Gesamtanzahl der Aufgaben, bei denen der Status geändert wurde<br>*Aufgabenname<br> 2}*Vorheriger Aufgabenstatus<br>*Neuer Aufgabenstatus<br>*Name des Benutzers, der den Status geändert hat<br>*Datum des täglichen Digest<br></td> 
   <td><strong>[!UICONTROL Täglich]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Der Status ändert sich für eines meiner Arbeitselemente</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn sich der Status in einem Problem ändert, dem Sie zugewiesen sind, es sei denn, Sie ändern den Status selbst. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>&lt;Name des Problems&gt; von &lt;Projektname&gt; ist &lt;neuer Status&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Datum der täglichen Digest&gt; </em></p> </td> 
   <td> Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Benutzers, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit der Statusänderung<br>Vorheriger Problemstatus<br><strong>Siehe Weitere Informationen</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br>*Gesamtzahl der Probleme, bei denen der Status geändert wurde<br>*Aufgabenname<br>*Status des vorherigen Problems<br>*Status des neuen Problems<br>*Name des Benutzers, der den Status geändert hat<br>*Datum des täglichen Digest </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
 </tbody> 
</table>
