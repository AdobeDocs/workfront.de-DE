---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: In Adobe Workfront verfügbare Ereignisbenachrichtigungen
description: Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen auf Objekten wie Projekten, Aufgaben und Problemen ausgelöst werden. In diesem Artikel werden die verfügbaren Arten von Ereignisbenachrichtigungen aufgeführt und beschrieben.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: d177f884a8754d0ced3d9c5d6f44c1b4964f1629
workflow-type: tm+mt
source-wordcount: '5087'
ht-degree: 8%

---

# In Adobe Workfront verfügbare Ereignisbenachrichtigungen

<!-- Audited: 1/2024 -->

Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen auf Objekten wie Projekten, Aufgaben und Problemen ausgelöst werden, wie hier beschrieben: [Ereignisbenachrichtigungen](../../../workfront-basics/using-notifications/event-notifications.md).

Diese Benachrichtigungen können auf System- und Gruppenebene konfiguriert werden:

* Informationen zum Konfigurieren von Ereignisbenachrichtigungen auf Systemebene finden Sie unter [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Informationen zum Konfigurieren von Ereignisbenachrichtigungen auf Gruppenebene finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Einzelne Benutzer können auch ihre individuellen Ereignisbenachrichtigungen in ihrem jeweiligen Profil aktivieren und deaktivieren. Weitere Informationen finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

In den folgenden Tabellen sind alle Adobe Workfront-Ereignisbenachrichtigungen aufgeführt, eine kurze Beschreibung des Ereignisses sowie Informationen dazu, ob das Ereignis standardmäßig aktiv oder inaktiv ist.

## Aktion erforderlich

Siehe auch [Benachrichtigungen: Erforderliche Aktion](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th>Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Zugriffsanforderung</p> </td> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Jemand bittet um Zugang von mir.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> <p> </p> </td> 
   <td> <p>Dokumentanforderung hinzufügen</p> </td> 
   <td> <p>Benutzer, von dem das Dokument angefordert wird</p> </td> 
   <td> <p>Jemand hat mich gebeten, Dokumente hochzuladen.</p> <p>Die Dokumentenanfrage erhält eine E-Mail-Benachrichtigung, wenn sie eine Anforderung zum Hochladen eines Dokuments erhält.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument ausstehend Genehmigung</p> </td> 
   <td> <p>Genehmigende Personen</p> </td> 
   <td> <p>Ich muss ein Dokument genehmigen.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problemzuweisung</p> </td> 
   <td> <p>Benutzer, der das Problem zugewiesen hat</p> </td> 
   <td> <p>Ich habe ein Problem.</p> <p>Der Problemverantwortliche erhält nur dann eine E-Mail-Benachrichtigung, wenn der Status des Projekts aktuell ist und der Status des Problems nicht geschlossen ist oder mit Geschlossen übereinstimmt.</p> <p>Benutzer mit einer Lizenz für Review oder Anfrage erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem mit ausstehender Genehmigung</p> </td> 
   <td> <p>Genehmigende Personen</p> </td> 
   <td> <p>Ich muss ein Problem genehmigen.</p> <p>Welche Benutzer eine E-Mail-Benachrichtigung für dieses Ereignis erhalten, hängt davon ab, ob die Einstellung "Genehmiger muss nicht im Projektteam sein (für Genehmigungsprozesse, die eine Rolle enthalten)"aktiviert ist (wie beschrieben in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Globale Genehmigungseinstellungen konfigurieren</a>). </p> <p>Wenn diese Option aktiviert ist</strong>, wird eine E-Mail-Benachrichtigung an alle Benutzer im System mit der Rolle "Genehmiger"gesendet.</p> <p>Wenn diese Option deaktiviert ist</strong>, erhalten nur Projektteams mit der Rolle "Genehmiger"eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird gesendet, wenn das Projekt den Status Planung oder Aktuell aufweist. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem mit ausstehender Genehmigung</p> </td> 
   <td> <p>Delegierter Genehmiger</p> </td> 
   <td> <p>Ich muss eine Problemvalidierung überprüfen, wenn ich "delegiert wurde.</p> <p>Wenn ein Benutzer eine Problemgenehmigung an einen anderen Benutzer delegiert, wird dieser benachrichtigt. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn das Projekt den Status Aktuell aufweist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projekt mit ausstehender Genehmigung</p> </td> 
   <td> <p>Genehmigende Personen</p> </td> 
   <td> <p>Ich muss ein Projekt genehmigen.</p> <p>Welche Benutzer eine E-Mail-Benachrichtigung für dieses Ereignis erhalten, hängt davon ab, ob die Einstellung "Genehmiger muss nicht im Projektteam sein (für Genehmigungsprozesse, die eine Auftragsrolle enthalten)"aktiviert ist (wie beschrieben in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Globale Genehmigungseinstellungen konfigurieren</a>).</p> <p>Wenn diese Option aktiviert ist</strong>, wird eine E-Mail-Benachrichtigung an alle Benutzer im System mit der Rolle "Genehmiger"gesendet.</p> <p>Wenn diese Option deaktiviert ist</strong>, erhalten nur Projektteams mit der Rolle "Genehmiger"eine E-Mail-Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Projekt mit ausstehender Genehmigung</td> 
   <td>Delegierter Genehmiger</td> 
   <td> <p>Ich muss eine Projektgenehmigung überprüfen, die mir übertragen wurde.</p> </td> 
   <td> Aktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenzuweisung</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen wurde</p> </td> 
   <td> <p>Ich bin der Hauptverantwortliche einer Aufgabe.</p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn er zum primären Verantwortlichen der Aufgabe gemacht wird, es sei denn, der Verantwortliche ist der Benutzer, der die Zuweisung vorgenommen hat.</p> <p>Eine Benachrichtigung wird gesendet, wenn der Projektstatus Aktuell ist und die Aufgabe nicht als abgeschlossen markiert ist.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabe mit ausstehender Genehmigung</p> </td> 
   <td> <p>Genehmigende Personen</p> </td> 
   <td> <p>Ich muss eine Aufgabe genehmigen.</p> <p>Welche Benutzer eine E-Mail-Benachrichtigung für dieses Ereignis erhalten, hängt davon ab, ob die Einstellung "Genehmiger muss nicht im Projektteam sein (für Genehmigungsprozesse, die eine Rolle enthalten)"aktiviert ist (wie beschrieben in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Globale Genehmigungseinstellungen konfigurieren</a>). </p> <p>Wenn diese Option aktiviert ist</strong>, wird eine E-Mail-Benachrichtigung an alle Benutzer im System mit der Rolle "Genehmiger"gesendet.</p> <p>Wenn diese Option deaktiviert ist</strong>, erhalten nur Projektteams mit der Rolle "Genehmiger"eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus zum Zeitpunkt der Anfrage aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabe mit ausstehender Genehmigung</p> </td> 
   <td> <p>Delegierter Genehmiger</p> </td> 
   <td> <p>Ich muss eine Aufgabengenehmigung überprüfen, die mir übertragen wurde.</p> <p>Wenn ein Benutzer eine Problemgenehmigung an einen anderen Benutzer delegiert, wird dieser benachrichtigt. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus zum Zeitpunkt der Anfrage aktuell ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Arbeitszeittabelle</p> </td> 
   <td> <p>Datenblatt Neu geöffnet</p> </td> 
   <td> <p>Benutzer, zu dem das Timesheet gehört</p> </td> 
   <td> <p>Mein Timesheet wird wieder geöffnet.</p> <p>Der Eigentümer des Datenblatts erhält beim erneuten Öffnen des Datenblatts eine E-Mail-Benachrichtigung, es sei denn, der Benutzer, der das Datenblatt erneut geöffnet hat, ist auch Eigentümer des Datenblatts.</p> <p>Eine E-Mail-Benachrichtigung wird nur gesendet, wenn der Status des Zeitblatts "Open"lautet.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Arbeitszeittabelle</p> </td> 
   <td> <p>Zurückweisung des Zeitplans</p> </td> 
   <td> <p>Benutzer, zu dem das Timesheet gehört</p> </td> 
   <td> <p>Mein Timesheet wird abgelehnt.</p> <p>Der Besitzer des Datenblatts erhält eine E-Mail-Benachrichtigung, wenn das Datenblatt abgelehnt wird, es sei denn, der Benutzer, der das Datenblatt abgelehnt hat, ist ebenfalls Eigentümer.</p> <p>Eine E-Mail-Benachrichtigung wird nur gesendet, wenn der Status des Zeitblatts Abgelehnt ist.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Arbeitszeittabelle</p> </td> 
   <td> <p>Übermittlung des Zeitplans</p> </td> 
   <td> <p>Genehmigende Person</p> </td> 
   <td> <p>Ich muss ein Timesheet genehmigen.</p> <p>Der Timesheet-Genehmiger erhält eine E-Mail-Benachrichtigung, wenn ein zu validierendes Zeitblatt übermittelt wird, es sei denn, der Benutzer, der das Datenblatt gesendet hat, ist auch der Timesheet-Genehmiger.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Status des Zeitblatts übermittelt wird.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Zuweisung</p> </td> 
   <td> <p>Arbeitselementanforderung</p> </td> 
   <td> <p>Mitglieder des Teams, für das der Artikel angefordert wird</p> </td> 
   <td> <p>Mein Team erhält eine neue Arbeitsanfrage.</p> <p>Team-Mitglieder erhalten eine E-Mail-Benachrichtigung, wenn das Team eine neue Arbeitsanfrage erhält. (Der Benutzer, der die Anfrage gesendet hat, erhält keine Benachrichtigung, wenn er Mitglied des Teams ist.)</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus zum Zeitpunkt der Arbeitsanforderung aktuell ist und der Status der Arbeitsanforderung "Neu"lautet.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Zuweisung</p> </td> 
   <td> <p>Arbeitselementanforderung</p> </td> 
   <td> <p>Benutzer, für den das Arbeitselement angefordert wird</p> </td> 
   <td> <p>Ich bekomme eine neue Arbeitsanfrage.</p> <p>Der Bevollmächtigte des Arbeitselements erhält eine E-Mail-Benachrichtigung, es sei denn, der Benutzer, der die Anfrage stellt, ist auch der Bevollmächtigte. </p> <p>Eine Benachrichtigung wird nicht gesendet, wenn der Aufgabenstatus Abgeschlossen oder der Problemstatus Abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus zum Zeitpunkt der Anfrage aktuell ist.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Von mir gestellte Anfragen

Siehe auch [Benachrichtigungen: Von mir gestellte Anforderungen](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th> Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Änderung des Genehmigungsstatus</p> </td> 
   <td> <p>Anfragender</p> </td> 
   <td> <p>Eine Anforderung zur Dokumentgenehmigung ist abgeschlossen.</p> <p>Der Dokumentanfragende erhält eine E-Mail-Benachrichtigung, wenn die Genehmigungsanforderung für das Dokument abgeschlossen ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Abschluss der Dokumentanforderung</p> </td> 
   <td> <p>Anfragender</p> </td> 
   <td> <p>Eine Anfrage zum Hochladen von Dokumenten wurde erfüllt.</p> <p>Der Dokumentanfragende erhält eine E-Mail-Benachrichtigung, wenn eine Anforderung zum Hochladen eines Dokuments erfüllt ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem hinzufügen</p> </td> 
   <td> <p>Primärer Ansprechpartner für Probleme</p> </td> 
   <td> <p>Ich füge einem Projekt ein Problem hinzu.</p> <p>Der Hauptkontakt zu einem Problem erhält eine Benachrichtigung, wenn er ein Problem in einem Projekt hinzufügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td>Problemzuweisung</td> 
   <td>Primärer Ansprechpartner für Probleme</td> 
   <td> <p>Jemand wird einem Problem zugeordnet, für das ich der Hauptkontakt bin.</p> <p>Der Hauptkontakt zu einem Problem erhält eine Benachrichtigung, wenn das Problem einem Benutzer zugewiesen wird. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> Inaktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problembeendigung</p> </td> 
   <td> <p>Primärer Ansprechpartner für Probleme</p> </td> 
   <td> <p>Ein Problem, bei dem ich der Hauptkontakt bin, ist abgeschlossen.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Änderung des Projektstatus</p> </td> 
   <td> <p>Benutzer, der das Projekt erstellt hat (eingegeben von)</p> </td> 
   <td> <p>Der Status ändert sich in einem Projekt, das ich erstellt habe.</p> <p>Der Benutzer, der das Projekt erstellt hat, erhält eine E-Mail-Benachrichtigung, wenn sich der Projektstatus ändert.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Anfrage hinzufügen</p> </td> 
   <td> <p>Primärer Ansprechpartner für Probleme</p> </td> 
   <td> <p>Ich sende eine Anfrage (Bestätigung).</p> <p>Der Primäre Kontakt zu diesem Problem erhält eine E-Mail-Benachrichtigung, wenn er ein Problem sendet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt die Ansicht "Is Help Desk"verwendet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Anforderungszuweisung</p> </td> 
   <td> <p>Primärer Ansprechpartner für Probleme</p> </td> 
   <td> <p>Jemand wird meiner Bitte zugewiesen.</p> <p>Der primäre Ansprechpartner des Problems erhält eine E-Mail-Benachrichtigung, wenn ein Benutzer dem Problem zugewiesen wird, es sei denn, der primäre Ansprechpartner und der zugewiesene Benutzer sind derselbe Benutzer.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt die Ansicht "Is Help Desk"verwendet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Anfrage abgeschlossen</p> </td> 
   <td> <p>Primärer Ansprechpartner für Probleme</p> </td> 
   <td> <p>Meine Anfrage ist geschlossen (Bestätigung).</p> <p>Der primäre Ansprechpartner des Problems erhält eine E-Mail-Benachrichtigung, wenn die Anfrage geschlossen wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt die Ansicht "Is Help Desk"verwendet.</p> <p>Wenn die Benachrichtigungen für "Problemabwicklung"aktiviert sind, werden sie immer anstelle der "Anfrage für Primären Kontakt ausgeben"Trigger. Wenn diese Benachrichtigung an den Trigger gesendet werden soll, müssen Sie die Benachrichtigungen zum Abschluss von Problemen deaktivieren.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument anfordern</p> </td> 
   <td> <p>Primärer Ansprechpartner für Probleme</p> </td> 
   <td> <p>Ein Dokument wird geändert oder hochgeladen, wenn es sich um ein Problem handelt, für das ich der Hauptkontakt bin.</p> <p>Der primäre Ansprechpartner des Problems erhält eine E-Mail-Benachrichtigung, wenn ein Dokument hochgeladen oder in einem Problem geändert wird, es sei denn, der Benutzer, der das Dokument hochgeladen oder geändert hat, ist ebenfalls der primäre Ansprechpartner.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und für das Projekt auf der Registerkarte Warteschlangeneinstellungen die Option "Als Warteschlange für Hilfeanfragen veröffentlichen"aktiviert ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Änderung des Anfragestatus</p> </td> 
   <td> <p>Primärer Ansprechpartner für Probleme</p> </td> 
   <td> <p>Der Status ändert sich in meiner Anfrage.</p> <p>Der Hauptkontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn sich der Problemstatus ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Hauptkontakt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt die Ansicht "Is Help Desk"verwendet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Kommunikation

Siehe auch [Mitteilungen: Kommunikation](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th> Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Kommentar zu Dokument</p> </td> 
   <td> <p>Dokumentbesitzer</p> </td> 
   <td> <p>Zu meinem Dokument wird ein Kommentar hinzugefügt.</p> <p>Der Dokumenteigentümer in Workfront erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar im Dokument veröffentlicht wird, es sei denn, der Benutzer, der den Kommentar veröffentlicht hat, ist auch Dokumenteigentümer.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist. </p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Kommentar zu &lt;request name=""&gt; on &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist:<em> Kommunikationsgrad &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Aktiv </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Notiz</p> </td> 
   <td> <p>Anmerkung anfordern</p> </td> 
   <td> <p>Primärer Ansprechpartner für Probleme</p> </td> 
   <td> <p>Wenn ein Kommentar zu einer Anfrage gepostet wird, senden Sie eine E-Mail an den Hauptkontakt des Problems.</p> <p>Der Hauptkontakt für ein Problem erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar auf einer Anfrage veröffentlicht wird, es sei denn, der Benutzer, der den Kommentar veröffentlicht hat, ist auch der primäre Ansprechpartner für das Problem.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td>Directed Update</td> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Jemand nimmt mich in ein direktes Update auf.</p> <p>Eine gezielte Aktualisierung ist der Fall, wenn ein Benutzer einen anderen Benutzer in eine Aktualisierung einbezieht, wie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagging anderer Benutzer auf Updates</a>.</p> <p>In diesem Fall erhält der Benutzer, der in der empfohlenen Aktualisierung enthalten ist, eine E-Mail-Benachrichtigung über die Aktualisierung.</p> <p>Die E-Mail-Benachrichtigung wird nur gesendet, wenn der Benutzer über Zugriffsrechte für das Objekt verfügt und es in seinem Profil aktiviert bleibt.  </p> <p>Diese Ereignisbenachrichtigung ist standardmäßig aktiviert und kann nicht deaktiviert werden.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Directed Update</p> </td> 
   <td> <p>Team-Mitglieder</p> </td> 
   <td> <p>Jemand bezieht mein Team in ein direktes Update ein.</p> <p>Eine gezielte Aktualisierung ist der Fall, wenn ein Benutzer einen anderen Benutzer in eine Aktualisierung einbezieht, wie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tagging anderer Benutzer auf Updates</a>.</p> <p>In diesem Fall erhält jedes Mitglied des Teams, das in der empfohlenen Aktualisierung enthalten ist, eine E-Mail-Benachrichtigung über die Aktualisierung.</p> <p>Die E-Mail-Benachrichtigung wird nur an Benutzer gesendet, die über Zugriffsberechtigungen für das Objekt der Aktualisierung verfügen.</p> <p>Wenn der Benutzer, der die gezielte Aktualisierung sendet, Mitglied des Teams ist, das eingeschlossen ist, erhält der Benutzer, der die Aktualisierung sendet, keine E-Mail-Benachrichtigung.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Notiz</p> </td> 
   <td> <p>Kommentar zu Arbeitselementen</p> </td> 
   <td> <p>Thread-Teilnehmer</p> </td> 
   <td> <p>Jemand kommentiert einen Faden, in dem ich bin.</p> <p>Teilnehmer im Thread und Benutzer, die in einer Direktnachricht enthalten sind, erhalten eine E-Mail-Benachrichtigung, wenn ein Benutzer einen Kommentar im Thread abgibt.</p> <p>Benutzer müssen Zugriff auf Ansicht haben, um eine Benachrichtigung zu erhalten.</p> <p>Die folgenden Benutzer erhalten keine Benachrichtigung:</p> 
    <ul> 
     <li> <p>In einer Direktnachricht enthaltene Teams</p> </li> 
     <li> <p>Der Eigentümer der Notiz</p> </li> 
     <li> <p>Der Primäre Kontakt</p> </li> 
    </ul> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Notiz</p> </td> 
   <td> <p>Kommentar zu Arbeitselementen</p> </td> 
   <td> <p>Arbeitselement-Zuweisung</p> </td> 
   <td> <p>Jemand kommentiert eines meiner Arbeitselemente.</p> <p>Der Verantwortliche des Arbeitselements erhält jedes Mal, wenn ein Benutzer ein Update zu einem Arbeitselement hinzufügt, eine E-Mail-Benachrichtigung, es sei denn, der Benutzer, der die Aktualisierung hinzufügt, ist auch der Verantwortliche.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Notiz</p> </td> 
   <td> <p>Antwort auf Arbeitsanforderung</p> </td> 
   <td> <p> Arbeitsanfrage</p> </td> 
   <td> <p>Jemand antwortet auf meine Anfrage.</p> <p>Nachdem ein Benutzer eine Anforderung gesendet hat und ein anderer Benutzer auf diese Anforderung antwortet, erhält der Benutzer, der die Anforderung gesendet hat, eine E-Mail-Benachrichtigung.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn:</p> 
    <ul> 
     <li> <p>Der Benutzer, der antwortet, ist derselbe Benutzer, der die Anfrage gestellt hat</p> </li> 
     <li> <p>Der Benutzer hat keinen Zugriff auf die Notiz.</p> </li> 
    </ul> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Validierungsinformationen

Siehe auch [Benachrichtigungen: Validierungsinformationen](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th> Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Genehmigungsdelegierung</p> </td> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Ich werde als Genehmiger beauftragt.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Delegierte Problemgenehmigung - Statusänderung</p> </td> 
   <td> <p>Benutzer, der die Genehmigung erteilt hat</p> </td> 
   <td> <p>Ein delegierter Genehmigungsantrag ist abgeschlossen. </p> <p>Wenn Sie eine Problemvalidierung an eine andere Person delegieren, erhalten Sie eine E-Mail-Benachrichtigung, wenn diese die Genehmigung abschließt (unabhängig davon, ob sie die Problemvalidierung validieren oder ablehnen). </p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Delegierte Projektgenehmigung - Statusänderung</p> </td> 
   <td> <p>Benutzer, der die Genehmigung erteilt hat</p> </td> 
   <td> <p>Ein delegierter Genehmigungsantrag für ein Projekt ist abgeschlossen.</p> <p>Wenn Sie eine Projektgenehmigung an eine andere Person delegieren, erhalten Sie eine E-Mail-Benachrichtigung, wenn diese Genehmigung abgeschlossen ist (unabhängig davon, ob sie die Projektgenehmigung genehmigt oder ablehnt).</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Delegierte Aufgabengenehmigung - Statusänderung</p> </td> 
   <td> <p>Benutzer, der die Genehmigung erteilt hat</p> </td> 
   <td> <p>Der Status der delegierten Aufgabenvalidierung ist abgeschlossen.</p> <p>Wenn Sie eine Aufgabenvalidierung an eine andere Person delegieren, erhalten Sie eine E-Mail-Benachrichtigung, wenn diese Validierung abgeschlossen ist (unabhängig davon, ob sie die Aufgabenvalidierung validieren oder ablehnen).</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Stornierung der Dokumentgenehmigung an genehmigende Person</p> </td> 
   <td> <p>Benutzer, der die Genehmigung erteilt hat</p> </td> 
   <td> <p>Eine Anforderung zur Dokumentgenehmigung wird abgebrochen.</p> <p>Der Dokumentenvalidierer des Dokuments erhält eine E-Mail-Benachrichtigung, wenn die Anforderung der Dokumentgenehmigung abgebrochen wird.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Arbeitszeittabelle</p> </td> 
   <td> <p>Genehmigung des Datenblatts</p> </td> 
   <td> <p>Benutzer, zu dem das Timesheet gehört</p> </td> 
   <td> <p>Mein Timesheet ist genehmigt.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informationen über die mir zugewiesene Arbeit

Siehe auch [Benachrichtigungen: Informationen über die mir zugewiesenen Aufgaben](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th> Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Aufgabe</td> 
   <td>Abschluss aller Vorgänger-Aufgaben</td> 
   <td>Abhängige Aufgaben zugewiesene Teammitglieder</td> 
   <td> <p>Alle Vorgänger der Aufgaben des Teams sind fertig gestellt.</p> <p>Die Aufgabenempfänger (alle Mitglieder des Teams) erhalten eine E-Mail-Benachrichtigung.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td>Inaktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Abschluss aller Vorgänger-Aufgaben</p> </td> 
   <td> <p>Benutzer, der abhängigen Aufgaben zugewiesen ist</p> </td> 
   <td> <p>Alle Vorgänger meiner Aufgaben sind abgeschlossen.</p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Validierungsentscheidung</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen wurde</p> </td> 
   <td> <p>Ein von mir gelöstes Problem wird genehmigt oder abgelehnt.</p> <p>Der Verantwortliche eines Problems erhält eine E-Mail-Benachrichtigung, wenn eine Genehmigungsentscheidung getroffen (genehmigt oder abgelehnt) wird.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Validierungsentscheidung</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Eine Aufgabe, die ich abschließe, wird genehmigt oder abgelehnt.</p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe genehmigt oder abgelehnt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problembeendigung</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen wurde</p> </td> 
   <td> <p>Ein Problem, dem ich zugewiesen bin, ist abgeschlossen.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Geplantes Abschlussdatum für Problem hat sich geändert</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen wurde</p> </td> 
   <td> <p>Das Fälligkeitsdatum ändert sich bei einem Problem, dem ich zugewiesen bin.</p> <p>Der Problemverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich das geplante Abschlussdatum ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Verantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus etwas Anderes als die Planung ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Änderung des Problemstatus</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen wurde</p> </td> 
   <td> <p>Der Status ändert sich für eines meiner Arbeitselemente.</p> <p>Der Bevollmächtigte des Problems erhält eine E-Mail-Benachrichtigung, wenn sich der Status ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Bevollmächtigte.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument anfordern</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen wurde</p> </td> 
   <td> <p>Dokumente werden bei Anforderungen, denen ich zugewiesen bin, hochgeladen oder geändert.</p> <p>Der Problemverantwortliche erhält eine E-Mail-Benachrichtigung, wenn Dokumente in einem von ihm hinzugefügten Problem hochgeladen oder geändert werden.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn der Benutzer, der an dem Problem teilgenommen hat, der Problemverantwortliche ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und für das Projekt auf der Registerkarte Warteschlangeneinstellungen die Option "Als Warteschlange für Hilfeanfragen veröffentlichen"aktiviert ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Eine Aufgabe, der ich zugewiesen bin, ist abgeschlossen.</p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe abgeschlossen ist. Nach Abschluss einer persönlichen Aufgabe werden keine Benachrichtigungen gesendet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> <p>Benutzer mit der Lizenz "Review"oder "Anforderer"erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Benutzer, der der abhängigen Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Ein Vorgänger einer meiner Aufgaben ist abgeschlossen.</p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn einer der Vorgänger seiner Aufgabe abgeschlossen ist.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Geplantes Abschlussdatum für Aufgabe hat sich geändert</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Das Fälligkeitsdatum ändert sich bei einer Aufgabe, der ich zugewiesen bin.</p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich das geplante Abschlussdatum der Aufgabe ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Aufgabenverantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus etwas Anderes als die Planung ist.</p> <p>Was persönliche Aufgaben betrifft, so wird keine Benachrichtigung gesendet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Statusänderung der Aufgabe</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Der Status ändert sich bei einer Aufgabe, der ich zugewiesen bin.</p> <p>Der Aufgabenverantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich der Status der Aufgabe ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Verantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Informationen zu Projekten, die ich verwende

Siehe auch [Benachrichtigungen: Informationen zu Projekten, die ich verwende](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th> Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Aktueller Projektstatus</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ein Projekt, an dem ich arbeite, wird aktiv.</p> <p>Benutzer des Projekts erhalten eine E-Mail-Benachrichtigung, sobald das Projekt aktiv wird.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument hinzufügen</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ein Dokument wird zu einem Projekt hinzugefügt, an dem ich arbeite.</p> <p>Benutzer des Projektteams erhalten eine E-Mail-Benachrichtigung, wenn ein Dokument zum Projekt hinzugefügt wird, mit Ausnahme des Benutzers, der das Dokument hinzugefügt hat.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus Aktuell und das Dokument nicht Privat ist. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem hinzufügen</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ein Problem wird zu einem Projekt hinzugefügt, an dem ich arbeite.</p> <p>Benutzer in einem Projekt erhalten eine E-Mail-Benachrichtigung, wenn dem Projekt ein Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problembeendigung</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ein Problem ist bei einem Projekt abgeschlossen, an dem ich arbeite.</p> <p>Jeder Benutzer im Projekt erhält eine Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Abschluss von Milestone-Aufgaben</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Eine Meilensteinaufgabe ist an einem Projekt abgeschlossen, an dem ich arbeite.</p> <p>Alle Benutzer im Projektteam erhalten eine Benachrichtigung, wenn eine Meilensteinaufgabe abgeschlossen ist. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektabschluss</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ein Projekt, in dem ich bin, ist abgeschlossen.</p> <p>Benutzer in einem Projektteam erhalten eine E-Mail-Benachrichtigung, wenn der Projektstatus Abgeschlossen ist.</p> <p>Tipp: Wenn Projekte regelmäßig abgeschlossen werden, kann die Aktivierung dieser Option eine Menge E-Mails für Benutzer erstellen, die eine begrenzte Anzahl von Aufgaben für viele Projekte haben. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Änderung des Projektstatus</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Der Status ändert sich bei einem Projekt, in dem ich bin.</p> <p>Benutzer im Projektteam erhalten eine E-Mail-Benachrichtigung, wenn sich der Status des Projekts ändert. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projektbenutzer</p> </td> 
   <td> <p>Projekt-Benutzer hinzufügen</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ich werde zu einem Projekt hinzugefügt.</p> <p>Der Benutzer, der zum Projekt hinzugefügt wurde, erhält beim Hinzufügen eine E-Mail-Benachrichtigung, es sei denn, der Benutzer wurde zum Projekt selbst hinzugefügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Eine Aufgabe ist an einem Projekt abgeschlossen, an dem ich arbeite.</p> <p>Mitglieder des Projektteams erhalten eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Nicht zugewiesenes Problem hinzugefügt</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ein nicht zugewiesenes Problem wird zu einem Projekt hinzugefügt, an dem ich arbeite.</p> <p>Benutzer eines Projekts erhalten eine E-Mail-Benachrichtigung, wenn dem Projekt ein Problem ohne Zuweisung hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informationen über Projekte, die ich besitze

Siehe auch [Benachrichtigungen: Informationen zu Projekten, die ich besitze](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th> Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument hinzufügen</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein Dokument wird zu einem Projekt hinzugefügt, dessen Eigentümer ich bin.</p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn ein Dokument zum Projekt hinzugefügt wird, es sei denn, der Benutzer, der das Dokument hinzugefügt hat, ist auch Projektinhaber.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus Aktuell und das Dokument nicht Privat ist.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem hinzufügen</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein Problem wird zu einem Projekt hinzugefügt, dessen Eigentümer ich bin.</p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Änderung des Verpflichtungsdatums für ein Problem</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Das Commit-Datum ändert sich für ein Problem in einem meiner Projekte.</p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn sich das Veröffentlichungsdatum für ein Problem im Projekt ändert, es sei denn, der Benutzer, der das Veröffentlichungsdatum ändert, ist derselbe Benutzer wie der Projekteigentümer.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problembeendigung</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein Problem ist bei einem Projekt abgeschlossen, dessen Eigentümer ich bin.</p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Abschluss von Milestone-Aufgaben</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Eine Meilensteinaufgabe wird an einem Projekt abgeschlossen, das ich besitze.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Zuweisung des Projekteigentümers</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ich bin der Besitzer eines neuen Projekts.</p> <p>Wenn ein Benutzer als Eigentümer eines Projekts zugewiesen wird, erhält er eine E-Mail-Benachrichtigung.</p> <p>Wenn der Projektinhaber derselbe Benutzer ist, der die Zuweisung vorgenommen hat, wird keine E-Mail-Benachrichtigung gesendet</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Änderung des Projektstatus</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein Projekt, das ich besitze, kommt zurück.</p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn das Projekt verspätet ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Änderung des Commit-Datums für Aufgabe</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Das Commit-Datum ändert sich für eine Aufgabe in einem meiner Projekte.</p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn sich das Veröffentlichungsdatum für eine Aufgabe im Projekt ändert, es sei denn, der Benutzer, der das Veröffentlichungsdatum geändert hat, ist auch Projektinhaber.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Eine Aufgabe wird an einem Projekt abgeschlossen, dessen Eigentümer ich bin.</p> <p>Der Projekteigentümer erhält eine Benachrichtigung. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Änderung beim Aufgabenfortschritt</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Eine Aufgabe an einem Projekt, das ich besitze, kommt zurück.</p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn eine Aufgabe im Projekt hinter den Zeitplan zurückfällt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Nicht zugewiesenes Problem hinzufügen</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein nicht zugewiesenes Problem wird zu einem Projekt hinzugefügt, dessen Eigentümer ich bin.</p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein nicht zugewiesenes Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informationen zu den von mir geförderten Projekten

Siehe auch [Benachrichtigungen: Informationen zu Projekten, die ich sponsere](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th> Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument hinzufügen</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Ein Dokument wird zu einem Projekt hinzugefügt, das ich sponsere.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein Dokument hinzugefügt wird, es sei denn, das Dokument wird vom Projektsponsor hinzugefügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus Aktuell ist und das Dokument nicht Privat ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem hinzufügen</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Ein Problem wird zu einem Projekt hinzugefügt, das ich sponsere.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problembeendigung</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Ein Problem ist bei einem Projekt abgeschlossen, das ich sponsere.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Abschluss von Milestone-Aufgaben</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Eine Meilensteinaufgabe wird an einem Projekt abgeschlossen, das ich sponsere.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn eine Meilensteinaufgabe an einem von ihm geförderten Projekt abgeschlossen wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Änderung des Projektstatus</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Ein Projekt, das ich sponsere, kommt zurück.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn das Projekt in Verzug gerät.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Zuweisung des Projektsponsors</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Ich bin der Sponsor eines Projekts.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn er als Sponsor eines Projekts eingestellt wird.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Eine Aufgabe wird an einem Projekt abgeschlossen, das ich sponsere.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Änderung beim Aufgabenfortschritt</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Eine Aufgabe an einem Projekt, das ich sponsere, kommt zurück.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn eine Aufgabe im Projekt hinter den Zeitplan zurückfällt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Nicht zugewiesenes Problem hinzufügen</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Ein nicht zugewiesenes Problem wird einem Projekt, das ich sponsere, hinzugefügt.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein nicht zugewiesenes Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verschiedene Informationen

Siehe auch [Mitteilungen: Verschiedene Informationen](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objekttyp</th> 
   <th>Ereignis</th> 
   <th>Empfänger</th> 
   <th>Beschreibung</th> 
   <th> Standardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ankündigung</td> 
   <td> <p>Ankündigng wurde hinzugefügt.</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Eine Nachricht wird an das Ankündigungszentrum gesendet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Abbrechen der Dokumentanforderung</p> </td> 
   <td> <p>Benutzer, von dem das Dokument angefordert wird</p> </td> 
   <td> <p>Abbrechen einer Anfrage zum Hochladen von Dokumenten von mir.</p> <p>Die Dokumentanforderung erhält eine E-Mail-Benachrichtigung, wenn eine Dokumentanforderung abgebrochen wird.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Fehlerbenachrichtigung</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Es wurde ein Fehler gefunden, der Ihre Aufmerksamkeit benötigt.</p> <p>Eine E-Mail-Benachrichtigung wird erzeugt, nachdem Workfront versucht hat, eine Verbindung zu einem POP-Konto herzustellen. Nach 25 Versuchen deaktiviert Workfront die Verbindung zum POP-Konto, um Ressourcen beizubehalten, und sendet eine Benachrichtigung. </p> <p>Die E-Mail-Benachrichtigung wird an den Projekteigentümer gesendet, wenn die POP-E-Mail mit einer Anforderungswarteschlange verknüpft ist, oder an die Workfront-Administratoren, wenn das POP-Konto mit der Funktion "Eingehende E-Mails"in der E-Mail-Einrichtung verknüpft ist.
   </p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problemzuweisung</p> </td> 
   <td> <p>Ressourceneigentümer</p> </td> 
   <td> <p>Eine Änderung bei der Zuweisung von Aufgaben betrifft eines meiner Mitarbeiter.</p> <p>Der Problemverantwortliche-Manager erhält eine E-Mail-Benachrichtigung, wenn eine Änderung einen von ihm verwalteten Benutzer betrifft.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"oder "Planung"lautet.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Neuer Benutzer</p> </td> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Wenn ein neuer Benutzer in Workfront erstellt wird, senden Sie eine E-Mail an den Benutzer.</p> <p>Nachdem der neue Benutzer erstellt wurde, erhält er eine Einladung in eine E-Mail, in der er darüber informiert wird, dass ein Workfront-Konto erstellt wurde, und er aufgefordert wird, sein Kennwort festzulegen.</p> <p>Bei der Erstellung eines neuen Benutzers können Benutzer die Option "Einladungs-E-Mail an diese Person senden"auswählen (siehe <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Benutzer hinzufügen</a><span style="font-weight: 400;">). Wenn jedoch die Option "Neuer Benutzer für Benutzer"global aktiviert ist, erhalten alle neuen Benutzer die Einladung per E-Mail, unabhängig davon, ob die Option "Einladungs-E-Mail an diese Person senden"ausgewählt ist.</span></p> </td> 
   <td> Inaktiv </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Objektfreigabe</p> </td> 
   <td> <p>Mitglieder des Teams, für das das Objekt freigegeben wurde</p> </td> 
   <td> <p>Jemand teilt ein Objekt mit meinem Team.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Objektfreigabe</p> </td> 
   <td> <p>Benutzer, für den das Objekt freigegeben wurde</p> </td> 
   <td> <p>Jemand teilt mir ein Objekt.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projektbenutzer</p> </td> 
   <td> <p>Projekt-Benutzer hinzufügen</p> </td> 
   <td> <p>Ressourceneigentümer</p> </td> 
   <td> <p>Einer meiner Mitarbeiter wird einem Projekt hinzugefügt.</p> <p>Ein Manager erhält eine E-Mail-Benachrichtigung, wenn einem Projekt ein direkter Bericht hinzugefügt wird.</p> <p>Benutzer mit einer Überprüfungslizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projekt einem Portfolio oder Programm hinzugefügt</p> </td> 
   <td> <p>Portfolio- oder Programmeigentümer</p> </td> 
   <td> <p>Jemand fügt einem Portfolio oder Programm, das ich besitze, ein Projekt hinzu.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenzuweisung</p> </td> 
   <td> <p>Ressourceneigentümer</p> </td> 
   <td> <p>Eine Aufgabenzuweisungsänderung betrifft eines meiner Leute.</p> <p>Der Manager des Aufgabenverantwortlichen erhält eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> Projekt <br>Aufgabe <br>Problem</td> 
   <td>Neues Update</td> 
   <td>Abonnent </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Eine E-Mail wird gesendet, wenn eine Aufgabe, ein Problem oder ein Projekt aktualisiert wird, für das ich angemeldet bin.</span> </p> </td> 
   <td>Aktiv</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## Delegierung

Siehe auch [Benachrichtigungen: Delegation](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Objekttyp | Ereignis | Empfänger | Beschreibung | Standardstatus |
|------------------|------|---------------------------------------------|--------------------------------------------------------------|---------------|
| Aufgaben und Probleme | Aufgaben- und Problemdelegierung | Zugewiesene Person | Ich delegiere meine Aufgaben und Probleme (Bestätigung) | Aktiv |
| Aufgaben und Probleme | Aufgabe anhalten und Delegation ausstellen | Zugewiesene Person | Ich beende die Delegierung meiner Aufgaben und Probleme (Bestätigung) | Aktiv |
| Aufgaben und Probleme | Aufgaben- und Problemdelegierung | Delegieren | Jemand delegiert Aufgaben und Probleme an mich. | Aktiv |
| Aufgaben und Probleme | Aufgaben anhalten und Delegation ausstellen | Delegieren | Jemand beendet die Delegierung von Aufgaben und Problemen an mich. | Aktiv |
