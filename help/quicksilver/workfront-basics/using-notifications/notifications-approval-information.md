---
content-type: reference
navigation-topic: notifications
title: '''Benachrichtigungen: Validierungsinformationen'
description: Die folgenden Benachrichtigungen informieren Sie über Validierungsaktivitäten für ein Arbeitselement, mit dem Sie befasst sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter Eigene Ereignisbenachrichtigungen aktivieren oder deaktivieren .
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# Benachrichtigungen: Validierungsinformationen

Die folgenden Benachrichtigungen informieren Sie über Validierungsaktivitäten für ein Arbeitselement, mit dem Sie befasst sind. Informationen zum Konfigurieren der Benachrichtigungen, die Sie erhalten, finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>Ein delegierter Anfragegenehmigungsantrag ist abgeschlossen.</strong> </p> <p>Eine an einen anderen Benutzer delegierte Problemgenehmigung wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Genehmigung eines Problems/Zurückweisung in Ihrem Namen von] &lt;user name=""&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Problemname<br>Projektname<br>Problemverweisnummer<br>Name des Benutzers, der das Problem in Ihrem Namen genehmigt/abgelehnt hat<br>Genehmigungsentscheidung<br>Problemstatus<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Referenz-Nummer des Projekts<br>*Projektname<br>*Gesamtzahl der delegierten Emissionsgenehmigungen<br>*Name des Problems<br>*Genehmiger-Name<br>*Datum der täglichen Zusammenfassung<br><br></p> </td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine delegierte Projektgenehmigungsanfrage ist abgeschlossen.</strong> </p> <p>Eine Projektgenehmigung, die Sie einem anderen Benutzer zugewiesen haben, wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Projektgenehmigung/ Ablehnung in Ihrem Namen von] &lt;user name=""&gt;</em></p> <p><em>Betreff der täglichen Digest-Benachrichtigung ist: [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> Projektname<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Projektnummer]<br>Name des Benutzers, der das Projekt in Ihrem Namen genehmigt/abgelehnt hat<br>[!UICONTROL Validierungsbeschluss]<br>[!UICONTROL Projektstatus]<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>[!UICONTROL Weitere Informationen]</strong> button<br>*Referenz-Nummer des Projekts<br>*Projektname<br>*Genehmiger-Name<br>[!UICONTROL *Datum des täglichen Digest]<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Eine delegierte Aufgabengenehmigungsanfrage ist abgeschlossen.</strong> </p> <p>Eine Aufgabengenehmigung, die Sie einem anderen Benutzer zugewiesen haben, wurde von diesem Benutzer genehmigt oder abgelehnt.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Task Validierung/ Zurückweisung in Ihrem Namen von] &lt;user name=""&gt;</em></p> <p>Betreff der täglichen Digest-Benachrichtigung ist:<em> [!UICONTROL Digest of Approval Information] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Aufgabenname<br>Projektname<br>Aufgabenverweisnummer<br>Name des Benutzers, der die Aufgabe in Ihrem Namen genehmigt/abgelehnt hat<br>Genehmigungsentscheidung<br>Aufgabenstatus<br>Name des Benutzers, der die Genehmigung angefordert hat<br><strong>Siehe Weitere Details</strong> button<br>*Referenz-Nummer des Projekts<br>*Projektname<br>*Gesamtzahl der Genehmigungen delegierter Aufgaben<br>*Aufgabenname<br>*Genehmiger-Name<br>*Datum der täglichen Zusammenfassung<br></td> 
   <td><strong>Täglich</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ein Ersuchen um Genehmigung eines Dokuments wurde zurückgenommen.</strong> </p> <p>Der Dokumentenvalidierer des Dokuments erhält eine E-Mail-Benachrichtigung, wenn die Anforderung der Dokumentgenehmigung abgebrochen wird.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>&lt;user name=""&gt; [!UICONTROL hat die Anforderung der Dokumentgenehmigung abgebrochen]</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </p> </td> 
   <td> Name des Benutzers, der die Genehmigungsanforderung abgebrochen hat<br>[!UICONTROL Dokumentname] </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ich wurde als genehmigende Person beauftragt</strong> </p> <p>Wenn Ihnen jemand eine Validierung zugewiesen hat, erhalten Sie eine E-Mail-Benachrichtigung. </p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Delegiert] &lt;object type=""&gt; [!UICONTROL Genehmigung - Bitte überprüfen] &lt;object name=""&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </p> </td> 
   <td> <p>[!UICONTROL Objektname]<br>Übergeordneter Objektname von [!UICONTROL]<br>[!UICONTROL Objektverweisnummer]<br>Name des Benutzers, der das Objekt zur Genehmigung gesendet hat<br>Name des Benutzers, für den Sie das Objekt genehmigen<br>Objektstatus<br>Datum und Uhrzeit der Anforderung der Genehmigung<br>Objektpriorität<br>Name des Genehmigungsschritts<br>[!UICONTROL Geplantes Abschlussdatum] des Objekts<br><strong>[!UICONTROL Genehmigungsentscheidung treffen]</strong> button</p> </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Meine Arbeitszeittabelle wurde genehmigt</strong> </p> <p>Wenn Ihr Timesheet validiert wurde, erhalten Sie eine E-Mail-Benachrichtigung.</p> <p>Betreff der E-Mail zur sofortigen Benachrichtigung ist: <em>[!UICONTROL Zeitblatt genehmigt]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>Hinweis: Sie können diese Benachrichtigung nicht für eine tägliche Digest-E-Mail konfigurieren.</p> </p> </td> 
   <td> Name des Benutzers, der Ihr Arbeitsblatt genehmigt hat<br>Datum und Uhrzeit der Validierung des Zeitplans<br>Status des Datenblatts ([!UICONTROL Genehmigt])<br>Startdatum und Enddatum des Zeitblatts<br>Gesamtbesuchszeit im Datenblatt<br>Im Timesheet angemeldete Überstunden </td> 
   <td><strong>Sofort</strong> </td> 
  </tr> 
 </tbody> 
</table>
