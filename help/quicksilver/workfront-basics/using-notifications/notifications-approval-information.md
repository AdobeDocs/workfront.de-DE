---
content-type: reference
navigation-topic: notifications
title: 'Benachrichtigungen: Genehmigungsinformationen'
description: Die folgenden Benachrichtigungen informieren Sie über Genehmigungsaktivitäten, die für ein Arbeitselement durchgeführt werden, an dem Sie beteiligt sind. Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter Ändern Ihrer eigenen E-Mail-Benachrichtigungen .
author: Courtney
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Benachrichtigungen: Genehmigungsinformationen

Die folgenden Benachrichtigungen informieren Sie über Genehmigungsaktivitäten, die für ein Arbeitselement durchgeführt werden, an dem Sie beteiligt sind. Informationen zum Konfigurieren der empfangenen Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Eine delegierte Anfragegenehmigungsanfrage wurde abgeschlossen</strong> </p> <p>Eine Problemgenehmigung, die Sie an einen anderen Benutzer delegiert haben, wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Problem Approval/ Rejection Made in Your Bevollmächtigte by] &lt;Benutzername&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Approval Information] &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> <p>Anfragename<br>Projektname<br>Anfragenummer<br>Name des Benutzers, der das Problem in Ihrem Auftrag genehmigt/abgelehnt hat<br>Genehmigungsentscheidung<br>Anfragenstatus<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>[!UICONTROL Weitere Details anzeigen]</strong> Schaltfläche<br>*Projektreferenznummer<br>*Projektname<br>*Gesamtzahl der delegierten Anfragengenehmigungen<br>*Anfragename<br>*Name des genehmigenden Benutzers<br>*Datum der täglichen Zusammenfassung<br><br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine delegierte Projektgenehmigungsanfrage ist abgeschlossen</strong> </p> <p>Eine Projektgenehmigung, die Sie an einen anderen Benutzer delegiert haben, wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Projektgenehmigung/ -ablehnung in Ihrem Auftrag von] &lt;Benutzername&gt;</em></p> <p><em>Der Betreff der täglichen Digest-Benachrichtigung ist: [!UICONTROL Digest of Approval Information] &lt;Datum der täglichen Digest&gt;</em> </p> </td> 
   <td> Projektname<br>[!UICONTROL Portfolio-Name]<br>[!UICONTROL-Projekt-Referenznummer]<br>Name des Benutzers, der das Projekt in Ihrem Auftrag genehmigt/abgelehnt hat<br>[!UICONTROL-Genehmigungsentscheidung]<br>[!UICONTROL-Projektstatus]<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>[!UICONTROL Weitere Details anzeigen]</strong>-Schaltfläche<br>*Projekt-Referenznummer<br>*Projektname<br>*Name des genehmigenden Benutzers<br>[!UICONTROL *Datum der täglichen Zusammenfassung]<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine delegierte Aufgabengenehmigungsanfrage ist abgeschlossen</strong> </p> <p>Eine Aufgabengenehmigung, die Sie an einen anderen Benutzer delegiert haben, wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Aufgabe in Ihrem Auftrag von] &lt;Benutzername&gt;</em></p> <p>Der Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Approval Information] &lt;Datum der täglichen Digest&gt;</em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenreferenznummer<br>Name des Benutzers, der die Aufgabe in Ihrem Auftrag genehmigt/abgelehnt hat<br>Genehmigungsentscheidung<br>Aufgabenstatus<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>Weitere Details anzeigen</strong> Schaltfläche<br>*Projektreferenznummer<br>*Projektname<br>*Gesamtzahl der delegierten Aufgabengenehmigungen<br>*Aufgabenname<br>*Genehmigername<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Ersuchen um Genehmigung eines Dokuments wurde zurückgenommen</strong> </p> <p>Der Dokument-Genehmiger des Dokuments erhält eine E-Mail-Benachrichtigung, wenn die Dokumentgenehmigungsanfrage storniert wird.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail lautet: <em>&lt;Benutzername&gt; [!UICONTROL hat die Dokumentgenehmigungsanfrage storniert]</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine Daily Digest -E-Mail konfigurieren.</p> </p> </td> 
   <td> Name des Benutzers, der die Genehmigungsanfrage storniert hat<br>[!UICONTROL Dokumentname] </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich wurde als genehmigende Person beauftragt</strong> </p> <p>Wenn Ihnen jemand eine Genehmigung delegiert hat, erhalten Sie eine E-Mail-Benachrichtigung. </p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Delegiert] &lt;Objekttyp&gt; [!UICONTROL Genehmigung - Bitte überprüfen] &lt;Objektname&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine Daily Digest -E-Mail konfigurieren.</p> </p> </td> 
   <td> <p>[!UICONTROL Objektname]<br>[!UICONTROL Übergeordneter Objektname]<br>[!UICONTROL Objektreferenznummer]<br>Name des Benutzers, der das Objekt zur Genehmigung eingereicht hat<br>Name des Benutzers, für den Sie das Objekt genehmigen<br>Objektstatus<br>Datum und Uhrzeit der Anforderung der Genehmigung<br>Objektpriorität<br>Genehmigungsschrittname<br>[!UICONTROL Geplantes Abschlussdatum] des Objekts<br><strong>[!UICONTROL Genehmigungsentscheidung treffen]</strong> Schaltfläche</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Meine Arbeitszeittabelle wurde genehmigt</strong> </p> <p>Wenn Ihre Arbeitszeittabelle genehmigt wurde, erhalten Sie eine E-Mail-Benachrichtigung.</p> <p>Der Betreff der sofortigen Benachrichtigungs-E-Mail ist: <em>[!UICONTROL Arbeitszeittabelle genehmigt]: &lt;Startdatum der Arbeitszeittabelle&gt; - &lt;Enddatum der Arbeitszeittabelle&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine Daily Digest -E-Mail konfigurieren.</p> </p> </td> 
   <td> Name des Benutzers, der Ihre Arbeitszeittabelle genehmigt hat<br>Datum und Uhrzeit der Genehmigung der Arbeitszeittabelle<br>Status der Arbeitszeittabelle ([!UICONTROL Genehmigt])<br>Startdatum und Enddatum der Arbeitszeittabelle<br>Gesamtstundenzahl, die in der Arbeitszeittabelle erfasst <br>Überstunden, die in der Arbeitszeittabelle erfasst sind </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
 </tbody> 
</table>
