---
content-type: reference
navigation-topic: notifications
title: 'Benachrichtigungen: Einheitliche Genehmigungen'
description: Die folgenden Benachrichtigungen informieren Sie über Genehmigungsaktivitäten für das Erlebnis „Einheitliche Genehmigungen“. Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter Ändern Ihrer eigenen E-Mail-Benachrichtigungen .
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 7957c410d4a0e39b23b4f5a3d29a794e5deec72a
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%
---
# Benachrichtigungen: Einheitliche Genehmigungen

{{highlighted-preview}}

Verwenden Sie die folgenden Benachrichtigungen, um über Aktivitäten für einheitliche Überprüfungen und Genehmigungen auf dem Laufenden zu bleiben. Informationen zum Konfigurieren der E-Mail-Benachrichtigungen, die Sie erhalten, finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Diese Benachrichtigungen sind nur als Sofortbenachrichtigungen verfügbar und nicht in einer täglichen Zusammenfassung.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Benachrichtigung</th> 
   <th>Enthaltene Felder</th> 
   <th>Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Genehmigung abgeschlossen - Genehmigt</strong> </p> <p>Eine Dokumentengenehmigung endet mit der endgültigen Entscheidung Genehmigt .</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Endgültige Entscheidung: (Dokument) wurde genehmigt</em></p> </td> 
   <td> <p>Endgültige Entscheidung<br>Dokument<br>Genehmigung angefordertes Datum<br>Fälligkeitsdatum<br> Schaltfläche „Zur Überprüfung gehen“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Genehmigung abgeschlossen - Mit Änderungen genehmigt</strong> </p> <p>Eine Dokumentengenehmigung endet mit der endgültigen Entscheidung Genehmigt mit Änderungen.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Endgültige Entscheidung: (Dokument) wird mit Änderungen genehmigt</em></p> </td> 
   <td> <p>Endgültige Entscheidung<br>Dokument<br>Genehmigung angefordertes Datum<br>Fälligkeitsdatum<br> Schaltfläche „Zur Überprüfung gehen“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Genehmigung abgeschlossen - Muss überarbeitet werden</strong> </p> <p>Eine Dokumentengenehmigung endet mit der endgültigen Entscheidung: „Überarbeitung erforderlich“.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Endgültige Entscheidung: (Dokument) Muss bearbeitet werden</em></p> </td> 
   <td> <p>Endgültige Entscheidung<br>Dokument<br>Genehmigung angefordertes Datum<br>Fälligkeitsdatum<br> Schaltfläche „Zur Überprüfung gehen“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Frist nähert sich</strong> </p> <p>Die Frist für eine Dokumentgenehmigung, der Sie angehören, nähert sich.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>Die Validierungsfrist nähert sich dem (Dokument)</em></p> </td> 
   <td> <p>Anforderer<br>Ihre Rolle<br>Team<br>Genehmigung angefordertes Datum<br>Fälligkeitsdatum<br> Schaltfläche „Zur Überprüfung gehen“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Deadline passed</strong> </p> <p>Eine Dokumentengenehmigung, der Sie angehören, verstreicht ihre Frist ohne eine endgültige Entscheidung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Genehmigungsfrist für (Dokument) abgelaufen</em></p> </td> 
   <td> <p>Behobenes <br>: Anforderungsdatum/<br>: Schaltfläche <br>Zur Überprüfung wechseln<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Enthalten, wenn Teil der Genehmigungsphase:</em><br>Staging</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Überprüfung abgeschlossen</strong> </p> <p>Ein Reviewer schließt die Überprüfung bei einer Dokumentgenehmigung ab.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>(Dokument) wurde geprüft</em></p> </td> 
   <td> <p>Reviewer<br>Document<br>„Zum Überprüfen wechseln“-Schaltfläche<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Limit für Videogenehmigungen nähert sich (80%)</strong> </p> <p>Eine Videogenehmigung erreicht 80 % des Video-Genehmigungslimits ihres Plans.</p> <p>Der Betreff der Sofort-Benachrichtigungs-E-Mail lautet: <em>Sie nähern sich dem Limit für Ihre jährliche Videogenehmigungsanfrage in Workfront</em></p> </td> 
   <td> HEADLINE- und TEXT<br>TEXT/VIDEO-GENEHMIGUNGEN ANGEFORDERT (aktuelle Verwendung)<br>Obergrenze insgesamt (das Limit)<br>Andere Empfänger<br> Schaltfläche „In Workfront anzeigen“<br>Schaltfläche „Auf FIO Enterprise aktualisieren“ </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Limit für Videogenehmigung erreicht</strong> </p> <p>Eine Videogenehmigung erreicht das Video-Genehmigungslimit ihres Plans.</p> <p>Der Betreff der Sofort-Benachrichtigungs-E-Mail lautet: <em>Sie haben das Limit für Ihre jährliche Videogenehmigungsanfrage in Workfront erreicht</em></p> </td> 
   <td> HEADLINE- und TEXT<br>TEXT/VIDEO-GENEHMIGUNGEN ANGEFORDERT (aktuelle Verwendung)<br>Obergrenze insgesamt (das Limit)<br>Andere Empfänger<br> Schaltfläche „In Workfront anzeigen“<br>Schaltfläche „Auf FIO Enterprise aktualisieren“ </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Entscheidung getroffen - Genehmigt</strong> </p> <p>Eine genehmigende Person trifft eine Entscheidung von genehmigt für ein Genehmigungs-Dokument.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>(Dokument) genehmigt von (Name)</em></p> </td> 
   <td> <p>Entscheidungsträger<br>Entscheidung<br>Dokument und Version<br> Schaltfläche „Zum Überprüfen wechseln“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Entscheidung getroffen - Mit Änderungen genehmigt</strong> </p> <p>Eine genehmigende Person trifft eine Entscheidung von Genehmigt mit Änderungen in einer Dokumentgenehmigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>(Dokument) mit Änderungen genehmigt von (Name)</em></p> </td> 
   <td> <p>Entscheidungsträger<br>Entscheidung<br>Dokument und Version<br> Schaltfläche „Zum Überprüfen wechseln“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Entscheidung getroffen - Muss überarbeitet werden</strong> </p> <p>Eine genehmigende Person trifft die Entscheidung, dass eine Dokumentgenehmigung erforderlich ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>(Dokument) muss bearbeitet werden von (Name)</em></p> </td> 
   <td> <p>Entscheidungsträger<br>Entscheidung<br>Dokument und Version<br> Schaltfläche „Zum Überprüfen wechseln“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dokumente, die einer gruppierten Genehmigung hinzugefügt oder daraus entfernt wurden</strong> </p> <p>Dokumente werden einer gruppierten Dokumentengenehmigung, der Sie angehören, hinzugefügt oder daraus entfernt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Ein Dokument wurde einer Genehmigung, der Sie angehören, hinzugefügt oder daraus entfernt</em></p> </td> 
   <td> <p><strong>Hinzugefügt:</strong><br>Anforderer<br>Gruppenname<br>Miniaturansicht<br>Datumsangaben<br> Schaltfläche „Zur Überprüfung wechseln“ <br>Detailblock: Gruppenname, Anzahl der Assets, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Benutzerdefinierte Nachricht<br>Projekt</p> <p><strong>Entfernt:</strong><br>Anforderer<br>Gruppenname<br>Miniaturvorschau (keine Schaltfläche oder Detailblock)</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alle Überprüfungen abgeschlossen</strong> </p> <p>Jeder Reviewer schließt seine Überprüfung bei einer Dokumentengenehmigung ab.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>Alle Bewertungen sind am (Dokument) abgeschlossen</em></p> </td> 
   <td> <p>Dokument<br>Genehmigung angefordert am<br>Fälligkeitsdatum<br> Schaltfläche „Zur Überprüfung wechseln“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Erinnerung - 24 Stunden</strong> </p> <p>Sie haben noch 24 Stunden, um das Dokument zu überprüfen und zu genehmigen.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Erinnerung: Ihre Genehmigung ist erforderlich für (Dokument)</em></p> </td> 
   <td> <p>Anforderer<br>Ihre Rolle<br>Team<br>Genehmigung angefordertes Datum<br>Fälligkeitsdatum<br> Schaltfläche „Zur Überprüfung gehen“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Erinnerung - 72 Stunden</strong> </p> <p>Sie haben noch 72 Stunden, um das Dokument zu überprüfen und zu genehmigen.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Erinnerung: Ihre Genehmigung ist erforderlich für (Dokument)</em></p> </td> 
   <td> <p>Anforderer<br>Ihre Rolle<br>Team<br>Genehmigung angefordertes Datum<br>Fälligkeitsdatum<br> Schaltfläche „Zur Überprüfung gehen“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Als genehmigende Person oder prüfende Person hinzugefügt</strong> </p> <p>Sie werden als genehmigende Person oder Prüfende Person zu einer Dokumentgenehmigung hinzugefügt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Ihre Genehmigung ist erforderlich für (Dokument)</em></p> </td> 
   <td> <p>Anforderer<br>Ihre Rolle<br>Team<br>Genehmigung angefordertes Datum<br>Fälligkeitsdatum<br> Schaltfläche „Zur Überprüfung gehen“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Benutzerdefinierte Nachricht<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Als genehmigende Person oder prüfende Person entfernt</strong> </p> <p>Sie werden als genehmigende Person oder Prüfende Person aus einer Dokumentgenehmigung entfernt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Ihre Genehmigung ist für (Dokument) nicht mehr erforderlich</em></p> </td> 
   <td> <p>Anforderer<br>Dokument und Version<br>Rolle<br>Team (keine Schaltfläche oder Detailblock)</p> <p><em>Enthalten bei Teil der Nachricht approval:</em><br>Document preview<br>custom</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rolle geändert</strong> </p> <p>Ihre Rolle als Genehmiger oder Prüfer ändert sich bei einer Dokumentgenehmigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Ihre Rolle in (Dokument) hat sich geändert</em></p> </td> 
   <td> <p>Anforderer<br>Dokument und Version<br>Richtung der Rollenänderung<br> Schaltfläche „Zur Überprüfung wechseln“<br>Detailblock: Dokumentname, Dokumentdetails, Alle Empfänger</p> <p><em>Im Rahmen der Genehmigung enthalten:</em><br>Dokumentvorschau<br>Phase<br>Projekt</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
