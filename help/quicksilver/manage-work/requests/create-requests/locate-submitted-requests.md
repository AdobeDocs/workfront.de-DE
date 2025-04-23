---
product-area: requests
navigation-topic: create-requests
title: Gesendete Anfragen suchen
description: Erfahren Sie mehr über die Bereiche von Adobe Workfront, in denen Sie Anfragen finden können, die Sie oder eine andere Person gesendet oder Anfragen, die Sie nie gesendet und als Entwürfe gespeichert haben.
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 1%

---

# Gesendete Anfragen suchen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>-->

Sie können die folgenden Arten von Anfragen finden, die von Ihnen oder einer anderen Person gesendet oder von Ihnen gestartet, aber nie fertig gesendet wurden. Sie können diese Anfragen in den folgenden Bereichen von Adobe Workfront finden:

* Die Registerkarte **Workfront** im Bereich Anfragen in Workfront: Suchen Sie in den folgenden Abschnitten nach Anfragen, die an Workfront-Anfrage-Warteschlangen gesendet wurden:
   * **Abschnitt „Gesendet**: Alle Anfragen, die Sie oder eine andere Person gesendet haben und auf die Sie zumindest Zugriff haben.
   * **Entwurfsabschnitt** : Alle Anfragen, die Sie gestartet, aber nie abgeschlossen und nie gesendet haben. Weitere Informationen zu Anfrageentwürfen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

  >[!TIP]
  >
  >Sie können nur Ihre eigenen Anforderungsentwürfe anzeigen.

* Die Registerkarte **Planung** im Bereich Anfragen in Workfront: Suchen Sie Anfragen, die an Workfront Planning-Anfrageformulare gesendet wurden. Ihr Unternehmen muss ein Workfront Planning-Paket erwerben. Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
   * [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md)


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Mitwirkender oder höher</p>
   Oder
   <p>Aktuell: Anforderung oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td><p>Zugriff auf Anfragen bearbeiten</p></td> 
  </tr>
  <tr>
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Anzeigen von Berechtigungen oder höher für die Anfragen</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gesendete Anfragen suchen

So suchen Sie nach von Ihnen oder anderen Benutzern gesendeten Anfragen:

{{step1-to-requests}}

1. (Bedingt) Wenn Ihr Unternehmen ein Workfront Planning-Paket erworben hat, klicken Sie auf die Registerkarte **Workfront** , um Workfront-Anfragen anzuzeigen.
1. Klicken Sie **linken** auf „Gesendet“, um alle gesendeten Anfragen anzuzeigen.

   Sie können bis zu 2.000 Anfragen anzeigen, die möglicherweise auf mehreren Seiten angezeigt werden.

   >[!TIP]
   >
   >Die Spalten in der Liste „Gesendete Anfrage“ können nicht angepasst werden.

   ![](assets/nwe-submitted-requests-new-list-350x57.png)


1. Die folgenden Spalten werden standardmäßig angezeigt:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Name</td> 
         <td> <p>Der Name der Anfrage.</p> <p>Klicken Sie auf den Namen einer Anfrage, um sie zu öffnen. </p> <p><b>TIPP</b>

   Wenn das Problem beim Konvertieren in eine Aufgabe oder ein Projekt nicht beibehalten wurde, ist der Name des Problems abgeblendet und kann nicht mehr angeklickt werden. Informationen zu Konvertierungsproblemen finden Sie unter <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Übersicht über die Konvertierung von Problemen in Adobe Workfront</a>. </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">Konvertiert in</td> 
         <td> <p>Der Name des Lösungsobjekts, bei dem es sich um eine Aufgabe oder ein Projekt handeln kann, in das die Anfrage konvertiert wurde. </p> <p>Klicken Sie auf den Namen der Aufgabe oder des Projekts, um sie bzw. es zu öffnen. </p> <p>Wenn die Anfrage nicht konvertiert wurde, ist dieses Feld leer. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Pfad</td> 
         <td>Der Name der Anfrage-Warteschlange, der Themengruppen und der Warteschlangenthemen, an die die Anfrage ursprünglich gesendet wurde. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Status</td> 
         <td>Der aktuelle Status der Anfrage oder des Lösungsobjekts (Aufgabe oder Projekt)</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Eingabedatum</td> 
         <td>Das Datum, an dem die Anfrage gesendet wurde, oder das Datum, an dem das Lösungsobjekt erstellt wurde, falls die Anfrage bei der Konvertierung gelöscht wurde. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Datum der letzten Aktualisierung</td> 
         <td> <p>Das Datum, an dem die Anfrage zuletzt aktualisiert wurde.</p> <p>Die Liste Gesendete Anfrage wird standardmäßig nach diesem Feld sortiert. </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. (Optional) Klicken Sie auf die Kopfzeile einer Spalte, um sie zu sortieren.

   >[!TIP]
   >
   >Wenn Sie die Liste Gesendete Anfragen verlassen, wird die ausgewählte Sortieroption beibehalten.

