---
content-type: reference
navigation-topic: notifications
title: '''Benachrichtigungen: Von mir gestellte Anfragen"'
description: Die folgenden Benachrichtigungen informieren Sie über Ihre Anfragen in Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 6%

---

# Benachrichtigungen: Ich habe

Die folgenden Benachrichtigungen informieren Sie über Ihre Anfragen in [!DNL Adobe Workfront].

Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Von mir eingereichte Anforderungen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Ersuchen um Genehmigung eines Dokuments wurde erstellt.</strong> </p> <p>Der Benutzer, der eine Genehmigung für ein Dokument angefordert hat, erhält eine E-Mail-Benachrichtigung, wenn die Anforderung zur Dokumentgenehmigung abgeschlossen ist.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist:<em> &lt;approver name=""&gt; has &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; dieses Dokument.</em></p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </td> 
   <td> Dokumentname<br>Name des Genehmigers </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Dokument zu einer Anfrage, für die ich der primäre Ansprechpartner bin, wurde geändert oder hochgeladen.</strong> </p> <p>Der primäre Ansprechpartner des Problems erhält eine E-Mail-Benachrichtigung, wenn ein Dokument hochgeladen oder in einem Problem geändert wird, es sei denn, der Benutzer, der das Dokument hochgeladen oder geändert hat, ist ebenfalls der primäre Ansprechpartner.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (wie beschrieben in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Anforderungswarteschlange erstellen]</a>).</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Dokument hinzugefügt zu &lt;issue name=""&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist: <em>Digest of Your Requests &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Objektname, in den das Dokument hochgeladen wurde<br>Übergeordneter Objektname<br>Dokumentenverweisnummer<br>Name des Benutzers, der das Dokument hochgeladen hat<br>Dokumentname<br>Datum hinzugefügt<br>Dokumentdetails (Format, Größe, Versionsnummer)<br>Dokumentminiatur<br><strong>[!UICONTROL Vorschau]</strong> und <strong>[!UICONTROL Download]</strong> Schaltflächen<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der hochgeladenen Dokumente<br>*Name des Dokuments<br>*Übergeordneter Objektname<br>*Name des Benutzers, der das Dokument hinzugefügt hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Anforderung zum Hochladen eines Dokuments wurde ausgeführt</strong> </p> <p>Der Dokumentanfragende erhält eine E-Mail-Benachrichtigung, wenn eine Anforderung zum Hochladen von Dokumenten erfüllt ist.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Ihre Dokumentanforderung von] &lt;user name=""&gt; erfüllt war</em></p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </td> 
   <td> <p>Name des Benutzers, der das Dokument hochgeladen hat<br>Objektname, in den das Dokument hochgeladen wurde<br>Dokumentname<br><br></p> </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine persönliche Aufgabe, die ich jemand anderem zugewiesen habe, ist abgeschlossen.</strong> </p> <p>Eine Benachrichtigung wird an den Benutzer gesendet, der einer anderen Person eine Ad-hoc-Aufgabe zugewiesen hat, wenn diese Aufgabe abgeschlossen ist. </p> <p>Weitere Informationen zu Ad-hoc-Aufgaben finden Sie unter <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">Arbeitselemente aus dem [!UICONTROL Home]-Bereich erstellen</a>.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>Task Complete: &lt;task name=""&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </p> </td> 
   <td> Aufgabenname<br>Standardprojektname (Personal Project des Benutzers, der die persönliche Aufgabe erhalten hat)<br>Aufgabenverweisnummer<br>Name des Aufgabenbesitzers<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Status der vorherigen Aufgabe<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br><br><br></td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Anfrage, für die ich der primäre Ansprechpartner bin, wurde abgeschlossen</strong> </p> <p>Der Hauptkontakt zu einem Problem erhält nach Abschluss des Problems eine Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Problemabwicklung]: &lt;issue name=""&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> Digest of your Requests &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> Problemname<br>Projektname<br>Problemverweisnummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Neuer Status<br>Datum und Uhrzeit des Abschlusses des Problems<br>Status des vorherigen Problems<br><strong>[!UICONTROL Weitere Informationen]</strong> button <br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Probleme<br>*Name des Problems<br>*Name des Benutzers, der das Problem abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich füge dem Projekt eine Anfrage hinzu</strong> </p> <p>Der Hauptkontakt zu einem Problem erhält eine Benachrichtigung, wenn er ein Problem in ein Projekt einfügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Problem gesendet]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> Digest of your Requests &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Projektname<br>Portfolio Name<br>Problemverweisnummer<br>Ihr Name<br>Problemname<br>Eingegebene Daten<br>Problempriorität<br>Problemstatus<br>Zugeordneter Name<br>Primärer Kontakt<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der hinzugefügten Probleme<br>*Name des Problems<br>*Datum der täglichen Zusammenfassung </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich sende eine Anfrage (Bestätigung)</strong> </p> <p>Der Primäre Kontakt zu diesem Problem erhält eine E-Mail-Benachrichtigung, wenn er ein Problem sendet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet und das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (siehe Beschreibung unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Anforderungswarteschlange erstellen]</a>).</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Anfrage gesendet]: &lt;request name=""&gt; on &lt;project request="" queue="" name=""&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> Digest of your Requests &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Projektname (Name der Anforderungswarteschlange)<br>Portfolio Name<br>Problemverweisnummer<br>Problemname<br>Eingegebene Daten<br>Problempriorität<br>Problemstatus<br>Zugeordneter Name<br>Primärer Kontakt<br>*Referenz-Nummer des Projekts<br>*Projektname<br>*Gesamtzahl der eingereichten Anträge<br>*Anforderungsname<br>*Anforderungspriorität<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Meine Anforderung ist geschlossen (Bestätigung)</strong> </p> <p>Der primäre Ansprechpartner des Problems erhält eine E-Mail-Benachrichtigung, wenn die Anfrage geschlossen wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (siehe <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a>).</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Ihre Anfrage wurde geschlossen]:"&lt;request name=""&gt;"</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Anforderungsname<br>Projektname<br>Referenz-Nummer des Antrags<br>Name des Benutzers, der die Anforderung geschlossen hat<br>Problemstatus<br>Datum und Uhrzeit des Schließens der Anforderung<br>Status der vorherigen Anfrage<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Referenz-Nummer des Projekts<br>*Projektname<br>*Gesamtzahl der geschlossenen Anforderungen<br>*Anforderungsname<br>*Name des Benutzers, der die Anforderung geschlossen hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand wurde mit meiner Anfrage beauftragt</strong> </p> <p>Der primäre Ansprechpartner für das Problem erhält eine E-Mail-Benachrichtigung, wenn ein Benutzer dem Problem zugewiesen wird, es sei denn, der primäre Ansprechpartner und der zugewiesene Benutzer sind derselbe Benutzer.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (siehe <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Anforderungswarteschlange erstellen]</a>).</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL wurde Ihrer Anfrage zugewiesen]: "&lt;request name=""&gt;"</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemverweisnummer<br>Anforderungsname<br>Anfragetyp<br>Eingegebene Daten<br>Problempriorität<br>Primärer Kontakt<br>Geplantes Abschlussdatum<br>Problemstatus<br><strong>Siehe Weitere Details</strong> button <br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der zugewiesenen Anfragen<br>*Anforderungsname<br>*Der Name zugewiesen<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Wenn sich der Status eines Projekts ändert, den Benutzer, der das Projekt eingegeben hat, per E-Mail benachrichtigen.</strong> </p> <p>Der Benutzer, der das Projekt erstellt hat, erhält eine E-Mail-Benachrichtigung, wenn sich der Projektstatus ändert.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Änderung des Projektstatus]: &lt;project name=""&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Projektname<br>Portfolio Name<br>Projektnummer<br>Name des Benutzers, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit der Änderung des Projektstatus<br>Vorheriger Projektstatus<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Neuer Projektstatus<br>*Name des Benutzers, der den Projektstatus geändert hat<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td> <p><strong>Sofort</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Die Statusänderungen zu meiner Anforderung</strong> </p> <p>Der Hauptkontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn sich der Problemstatus ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Hauptkontakt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (wie beschrieben in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Anforderungswarteschlange erstellen]</a>).</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>&lt;request name=""&gt; is &lt;new status=""&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> Digest of your Requests &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> Anforderungsname<br>Projektname<br>Referenz-Nummer des Antrags<br>Name des Benutzers, der den Status der Anforderung geändert hat<br>Neuer Status<br>Datum und Uhrzeit der Änderung des Status der Anforderung<br>Status der vorherigen Anfrage<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der Anfragen, deren Status sich geändert hat<br>*Anforderungsname<br>*Status der vorherigen Anfrage<br>*Neuer Anforderungsstatus<br>*Name des Benutzers, der den Status geändert hat<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td> <p><strong>Täglich</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
