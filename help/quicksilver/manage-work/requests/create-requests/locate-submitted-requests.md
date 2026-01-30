---
product-area: requests
navigation-topic: create-requests
title: Gesendete Anfragen anzeigen
description: Erfahren Sie mehr über die Bereiche von Adobe Workfront, in denen Sie von Ihnen oder einer anderen Person gesendete Anfragen oder Anfragen anzeigen können, die Sie nie gesendet und als Entwürfe gespeichert haben.
author: Becky
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '1483'
ht-degree: 2%

---

# Eingereichte Anfragen anzeigen

Sie können die Anfragen anzeigen, die Sie oder eine andere Person gesendet haben, oder die Anfragen, die Sie begonnen haben, aber nie abgeschlossen haben. Die nicht abgeschlossenen Anfragen werden als Entwürfe gespeichert.

Gesendete Anfragen können in den folgenden Bereichen von Adobe Workfront gefunden werden:

* Der Bereich Anfragen von Workfront
* Das Widget „Meine Anfragen“ auf der Startseite

Im Bereich Anfragen werden je nach Anzeige die folgenden Anfragen angezeigt:

* Workfront fordert bei Verwendung des Legacy-Erlebnisses an
* Workfront sowie Planungsanfragen bei Verwendung des neuen Erlebnisses.

  >[!NOTE]
  >
  >* Sie können nur Ihre eigenen Anforderungsentwürfe anzeigen.
  >* In der neuen anfordernden -Version befinden sich gesendete Anfragen und Entwürfe in derselben Liste.
  >* In der veralteten -Version erstellte Entwürfe werden in der neuen -Version, in der die Anfrage gestellt wird, nicht angezeigt.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
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
  <tr> 
   <td role="rowheader"> Produkt</td> 
   <td> <ul><li>Adobe Workfront</li><li>Sie müssen über Adobe Workfront Planning verfügen, um Planungsanfragen oder Anfrageformulare anzuzeigen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen gesendeter Anfragen im Bereich Anfragen

Die Anzeige gesendeter Anfragen unterscheidet sich je nachdem, ob Sie das neue oder das veraltete anfragende Erlebnis verwenden.

