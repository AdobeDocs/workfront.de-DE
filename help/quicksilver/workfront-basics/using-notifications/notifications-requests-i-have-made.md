---
content-type: reference
navigation-topic: notifications
title: 'Benachrichtigungen: Von mir eingereichte Anfragen'
description: Die folgenden Benachrichtigungen informieren Sie über Anfragen, die Sie in Adobe Workfront gestellt haben.
author: Courtney
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# Benachrichtigungen: Von mir eingereichte Anfragen

Die folgenden Benachrichtigungen informieren Sie über Anfragen, die Sie in [!DNL Adobe Workfront] gestellt haben.

Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Siehe auch [Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>Von mir eingereichte Anfragen</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Ersuchen um Genehmigung eines Dokuments wurde abgeschlossen</strong> </p> <p>Der Benutzer, der eine Genehmigung für ein Dokument angefordert hat, erhält eine E-Mail-Benachrichtigung, wenn die Anforderung zur Dokumentgenehmigung abgeschlossen ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist:<em> &lt;Name der genehmigenden Person&gt; hat &lt;Genehmigungsentscheidung ([!UICONTROL genehmigt], [!UICONTROL mit Änderungen genehmigt], [!UICONTROL abgelehnt])&gt; dieses Dokument.</em></p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine Daily Digest -E-Mail konfigurieren.</p> </td> 
   <td> Name/<br> der genehmigenden Person </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Dokument zu einem Problem, für das ich der primäre Ansprechpartner bin, wurde geändert oder hochgeladen</strong> </p> <p>Der primäre Kontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn ein Dokument zu dem Problem hochgeladen oder geändert wird, es sei denn, der Benutzer, der das Dokument hochgeladen oder geändert hat, ist auch der primäre Kontakt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (wie in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue] beschrieben</a>.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Dokument hinzugefügt zu &lt;Name des Problems&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist: <em>Zusammenfassung Ihrer Anfragen &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> Objektname, in den das Dokument hochgeladen wurde<br>Übergeordneter Objektname<br>Dokumentreferenznummer<br>Name des Benutzers, der das Dokument hochgeladen hat<br>Dokumentname<br>Am Datum hinzugefügt<br>Dokumentdetails (Format, Größe, Versionsnummer)<br>Dokumentminiaturansicht<br><strong>[!UICONTROL -Vorschau]</strong> und <strong>[!UICONTROL -Download]</strong>-Schaltflächen<br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der hochgeladenen Dokumente<br>*Name des Dokuments<br>*Name des übergeordneten Objekts<br>*Name des Benutzers, der das Dokument hinzugefügt hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Anforderung zum Hochladen eines Dokuments wurde ausgeführt</strong> </p> <p>Der Antragsteller erhält eine E-Mail-Benachrichtigung, wenn eine Anforderung zum Hochladen eines Dokuments erfüllt wird.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Ihre Dokumentanforderung von] &lt;Benutzername&gt; wurde erfüllt</em></p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine Daily Digest -E-Mail konfigurieren.</p> </td> 
   <td> <p>Name des Benutzers, der das Dokument hochgeladen hat<br>Objektname, in den das Dokument hochgeladen wurde<br>Dokumentname<br><br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine persönliche Aufgabe, die ich jemand anderem zugewiesen habe, ist abgeschlossen</strong> </p> <p>Wenn diese Anforderung abgeschlossen ist, wird eine Benachrichtigung an den Benutzer gesendet, der eine persönliche Arbeitsanfrage an eine andere Person zugewiesen hat. </p>  <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>Aufgabenabschluss: &lt;Aufgabenname&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine Daily Digest -E-Mail konfigurieren.</p> </p> </td> 
   <td> Aufgabenname<br>Standardprojektname (Persönliches Projekt des Benutzers, der die persönliche Aufgabe erhalten hat)<br>Aufgabenreferenznummer<br>Name des Aufgabenbesitzers<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Vorheriger Aufgabenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br><br><br></td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Problem, für das ich der primäre Ansprechpartner bin, wurde abgeschlossen</strong> </p> <p>Der primäre Kontakt für ein Problem erhält eine Benachrichtigung, wenn das Problem abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] oder [!UICONTROL Planning] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Problem Completion]: &lt;Issue Name&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Zusammenfassung Ihrer Anfragen &lt;Datum der täglichen Digest&gt;</em></p> <p> </p> </td> 
   <td> Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Neuer Status<br>Datum und Uhrzeit des Abschlusses des Problems<br>Vorheriger Anfragenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche <br>*Projektname<br>*Projektreferenznummer<br>*Gesamtzahl der abgeschlossenen Probleme<br>*Anfragename<br>*Name des Benutzers, der das Problem abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich füge einem Projekt eine Anfrage hinzu</strong> </p> <p>Der primäre Kontakt für ein Problem erhält eine Benachrichtigung, wenn er ein Problem in einem Projekt hinzufügt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] oder [!UICONTROL Planning] ist.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Problem gesendet]: &lt;Problemname&gt; am &lt;Projektname&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Zusammenfassung Ihrer Anfragen &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> Projektname<br>Portfolio Primär-Name<br>Problem-Referenznummer<br>Ihr Name<br>Problem-Name<br>Datum eingegeben<br>Problem-Priorität<br>Problem-Status<br>Zugeordneter Kontakt<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der hinzugefügten Probleme<br>*Problem-Name<br>*Datum der täglichen Zusammenfassung<br> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich sende eine Anfrage (Bestätigung)</strong> </p> <p>Der Primäre Kontakt für das Problem erhält eine E-Mail-Benachrichtigung, wenn er ein Problem sendet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Current] ist und wenn das Projekt als [!UICONTROL Help Request Queue] eingerichtet ist (wie in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue] beschrieben</a>).</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Anfrage gesendet]: &lt;Anfragename&gt; unter &lt;Name der Projektanfragewarteschlange&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Zusammenfassung Ihrer Anfragen &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> <p>Projektname (Name der Anfrage-Warteschlange)<br>Portfolio-Name<br>Anfrage-Referenznummer<br>Anfragename<br>Datum eingegeben<br>Anfragepriorität<br>Anfragestatus<br>Dem Namen zugewiesen<br>Primärer Kontakt<br>*Projekt-Referenznummer<br>*Projektname<br>*Gesamtzahl der gesendeten Anfragen<br>*Anfragename<br>*Anfragepriorität<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td> <p><strong>Instant</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Meine Anfrage ist geschlossen (Bestätigung)</strong> </p> <p>Der primäre Kontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn die Anfrage geschlossen wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und wenn das Projekt als [!UICONTROL Warteschlange für Hilfeanfragen] eingerichtet ist (wie unter <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anfragewarteschlange</a> beschrieben).</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Ihre Anfrage wurde geschlossen]:“&lt;Name der Anfrage&gt;"</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der die Anfrage geschlossen hat<br>Anfragenstatus<br>Datum und Uhrzeit, zu der die Anfrage geschlossen wurde<br>Vorheriger Anfragenstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br>*Projekt-Referenznummer<br>*Projektname<br>*Gesamtzahl der geschlossenen Anfragen<br>*Anfragename<br>*Name des Benutzers, der die Anfrage geschlossen hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Jemand wurde meiner Anfrage zugewiesen</strong> </p> <p>Der primäre Kontakt für das Problem erhält eine E-Mail-Benachrichtigung, wenn ein Benutzer dem Problem zugewiesen ist, es sei denn, der primäre Kontakt und der zugewiesene Benutzer sind dieselben Benutzer.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und wenn das Projekt als [!UICONTROL Warteschlange für Hilfeanfragen] eingerichtet ist (wie in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Warteschlange für Anfragen erstellen] beschrieben</a>.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>&lt;Name des Benutzers, der Ihrer Anfrage zugewiesen ist&gt; [!UICONTROL wurde Ihrer Anfrage zugewiesen]: "&lt;Anfragename&gt;"</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> <p>Anfragename<br>Projektname<br>Anfragenummer<br>Anfragename<br>Anfragetyp<br>Eingegebenes Datum<br>Anfragepriorität<br>Primärer Kontakt<br>Geplantes Abschlussdatum<br>Anfragestatus<br><strong>Weitere Details anzeigen</strong>*<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der zugewiesenen Anfragen<br>*Anfragename<br>*Name zugewiesen<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Der Status eines von mir erstellten Projekts ändert sich</strong> </p> <p>Der Benutzer, der das Projekt erstellt hat, erhält eine E-Mail-Benachrichtigung, wenn sich der Projektstatus ändert.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Projektstatusänderung]: &lt;Projektname&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of your Requests] &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> <p>Projektname<br>Portfolio-Name<br>Projekt-Referenznummer<br>Name des Benutzers, der den Status geändert hat<br>Neuer Status<br>Datum und Uhrzeit, zu der der Projektstatus geändert wurde<br>Vorheriger Projektstatus<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>-Schaltfläche<br>*Projektname<br>*Projekt-Referenznummer<br>*Projekt-Neuer Status<br>*Name des Benutzers, der den Projektstatus geändert hat<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td> <p><strong>Instant</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Der Status meiner Anfrage ändert sich</strong> </p> <p>Der primäre Kontakt des Problems erhält eine E-Mail-Benachrichtigung, wenn sich der Problemstatus ändert, es sei denn, der Benutzer, der den Status geändert hat, ist auch der primäre Kontakt.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus „Aktuell“ ist und das Projekt als [!UICONTROL Warteschlange für Hilfeanfragen] eingerichtet ist (wie in <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Warteschlange für Anfragen erstellen] beschrieben</a>.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>&lt;Name der Anfrage&gt; ist &lt;Neuer Status&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist: <em> Zusammenfassung Ihrer Anfragen &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der den Status der Anfrage geändert hat<br>Neuer Status<br>Datum und Uhrzeit, zu der der Status der Anfrage geändert wurde<br>Status der vorherigen Anfrage<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>-Schaltfläche<br>*Projektname<br>*Projekt-Referenznummer<br>*Gesamtzahl der Anfragen, deren Status geändert wurde<br>*Name der Anfrage<br>*Status der vorherigen Anfrage<br>*Neuer Anfragenstatus<br>*Name des Benutzers, der den Status geändert hat<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td> <p><strong>Täglich</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
