---
content-type: reference
navigation-topic: notifications
title: '''Benachrichtigungen: Informationen über die Arbeit, die mir zugewiesen wurde'
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die mit einem Ihnen zugewiesenen Arbeitselement stattfinden.
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 39ba9e93a8597d4354472a19b1ac1c5f530f4398
workflow-type: tm+mt
source-wordcount: '2092'
ht-degree: 6%

---

# Benachrichtigungen: Informationen über die mir zugewiesene Arbeit

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die mit einem Ihnen zugewiesenen Arbeitselement stattfinden.

Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th> <p>Einbezogene Felder </p> <p> *Nur täglich Digest-Felder</p> </th> 
   <th>Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>Eine Vorgängeraufgabe für eine meinem Team zugewiesene Aufgabe ist abgeschlossen.</strong> </p> <p>Das zugewiesene Team erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben abgeschlossen ist. </p> <p>Benutzer mit der Lizenz [!UICONTROL Review] oder Re[!UICONTROL Antragsteller]questor erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Abgeschlossen: &lt;task name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Vorgänger-Aufgabenname<br>Vorgänger-Task-Projekt<br>Referenz zur Vorgängeraufgabe<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit der Fertigstellung des Vorgängers<br>Vorheriger Status der Vorgängeraufgabe<br><strong>Siehe Weitere Details</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Vorgänger<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </p> </td> 
   <td><strong>Täglich</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Wenn eine Aufgabe abgeschlossen ist, die primär zugewiesenen Benutzer aller abhängigen Aufgaben per E-Mail benachrichtigen.</strong> </p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben abgeschlossen ist. </p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Vorgänger-Aufgabenname<br>Vorgänger-Task-Projekt<br>Referenz zur Vorgängeraufgabe<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit der Fertigstellung des Vorgängers<br>Vorheriger Status der Vorgängeraufgabe<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Vorgänger<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </p> </td> 
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
   <td> <p><strong>Wenn eine Genehmigungsaufgabe genehmigt oder abgelehnt wird, den zugewiesenen Benutzer per E-Mail benachrichtigen</strong> </p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe genehmigt oder abgelehnt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Name des Benutzers, der die Genehmigung erteilt hat<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit der Validierung oder Zurückweisung der Aufgabe<br>Status der vorherigen Aufgabe<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der genehmigten oder abgelehnten Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe genehmigt oder abgelehnt hat<br>*Genehmigungsentscheidung ([!UICONTROL Genehmigt]/ [!UICONTROL Abgelehnt])<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Nach Abschluss einer Aufgabe den zugewiesenen Benutzer per E-Mail benachrichtigen</strong> </p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, wird im Betreff der E-Mail weiterhin "Complete"angezeigt.</p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Status der vorherigen Aufgabe<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Alle Vorgängeraufgaben für eine meinem Team zugewiesene Aufgabe sind abgeschlossen.</strong> </p> <p>Das zugewiesene Team erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben als abgeschlossen markiert wurde.</p> <p>Benutzer mit der Lizenz "Review"oder "Anforderer"erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Aufgabe abgeschlossen: &lt;name&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> Ihnen zugewiesener Arbeitstitel &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aufgabenname<br>Aufgabenprojekt<br>Aufgabenverweisnummer<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit der Fertigstellung des Vorgängers<br>Vorheriger Status der Vorgängeraufgabe<br><strong>Siehe Weitere Details</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </td>
   <td><strong>Sofort</strong> </td> 
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
   <td> <p><strong>Wenn alle Vorgängeraufgaben komplett abgeschlossen sind, allen primär zugewiesenen Benutzern aller abhängigen Aufgaben eine E-Mail senden.</strong> </p> <p>Der Aufgabenverantwortliche erhält für jeden abgeschlossenen Vorgänger eine E-Mail-Benachrichtigung.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;task name=""&gt;</em><br></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aufgabenname<br>Aufgabenprojekt<br>Aufgabenverweisnummer<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit der Fertigstellung des Vorgängers<br>Vorheriger Status der Vorgängeraufgabe<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Sofort</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>Eine von mir bearbeitete Anfrage wurde genehmigt oder abgelehnt</strong> </p> <p>Der Verantwortliche eines Problems erhält eine E-Mail-Benachrichtigung, wenn eine Genehmigungsentscheidung getroffen (genehmigt oder abgelehnt) wird.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Problem ausstehend Genehmigung: &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; in &lt;project name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> Ihnen zugewiesener Arbeitstitel &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Problemname<br>Projektname<br>Problemverweisnummer<br>Name des Benutzers, der das Problem genehmigt oder abgelehnt hat<br>Genehmigungsentscheidung (genehmigt oder abgelehnt)<br>Problemstatus<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der genehmigten oder abgelehnten Probleme<br>*Name des Problems<br>*Name des Benutzers, der das Problem genehmigt oder abgelehnt hat<br>*Genehmigungsentscheidung (genehmigt oder abgelehnt)<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Den zugewiesenen Benutzer per E-Mail benachrichtigen, sobald die Bearbeitung einer Anfrage abgeschlossen ist.</strong> </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Abgeschlossen: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p><em> Betreff der täglichen Digest-Benachrichtigung ist: Ihnen zugewiesener Arbeitstitel &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> Problemname<br>Projektname<br>Problemverweisnummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Status eines neuen Problems<br>Datum und Uhrzeit des Abschlusses des Problems<br>Status der vorherigen Aufgabe<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Probleme<br>*Name des Problems<br>*Name des Benutzers, der das Problem abgeschlossen hat<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dokumente zu meiner Anfrage werden hochgeladen oder geändert</strong> </p> <p>Der Problemverantwortliche erhält eine E-Mail-Benachrichtigung, wenn Dokumente hochgeladen werden oder Dokumentdetails zu einem von ihm hinzugefügten Problem geändert werden.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn der Benutzer, der das Problem ausgelöst hat, der Problemverantwortliche ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet und das Projekt als Warteschlange für Hilfeanfragen eingerichtet ist (siehe <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a>).</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Dokument hinzugefügt zu] &lt;request name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Anforderungsname<br>Projektname (Name der Anforderungswarteschlange)<br>Dokumentenverweisnummer <br>Name des Benutzers, der das Dokument hochgeladen hat<br>Dokumentname <br>Datum hinzugefügt<br>Dokumentdetails (Format, Größe, Versionsnummer)<br>Dokumentminiatur<br><strong>[!UICONTROL Vorschau]</strong> und <strong>[!UICONTROL Download]</strong> Schaltflächen<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der hochgeladenen oder geänderten Dokumente<br>*Dokumentname<br>*Objektname<br>*Name des Benutzers, der das Dokument hochgeladen hat<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Den zugewiesenen Benutzer per E-Mail benachrichtigen, wenn sich das geplante Abschlussdatum der Aufgabe ändert</strong> </p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich das geplante Abschlussdatum der Aufgabe ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Aufgabenverantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus etwas Anderes als die [!UICONTROL Planung] ist.</p> <p>Was persönliche Aufgaben betrifft, so wird keine Benachrichtigung gesendet.</p> <p> Benutzer mit der Lizenz "Review"oder "Anforderer"erhalten keine Benachrichtigung. </p> <p> Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Das Fälligkeitsdatum von [!UICONTROL wurde geändert.]</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Neues Fälligkeitsdatum ([!UICONTROL Geplantes Abschlussdatum])<br>Datum und Uhrzeit der Änderung des Fälligkeitsdatums<br>Der Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der Aufgaben, bei denen sich das Fälligkeitsdatum (geplantes Abschlussdatum) geändert hat<br>*Aufgabenname<br>*Neues geplantes Abschlussdatum<br>*Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Den zugewiesenen Benutzer per E-Mail informieren, wenn sich das geplante Abschlussdatum einer Anfrage ändert</strong> </p> <p>Der Problemverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich das geplante [!UICONTROL Abschlussdatum] ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Verantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus etwas Anderes als die [!UICONTROL Planung] ist.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Fälligkeitsdatum wurde geändert]</em></p> <p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemverweisnummer<br>Neues Fälligkeitsdatum ([!UICONTROL Geplantes Abschlussdatum])<br>Datum und Uhrzeit der Änderung des Fälligkeitsdatums<br>Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der Probleme, bei denen sich das Fälligkeitsdatum ([!UICONTROL Planes Abschlussdatum]) geändert hat<br>*Name des Problems<br>*Neues [!UICONTROL Geplantes Abschlussdatum]<br>*Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Der Status einer Aufgabe, der ich zugeteilt bin, ändert sich.</strong> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich der Status der Aufgabe ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Verantwortliche.</p> <p>Hinweis: Diese Benachrichtigung wird nicht gesendet, wenn sich der Aufgabenstatus zu "complete"ändert. Für abgeschlossene Aufgaben wird eine separate Benachrichtigung verwendet. Siehe <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Eine Aufgabe, der ich zugewiesen bin, ist abgeschlossen.</a>, weiter oben.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>&lt;task name=""&gt; von &lt;project name=""&gt; is &lt;new status=""&gt;</em></p> <p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Name des Benutzers, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit der Statusänderung<br>Vorschaustatus<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der Aufgaben, bei denen der Status geändert wurde<br>*Aufgabenname<br>*Status der vorherigen Aufgabe<br>*Neuer Aufgabenstatus<br>*Name des Benutzers, der den Status geändert hat<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>[!UICONTROL Täglich]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Die Statusänderungen eines meiner Arbeitselemente</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn sich der Status in einem Problem ändert, dem Sie zugewiesen sind, es sei denn, Sie ändern den Status selbst. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review] - oder [!UICONTROL Antragsteller] -Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>&lt;issue name=""&gt; von &lt;project name=""&gt; is &lt;new status=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Arbeitstitel für Sie] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Problemname<br>Projektname<br>Problemverweisnummer<br>Name des Benutzers, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit der Statusänderung<br>Status des vorherigen Problems<br><strong>Siehe Weitere Details</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der Probleme, bei denen sich der Status geändert hat<br>*Aufgabenname<br>*Status des vorherigen Problems<br>*Status eines neuen Problems<br>*Name des Benutzers, der den Status geändert hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
 </tbody> 
</table>
