---
content-type: reference
navigation-topic: notifications
title: "Benachrichtigungen: Anfragen, die ich gestellt habe"
description: Die folgenden Benachrichtigungen informieren Sie über Ihre Anfragen in Adobe Workfront.
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# Benachrichtigungen: Von mir gestellte Anforderungen

Die folgenden Benachrichtigungen teilen Ihnen mit, welche Anforderungen Sie in [!DNL Adobe Workfront] gestellt haben.

Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Ändern Ihrer eigenen E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Anforderungen, die ich gestellt habe</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Anforderung zur Dokumentgenehmigung ist abgeschlossen</strong> </p> <p>Der Benutzer, der eine Genehmigung für ein Dokument angefordert hat, erhält eine E-Mail-Benachrichtigung, wenn die Anforderung zur Dokumentgenehmigung abgeschlossen ist.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist:<em> &lt;Genehmigername&gt; hat &lt;Genehmigungsentscheidung ([!UICONTROL Genehmigt], [!UICONTROL Mit Änderungen genehmigt], [!UICONTROL Abgelehnt])&gt; dieses Dokument.</em></p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </td> 
   <td> Dokumentname<br>Genehmigername </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Dokument wird geändert oder in ein Problem hochgeladen, bei dem ich der primäre Ansprechpartner bin</strong> </p> <p>Der primäre Ansprechpartner des Problems erhält eine E-Mail-Benachrichtigung, wenn ein Dokument hochgeladen oder in einem Problem geändert wird, es sei denn, der Benutzer, der das Dokument hochgeladen oder geändert hat, ist ebenfalls der primäre Ansprechpartner.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (wie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Anforderungswarteschlange erstellen]</a> beschrieben).</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>Dokument hinzugefügt zu &lt;Name des Problems&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist: <em>Digest of Your Requests &lt;Datum des täglichen Digest&gt;</em></p> </td> 
   <td> Objektname, in den das Dokument hochgeladen wurde<br>Übergeordneter Objektname<br>Dokumentenverweisnummer<br>Name des Benutzers, der das Dokument hochgeladen hat<br>Dokumentname<br>Hinzugefügt am Datum<br>Dokumentdetails (Format, Größe, Versionsnummer)<br>Dokumentminiatur<br><strong>[!UICONTROL Vorschau]</strong> und <strong>[!UICONTROL Download]</strong>}*Projektname<br>*Projektnummer<br>*Gesamtanzahl der hochgeladenen Dokumente<br>*Name des Dokuments<br>*Übergeordneter Objektname<br>*Name des Benutzers, der das Dokument hinzugefügt hat<br>*Datum des täglichen Digest<br> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Anforderung zum Hochladen von Dokumenten ist erfüllt</strong> </p> <p>Der Dokumentanfragende erhält eine E-Mail-Benachrichtigung, wenn eine Anforderung zum Hochladen von Dokumenten erfüllt ist.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Ihre Dokumentanforderung von] &lt;Benutzername&gt; wurde erfüllt</em></p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </td> 
   <td> <p>Name des Benutzers, der das Dokument hochgeladen hat<br>Objektname, in den das Dokument hochgeladen wurde<br>Dokumentname<br><br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine persönliche Aufgabe, die ich jemand anderem zugewiesen habe, ist abgeschlossen</strong> </p> <p>Eine Benachrichtigung wird an den Benutzer gesendet, der eine persönliche Arbeitsanfrage an eine andere Person delegiert hat, wenn diese Anfrage abgeschlossen ist. </p>  <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>Task Complete: &lt;Task Name&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </p> </td> 
   <td> Aufgabenname<br>Standardprojektname (Personal Project des Benutzers, der die persönliche Aufgabe erhalten hat)<br>Aufgabenverweisnummer<br>Name des Aufgabeneigentümers<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Weitere Informationen]</strong> Schaltfläche<br><br><br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Problem, bei dem ich der Hauptkontakt bin, ist abgeschlossen</strong> </p> <p>Der Hauptkontakt zu einem Problem erhält nach Abschluss des Problems eine Benachrichtigung.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Problemabwicklung]: &lt;Problemname&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> Digest of your Requests &lt;Datum der täglichen Digest&gt;</em></p> <p> </p> </td> 
   <td> Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Neuer Status<br>Datum und Uhrzeit, zu dem das Problem abgeschlossen wurde<br>Vorheriger Problemstatus<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche <br>*Projektname<br>*Projektverweisnummer<br>*Gesamtzahl abgeschlossener Probleme<br>*Problemname 12}*Name des Benutzers, der das Problem abgeschlossen hat<br>*Datum des täglichen Digest<br> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich füge einem Projekt ein Problem hinzu</strong> </p> <p>Der Hauptkontakt zu einem Problem erhält eine Benachrichtigung, wenn er ein Problem in ein Projekt einfügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Problem gesendet]: &lt;Name des Problems&gt; unter &lt;Projektname&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> Digest of your Requests &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> Projektname<br>Projektname<br>Problemreferenz-Nummer<br>Ihr Portfolio<br>Problemname<br>Eingegebene Datum<br>Problempriorität<br>Problemstatus<br>Zugeordneter Name<br>Primärer Kontakt<br>*Projektname<br>*Projektnummer<br>*Gesamtzahl der hinzugefügten Probleme<br>*Problemname{daily3} Datum Digest<br> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und Täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich sende eine Anforderung (Bestätigung)</strong> </p> <p>Der Primäre Kontakt zu diesem Problem erhält eine E-Mail-Benachrichtigung, wenn er ein Problem sendet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet und das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (wie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Anforderungswarteschlange erstellen]</a> beschrieben).</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Request Submitted]: &lt;Request Name&gt; on &lt;Project (Request Queue) Name&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> Digest of your Requests &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> <p>Projektname (Anforderungswarteschlangenname)<br>Portfolio-Name<br>Problemreferenz-Nummer<br>Problemname<br>Eingegebene Datum<br>Problempriorität<br>Problemstatus<br>Zugeordneter <br>Primärer Kontakt<br>*Projektnummer<br>*Projektname<br>*Gesamtzahl der gesendeten Anforderungen<br>*Anforderungsname<br>*Priorität 3}*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und Täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Meine Anfrage ist geschlossen (Bestätigung)</strong> </p> <p>Der primäre Ansprechpartner des Problems erhält eine E-Mail-Benachrichtigung, wenn die Anfrage geschlossen wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus "Aktuell"lautet und das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (wie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a> beschrieben).</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Ihre Anfrage wurde geschlossen]:"&lt;Anforderungsname&gt;"</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> Anforderungsname<br>Projektname<br>Anforderungsreferenz-Nummer<br>Name des Benutzers, der die Anforderung geschlossen hat<br>Fehlerstatus<br>Datum und Uhrzeit der Schließung der Anforderung<br>Vorheriger Anforderungsstatus<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche<br>*Projektnummer<br>*Projektname<br>*Gesamtzahl der geschlossenen Anforderungen<br>*Anforderungsname<br>}*Name des Benutzers, der die Anforderung geschlossen hat<br>*Datum des täglichen Digest </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Einer meiner Anfrage zugewiesen ist</strong> </p> <p>Der primäre Ansprechpartner für das Problem erhält eine E-Mail-Benachrichtigung, wenn ein Benutzer dem Problem zugewiesen wird, es sei denn, der primäre Ansprechpartner und der zugewiesene Benutzer sind derselbe Benutzer.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt als [!UICONTROL Warteschlange für Hilfeanfragen] eingerichtet ist (wie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Anforderungswarteschlange erstellen]</a> beschrieben).</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>&lt;Name des Benutzers, der Ihrer Anfrage zugewiesen ist&gt; [!UICONTROL wurde Ihrer Anfrage zugewiesen]: "&lt;Anforderungsname&gt;"</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemreferenz-Nummer<br>Anforderungsname<br>Anforderungstyp<br>Eingegebene Datum<br>Problempriorität<br>Primärer Kontakt<br>Geplantes Abschlussdatum<br>Problemstatus<br><strong>Siehe Weitere Informationen</strong> Schaltfläche <br>*Projektname<br>*Projektnummer<br> Gesamtzahl der zugewiesenen Anforderungen{11 4}*Anforderungsname<br>*Zugeordneter Name<br>*Datum des täglichen Digest<br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Der Status ändert sich bei einem Projekt, das ich erstellt habe</strong> </p> <p>Der Benutzer, der das Projekt erstellt hat, erhält eine E-Mail-Benachrichtigung, wenn sich der Projektstatus ändert.</p> <p>Betreff der E-Mail mit sofortiger Benachrichtigung ist: <em>[!UICONTROL Project Status Change]: &lt;Projektname&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> <p>Projektname<br>Projektname<br>Projektnummer<br>Name des Portfolios, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit der Änderung des Projektstatus<br>Vorheriger Projektstatus<br><strong>[!UICONTROL Weitere Informationen]</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br>*Neuer Projektstatus<br>*Name des Benutzers, der den den den Projektstatus<br>*Datum des täglichen Digest</p> </td> 
   <td> <p><strong>Instant</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Der Status ändert sich in meiner Anfrage</strong> </p> <p>Der Hauptkontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn sich der Problemstatus ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der Hauptkontakt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus aktuell ist und das Projekt als [!UICONTROL Warteschlange für Hilfeanfragen] eingerichtet ist (wie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Anforderungswarteschlange erstellen]</a> beschrieben).</p> <p>Der Betreff der E-Mail mit der sofortigen Benachrichtigung lautet: <em>&lt;Anforderungsname&gt; ist &lt;neuer Status&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> Digest of your Requests &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> Anforderungsname<br>Projektname<br>Anforderungsreferenz-Nummer<br>Name des Benutzers, der den Status der Anforderung geändert hat<br>Neuer Status<br>Datum und Uhrzeit der Änderung des Status der Anforderung<br>Vorheriger Anforderungsstatus<br><strong>[!UICONTROL Siehe Weitere Details]</strong> Schaltfläche<br>*Projektname<br>*Projektnummer<br>*Gesamtzahl der Anforderungen, deren Status geändert wurde<br>*Anforderungsname<br>*Vorheriger Anforderungsstatus<br>*Neuer Anforderungsstatus<br>*Name des Benutzers, der den Status geändert hat<br>*Datum des täglichen Digest<br></td> 
   <td> <p><strong>Täglich</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