* [Anzeigen gesendeter Anfragen in der neuen anfordernden Version](#view-submitted-requests-in-the-new-requesting-experience)
* [Anzeigen gesendeter Anfragen in der Legacy-Anfrage](#view-submitted-requests-in-the-legacy-requesting-experience)

### Anzeigen gesendeter Anfragen in der neuen anfordernden Version

Gesendete Anfragen können im Bereich Anfragen angezeigt werden. Dieser enthält Links zu Objekten, die von Planning-Anfragen erstellt wurden.

>[!NOTE]
>
>Links zu erstellten Objekten sind in der neuen anfordernden Version nur für Planungsanfragen verfügbar, wenn die Anfrage selbst ein Objekt erstellt hat. Wenn eine Workfront-Anfrage in ein Projekt oder ein anderes Objekt konvertiert wird, ist in der Anfrageliste in der neuen anfragenden -Version kein Link zu diesem konvertierten Objekt verfügbar.

So zeigen Sie Anfragen an, die Sie oder andere Benutzende in der neuen anfordernden Version gesendet haben:

{{step1-to-requests}}

1. Stellen Sie sicher **dass der Umschalter** Neues Erlebnis verwenden“ in der rechten oberen Ecke des Bildschirms aktiviert ist.

   Die Liste Anfragen wird angezeigt.

1. (Optional) Um nach einer Anfrage zu suchen, beginnen Sie, etwas in die Suchleiste oben rechts in der Liste einzugeben. Suchergebnisse werden während der Eingabe angezeigt.
1. (Optional) Klicken Sie **Filter** und beginnen Sie mit dem Hinzufügen von Bedingungen für die Anfragen, die Sie anzeigen möchten.

   Sie können nach den folgenden Feldern filtern:

   * **Workspace**: Der Arbeitsbereich, mit dem das Anfrageformular verknüpft ist.
   * **Datensatztyp**: Der Datensatztyp, mit dem das Anfrageformular verknüpft ist.
   * **Eingabedatum** Das Datum, an dem die Anfrage gesendet wurde.
   * **Anfrageformular**: Der Name des Anfrageformulars, das zum Senden der Anfrage verwendet wird.
   * **Status**: Der Status der Anfrage.
   * **Eingegeben von**: Der Name des Benutzers, der die Anfrage hinzugefügt hat. Wenn die Anfrage von einer Person außerhalb von Workfront hinzugefügt wurde, wird im Feld **Eingegeben von** `N/A` angezeigt.

   Es können mehrere Filter entweder durch „Und **oder** Oder **verbunden**.
Die Anfrageliste wird automatisch gefiltert, wenn Sie die Filterbedingungen hinzufügen.
1. (Optional) Verwenden Sie Ansichten, um sich auf die Anfragen zu konzentrieren, die Sie anzeigen möchten.

   Anweisungen finden Sie unter [Erstellen oder Bearbeiten von Ansichten im Bereich Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md).
1. (Optional) Überprüfen Sie den Status einer Anfrage, indem Sie die Spalte Status überprüfen. In der neuen anfragenden -Version sind die folgenden Status verfügbar:

   * **Entwurf**: Diese Anfrage wurde noch nicht übermittelt.
   * **Ausstehende Prüfung**: (Nur Planung) Diese Anfrage enthält genehmigende Personen, und keine der genehmigenden Personen hat die Anfrage geöffnet.
   * **In Prüfung**: (Nur Planung) Diese Anforderung enthält genehmigende Personen und mindestens eine genehmigende Person hat die Anforderung geöffnet, es wurde jedoch keine Entscheidung getroffen.
   * **Abgelehnt**: (Nur Planung) Diese Anforderung wurde von genehmigenden Personen abgelehnt.
   * **In Bearbeitung**:
      * Workfront-Anfragen: Die Anfrage wurde konvertiert und die Arbeit ist im Gange.
      * Workfront Planning-Anfragen: Der Anforderungsabschluss ist einem bestimmten Planning-Feld zugeordnet, und der Feldwert stimmt noch nicht mit dem Abschlusswert überein.

        Weitere Informationen finden Sie unter [Einrichten von Konfigurationsdetails](/help/quicksilver/planning/requests/create-request-form.md#set-up-configuration-details) im Artikel Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning.
   * **Abschließen**: Die Anfrage wurde abgeschlossen.

>[!NOTE]
>
>* Wenn Sie über Workfront Planning verfügen, werden Ihre Workfront- und Planning-Anfragen in derselben Liste angezeigt. Workfront-Anfragen zeigen den in der Spalte Objekttyp `Issue` Wert an.
>* Die Anfragenliste wird mit 50 angezeigten Anfragen angezeigt. Um weitere Anfragen anzuzeigen, scrollen Sie zum unteren Rand der Liste.

### Anzeigen gesendeter Anfragen in der Legacy-Anfrage

So zeigen Sie Anfragen an, die Sie oder andere Benutzende in der Legacy-Anfrage gesendet haben:

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
         <td role="rowheader">Path</td> 
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
      <td> <p>Von Ihnen gesendete Anfragen, die noch offen sind. </p> <p>Anfragen ohne tatsächliches Abschlussdatum oder Anfragen, deren Lösungsobjekt kein tatsächliches Abschlussdatum hat, werden auf der Unterregisterkarte Meine offenen Anfragen aufgeführt. </p> <p><b>TIPP</b>

   Anfragen, deren Status nicht mit Geschlossen übereinstimmt, werden als offen betrachtet.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie auf das **Seite filtern**-Symbol oben ![](assets/search-icon.png) in der Liste, um nach einer Anfrage anhand des Namens zu suchen. Die Liste wird mit Ergebnissen aktualisiert, die Ihren Suchkriterien entsprechen.

1. (Bedingt) Um nur Workfront-Anfragewarteschlangen anzuzeigen, suchen oder filtern Sie nach `Issue` Objekttypen.</span>


   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. Klicken Sie **Entwürfe**, um alle Entwürfe der Anfragen anzuzeigen. Workfront speichert für jede Anfrage-Warteschlange in diesem Ordner eine unbegrenzte Anzahl von Entwürfen. Wenn Sie eine neue Anfrage für ein Warteschlangen-Thema eingeben, für das bereits ein Entwurf vorhanden ist, werden Sie aufgefordert, einen vorhandenen Entwurf zu verwenden. Weitere Informationen finden Sie unter [Erstellen von Anfragen aus Entwürfen](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).

1. (Optional und bedingt) Wenn Ihr Unternehmen ein Workfront Planning-Paket erworben hat, klicken Sie auf die Registerkarte **Planning** und dann **Gesendet** im linken Bereich, um Workfront Planning-Anfragen anzuzeigen.

   Verwenden Sie **Filter** und **Spalten**, um die Informationen in der Planning-Anfrageliste zu aktualisieren.

   ![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)

   Weitere Informationen finden Sie unter [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).


1. (Optional) Überprüfen Sie den Status einer Anfrage, indem Sie die Spalte Status überprüfen. In der neuen anfragenden -Version sind die folgenden Status verfügbar:

   * Entwurf: Diese Anfrage wurde noch nicht eingereicht.
   * In Arbeit
   * Abgeschlossen


