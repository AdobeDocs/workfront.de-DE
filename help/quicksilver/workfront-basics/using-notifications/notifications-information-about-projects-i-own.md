---
content-type: reference
navigation-topic: notifications
title: '''Benachrichtigungen: Informationen über Projekte, deren Inhaber ich bin"'
description: Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die in einem Projekt durchgeführt werden, dessen Eigentümer Sie sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter Eigene Ereignisbenachrichtigungen aktivieren oder deaktivieren .
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# Benachrichtigungen: Informationen über Projekte, die ich besitze

Die folgenden Benachrichtigungen informieren Sie über Aktivitäten, die in einem Projekt durchgeführt werden, dessen Eigentümer Sie sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Ein Dokument wurde einem Projekt hinzugefügt, dessen Besitzer ich bin.</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn ein Dokument zum Projekt hinzugefügt wird, es sei denn, der Benutzer, der das Dokument hinzugefügt hat, ist auch Projektinhaber.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet und das Dokument nicht privat ist.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Dokument hinzugefügt zu] &lt;project name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Projektname<br>Portfolio Name<br>Projektnummer<br>Name des Benutzers, der das Dokument hinzugefügt hat<br>Dokumentname<br>Datum hinzugefügt<br>Dokumentdetails (Format, Größe, Versionsnummer)<br><strong>[!UICONTROL Vorschau]</strong> und <strong>[!UICONTROL Download]</strong> Schaltflächen<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der hinzugefügten Dokumente<br>*Dokumentname<br>*Name des Benutzers, der das Dokument hinzugefügt hat<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Wenn eine Meilensteinaufgabe abgeschlossen ist, den Projektbesitzer per E-Mail informieren.</strong> </p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, zeigt der Betreff der E-Mail weiterhin "[!UICONTROL Complete]"an.</p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat<br>Neuer Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Status der vorherigen Aufgabe<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Aufgaben<br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Projekt, das in meinem Besitz ist, ist in Verzug geraten.</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn das Projekt verspätet ist. Ein Projekt liegt hinter dem Zeitplan, wenn der Fortschrittsstatus "[!UICONTROL At Risk]", "[!UICONTROL Behind]"oder "[!UICONTROL Late]"lautet.</p> <p>Es empfiehlt sich, diese Benachrichtigung aktiv zu halten. </p> <p>Benutzer mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Projektfortschritt ändern]: &lt;project name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektname<br>Portfolio Name<br>Projektnummer<br>Projektfortstatus<br>Projekt [!UICONTROL Geplantes Startdatum]<br>Projekt [!UICONTROL Geplantes Abschlussdatum]<br>Projekt [!UICONTROL Voraussichtlicher Starttermin]<br>Projekt [!UICONTROL Projektzeitpunkt]<br>Projektanprozentsatz abgeschlossen<br>Projektstatus<br>Projektinhaber<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Projektfortstatus<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Anfrage wird einem Projekt in meinem Besitz hinzugefügt</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Problem hinzugefügt zu] &lt;project name=""&gt;</em></p> <p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektname<br>Portfolio Name<br>Problemverweisnummer<br>Name des Benutzers, der das Problem hinzugefügt hat<br>Problemname<br>Problemtyp<br>Eingegebene Daten<br>Problempriorität<br>Zugeordneter Name <br>Problemstatus<br>Primärer Kontakt<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der dem Projekt hinzugefügten Probleme<br>*Name des Problems<br>*Name des Benutzers, der das Problem hinzugefügt hat<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Wenn eine Aufgabe abgeschlossen ist, den Projektbesitzer per E-Mail informieren.</strong> </p> <p>Der Projekteigentümer erhält eine Benachrichtigung, wenn eine Aufgabe in seinem Projekt abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>Hinweis: Wenn die Aufgabe in einen Status geändert wird, der [!UICONTROL Complete] entspricht, zeigt der Betreff der E-Mail weiterhin "[!UICONTROL Complete]"an.</p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Name des Benutzers, der die Aufgabe abgeschlossen hat <br>Aufgabenstatus<br>Datum und Uhrzeit des Abschlusses der Aufgabe<br>Status der vorherigen Aufgabe<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Aufgaben <br>*Aufgabenname<br>*Name des Benutzers, der die Aufgabe abgeschlossen hat<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Aufgabe in einem Projekt, dessen Besitzer ich bin, ist in Verzug geraten.</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn eine Aufgabe im Projekt hinter den Zeitplan zurückfällt. Eine Aufgabe liegt hinter dem Zeitplan, wenn der Fortschrittsstatus "[!UICONTROL At Risk]"oder "[!UICONTROL Behind]"oder "[!UICONTROL Late]"lautet.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Task Progress Change]: &lt;task name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Neuer Aufgabenfortstatus<br>Aufgabe [!UICONTROL Geplantes Startdatum]<br>Aufgabe [!UICONTROL Geplantes Abschlussdatum]<br>Task [!UICONTROL Projected Start Date]<br>Aufgabe [!UICONTROL Projektionsdatum]<br>Task Percent Complete<br>Aufgabenstatus<br>Zugeordneter Name<br>Eingabe nach Name<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der Aufgaben, die hinter dem Zeitplan liegen<br>*Aufgabenname<br>*Der Name zugewiesen<br>*Datum der täglichen Zusammenfassung </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine Anfrage wurde gelöst in einem Projekt, dessen Besitzer ich bin.</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn ein Problem in seinem Projekt abgeschlossen ist.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Benutzer mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung. </p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Complete]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> Problemname<br>Projektname<br>Problemverweisnummer<br>Name des Benutzers, der das Problem abgeschlossen hat<br>Problemstatus<br>Datum und Uhrzeit des Abschlusses des Problems<br>Status des vorherigen Problems<br><strong>[!UICONTROL Weitere Informationen]</strong> button <br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der abgeschlossenen Probleme<br>*Name des Problems<br>*Name des dem Problem zugewiesenen Benutzers<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Wenn eine nicht zugewiesene Anfrage hinzugefügt wird, den Projektbesitzer per E-Mail informieren.</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn dem Projekt ein nicht zugewiesenes Problem hinzugefügt wird.</p> <p>Eine Benachrichtigung wird nur gesendet, wenn der Projektstatus [!UICONTROL Aktuell] oder [!UICONTROL Planung] lautet.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Wer sollte dieser neuen Ausgabe zugewiesen werden] &lt;project name=""&gt;?</em></p> <p> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> Eigene Projekte &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Projektname<br>Portfolio Name<br>Problemverweisnummer<br>Name des Benutzers, der das Problem hinzugefügt hat<br>Problemname<br>Problemtyp<br>Eingegebene Daten<br>Problempriorität<br>Zugeordneter Name (leer)<br>Problemstatus<br>Primärer Kontakt<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der hinzugefügten Probleme<br>*Name des Problems<br>*Name des Benutzers, der das Problem hinzugefügt hat<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und täglich</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich bin bei einem neuen Projekt als Besitzer festgelegt</strong> </p> <p>Wenn ein Benutzer als Eigentümer eines Projekts zugewiesen wird, erhält er eine E-Mail-Benachrichtigung.</p> <p>Wenn der Projekteigentümer derselbe Benutzer ist, der die Zuweisung vorgenommen hat, wird keine E-Mail-Benachrichtigung gesendet.</p> <p>Benutzer mit einer [!UICONTROL Review]-Lizenz erhalten keine Benachrichtigung.</p> <p>Schalten Sie das ein, weil ihnen etwas zugeordnet wird. </p> <p> Zuweisen von etwas, Teilen von etwas, Zugriff auf etwas.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Sie sind jetzt Projektinhaber von] &lt;project name=""&gt;</em></p> <p>Der folgende Text ist im Text der E-Mail-Benachrichtigung enthalten:<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL hat Sie zum Eigentümer von] &lt;project name=""&gt;. [!UICONTROL Als Projekteigentümer erhalten Sie möglicherweise zusätzliche E-Mail-Benachrichtigungen über die Projektaktivität, müssen die Stunden für das Projekt genehmigen oder an der Genehmigung der mit dem Projekt verbundenen Arbeit beteiligt sein. Das ist alles deins.]</em> </p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>Projektname<br>Portfolio Name<br>Projektnummer<br>Abschlussdatum des Projekts<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Datum der täglichen Zusammenfassung</p> </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Den Projektbesitzer per E-Mail benachrichtigen, wenn sich das Commit-Datum einer Aufgabe ändert</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn sich das Veröffentlichungsdatum für eine Aufgabe im Projekt ändert, es sei denn, der Benutzer, der das Veröffentlichungsdatum geändert hat, ist auch Projektinhaber.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Datum für] &lt;task name=""&gt; [!UICONTROL ist jetzt] &lt;new commit="" date=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> Eigene Projekte &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Name des Benutzers, der das Datum der Übermittlung geändert hat<br>Neues Veröffentlichungsdatum<br>Aufgabe [!UICONTROL Geplantes Abschlussdatum]<br>Informationen darüber, wie sich diese Änderung auf die Projekt-Timeline auswirkt<br>Zugeordneter Name<br>Eingabe nach Name<br>Projektinhaber<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der Aufgaben, deren Veröffentlichungsdatum geändert wurde<br>*Aufgabenname<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und [!UICONTROL Täglich]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Das Commmit-Datum für eine Anfrage ändert sich für eines meiner Projekte</strong> </p> <p>Der Projekteigentümer erhält eine E-Mail-Benachrichtigung, wenn sich das Veröffentlichungsdatum für ein Problem im Projekt ändert, es sei denn, der Benutzer, der das Veröffentlichungsdatum ändert, ist derselbe Benutzer wie der Projekteigentümer.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Datum für] &lt;issue name=""&gt; [!UICONTROL ist jetzt] &lt;new commit="" date=""&gt;</em></p> <p> Betreff der täglichen Digest-Benachrichtigung ist: <em> [!UICONTROL Digest of Projects Your Own] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemverweisnummer<br>Name des Benutzers, der das Datum der Übermittlung geändert hat<br>Neues Veröffentlichungsdatum<br>Geplantes Abschlussdatum des Problems<br>Zugeordneter Name<br>Eingabe nach Name<br>Projektinhaber<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Projektname<br>*Referenz-Nummer des Projekts<br>*Gesamtzahl der Probleme, deren Veröffentlichungsdatum sich geändert hat<br>*Name des Problems<br>*Datum der täglichen Zusammenfassung<br></p> </td> 
   <td> <p><strong>Sofort</strong> </p> <p><strong>und [!UICONTROL Täglich]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
