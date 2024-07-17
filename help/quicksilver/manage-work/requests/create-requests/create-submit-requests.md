---
product-area: requests
navigation-topic: create-requests
title: Erstellen und Senden von Adobe Workfront-Anforderungen
description: Geplante Arbeiten werden in Adobe Workfront durch Projekte und Aufgaben repräsentiert. Sie können jedoch in einer Umgebung arbeiten, in der ungeplante Arbeiten - in Form von zufälligen Anfragen - jederzeit eintreten können. Workfront bietet einen Workflow, mit dem dieser Umgebungstyp mithilfe von Anforderungswarteschlangen berücksichtigt werden kann.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 1%

---

# Erstellen und Senden von Adobe Workfront-Anforderungen

<!--Audited: 12/2023-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE: If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

Geplante Arbeiten werden in Adobe Workfront durch Projekte und Aufgaben repräsentiert. Sie können jedoch in einer Umgebung arbeiten, in der ungeplante Arbeiten in Form von Anfragen jederzeit eingehen können. Workfront bietet einen Workflow, mit dem dieser Umgebungstyp mithilfe von Anforderungswarteschlangen berücksichtigt werden kann.

Nachdem Sie eine Anforderung in einer Anforderungswarteschlange erstellt haben, können Sie sie entweder zum Abschluss zuweisen oder in eine Aufgabe oder ein Projekt konvertieren.\
Weitere Informationen zum Konvertieren von Problemen in eine Aufgabe oder ein Projekt finden Sie im Artikel [Überblick über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Sie können eine Anforderung wie folgt erstellen:

* Wie in diesem Artikel beschrieben, ist von Grund auf neu.
* Aus Entwürfen. Weitere Informationen finden Sie unter [Anforderungen aus Entwürfen erstellen](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* durch Kopieren und Senden einer Kopie von einer bestehenden Anforderung ausgehend. Weitere Informationen finden Sie unter [Anforderungen kopieren und senden](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Mitarbeiter oder höher</p>
   Oder
   <p>Aktuell: Anforderung oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen für die Verwendung von Anforderungswarteschlangen

Ein Workfront-Administrator muss Anforderungswarteschlangen erstellen und sie Benutzern zur Verfügung stellen, bevor er diese Funktion verwenden kann. Ein Benutzer mit einer Planner-Lizenz und mit Bearbeitungszugriff auf Projekte und Verwaltungsberechtigungen für ein bestimmtes Projekt kann auch Anforderungswarteschlangen erstellen.

Informationen zum Erstellen von Anforderungswarteschlangen finden Sie im Artikel [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Ein Workfront-Administrator muss die folgenden Komponenten einer Anforderungswarteschlange erstellen:

* Ein Projekt mit dem aktuellen Status, das als Warteschlange für Hilfeanfragen veröffentlicht wird.
* Warteschlangenthemen.\
  Weitere Informationen finden Sie im Artikel [Themen der Warteschlange erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Routing-Regeln.\
  Weitere Informationen finden Sie im Artikel [Erstellen von Routing-Regeln](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Optional) Themengruppen.\
  Weitere Informationen finden Sie im Artikel [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Optional) Anfordern Sie ein benutzerdefiniertes Formular.\
  Weitere Informationen finden Sie im Artikel [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* (Optional) Genehmigungsprozess anfordern.\
  Weitere Informationen finden Sie im Artikel [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Erstellen von Anforderungen und Generieren von Entwürfen in der Workfront-Webanwendung

Wenn Sie eine Anforderung in der Workfront-Web-App erstellen, speichert Workfront die Anforderung als Entwurf, bevor Sie sie senden. Workfront erstellt einen Entwurf, sobald Sie Ihre Anforderungswarteschlange auswählen und mit der Eingabe von Informationen beginnen.

Sie können die Anfrage fortsetzen, oder Sie können so viele Informationen wie verfügbar ausfüllen und von ihr weg navigieren, um sie später abzuschließen. Workfront speichert die von Ihnen gestartete Anforderung im Ordner &quot;Entwürfe&quot;.

>[!IMPORTANT]
>
>Beachten Sie beim Arbeiten mit Entwürfen Folgendes:
>
>* Workfront erstellt keine Entwürfe von Anforderungen, wenn Sie sie von einer Drittanbieteranwendung übermitteln, z. B. per E-Mail an Workfront oder durch die Erstellung mit einer anderen Anwendung. Wenn Sie eine Anforderung von außerhalb der Workfront-Web-App senden, wird die Anforderung im Abschnitt &quot;Gesendet&quot;gespeichert.
>* Wenn sich die Struktur einer Anforderungswarteschlange ändert, können Sie nicht mehr auf vorhandene Entwürfe zugreifen. Wenn beispielsweise ein Warteschlangenthema entfernt oder eine Themengruppe hinzugefügt wird, können die gespeicherten Entwürfe nicht mehr aufgerufen werden.
>

Informationen zum Erstellen von Anforderungen aus vorhandenen Entwürfen finden Sie unter [Anforderungen aus Entwürfen erstellen](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). Weitere Informationen zum Löschen von Anfrageentwürfen finden Sie unter auch unter [Einen Anfrageentwurf löschen](../../../manage-work/requests/create-requests/delete-request-draft.md).

So erstellen Sie eine Anforderung in der Workfront-Webanwendung:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. Klicken Sie auf **Anforderungen** und dann oben rechts auf der Seite auf **Neue Anforderung** .

   >[!TIP]
   >
   >* Sie können über jeden Bereich im Bereich Anforderungen auf die Option Neue Anforderung zugreifen.
   >* Die Option &quot;Neue Anforderung&quot;ist abgeblendet, wenn Sie keinen Zugriff zum Erstellen von Problemen haben.

1. (Bedingt) Klicken Sie in das Feld **Anforderungstyp** und führen Sie einen der folgenden Schritte aus:

   * Wählen Sie im Abschnitt **Letzte Pfade** einen Pfad aus, den Sie kürzlich zum Öffnen einer Anforderungswarteschlange verwendet haben. Ein Pfad enthält die Anforderungswarteschlange, die Themengruppen und das Warteschlangenthema, das Sie kürzlich an gesendet haben. Die letzten drei Pfade werden standardmäßig angezeigt.

     >[!NOTE]
     >
     >Workfront speichert einen Pfad nur, wenn Sie tatsächlich eine Anfrage an ihn gesendet haben. Es werden keine Pfade für entworfene Anforderungen erstellt.

     ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * Wählen Sie im Abschnitt **Anforderungswarteschlangen** eine Anforderungswarteschlange aus.
   * Geben Sie einen Suchbegriff ein, der zu einem zuvor aufgerufenen Pfad gehört, um nach einer Anforderungswarteschlange zu suchen.

     Wenn Sie beispielsweise über eine Anforderungswarteschlange mit dem Namen &quot;Help Desk&quot;mit einer Themengruppe mit dem Namen &quot;Location&quot;und einem Warteschlangenthema mit dem Namen &quot;Remote&quot;verfügen, können Sie &quot;remote&quot;eingeben und alle Anforderungswarteschlangen mit &quot;remote&quot;in einem beliebigen Element ihres Pfads anzeigen.

     >[!TIP]
     >
     >Wenn Sie einen Namen eingeben, der ein Sonderzeichen enthält, wird die Anforderungswarteschlange, das Warteschlangenthema oder die Themengruppe auch dann angezeigt, wenn Sie die Eingabe des Zeichens weglassen.

     ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

     Die Liste der verfügbaren Anforderungswarteschlangen und der zuletzt verwendeten Pfade wird dynamisch aktualisiert und umfasst nur Pfade, die das in den Ergebnissen hervorgehobene Keyword enthalten.

     Die Suchergebnisse werden unter den folgenden Bereichen angezeigt:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Anfrage-Warteschlangen</td> 
        <td>Anforderungswarteschlangen, die den Suchbegriff in ihrem Namen enthalten</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Anfrage-Pfade</td> 
        <td> <p>Pfade (einschließlich Anfragewarteschlangen, Themengruppen, Warteschlangenthemen), die das Keyword in einem der Namen ihrer Elemente enthalten</p> </td> 
       </tr> 
      </tbody> 
     </table>

   >[!TIP]
   >
   >* Die ersten 200 Anforderungswarteschlangen werden standardmäßig in alphabetischer Reihenfolge angezeigt.
   >* Der Name der Anforderungswarteschlange ist der Name des Projekts, das als Warteschlange für Hilfeanfragen veröffentlicht wurde.
   >* Die Beschreibung des Projekts, das als ausgewählte Anforderungswarteschlange konfiguriert wurde, wird rechts neben dem Namen der Anforderungswarteschlange angezeigt.
   >   
   >Weitere Informationen zum Veröffentlichen eines Projekts als Warteschlange für Hilfeanfragen finden Sie im Artikel [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Führen Sie im Formular **Neue Anforderung** einen der folgenden Schritte aus:

   * (Bedingt) Wählen Sie einen verfügbaren Entwurf aus der Benachrichtigungsmeldung aus, die im Feld Anfragetyp angezeigt wird.

     Dieser Bereich wird nur angezeigt, wenn Sie Entwürfe gespeichert haben, bevor Sie sie gesendet haben.

     Die drei letzten Entwürfe aus drei verschiedenen Themen der Warteschlange werden standardmäßig angezeigt.

     ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Starten Sie die Eingabe einer neuen Anforderung in die ausgewählte Warteschlange.

     Nachdem Sie mit der Eingabe von Informationen für die neue Anforderung begonnen und der Anfrage im Feld Betreff einen Namen gegeben haben, wird automatisch ein neuer Entwurf im Abschnitt Entwürfe gespeichert.

1. (Optional) Wenn Ihre Anforderungswarteschlange Themengruppen enthält, wählen Sie im ersten Dropdown-Feld den Namen der Themengruppe aus. Wählen Sie andernfalls ein Warteschlangenthema aus.

   >[!TIP]
   >
   >Wenn Sie den Mauszeiger über eine Themengruppe oder ein Warteschlangenthema bewegen, wird rechts das Feld Beschreibung angezeigt. Dies enthält zusätzliche Informationen über die Themengruppe oder das Warteschlangenthema.
   >
   >
   >![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >
   >

   Sie können bis zu 10 Stufen von Themengruppen in Ihre Anforderungswarteschlange integrieren.\
   Weitere Informationen zum Erstellen von Themengruppen finden Sie im Artikel [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Weitere Informationen zum Erstellen von Warteschlangenthemen finden Sie im Artikel [Themen für Warteschlangen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   >
   >Wenn Sie einen Entwurf oder einen vorherigen Pfad ausgewählt haben, sind die Themengruppen und Warteschlangenthemen bereits ausgewählt. Sie können bei Bedarf eine andere auswählen.

1. Je nachdem, welche Felder der Workfront-Administrator auf der Unterregisterkarte **Warteschlangendetails** im Abschnitt **Neue Problemfelder** des Projekts aktiviert hat, können Sie beim Senden einer neuen Anforderung eines der folgenden Felder finden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Betreff</strong> </td> 
      <td>Geben Sie einen Namen für Ihre Anforderung an. Dies ist ein Pflichtfeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Geben Sie eine Beschreibung für Ihre Anforderung an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Geben Sie eine URL an, die sich auf Ihre Anfrage beziehen kann.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorität</strong> </td> 
      <td> <p>Geben Sie eine Priorität für Ihre Anforderung an. Mit der Priorität sollte definiert werden, wie schnell diese Anfrage Ihrer Meinung nach gelöst werden sollte. Die Standardoptionen sind: </p> 
       <ul> 
        <li>Keine</li> 
        <li>Niedrig </li> 
        <li>Normal</li> 
        <li>Hoch</li> 
        <li>Dringend</li> 
       </ul> <p>Ihr Systemadministrator kann die Namen der Prioritäten ändern.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schweregrad</strong> </td> 
      <td> <p>Geben Sie einen Schweregrad für Ihre Anfrage an. Der Schweregrad sollte die Auswirkungen dieser Anfrage auf Ihre Arbeit definieren, sollte sie nicht rechtzeitig gelöst werden. Die Standardoptionen sind:</p> 
       <ul> 
        <li>Kosmetisch</li> 
        <li>Verwirrend</li> 
        <li>Programmfehler mit Umgehungslösung</li> 
        <li>Programmfehler ohne Umgehungslösung</li> 
        <li>Schwerer Fehler</li> 
       </ul> <p>Ihr Systemadministrator kann die Namen der Schweregrade ändern.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primärer Kontakt</strong> </td> 
      <td>Der Primäre Kontakt einer Anfrage ist standardmäßig auf Sie festgelegt, da Sie als Ansprechpartner für alle Fragen im Zusammenhang mit der Anfrage fungieren. Sie können dies jedoch in einen anderen Workfront-Benutzer ändern.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Arbeitsaufträge</strong> </td> 
      <td> <p><span>Geben Sie den Namen eines aktiven Benutzers, einer Job-Rolle oder eines Teams an, dem die Anforderung zugewiesen werden soll.</span> </p> <p>Sie können nur ein Team angeben.</p>

   <p> Je nachdem, wie die Anforderungswarteschlange eingerichtet wurde, können Sie der Anforderung möglicherweise nur einen oder zwei Ressourcentypen anstelle aller drei Typen zuweisen (beispielsweise können Sie die Anforderung nur Benutzern zuweisen).</p>

   <p>Wenn eine Routing-Regel auch mit der Anforderungswarteschlange verknüpft ist und die Anforderung automatisch an einen anderen Ressourcentyp weitergeleitet wird (z. B. ein Team), wird Ihre Anforderung sowohl der Entität zugewiesen, die Sie beim Senden der Anforderung manuell angeben (Benutzer), als auch der in der Routing-Regel angegebenen Ressource (Team). </p>

   <p> Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Routing-Regeln erstellen</a> <br> </p> </li> 
      </ul> </p>

   <p><span>Wir empfehlen die Verwendung von Routing-Regeln für Ihre Anforderungswarteschlangen, damit sie automatisch an die entsprechenden Ressourcen weitergeleitet werden.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Geplante Stunden</strong> </td> 
      <td> <p>Schätzen Sie, wie viele Stunden es dauern würde, bis diese Anfrage abgeschlossen ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplantes Startdatum</strong> </td> 
      <td> <p>Geben Sie das Datum an, an dem die Arbeit an dieser Anforderung beginnen soll.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplantes Abschlussdatum</strong> </td> 
      <td>Geben Sie das Datum an, an dem diese Anfrage aufgelöst werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>Der Standardstatus einer neuen Anforderung lautet "Neu". Ihr Systemadministrator hat den Namen dieses Status möglicherweise geändert. Sie können den Status auch in etwas Anderes über dieses Dropdown-Menü ändern.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dokumente</strong> </td> 
      <td> <p>Fügen Sie Ihrer Anforderung Dokumente hinzu. </p> <p> Je nachdem, wie die Anforderungswarteschlange eingerichtet wurde, wird der Abschnitt Dokumente möglicherweise vor oder nach den benutzerdefinierten Feldern angezeigt. </p> <p>Dokumente, die Sie in Workfront hochladen, werden 24 Stunden lang in einer entworfenen Anfrage gespeichert. Danach müssen Sie sie erneut anhängen, wenn Sie zum Bearbeiten und Senden des Entwurfs zurückkehren. Dokumente, die mit anderen Laufwerken verknüpft sind, werden dauerhaft im Entwurf gespeichert. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wenn Ihr Workfront-Administrator ein benutzerdefiniertes Formular mit der Anforderungswarteschlange oder dem Warteschlangenthema verknüpft hat, geben Sie die Felder im benutzerdefinierten Formular an.\
   Benutzerdefinierte Formulare unterscheiden sich für jede Workfront-Instanz.
1. (Optional und bedingt) Klicken Sie während der Eingabe der Anforderung auf [!UICONTROL **Entwurf verwerfen**] , wenn Sie den automatisch erstellten Entwurf löschen möchten. Dadurch wird der Entwurf gelöscht, der nicht wiederhergestellt werden kann. Es wird eine Bestätigungsmeldung angezeigt, die bestätigt, dass Sie den Entwurf löschen.

1. (Optional) Klicken Sie in der Bestätigungsmeldung auf [!UICONTROL **Rückgängig**] , wenn Sie Ihre Aktion wiederherstellen und den Entwurf beibehalten möchten.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Senden** , wenn Sie bereit sind, die Anfrage zu senden. Die Anforderung wird im Abschnitt Gesendet gespeichert. Abhängig von der Routing-Regel der Anforderungswarteschlange kann diese Anforderung an ein anderes Projekt als an das als Anforderungswarteschlange bestimmte weitergeleitet werden. Informationen zu Routing-Regeln finden Sie unter [Erstellen von Routing-Regeln](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Oder

     Klicken Sie auf **Schließen** , wenn Sie nicht ganz bereit sind, die Datei zu übermitteln, und Sie können sie später erneut abschließen. Ihre Anforderung wird im Abschnitt Entwürfe gespeichert und steht Ihnen beim nächsten Senden einer Anforderung für diese Anforderungswarteschlange zur Verfügung.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

   Wenn Sie die Anforderung senden, wird der Entwurf automatisch gelöscht und kann nicht wiederhergestellt werden.

   Weitere Informationen zum Umgang mit eingehenden Anforderungen finden Sie im Artikel [Verwalten von Arbeits- und Teamanfragen](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   Informationen zum Auffinden gesendeter oder entworfener Anforderungen finden Sie auch unter [Gesendete Anforderungen lokalisieren](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Anforderungen von außerhalb von Workfront erstellen

Sie können einen direkten Link zu einer Anforderungswarteschlange freigeben, wenn Sie eine neue Anforderung senden, und ihn in andere Anwendungen einbetten. Benutzer, die über das Internet oder andere Anwendungen auf diesen Link zugreifen, müssen ebenfalls mit einem aktiven Workfront-Konto angemeldet sein, um auf diese Warteschlange zugreifen und Anfragen an sie senden zu können. Weitere Informationen finden Sie unter [Link zu einer Anforderungswarteschlange freigeben](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Erstellen von Anforderungen per E-Mail an Workfront

Wenn Ihre Anforderungswarteschlange für den Empfang von Anfragen per E-Mail aktiviert ist, können Sie Ihre Anfragen direkt an die E-Mail-Adresse senden, die mit der Anforderungswarteschlange verknüpft ist.

Der Haupttext der E-Mail wird als Anforderungsbeschreibung hinzugefügt.

>[!NOTE]
>
>Die HTML-Formatierung wird entfernt, wenn die Anforderung in Workfront eingeht, aber Signaturen und vorhandene Reply-to-Thread-Inhalte werden nicht entfernt und in der Anforderungsbeschreibung angezeigt.

Informationen dazu, wie Sie eine Anforderungswarteschlange aktivieren, um Anfragen per E-Mail zu empfangen, finden Sie unter [Aktivieren von Benutzern, ein Problem per E-Mail an ein Anforderungswarteschlangenprojekt zu senden](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Anforderungen mit dem Outlook-Client erstellen

Sie können Anforderungen mit dem Outlook-Client senden. Sie können eine neue Anforderung erstellen oder eine E-Mail in eine Anforderung konvertieren.

Informationen zum Senden von Anforderungen mit dem Outlook-Client finden Sie im Artikel [Erstellen einer Adobe Workfront-Anfrage von einer Outlook-E-Mail](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Erstellen von Anforderungen mithilfe der mobilen Workfront-App

Sie können Anfragen über die Mobile App auf Ihrem Smartphone senden. Sie können eine neue Anforderung erstellen und an die Anforderungswarteschlangen senden, auf die Sie in der Webanwendung Zugriff haben.

Informationen zum Senden von Anfragen über die mobile App finden Sie im Abschnitt Anforderungen in den Artikeln:

* [Adobe Workfront für Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests)
* [Adobe Workfront für iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md#requests)

## Anforderungen aus anderen Anwendungen erstellen

Sie können Anfragen mit allen Anwendungen senden, die in Workfront integriert wurden:

* Sie können eine benutzerdefinierte Integration zwischen Workfront und einer anderen Anwendung erstellen, mit der Sie Anforderungen von der anderen Anwendung an Workfront senden können.\
  Weitere Informationen zu benutzerdefinierten Workfront-Integrationen finden Sie im Artikel [Adobe Workfront-Integrationen](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* Sie können Anfragen von Salesforce senden, wenn Sie die Workfront-App für Salesforce installiert haben.\
  Informationen zum Senden von Anfragen von Salesforce mithilfe unserer Workfront-App für Salesforce finden Sie im Artikel [Senden von Adobe Workfront-Anfragen von Salesforce-Objekten](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## Gesendete Anforderungen suchen

Informationen zum Auffinden gesendeter oder entworfener Anforderungen finden Sie unter [Gesendete Anforderungen suchen](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
