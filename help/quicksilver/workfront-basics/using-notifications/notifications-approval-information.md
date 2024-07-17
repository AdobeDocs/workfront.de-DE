---
content-type: reference
navigation-topic: notifications
title: 'Benachrichtigungen: Validierungsinformationen'
description: Die folgenden Benachrichtigungen informieren Sie über Validierungsaktivitäten für ein Arbeitselement, mit dem Sie befasst sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter Ändern Ihrer eigenen E-Mail-Benachrichtigungen.
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Benachrichtigungen: Validierungsinformationen

Die folgenden Benachrichtigungen informieren Sie über Validierungsaktivitäten für ein Arbeitselement, mit dem Sie befasst sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Eine Anfrage zur Genehmigung eines delegierten Problems ist abgeschlossen</strong> </p> <p>Eine an einen anderen Benutzer delegierte Problemgenehmigung wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Issue Approval/Rejection Made in your own by] &lt;Benutzername&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Approval Information] &lt;Datum des täglichen Digest&gt;</em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Benutzers, der das Problem in Ihrem Namen genehmigt/abgelehnt hat<br>Genehmigungsentscheidung<br>Problemstatus<br>Name des Benutzers, der die Genehmigung beantragt hat<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche<br>*Projektverweisnummer<br>*Projektname<br>*Gesamtzahl der delegierten Ausgabengenehmigungen<br>*Name des Problems<br>*Name des Genehmigers<br>*Datum des täglichen Digest<br><br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine delegierte Projektgenehmigungsanforderung ist abgeschlossen</strong> </p> <p>Eine Projektgenehmigung, die Sie einem anderen Benutzer zugewiesen haben, wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Projektbestätigung/ Zurückweisung in Ihrem Namen durch] &lt;Benutzername&gt;</em></p> <p><em>Betreff der täglichen Digest-Benachrichtigung ist: [!UICONTROL Digest of Approval Information] &lt;Datum des täglichen Digest&gt;</em> </p> </td> 
   <td> Projektname<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Project Reference Number]<br>Name des Benutzers, der das Projekt in Ihrem Namen genehmigt/abgelehnt hat<br>[!UICONTROL Approval Decision]<br>[!UICONTROL Project Status]<br>Name des , der die Genehmigung angefordert hat<br><strong>[!UICONTROL Siehe Weitere Informationen]</strong> Schaltfläche<br>}*Projektname<br>*Genehmigername<br>[!UICONTROL *Datum des täglichen Digest]<br><br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Anfrage zur Genehmigung delegierter Aufgaben ist abgeschlossen</strong> </p> <p>Eine Aufgabengenehmigung, die Sie einem anderen Benutzer zugewiesen haben, wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Task Approval/ Rejection Made in your own by] &lt;Benutzername&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Approval Information] &lt;Datum des täglichen Digest&gt;</em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenz-Nummer<br>Name des Benutzers, der die Aufgabe in Ihrem Namen genehmigt/abgelehnt hat<br>Genehmigungsentscheidung<br>Aufgabenstatus<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>Siehe Mehr Details</strong> Schaltfläche<br>*Projektreferenz-Nummer<br>*Projektname<br>*Gesamtzahl der delegierten Aufgabengenehmigungen<br>*Aufgabenname<br> Name des Genehmigers<br>*Datum des täglichen Digest<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Anforderung zur Dokumentgenehmigung wird abgebrochen</strong> </p> <p>Der Dokumentenvalidierer des Dokuments erhält eine E-Mail-Benachrichtigung, wenn die Anforderung der Dokumentgenehmigung abgebrochen wird.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>&lt;Benutzername&gt; [!UICONTROL hat die Anforderung der Dokumentgenehmigung abgebrochen]</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </p> </td> 
   <td> Name des Benutzers, der die Genehmigungsanforderung abgebrochen hat<br>[!UICONTROL Dokumentname] </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich werde als Genehmiger delegiert</strong> </p> <p>Wenn Ihnen jemand eine Validierung zugewiesen hat, erhalten Sie eine E-Mail-Benachrichtigung. </p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Delegierter] &lt;Objekttyp&gt; [!UICONTROL Genehmigung - Bitte überprüfen] &lt;Objektname&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </p> </td> 
   <td> <p>[!UICONTROL Objektname]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>Name des Benutzers, der das Objekt zur Genehmigung gesendet hat<br>Name des Benutzers, für den Sie das Objekt genehmigen,<br>Objektstatus<br>Datum und Uhrzeit der Anforderung der Genehmigung<br>Objektpriorität<br>Genehmigungsschrittname<br>[!UICONTROL Planen Abschlussdatum] der Schaltfläche "Objekt<br><strong>[!UICONTROL Genehmigungsentscheidung treffen]</strong>"</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Mein Timesheet ist genehmigt</strong> </p> <p>Wenn Ihr Timesheet validiert wurde, erhalten Sie eine E-Mail-Benachrichtigung.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Timesheet Genehmigt]: &lt;Startdatum des Datenblatts&gt; - &lt;Enddatum des Datenblatts&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </p> </td> 
   <td> Name des Benutzers, der Ihr Datenblatt validiert hat<br>Datum und Uhrzeit der Validierung des Datenblatts<br>Status des Datenblatts ([!UICONTROL Genehmigt])<br>Startdatum und Enddatum des Datenblatts<br>Gesamtstunden, die im Datenblatt protokolliert sind<br>Überstunden, die im Datenblatt protokolliert sind </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
