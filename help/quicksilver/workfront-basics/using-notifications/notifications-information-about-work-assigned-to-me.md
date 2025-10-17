---
content-type: reference
navigation-topic: notifications
title: 'Benachrichtigungen: Informationen zu meiner Arbeit'
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die in einem Ihnen zugewiesenen Arbeitselement stattfinden.
author: Courtney
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 1%

---

# Benachrichtigungen: Informationen zu meiner Arbeit

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die in einem Ihnen zugewiesenen Arbeitselement stattfinden.

Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Ein Vorgänger einer meinem Team zugewiesenen Aufgabe ist abgeschlossen</strong> </p> <p>Das zugewiesene Team erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben abgeschlossen ist. </p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Abgeschlossen: &lt;Aufgabenname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> <p>Name der Vorgängeraufgabe<br>Vorgängervorgangsprojekt<br>Referenznummer der Vorgängeraufgabe<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit, zu der der Vorgänger abgeschlossen wurde<br>Vorheriger Status der Vorgängeraufgabe<br><strong>Weitere Details anzeigen</strong> button<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der Vorgänger abgeschlossen<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </p> </td> 
   <td><strong>Täglich</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>Wenn eine Aufgabe abgeschlossen ist, die primär zugewiesenen Benutzer aller abhängigen Aufgaben per E-Mail benachrichtigen</strong> </p> <p>Der Aufgabenzugewiesene erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben abgeschlossen ist. </p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Complete]: &lt;Aufgabenname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> <p>Name der Vorgängeraufgabe<br>Vorgängeraufgabe-Projekt<br>Referenznummer der Vorgängeraufgabe<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit, zu der der Vorgänger abgeschlossen wurde<br>Vorheriger Status der Vorgängeraufgabe<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der abgeschlossenen Vorgänger<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </p> </td> 
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
   <td> <p><strong>Eine von mir abgeschlossene Aufgabe wurde genehmigt oder abgelehnt</strong> </p> <p>Der Aufgabenbearbeiter erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe genehmigt oder abgelehnt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Complete]: &lt;Aufgabenname&gt; auf &lt;Projektname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenznummer<br>Name des Benutzers, der die Genehmigung erteilt hat<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit, zu der die Aufgabe genehmigt oder abgelehnt wurde<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der Aufgaben genehmigt oder abgelehnt<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe genehmigt oder abgelehnt hat<br>*Genehmigungsentscheidung ([!UICONTROL genehmigt]/ [!UICONTROL abgelehnt])<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>Eine Aufgabe, der ich zugewiesen bin, wurde abgeschlossen</strong> </p> <p>Der Aufgabenbevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist.</p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Complete]: &lt;Aufgabenname&gt; auf &lt;Projektname&gt;</em></p> <p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, wird im Betreff der E-Mail weiterhin „Complete“ angezeigt.</p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> <p>Aufgabenname<br>Projektname<br>Aufgabenreferenznummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat<br>Datum und Uhrzeit, zu der die Aufgabe abgeschlossen wurde<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum des täglichen Digest<br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>Alle Vorgänger einer meinem Team zugewiesenen Aufgabe sind abgeschlossen</strong> </p> <p>Das zugewiesene Team erhält eine E-Mail-Benachrichtigung, wenn ein Vorgänger einer seiner Aufgaben als „Abgeschlossen“ markiert ist.</p> <p>Benutzende mit einer Prüfungs- oder Antragstellerlizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Aufgabe abgeschlossen: &lt;Name&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Digest of Work Assigned To You &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Aufgabenprojekt<br>Aufgabenreferenznummer<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit, zu der der Vorgänger abgeschlossen wurde<br>Vorheriger Status der Vorgängeraufgabe<br><strong>Weitere Details anzeigen</strong> Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </td>
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
   <td> <p><strong>Alle Vorgänger meiner Aufgaben sind abgeschlossen</strong> </p> <p>Der Aufgabenempfänger erhält für jeden abgeschlossenen Vorgänger eine E-Mail-Benachrichtigung.</p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Complete]: &lt;Aufgabenname&gt;</em><br></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Aufgabe Projekt<br>Aufgabenreferenznummer<br>Name des Benutzers, der die Vorgängeraufgabe abgeschlossen hat<br>Status der Vorgängeraufgabe<br>Datum und Uhrzeit des Abschlusses des Vorgängers<br>Vorheriger Status der Vorgängeraufgabe<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>-Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </td> 
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
   <td> <p><strong>Ein von mir bearbeitetes Problem wurde genehmigt oder abgelehnt</strong> </p> <p>Der Verantwortliche für ein Problem erhält eine E-Mail-Benachrichtigung, wenn eine Genehmigungsentscheidung getroffen (genehmigt oder abgelehnt) wird.</p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>Problem mit ausstehender Genehmigung: &lt;geplantes Startdatum&gt; &lt;Problem-Referenznummer&gt; - &lt;Problem-Name&gt; in &lt;Projektname&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Digest of Work Assigned To You &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der das Problem genehmigt oder abgelehnt hat<br>Genehmigungsentscheidung (genehmigt oder abgelehnt)<br>Anfragenstatus<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der genehmigten oder abgelehnten Probleme<br>*Anfragename<br>*Name des Benutzers, der das Problem genehmigt oder abgelehnt hat<br>*Genehmigungsentscheidung (genehmigt oder abgelehnt)<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>Ein Problem, dem ich zugewiesen bin, wurde abgeschlossen</strong> </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] oder [!UICONTROL Planning] ist.</p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Abgeschlossen: &lt;Problemname&gt; auf &lt;Projektname&gt;</em></p> <p><em> Der Betreff der täglichen Digest-Benachrichtigung ist: Zusammenfassung der Ihnen zugewiesenen Arbeit &lt;Datum der täglichen Digest&gt; </em> </p> </td> 
   <td> Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Neuer Anfragestatus<br>Datum und Uhrzeit des Abschlusses des Problems<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>-Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der abgeschlossenen Probleme<br>*Anfragename<br>*Name des Benutzers, der das Problem abgeschlossen hat<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dokumente zu Anfragen, denen ich zugewiesen bin, werden hochgeladen oder geändert</strong> </p> <p>Der Problembearbeiter erhält eine E-Mail-Benachrichtigung, wenn Dokumente hochgeladen oder Dokumentdetails zu einem von ihm hinzugefügten Problem geändert werden.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn die Person, die das Problem ausgelöst hat, die Person ist, die das Problem zugewiesen hat.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] ist und wenn das Projekt als eine Hilfe-Anfrage-Warteschlange eingerichtet ist (wie in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anfrage-Warteschlange</a> beschrieben).</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Dokument hinzugefügt zu] &lt;Name der Anfrage&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> <p>Anfragename<br>Projektname (Name der Anfragewarteschlange)<br>Dokumentreferenz <br>Name des Benutzers, der das Dokument hochgeladen hat<br>Dokumentname <br>Am Datum hinzugefügt<br>Dokumentdetails (Format, Größe, Versionsnummer)<br>Dokumentminiatur<br><strong>[!UICONTROL -Vorschau]</strong> und <strong>[!UICONTROL -Download]</strong> Schaltflächen<br>*Projektname<br>*Projektreferenz<br>*Gesamtzahl der hochgeladenen oder geänderten Dokumente<br>*Dokumentname<br>*Objektname<br>*Name des Benutzers, der das Dokument hochgeladen hat<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Den zugewiesenen Benutzer per E-Mail benachrichtigen, wenn sich das geplante Abschlussdatum der Aufgabe ändert</strong> </p> <p>Der Aufgabenbevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn sich das geplante Abschlussdatum der Aufgabe (Geplant) ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Aufgabenbevollmächtigte.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus nicht [!UICONTROL Planning] ist.</p> <p>Es wird keine Benachrichtigung bezüglich persönlicher Aufgaben gesendet.</p> <p> Benutzende mit einer Prüfungs- oder Antragstellerlizenz erhalten keine Benachrichtigung. </p> <p> Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Fälligkeitsdatum wurde geändert.]</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenznummer<br>Neues Fälligkeitsdatum ([!UICONTROL Geplantes Abschlussdatum])<br>Datum und Uhrzeit der Änderung des Fälligkeitsdatums<br>Der Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der Aufgaben, bei denen sich das Fälligkeitsdatum (Geplantes Abschlussdatum) geändert hat<br>*Aufgabenname<br>*Neues geplantes Abschlussdatum<br>*Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Das Fälligkeitsdatum eines Problems, dem ich zugewiesen bin, ändert sich</strong> </p> <p>Der Problembevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn sich das geplante Abschlussdatum von  ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum von  geändert hat, ist auch der Bevollmächtigte.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus nicht [!UICONTROL Planning] ist.</p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>[!UICONTROL Fälligkeitsdatum wurde geändert]</em></p> <p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of Daily Digest&gt;</em></p> </td> 
   <td> <p>Anfragename<br>Projektname<br>Anfragenummer<br>Neues Fälligkeitsdatum ([!UICONTROL Geplantes Abschlussdatum])<br>Datum und Uhrzeit, an dem das Fälligkeitsdatum geändert wurde<br>Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der Probleme, an denen sich das Fälligkeitsdatum ([!UICONTROL Geplantes Abschlussdatum]) geändert hat<br>*Anfragename<br>*Neues [!UICONTROL Geplantes Abschlussdatum]<br>*Name des Benutzers, der das Fälligkeitsdatum geändert hat<br>*der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Der Status einer mir zugewiesenen Aufgabe ändert sich</strong> <p>Der Aufgabenbevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn sich der Status der Aufgabe ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Bevollmächtigte.</p> <p>Hinweis: Diese Benachrichtigung wird nicht gesendet, wenn sich der Aufgabenstatus in „Abgeschlossen“ ändert. Für abgeschlossene Aufgaben wird eine separate Benachrichtigung verwendet. Siehe <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">Eine Aufgabe, der ich zugewiesen bin, wurde abgeschlossen</a> oben.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist.</p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>&lt;Aufgabenname&gt; von &lt;Projektname&gt; ist &lt;Neuer Status&gt;</em></p> <p> </p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenznummer<br>Name des Benutzers, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit, zu der der Status geändert wurde<br>Vorschaustatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der Aufgaben, bei denen der Status geändert wurde<br>*Aufgabenname<br>*Vorheriger Aufgabenstatus<br>*Neuer Aufgabenstatus<br>*Name des Benutzers, der den Status geändert hat<br>*Datum des täglichen Digest<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Der Status eines meiner Arbeitselemente ändert sich</strong> </p> <p>Sie erhalten eine E-Mail-Benachrichtigung, wenn sich der Status eines Problems ändert, dem Sie zugewiesen sind, es sei denn, Sie ändern den Status selbst. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist.</p> <p>Benutzende mit einer [!UICONTROL Review]- oder [!UICONTROL Requestor]-Lizenz erhalten keine Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>&lt;Name des Problems&gt; von &lt;Projektname&gt; ist &lt;Neuer Status&gt;</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Work Assigned To You] &lt;Date of daily Digest&gt; </em></p> </td> 
   <td> Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit, zu der der Status geändert wurde<br>Vorheriger Anfragenstatus<br><strong>Weitere Details anzeigen</strong> Schaltfläche<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der Probleme, bei denen der Status geändert wurde<br>*Aufgabenname<br>*Vorheriger Anfragenstatus<br>*Neuer Anfragenstatus<br>*Name des Benutzers, der den Status geändert hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
 </tbody> 
</table>
