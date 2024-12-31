---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Typen von Ereignisbenachrichtigungen
description: Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen für Objekte wie Projekte, Aufgaben und Probleme ausgelöst werden. In diesem Artikel werden die verfügbaren Arten von Ereignisbenachrichtigungen aufgelistet und beschrieben.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '5201'
ht-degree: 7%

---

# Typen von Ereignisbenachrichtigungen

<!-- Audited: 1/2024 -->

Ereignisbenachrichtigungen sind E-Mails, die von verschiedenen Ereignistypen für Objekte wie Projekten, Aufgaben und Problemen ausgelöst werden, wie in [Ereignisbenachrichtigungen](../../../workfront-basics/using-notifications/event-notifications.md) erläutert.

Diese Benachrichtigungen können auf System- und Gruppenebene konfiguriert werden:

* Informationen zum Konfigurieren von Ereignisbenachrichtigungen auf Systemebene finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* Informationen zum Konfigurieren von Ereignisbenachrichtigungen auf Gruppenebene finden Sie unter [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

Einzelne Benutzer können ihre individuellen Ereignisbenachrichtigungen auch in ihrem individuellen Profil aktivieren und deaktivieren. Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

In den folgenden Tabellen sind alle Adobe Workfront-Ereignisbenachrichtigungen mit einer kurzen Beschreibung des Ereignisses aufgeführt und es wird angegeben, ob das Ereignis standardmäßig aktiv oder inaktiv ist.

>[!NOTE]
>
>Benachrichtigungen mit dem Wert „Aktiv“ in der Spalte Standardstatus sind standardmäßig sowohl für sofortige als auch für tägliche Benachrichtigungen aktiv, sofern nicht anders angegeben.

## Aktion erforderlich

Siehe auch [Benachrichtigungen: Aktion erforderlich](../../../workfront-basics/using-notifications/notifications-action-needed.md).

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
   <th>Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Zugriffsanforderung</p> </td> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Jemand fordert Zugriff von mir an.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> <p> </p> </td> 
   <td> <p>Dokumentanforderung hinzugefügt</p> </td> 
   <td> <p>Benutzer, von dem das Dokument angefordert wird</p> </td> 
   <td> <p>Jemand hat mich gebeten, Dokument(e) hochzuladen.</p> <p>Der Empfänger des Dokuments erhält eine E-Mail-Benachrichtigung, wenn er eine Anfrage zum Hochladen eines Dokuments erhält.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument mit ausstehender Genehmigung</p> </td> 
   <td> <p>Genehmigende Personen</p> </td> 
   <td> <p>Ich muss ein Dokument genehmigen.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problemzuweisung</p> </td> 
   <td> <p>Benutzer, dem dieses Problem zugewiesen ist</p> </td> 
   <td> <p>Ich wurde einem Problem zugewiesen.</p> <p>Der Anfragebearbeiter erhält nur dann eine E-Mail-Benachrichtigung, wenn der Status des Projekts „Aktuell“ und der Status des Problems „Nicht geschlossen“ oder etwas ist, das mit „Geschlossen“ übereinstimmt.</p> <p>Benutzende mit einer Light-, Contributor-, Review- oder Request-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem mit ausstehender Genehmigung</p> </td> 
   <td> <p>Genehmigende Personen</p> </td> 
   <td> <p>Ich muss eine Anfrage genehmigen.</p> <p>Welche Benutzer eine E-Mail-Benachrichtigung für dieses Ereignis erhalten, hängt davon ab, ob die Einstellung „Genehmigende Person muss nicht dem Projektteam angehören (für Genehmigungsprozesse, die eine Rolle beinhalten)“ aktiviert ist (wie in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurieren globaler Genehmigungseinstellungen</a> beschrieben). </p> <p>Wenn diese Option </strong> ist, wird eine E-Mail-Benachrichtigung an alle Benutzer im System mit dem Aufgabengebiet „Genehmiger“ gesendet.</p> <p>Wenn diese Option deaktiviert ist</strong> erhalten nur Mitglieder des Projektteams mit dem Aufgabengebiet „Genehmiger“ eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird gesendet, wenn sich das Projekt im Status Planung oder Aktuell befindet. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problem mit ausstehender Genehmigung</p> </td> 
   <td> <p>Delegierte genehmigende Person</p> </td> 
   <td> <p>Ich muss eine an mich delegierte Problemgenehmigung prüfen.</p> <p>Wenn jemand eine Problemgenehmigung an einen anderen Benutzer delegiert, wird dieser Benutzer benachrichtigt. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn sich das Projekt im Status Aktuell befindet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projekt mit ausstehender Genehmigung</p> </td> 
   <td> <p>Genehmigende Personen</p> </td> 
   <td> <p>Ich muss ein Projekt genehmigen.</p> <p>Welche Benutzer eine E-Mail-Benachrichtigung für dieses Ereignis erhalten, hängt davon ab, ob die Einstellung „Genehmigende Person muss nicht dem Projektteam angehören (für Genehmigungsprozesse, die ein Aufgabengebiet enthalten)“ aktiviert ist (wie in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurieren globaler Genehmigungseinstellungen</a> beschrieben).</p> <p>Wenn diese Option </strong> ist, wird eine E-Mail-Benachrichtigung an alle Benutzer im System mit dem Aufgabengebiet „Genehmiger“ gesendet.</p> <p>Wenn diese Option deaktiviert ist</strong> erhalten nur Mitglieder des Projektteams mit dem Aufgabengebiet „Genehmiger“ eine E-Mail-Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Projekt mit ausstehender Genehmigung</td> 
   <td>Delegierte genehmigende Person</td> 
   <td> <p>Ich muss eine an mich delegierte Projektgenehmigung prüfen.</p> </td> 
   <td> Aktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenzuweisung</p> </td> 
   <td> <p>Benutzer, dem diese Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Ich wurde als primärer Beauftragter für eine Aufgabe festgelegt.</p> <p>Der Aufgabenbevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn er zum primären Bevollmächtigten der Aufgabe ernannt wird, es sei denn, der Bevollmächtigte ist der Benutzer, der die Zuweisung vorgenommen hat.</p> <p>Eine Benachrichtigung wird gesendet, wenn der Projektstatus Aktuell ist und die Aufgabe nicht als Abgeschlossen markiert ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabe mit ausstehender Genehmigung</p> </td> 
   <td> <p>Genehmigende Personen</p> </td> 
   <td> <p>Ich muss eine Aufgabe genehmigen.</p> <p>Welche Benutzer eine E-Mail-Benachrichtigung für dieses Ereignis erhalten, hängt davon ab, ob die Einstellung „Genehmigende Person muss nicht dem Projektteam angehören (für Genehmigungsprozesse, die eine Rolle beinhalten)“ aktiviert ist (wie in <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Konfigurieren globaler Genehmigungseinstellungen</a> beschrieben). </p> <p>Wenn diese Option </strong> ist, wird eine E-Mail-Benachrichtigung an alle Benutzer im System mit dem Aufgabengebiet „Genehmiger“ gesendet.</p> <p>Wenn diese Option deaktiviert ist</strong> erhalten nur Mitglieder des Projektteams mit dem Aufgabengebiet „Genehmiger“ eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus zum Zeitpunkt der Anfrage aktuell ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabe mit ausstehender Genehmigung</p> </td> 
   <td> <p>Delegierte genehmigende Person</p> </td> 
   <td> <p>Ich muss eine an mich delegierte Aufgabengenehmigung prüfen.</p> <p>Wenn jemand eine Problemgenehmigung an einen anderen Benutzer delegiert, wird dieser Benutzer benachrichtigt. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus zum Zeitpunkt der Anfrage aktuell ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Arbeitszeittabelle</p> </td> 
   <td> <p>Arbeitszeittabelle wieder geöffnet</p> </td> 
   <td> <p>Benutzer, zu dem die Arbeitszeittabelle gehört</p> </td> 
   <td> <p>Meine Arbeitszeittabelle ist wieder geöffnet.</p> <p>Der Arbeitszeittabellen-Besitzer erhält eine E-Mail-Benachrichtigung, wenn die Arbeitszeittabelle erneut geöffnet wird, es sei denn, der Benutzer, der die Arbeitszeittabelle erneut geöffnet hat, ist auch Besitzer der Arbeitszeittabelle.</p> <p>Eine E-Mail-Benachrichtigung wird nur gesendet, wenn der Arbeitszeittabellen-Status Offen ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Arbeitszeittabelle</p> </td> 
   <td> <p>Arbeitszeittabellen-Ablehnung</p> </td> 
   <td> <p>Benutzer, zu dem die Arbeitszeittabelle gehört</p> </td> 
   <td> <p>Meine Arbeitszeittabelle wurde abgelehnt.</p> <p>Der Arbeitszeittabellen-Besitzer erhält eine E-Mail-Benachrichtigung, wenn die Arbeitszeittabelle abgelehnt wird, es sei denn, der Benutzer, der die Arbeitszeittabelle abgelehnt hat, ist auch der Besitzer.</p> <p>Eine E-Mail-Benachrichtigung wird nur gesendet, wenn der Arbeitszeittabellen-Status Abgelehnt ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Arbeitszeittabelle</p> </td> 
   <td> <p>Einreichung der Arbeitszeittabelle</p> </td> 
   <td> <p>Genehmigende Person</p> </td> 
   <td> <p>Ich muss eine Arbeitszeittabelle genehmigen.</p> <p>Die genehmigende Person für Arbeitszeittabellen erhält eine E-Mail-Benachrichtigung, wenn eine Arbeitszeittabelle eingereicht wird, die sie genehmigen muss, es sei denn, die Person, die die Arbeitszeittabelle gesendet hat, ist auch die genehmigende Person für Arbeitszeittabellen.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Status der Arbeitszeittabelle übermittelt wurde.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Zuweisung</p> </td> 
   <td> <p>Arbeitsauftrag</p> </td> 
   <td> <p>Mitglieder des Teams, für das das Element angefordert wird</p> </td> 
   <td> <p>Mein Team erhält einen neuen Arbeitsauftrag.</p> <p>Teammitglieder erhalten eine E-Mail-Benachrichtigung, wenn das Team eine neue Arbeitsanfrage erhält. (Der Benutzer, der die Anfrage gesendet hat, erhält keine Benachrichtigung, wenn er Mitglied des Teams ist.)</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus zum Zeitpunkt der Arbeitsanfrage aktuell und der Arbeitsanfragestatus Neu ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Zuweisung</p> </td> 
   <td> <p>Arbeitsauftrag</p> </td> 
   <td> <p>Benutzer, für den das Arbeitselement angefordert wird</p> </td> 
   <td> <p>Ich erhalte einen neuen Arbeitsauftrag.</p> <p>Der Bevollmächtigte des Arbeitselements erhält eine E-Mail-Benachrichtigung, es sei denn, der Benutzer, der die Anfrage stellt, ist auch der Bevollmächtigte. </p> <p>Eine Benachrichtigung wird nicht gesendet, wenn der Aufgabenstatus „Abgeschlossen“ oder der Problemstatus „Geschlossen“ ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus zum Zeitpunkt der Anfrage aktuell ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Von mir eingereichte Anfragen

Siehe auch [Benachrichtigungen: Von mir eingereichte Anfragen](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

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
   <th> Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Statusänderung der Dokumentengenehmigung</p> </td> 
   <td> <p>Anfragender</p> </td> 
   <td> <p>Eine Dokumentengenehmigungsanfrage ist abgeschlossen.</p> <p>Der Antragsteller erhält eine E-Mail-Benachrichtigung, wenn die Anforderung zur Dokumentgenehmigung abgeschlossen ist.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokumentanforderung abgeschlossen</p> </td> 
   <td> <p>Anfragender</p> </td> 
   <td> <p>Anforderung zum Hochladen eines Dokuments wurde ausgeführt.</p> <p>Der Antragsteller erhält eine E-Mail-Benachrichtigung, wenn eine Anforderung zum Hochladen eines Dokuments erfüllt ist.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Anfrage hinzufügen</p> </td> 
   <td> <p>Anfrage Primärer Kontakt</p> </td> 
   <td> <p>Ich füge einem Projekt eine Anfrage hinzu.</p> <p>Der primäre Kontakt für ein Problem erhält eine Benachrichtigung, wenn er ein Problem in einem Projekt hinzufügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td>Problemzuweisung</td> 
   <td>Anfrage Primärer Kontakt</td> 
   <td> <p>Jemand wurde einem Problem zugewiesen, für das ich der primäre Ansprechpartner bin.</p> <p>Der primäre Kontakt für ein Problem erhält eine Benachrichtigung, wenn das Problem einem Benutzer zugewiesen wird. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> Inaktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Abgeschlossenes Problem</p> </td> 
   <td> <p>Anfrage Primärer Kontakt</p> </td> 
   <td> <p>Eine Anfrage, für die ich der primäre Ansprechpartner bin, wurde abgeschlossen.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektstatusänderung</p> </td> 
   <td> <p>Benutzer, der das Projekt erstellt hat (eingegeben von)</p> </td> 
   <td> <p>Der Status eines von mir erstellten Projekts ändert sich.</p> <p>Der Benutzer, der das Projekt erstellt hat, erhält eine E-Mail-Benachrichtigung, wenn sich der Projektstatus ändert.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Hinzufügung anfordern</p> </td> 
   <td> <p>Anfrage Primärer Kontakt</p> </td> 
   <td> <p>Ich sende eine Anfrage (Bestätigung).</p> <p>Der Primäre Kontakt für das Problem erhält eine E-Mail-Benachrichtigung, wenn er ein Problem sendet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und wenn das Projekt eine Helpdesk-Ansicht verwendet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Zuweisung anfordern</p> </td> 
   <td> <p>Anfrage Primärer Kontakt</p> </td> 
   <td> <p>Jemand wurde meiner Anfrage zugewiesen.</p> <p>Der primäre Kontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn ein Benutzer dem Problem zugewiesen ist, es sei denn, der primäre Kontakt und der zugewiesene Benutzer sind dieselben Benutzer.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und wenn das Projekt eine Helpdesk-Ansicht verwendet.</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Anforderung geschlossen</p> </td> 
   <td> <p>Anfrage Primärer Kontakt</p> </td> 
   <td> <p>Meine Anfrage ist geschlossen (Bestätigung).</p> <p>Der primäre Kontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn die Anfrage geschlossen wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und wenn das Projekt eine Helpdesk-Ansicht verwendet.</p> <p>Wenn die Benachrichtigungen für „Abschließen von Problemen“ aktiviert sind, erfolgt immer der Trigger statt des Felds „Abgeschlossene Anfrage an Primären Kontakt für das Problem“. Wenn Sie möchten, dass diese Benachrichtigung zu einem Trigger wird, müssen Sie die Benachrichtigungen zum Abschluss von Problemen deaktivieren.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokumentanforderung hinzugefügt</p> </td> 
   <td> <p>Anfrage Primärer Kontakt</p> </td> 
   <td> <p>Ein Dokument zu einem Problem, für das ich der primäre Ansprechpartner bin, wurde geändert oder hochgeladen.</p> <p>Der primäre Kontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn ein Dokument zu dem Problem hochgeladen oder geändert wird, es sei denn, der Benutzer, der das Dokument hochgeladen oder geändert hat, ist auch der primäre Kontakt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und wenn für das Projekt "Publish als Warteschlange für Hilfeanfragen“ auf der Registerkarte „Warteschlangeneinrichtung“ aktiviert ist.</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Änderung des Anforderungsstatus</p> </td> 
   <td> <p>Anfrage Primärer Kontakt</p> </td> 
   <td> <p>Der Status meiner Anfrage ändert sich.</p> <p>Der primäre Kontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn sich der Problemstatus ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der primäre Kontakt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und das Projekt eine Helpdesk-Ansicht verwendet.</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## Kommunikation

Siehe auch [Benachrichtigungen: Kommunikation](../../../workfront-basics/using-notifications/notifications-communication.md).

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
   <th> Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Kommentar zu Dokument</p> </td> 
   <td> <p>Dokumentbesitzer</p> </td> 
   <td> <p>Ein Kommentar zu meinem Dokument wird hinzugefügt.</p> <p>Der Verantwortliche für ein Dokument in Workfront erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar zu einem Dokument veröffentlicht wird, es sei denn, der Benutzer, der den Kommentar veröffentlicht hat, ist auch der Verantwortliche für das Dokument.</p> <p>Alle Benutzer, die direkt in den Kommentar eingeschlossen sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist. </p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Kommentar zu &lt;Anfragename&gt; auf &lt;Projektname&gt; (ref# &lt;Anfragenummer&gt;)</em></p> <p> Der Betreff der täglichen Digest-Benachrichtigung ist: <em> der Kommunikation &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Notiz</p> </td> 
   <td> <p>Hinzufügung von Notizen anfordern</p> </td> 
   <td> <p>Anfrage Primärer Kontakt</p> </td> 
   <td> <p>Wenn ein Kommentar zu einer Anfrage gepostet wird, senden Sie eine E-Mail an den primären Kontakt für das Problem.</p> <p>Der primäre Kontakt für ein Problem erhält eine E-Mail-Benachrichtigung, wenn ein Kommentar zu einer Anfrage gepostet wird, es sei denn, der Benutzer, der den Kommentar gepostet hat, ist auch der primäre Kontakt für das Problem.</p> <p>Alle Benutzer, die direkt in dem Kommentar enthalten sind, erhalten ebenfalls eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td>Gezielte Aktualisierung</td> 
   <td>Benutzerin oder Benutzer</td> 
   <td> <p>Jemand schließt mich in eine direkte Aktualisierung ein.</p> <p>Eine direkte Aktualisierung liegt vor, wenn ein Benutzer einen anderen Benutzer explizit in eine Aktualisierung einbezieht, wie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Andere bei Aktualisierungen </a>.</p> <p>In diesem Fall erhält der Benutzer, der an der weitergeleiteten Aktualisierung beteiligt ist, eine E-Mail-Benachrichtigung über die Aktualisierung.</p> <p>Die E-Mail-Benachrichtigung wird nur gesendet, wenn der/die Benutzende Zugriffsrechte auf das Objekt hat und es im Profil aktiviert lässt.  </p> <p>Diese Ereignisbenachrichtigung ist standardmäßig aktiviert und kann nicht deaktiviert werden.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Gezielte Aktualisierung</p> </td> 
   <td> <p>Team-Mitglieder</p> </td> 
   <td> <p>Jemand schließt mein Team in eine direkte Aktualisierung ein.</p> <p>Eine direkte Aktualisierung liegt vor, wenn ein Benutzer einen anderen Benutzer explizit in eine Aktualisierung einbezieht, wie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Andere bei Aktualisierungen </a>.</p> <p>In diesem Fall erhält jedes Teammitglied, das an der weitergeleiteten Aktualisierung beteiligt ist, eine E-Mail-Benachrichtigung über die Aktualisierung.</p> <p>Die E-Mail-Benachrichtigung wird nur an Benutzer gesendet, die über Zugriffsrechte für das Objekt der Aktualisierung verfügen.</p> <p>Wenn der Benutzer, der die direkte Aktualisierung sendet, Mitglied des Teams ist, das die Aktualisierung sendet, erhält der Benutzer, der die Aktualisierung sendet, keine E-Mail-Benachrichtigung.</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Notiz</p> </td> 
   <td> <p>Kommentar zum Arbeitselement</p> </td> 
   <td> <p>Thread-Teilnehmer</p> </td> 
   <td> <p>Jemand kommentiert einen Thread, an dem ich teilnehme.</p> <p>Teilnehmer am Thread und Benutzer, die in einer Direktnachricht enthalten sind, erhalten eine E-Mail-Benachrichtigung, wenn ein Benutzer einen Kommentar im Thread abgibt.</p> <p>Benutzer müssen Lesezugriff haben, um eine Benachrichtigung zu erhalten.</p> <p>Die folgenden Benutzer erhalten keine Benachrichtigung:</p> 
    <ul> 
     <li> <p>Teams, die in einer Direktnachricht enthalten sind</p> </li> 
     <li> <p>Der Besitzer der Notiz</p> </li> 
     <li> <p>Der Primäre Ansprechpartner</p> </li> 
    </ul> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Notiz</p> </td> 
   <td> <p>Kommentar zum Arbeitselement</p> </td> 
   <td> <p>Zugewiesenes Arbeitselement</p> </td> 
   <td> <p>Jemand kommentiert eines meiner Arbeitselemente.</p> <p>Der Bevollmächtigte des Arbeitselements erhält jedes Mal eine E-Mail-Benachrichtigung, wenn ein Benutzer ein Update zu einem Arbeitselement hinzufügt, es sei denn, der Benutzer, der das Update hinzufügt, ist auch der Bevollmächtigte.</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Notiz</p> </td> 
   <td> <p>Antwort auf Arbeitsauftrag</p> </td> 
   <td> <p> Arbeitsauftrag</p> </td> 
   <td> <p>Jemand antwortet auf meine Anfrage.</p> <p>Nachdem ein(e) Benutzende(r) eine Anfrage gesendet hat und ein(e) andere(r) Benutzende(r) auf diese Anfrage antwortet, erhält der/die Benutzende, der/die die Anfrage gesendet hat, eine E-Mail-Benachrichtigung.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn:</p> 
    <ul> 
     <li> <p>Der Benutzer, der antwortet, ist derselbe Benutzer, der die Anfrage gestellt hat</p> </li> 
     <li> <p>Der/die Benutzende hat keinen Zugriff, um die Anmerkung anzuzeigen</p> </li> 
    </ul> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## Genehmigungsinformationen

Siehe auch [Benachrichtigungen: Genehmigungsinformationen](../../../workfront-basics/using-notifications/notifications-approval-information.md).

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
   <th> Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Genehmigungsdelegierung</p> </td> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Ich wurde als genehmigende Person beauftragt.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Delegierte Problemgenehmigung - Statusänderung</p> </td> 
   <td> <p>Benutzer, der die Genehmigung delegiert hat</p> </td> 
   <td> <p>Eine delegierte Anfragegenehmigungsanfrage wurde abgeschlossen. </p> <p>Wenn Sie eine Problemgenehmigung an eine andere Person delegieren, erhalten Sie eine E-Mail-Benachrichtigung, sobald diese die Genehmigung für das Problem abgeschlossen hat (unabhängig davon, ob sie die Problemgenehmigung genehmigt oder ablehnt). </p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Delegierte Projektgenehmigung - Statusänderung</p> </td> 
   <td> <p>Benutzer, der die Genehmigung delegiert hat</p> </td> 
   <td> <p>Eine delegierte Projektgenehmigungsanfrage ist abgeschlossen.</p> <p>Wenn Sie eine Projektgenehmigung an eine andere Person delegieren, erhalten Sie nach Abschluss der Genehmigung eine E-Mail-Benachrichtigung (unabhängig davon, ob diese Person die Projektgenehmigung genehmigt oder ablehnt).</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Delegierte Aufgabengenehmigung - Statusänderung</p> </td> 
   <td> <p>Benutzer, der die Genehmigung delegiert hat</p> </td> 
   <td> <p>Ein delegierter Aufgabengenehmigungsstatus ist abgeschlossen.</p> <p>Wenn Sie eine Aufgabengenehmigung an eine andere Person delegieren, erhalten Sie nach Abschluss der Genehmigung eine E-Mail-Benachrichtigung (unabhängig davon, ob diese Person die Aufgabengenehmigung genehmigt oder ablehnt).</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Stornierung der Dokumentgenehmigung an genehmigende Person</p> </td> 
   <td> <p>Benutzer, der die Genehmigung delegiert hat</p> </td> 
   <td> <p>Ein Ersuchen um Genehmigung eines Dokuments wurde zurückgenommen.</p> <p>Der Dokument-Genehmiger des Dokuments erhält eine E-Mail-Benachrichtigung, wenn die Dokumentgenehmigungsanfrage storniert wird.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Arbeitszeittabelle</p> </td> 
   <td> <p>Arbeitszeittabellen-Genehmigung</p> </td> 
   <td> <p>Benutzer, zu dem die Arbeitszeittabelle gehört</p> </td> 
   <td> <p>Meine Arbeitszeittabelle wurde genehmigt.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informationen über mir zugewiesene Arbeiten

Siehe auch [Benachrichtigungen: Informationen zu meiner Arbeit](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

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
   <th> Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Aufgabe</td> 
   <td>Alle Vorgängeraufgaben abgeschlossen</td> 
   <td>Mitglieder des Teams, die abhängigen Aufgaben zugewiesen wurden</td> 
   <td> <p>Alle Vorgängeraufgaben des Teams sind abgeschlossen.</p> <p>Die Verantwortlichen für die Aufgabe (alle Mitglieder des Teams) erhalten eine E-Mail-Benachrichtigung.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td>Inaktiv</td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Alle Vorgängeraufgaben abgeschlossen</p> </td> 
   <td> <p>Benutzer, der abhängigen Aufgaben zugewiesen wurde</p> </td> 
   <td> <p>Alle Vorgänger meiner Aufgaben sind abgeschlossen.</p> <p>Der Aufgabenbevollmächtigte erhält eine E-Mail-Benachrichtigung.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Genehmigungsentscheidung</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen ist</p> </td> 
   <td> <p>Ein von mir bearbeitetes Problem wurde genehmigt oder abgelehnt.</p> <p>Der Verantwortliche für ein Problem erhält eine E-Mail-Benachrichtigung, wenn eine Genehmigungsentscheidung getroffen (genehmigt oder abgelehnt) wird.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Genehmigungsentscheidung</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Eine von mir abgeschlossene Aufgabe wird genehmigt oder abgelehnt.</p> <p>Der Aufgabenbearbeiter erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe genehmigt oder abgelehnt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Abgeschlossenes Problem</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen ist</p> </td> 
   <td> <p>Ein Problem, das mir zugewiesen ist, wurde abgeschlossen.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Geplantes Abschlussdatum für Problem hat sich geändert</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen ist</p> </td> 
   <td> <p>Das Fälligkeitsdatum eines Problems, dem ich zugewiesen bin, ändert sich.</p> <p>Der Problem-Verantwortliche erhält eine E-Mail-Benachrichtigung, wenn sich das geplante Abschlussdatum ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Verantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus nicht „Planung“ lautet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Änderung des Anfragestatus</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen ist</p> </td> 
   <td> <p>Der Status eines meiner Arbeitselemente ändert sich.</p> <p>Der Verantwortliche für das Problem erhält eine E-Mail-Benachrichtigung, wenn sich der Status ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Verantwortliche.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokumentanforderung hinzugefügt</p> </td> 
   <td> <p>Benutzer, dem das Problem zugewiesen ist</p> </td> 
   <td> <p>Dokumente zu Anfragen, denen ich zugewiesen bin, werden hochgeladen oder geändert.</p> <p>Der Anfragebevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn Dokumente zu einem von ihm hinzugefügten Problem hochgeladen oder geändert werden.</p> <p>Eine E-Mail-Benachrichtigung wird nicht gesendet, wenn der Benutzer, der das Problem eingegeben hat, der Problembearbeiter ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und wenn für das Projekt "Publish als Warteschlange für Hilfeanfragen“ auf der Registerkarte „Warteschlangeneinrichtung“ aktiviert ist.</p> </td> 
   <td> <p>Aktiv (nur täglich)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Eine Aufgabe, der ich zugewiesen bin, wurde abgeschlossen.</p> <p>Der Aufgabenbevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn die Aufgabe abgeschlossen ist. Nach Abschluss einer persönlichen Aufgabe werden keine Benachrichtigungen gesendet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> <p>Benutzende mit einer Light-, Contributor-, Review- oder Requestor-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Der abhängigen Aufgabe zugewiesener Benutzer</p> </td> 
   <td> <p>Ein Vorgänger einer meiner Aufgaben ist abgeschlossen.</p> <p>Der Aufgabenbevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn einer der Vorgänger seiner Aufgabe abgeschlossen wurde.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Geplantes Abschlussdatum für Aufgabe hat sich geändert</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Das Fälligkeitsdatum einer Aufgabe, der ich zugewiesen bin, ändert sich.</p> <p>Der Aufgabenbearbeiter erhält eine E-Mail-Benachrichtigung, wenn sich das geplante Abschlussdatum der Aufgabe ändert, es sei denn, der Benutzer, der das geplante Abschlussdatum geändert hat, ist auch der Aufgabenbearbeiter.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus nicht „Planung“ lautet.</p> <p>Es wird keine Benachrichtigung bezüglich persönlicher Aufgaben gesendet.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Statusänderung der Aufgabe</p> </td> 
   <td> <p>Benutzer, dem die Aufgabe zugewiesen ist</p> </td> 
   <td> <p>Der Status einer Aufgabe, der ich zugewiesen bin, ändert sich.</p> <p>Der Aufgabenbevollmächtigte erhält eine E-Mail-Benachrichtigung, wenn sich der Status der Aufgabe ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Bevollmächtigte.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## Informationen über Projekte, an denen ich mitwirke

Siehe auch [Benachrichtigungen: Informationen zu Projekten, an denen ich mitwirke](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

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
   <th> Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Aktueller Projektstatus</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ein Projekt, an dem ich mitarbeite, ist jetzt aktiv.</p> <p>Projektbenutzer erhalten eine E-Mail-Benachrichtigung, wenn das Projekt aktiv wird.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument hinzufügen</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Einem Projekt, an dem ich mitarbeite, wurde ein Dokument hinzugefügt.</p> <p>Benutzende im Projekt-Team erhalten eine E-Mail-Benachrichtigung, wenn ein Dokument zum Projekt hinzugefügt wird, mit Ausnahme der Benutzenden, die das Dokument hinzugefügt haben.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ und das Dokument nicht „Privat“ ist. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Anfrage hinzufügen</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Einem Projekt, an dem ich mitarbeite, wurde eine Anfrage hinzugefügt.</p> <p>Benutzer in einem Projekt erhalten eine E-Mail-Benachrichtigung, wenn ein Problem zum Projekt hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Abgeschlossenes Problem</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>In einem Projekt, an dem ich mitarbeite, wurde eine Anfrage gelöst.</p> <p>Jeder Benutzer im Projekt erhält eine Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Meilensteinaufgabe abgeschlossen</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>In einem Projekt, an dem ich mitarbeite, wurde eine Meilensteinaufgabe abgeschlossen.</p> <p>Alle Benutzer im Projektteam erhalten eine Benachrichtigung, wenn eine Meilensteinaufgabe abgeschlossen ist. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektabschluss</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ein Projekt, an dem ich mitarbeite, ist abgeschlossen.</p> <p>Benutzer eines Projekt-Teams erhalten eine E-Mail-Benachrichtigung, wenn der Projektstatus „abgeschlossen“ ist.</p> <p>Tipp: Wenn Projekte regelmäßig abgeschlossen werden, kann durch Aktivieren dieser Option eine große Anzahl von E-Mails für Benutzer erstellt werden, die nur über eine begrenzte Anzahl von Aufgaben in vielen Projekten verfügen. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektstatusänderung</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Der Status eines Projekts, an dem ich mitarbeite, ändert sich.</p> <p>Benutzer im Projektteam erhalten eine E-Mail-Benachrichtigung, wenn sich der Status des Projekts ändert. </p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projektbenutzer</p> </td> 
   <td> <p>Projektbenutzer hinzufügen</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Ich werde zu einem Projekt hinzugefügt.</p> <p>Der Benutzer, der zum Projekt hinzugefügt wurde, erhält eine E-Mail-Benachrichtigung, wenn er hinzugefügt wird, es sei denn, der Benutzer wurde selbst zum Projekt hinzugefügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>In einem Projekt, an dem ich mitarbeite, wurde eine Aufgabe abgeschlossen.</p> <p>Mitglieder des Projektteams erhalten eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Nicht zugewiesene Anfrage hinzugefügt</p> </td> 
   <td> <p>Mitglieder des Projektteams</p> </td> 
   <td> <p>Einem Projekt, an dem ich mitarbeite, wurde eine nicht zugewiesene Anfrage hinzugefügt.</p> <p>Projektbenutzer erhalten eine E-Mail-Benachrichtigung, wenn ein nicht zugewiesenes Problem zum Projekt hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informationen über Projekte in meinem Besitz

Siehe auch [Benachrichtigungen: Informationen zu Projekten in meinem Besitz](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

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
   <th> Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument hinzufügen</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein Dokument wird einem Projekt in meinem Besitz hinzugefügt.</p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn ein Dokument zum Projekt hinzugefügt wird, es sei denn, der Benutzer, der das Dokument hinzugefügt hat, ist auch der Projektbesitzer.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ und das Dokument nicht „Privat“ ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Anfrage hinzufügen</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein Problem wird einem Projekt in meinem Besitz hinzugefügt.</p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn ein Problem zum Projekt hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Änderung des Verpflichtungsdatums für ein Problem</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Das Commit-Datum ändert sich für ein Problem in einem meiner Projekte.</p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn sich das Commit-Datum für ein Problem im Projekt ändert, es sei denn, der Benutzer, der das Commit-Datum ändert, ist derselbe Benutzer wie der Projektbesitzer.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Abgeschlossenes Problem</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein Problem wurde in einem Projekt abgeschlossen, dessen Besitzer ich bin.</p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Meilensteinaufgabe abgeschlossen</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Eine Meilensteinaufgabe wurde in einem Projekt abgeschlossen, dessen Besitzer ich bin.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektbesitzer-Zuweisung</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ich wurde als Besitzer eines neuen Projekts festgelegt.</p> <p>Wenn ein Benutzer als Eigentümer eines Projekts zugewiesen wird, erhält dieser Benutzer eine E-Mail-Benachrichtigung.</p> <p>Wenn der Projektbesitzer derselbe Benutzer ist, der den Arbeitsauftrag erteilt hat, wird keine E-Mail-Benachrichtigung gesendet</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Änderung des Projektstatus</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Ein Projekt, dessen Besitzer ich bin, steht hinter mir.</p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn das Projekt in Verzug ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Änderung des Commit-Datums für Aufgabe</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Das Commit-Datum ändert sich für eine Aufgabe in einem meiner Projekte.</p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn sich das Commit-Datum für eine Aufgabe im Projekt ändert, es sei denn, der Benutzer, der das Commit-Datum geändert hat, ist auch der Projektbesitzer.</p> </td> 
   <td> <p>Aktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Eine Aufgabe wird in einem Projekt abgeschlossen, dessen Besitzer ich bin.</p> <p>Der Projektbesitzer erhält eine Benachrichtigung. </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Änderung beim Aufgabenfortschritt</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Eine Aufgabe aus einem Projekt, dessen Besitzer ich bin, steht hinter mir.</p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn eine Aufgabe für das Projekt in Verzug gerät.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Nicht zugewiesene Anfrage hinzufügen</p> </td> 
   <td> <p>Projektbesitzer</p> </td> 
   <td> <p>Einem Projekt in meinem Besitz wird eine nicht zugewiesene Anfrage hinzugefügt.</p> <p>Der Projektbesitzer erhält eine E-Mail-Benachrichtigung, wenn ein nicht zugewiesenes Problem zum Projekt hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Informationen über Projekte, die ich sponsere

Siehe auch [Benachrichtigungen: Informationen zu Projekten, die ich als Sponsor unterstütze](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

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
   <th> Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokument hinzufügen</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Einem Projekt, dessen Sponsor ich bin, wird ein Dokument hinzugefügt.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn ein Dokument zum Projekt hinzugefügt wird, es sei denn, das Dokument wird vom Projektsponsor hinzugefügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ und das Dokument nicht „Privat“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Anfrage hinzufügen</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Einem Projekt, das ich als Sponsor unterstütze, wird eine Anfrage hinzugefügt.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn ein Problem zum Projekt hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Abgeschlossenes Problem</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>In einem Projekt, das ich als Sponsor unterstütze, wurde eine Anfrage gelöst.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Meilensteinaufgabe abgeschlossen</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>In einem Projekt, das ich als Sponsor unterstütze, wurde eine Meilensteinaufgabe abgeschlossen.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn eine Meilensteinaufgabe für ein Projekt abgeschlossen wurde, das er als Sponsor unterstützt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Änderung des Projektstatus</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Ein Projekt, das ich als Sponsor unterstütze.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn das Projekt in Verzug gerät.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projektsponsor-Zuweisung</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Ich bin als Sponsor für ein Projekt festgelegt.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn er als Sponsor eines Projekts festgelegt wird.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenabschluss</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>In einem Projekt, das ich als Sponsor unterstütze, wird eine Aufgabe abgeschlossen.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Änderung beim Aufgabenfortschritt</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Eine Aufgabe aus einem Projekt, das ich als Sponsor unterstütze.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn eine Aufgabe für das Projekt in Verzug gerät.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Nicht zugewiesene Anfrage hinzufügen</p> </td> 
   <td> <p>Projektsponsor</p> </td> 
   <td> <p>Einem Projekt, das ich als Sponsor unterstütze, wird eine nicht zugewiesene Anfrage hinzugefügt.</p> <p>Der Projektsponsor erhält eine E-Mail-Benachrichtigung, wenn ein nicht zugewiesenes Problem zum Projekt hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verschiedene Informationen

Siehe auch [Benachrichtigungen: Sonstige Informationen](../../../workfront-basics/using-notifications/notifications-misc-information.md).

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
   <th> Standardzustand</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ankündigung</td> 
   <td> <p>Ankündigng wurde hinzugefügt.</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Eine Nachricht wird an die Ankündigungszentrale gesendet.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument</p> </td> 
   <td> <p>Dokumentanforderung abbrechen</p> </td> 
   <td> <p>Benutzer, von dem das Dokument angefordert wird</p> </td> 
   <td> <p>Bricht eine Anfrage zum Hochladen eines Dokuments ab.</p> <p>Der angeforderte Dokumentverantwortliche erhält eine E-Mail-Benachrichtigung, wenn eine Dokumentanforderung abgebrochen wird.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>Fehlerbenachrichtigung</p> </td> 
   <td> <p></p> </td> 
   <td> <p>Es wurde ein Fehler gefunden, der Ihre Aufmerksamkeit erfordert.</p> <p>Nach dem Versuch von Workfront, eine Verbindung zu einem POP-Konto herzustellen, wird eine E-Mail-Benachrichtigung generiert. Nach 25 Versuchen deaktiviert Workfront die Verbindung zum POP-Konto, um Ressourcen zu erhalten, und sendet eine Benachrichtigung. </p> <p>Die E-Mail-Benachrichtigung wird an den Projektbesitzer gesendet, wenn die POP-E-Mail mit einer Anfrage-Warteschlange verknüpft ist, oder an die Workfront-Administratoren, wenn das POP-Konto mit der Funktion „Eingehende E-Mails“ im E-Mail-Setup verknüpft ist.
   </p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Problem</p> </td> 
   <td> <p>Problemzuweisung</p> </td> 
   <td> <p>Ressourcenbesitzer</p> </td> 
   <td> <p>Eine Änderung bei einer Problemzuweisung wirkt sich auf mein Team aus.</p> <p>Der Manager des Problemzugewiesenen erhält eine E-Mail-Benachrichtigung, wenn eine Änderung einen von ihm verwalteten Benutzer betrifft.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ oder „Planung“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Neuer Benutzer</p> </td> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Wenn ein neuer Benutzer in Workfront erstellt wird, den Benutzer per E-Mail benachrichtigen.</p> <p>Nachdem der neue Benutzer erstellt wurde, erhält er eine E-Mail-Einladung, die ihn darüber informiert, dass ein Workfront-Konto erstellt wurde, und ihn auffordert, sein Kennwort festzulegen.</p> <p>Beim Erstellen eines neuen Benutzers können Benutzer die Option „Einladungs-E-Mail an diese Person senden“ auswählen (wie in <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Benutzer hinzufügen</a><span style="font-weight: 400;"> beschrieben). Wenn die Option „Neuer Benutzer an Benutzer“ jedoch global aktiviert ist, erhalten alle neuen Benutzer die E-Mail-Einladung, unabhängig davon, ob die Option „Einladungs-E-Mail an diese Person senden“ ausgewählt ist.</span></p> </td> 
   <td> Inaktiv </td> 
  </tr> 
  <tr> 
   <td> <p>Team</p> </td> 
   <td> <p>Objektfreigabe</p> </td> 
   <td> <p>Mitglieder des Teams, für das das Objekt freigegeben wurde</p> </td> 
   <td> <p>Jemand hat ein Objekt für mein Team freigegeben.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzerin oder Benutzer</p> </td> 
   <td> <p>Objektfreigabe</p> </td> 
   <td> <p>Benutzer, für den das Objekt freigegeben wurde</p> </td> 
   <td> <p>Jemand hat ein Objekt für mich freigegeben.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projektbenutzer</p> </td> 
   <td> <p>Projektbenutzer hinzufügen</p> </td> 
   <td> <p>Ressourcenbesitzer</p> </td> 
   <td> <p>Einer meiner Mitarbeiter wird einem Projekt hinzugefügt.</p> <p>Ein Manager erhält eine E-Mail-Benachrichtigung, wenn einem Projekt ein Direktbericht hinzugefügt wird.</p> <p>Benutzende mit einer Light- oder Review-Lizenz erhalten keine Benachrichtigung.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>Projekt einem Portfolio oder Programm hinzugefügt</p> </td> 
   <td> <p>Portfolio- oder Programmbesitzer</p> </td> 
   <td> <p>Jemand fügt ein Projekt einem Portfolio oder Programm hinzu, dessen Besitzer ich bin.</p> </td> 
   <td> <p>Aktiv (nur Sofort)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe</p> </td> 
   <td> <p>Aufgabenzuweisung</p> </td> 
   <td> <p>Ressourcenbesitzer</p> </td> 
   <td> <p>Eine Aufgabenzuweisung wirkt sich auf einen meiner Mitarbeiter aus.</p> <p>Der Manager des Aufgabenempfängers erhält eine E-Mail-Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist.</p> </td> 
   <td> <p>Inaktiv</p> </td> 
  </tr> 
  <tr> 
   <td> Projekt <br>Aufgabe <br>Problem</td> 
   <td>Neues Update</td> 
   <td>Abonnent </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">Eine E-Mail wird gesendet, wenn eine Aktualisierung für eine Aufgabe, ein Problem oder ein Projekt durchgeführt wird, die bzw. das ich abonniert habe.</span> </p> </td> 
   <td>Aktiv (nur Sofort)</td> 
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

Siehe auch [Benachrichtigungen: Delegierung](../../../workfront-basics/using-notifications/notifications-delegation.md).

| Objekttyp | Ereignis | Empfänger | Beschreibung | Standardzustand |
|------------------|--------------------------------------------|-----------|--------------------------------------------------------------|-----------------------|
| Aufgaben und Probleme | Delegierung von Aufgaben und Problemen | Zugewiesene Person | Ich delegiere meine Aufgaben und Probleme (Bestätigung) | Aktiv (nur Sofort) |
| Aufgaben und Probleme | Delegierung von Aufgaben und Problemen beenden | Zugewiesene Person | Ich beende die Delegierung meiner Aufgaben und Probleme (Bestätigung) | Aktiv (nur Sofort) |
| Aufgaben und Probleme | Delegierung von Aufgaben und Problemen | Delegieren | Jemand delegiert Aufgaben und Probleme an mich. | Aktiv (nur Sofort) |
| Aufgaben und Probleme | Beenden der Delegierung von Aufgaben und Problemen | Delegieren | Jemand beendet die Delegierung von Aufgaben und Problemen an mich. | Aktiv (nur Sofort) |