1. (Optional) Wählen Sie eine Anfrage in der Liste aus und klicken Sie dann auf das Symbol **Zusammenfassung öffnen**, ![](assets/open-summary-with-text-nwe.png) das Bedienfeld Zusammenfassung zu öffnen und zusätzliche Informationen über die Anfrage anzuzeigen, Kommentare hinzuzufügen, Dokumente hinzuzufügen oder sie zuzuweisen. Weitere Informationen über das Bedienfeld Zusammenfassung finden Sie unter [Übersicht](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >Wenn das Bedienfeld Zusammenfassung bereits geöffnet ist, ändert sich das Symbol Zusammenfassung öffnen in Zusammenfassung schließen .

1. (Optional und bedingt) Klicken Sie auf das Symbol **X** oben rechts oder auf das Symbol **Zusammenfassung schließen** ![](assets/close-summary-with-text-nwe.png), um das Bedienfeld Zusammenfassung zu schließen.

   Wenn ein Problem in eine Aufgabe oder ein Projekt konvertiert wurde und das Problem im Konvertierungsprozess gelöscht wurde, ist das Bedienfeld Zusammenfassung leer. Informationen zu Konvertierungsproblemen finden Sie unter [Übersicht über die Konvertierung von Problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Wählen Sie über **Symbol** oben rechts ![](assets/filter-nwepng.png) der Liste einen der in der folgenden Tabelle aufgelisteten Filter aus.

   >[!TIP]
   >
   >Filter im Abschnitt Gesendet im Bereich Anfragen können nicht geändert werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle</td> 
      <td>Alle eingereichten Anfragen, unabhängig vom Status oder wer sie gesendet hat.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Öffnen</td> 
      <td> <p>Alle gesendeten Anfragen, die derzeit offen sind, unabhängig davon, wer sie gesendet hat. Nur -Anfragen, für die Sie mindestens über die Berechtigung zum Anzeigen verfügen, werden hier angezeigt, wenn Sie sie nicht selbst gesendet haben. </p> <p>Anfragen ohne tatsächliches Abschlussdatum oder Anfragen, deren Lösungsobjekt kein tatsächliches Abschlussdatum hat, werden auf der Unterregisterkarte Öffnen aufgeführt.</p> <p><b>TIPP</b>

   Anfragen mit einem Status, der nicht mit Geschlossen übereinstimmt, werden als offen betrachtet.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Meine Anfragen</td> 
      <td>Von Ihnen gesendete Anfragen, unabhängig vom Status. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meine offenen Anfragen</td> 
      <td> <p>Von Ihnen gesendete Anfragen, die noch offen sind. </p> <p>Anfragen ohne tatsächliches Abschlussdatum oder Anfragen, deren Lösungsobjekt kein tatsächliches Abschlussdatum hat, werden auf der Unterregisterkarte Meine offenen Anfragen aufgeführt. </p> <p><b>TIPP</b>

   Anfragen, deren Status nicht mit Geschlossen übereinstimmt, werden als offen betrachtet.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie auf das **Seite filtern**-Symbol oben ![](assets/search-icon.png) in der Liste, um nach einer Anfrage anhand des Namens zu suchen. Die Liste wird mit Ergebnissen aktualisiert, die Ihren Suchkriterien entsprechen.

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the&nbsp;<strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:&nbsp; &nbsp;(NOTE:&nbsp;this step will stay drafted even after release. We can't see Completed at this time!) &nbsp;
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria:&nbsp;
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name.&nbsp;</li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted.&nbsp;</li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status.&nbsp;</li>
   </ul></li>
   -->

1. Klicken Sie **Entwürfe**, um alle Entwürfe der Anfragen anzuzeigen. Workfront speichert für jede Anfrage-Warteschlange in diesem Ordner eine unbegrenzte Anzahl von Entwürfen. Wenn Sie eine neue Anfrage für ein Warteschlangen-Thema eingeben, für das bereits ein Entwurf vorhanden ist, werden Sie aufgefordert, einen vorhandenen Entwurf zu verwenden. Weitere Informationen finden Sie unter [Erstellen von Anfragen aus Entwürfen](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).

1. (Optional und bedingt) Wenn Ihr Unternehmen ein Workfront Planning-Paket erworben hat, klicken Sie auf die Registerkarte **Planning** und dann **Gesendet** im linken Bereich, um Workfront Planning-Anfragen anzuzeigen.

   ![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)

   Weitere Informationen finden Sie unter [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).

 

 

 
