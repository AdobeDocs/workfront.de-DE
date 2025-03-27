---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Anfrage-Warteschlange erstellen
description: Sie können eine Anfrage-Warteschlange einrichten, in der Benutzer gelegentliche Anfragen eingeben können, die nicht für die Arbeit an einem Projekt geplant sind. Beispielsweise kann eine Helpdesk-Anfragewarteschlange eingerichtet werden, um alle Benutzeranfragen zu erfassen, die an eine IT-Abteilung gesendet werden.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '5167'
ht-degree: 2%

---


# Anfrage-Warteschlange erstellen

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--hide/ comment out the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Sie können eine Anfrage-Warteschlange einrichten, in der Benutzer gelegentliche Anfragen eingeben können, die nicht für die Arbeit an einem Projekt geplant sind. Beispielsweise kann eine Helpdesk-Anfragewarteschlange eingerichtet werden, um alle Benutzeranfragen zu erfassen, die an eine IT-Abteilung gesendet werden.

Anfragen werden zu Problemen in Adobe Workfront und werden zu Projekten hinzugefügt.

Das Einrichten einer Anfrage-Warteschlange hilft beim Formalisieren von Informationen zu Problemen, die einem Projekt hinzugefügt werden. Alle an das Projekt gesendeten Probleme werden auf die gleiche Weise gesendet und folgen demselben Pfad zum Abschluss.

Sie können die folgenden Objekte als Anfrage-Warteschlangen in Workfront einrichten:

* Projekte
* Vorlagen. Projekte, die aus Vorlagen erstellt werden, die als Anforderungswarteschlangen eingerichtet wurden, werden zu Anforderungswarteschlangen.

Um ein Projekt oder eine Vorlage als Anfrage-Warteschlange einzurichten, müssen Sie den Bereich Warteschlangendetails des Projekts oder der Vorlage bearbeiten.

In diesem Artikel wird beschrieben, wie Sie ein Projekt als Anfrage-Warteschlange konfigurieren können, in der Benutzer Anfragen senden können. Das Einrichten von Warteschlangendetails für eine Vorlage ähnelt dem Einrichten dieser Details für das Projekt.

Weitere Informationen zum Senden einer neuen Anfrage an eine Anfrage-Warteschlange finden Sie unter [Anforderungen kopieren und senden](../create-requests/copy-and-submit-requests.md).

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
   <td> 
   <p>Neue Lizenz: Standard </p>
   Oder
   <p>Aktuelle Lizenz: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Verwalten von Berechtigungen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Übersicht über Anfrage-Warteschlangen

Sie richten eine Anfrage-Warteschlange als Projekt ein. Wenn Sie das Projekt als Anfrage-Warteschlange festlegen, kann über den Bereich Anfragen in Adobe Workfront auf die Warteschlange zugegriffen werden. Wenn Sie die Anfrage-Warteschlange anpassen, passen Sie auch die Formularbenutzer an, die beim Senden der Anfragen ausgefüllt werden.

In diesem Artikel wird beschrieben, wie Sie eine Anfrage-Warteschlange aus einem vorhandenen Projekt erstellen. Um jedoch Konsistenz für den Anfrageeingangsprozess zu gewährleisten oder um mehrere Ebenen für Reporting-Zwecke und eine bessere Verwaltung hinzuzufügen, können Sie auch zusätzliche Bausteine einer Anfragewarteschlange konfigurieren, die in der folgenden Tabelle beschrieben werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Warteschlangendetails</td> 
   <td> <p>Sie müssen ein Projekt als Anfrage-Warteschlange im Bereich Warteschlangendetails einrichten. Dieser Schritt ist obligatorisch. </p> <p>Weitere Informationen finden Sie im <a href="#create-a-request-queue" class="MCXref xref">Erstellen einer Anfrage</a>Warteschlange) in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Themengruppen</td> 
   <td> <p>Hierbei handelt es sich um zusätzliche Menüs, in denen Anfragen anhand gängiger Funktionen klassifiziert werden. Beispielsweise empfiehlt es sich für eine IT-Anfrage-Warteschlange, Themengruppen „Vor Ort“ und „Remote“ zu verwenden. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Themengruppen erstellen</a>. </p> <p>Dies ist optional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Warteschlangenthemen</td> 
   <td> <p>Hierbei handelt es sich um zusätzliche Menüs, in denen Anfragen, die derselben Themengruppe angehören, basierend auf gemeinsamen Funktionen klassifiziert werden. Eine Themengruppe kann mehrere Warteschlangenthemen enthalten. </p> <p>Beispielsweise kann die Themengruppe „Vor-Ort“ für die IT-Anforderungswarteschlange die Warteschlangenthemen „Hardware“, „Software“ und „Netzwerk“ enthalten. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Warteschlangenthemen erstellen</a>. </p> <p>Dies ist optional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Routing-Regeln</td> 
   <td> <p>Sie ermöglichen es Ihnen, jede Anfrage an einen Benutzer, ein Aufgabengebiet, ein Team oder ein Projekt weiterzuleiten. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Routing-Regeln erstellen</a>. </p> <p>Dies ist optional.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anfrage-Warteschlange erstellen

<!--at production release on April 10, do the following: take the first sentence here out; hide/ comment out the first section (Create a Request Queue in the Production environment); remove the title of the "Create a Request Queue in the Preview environment and leave that section as the only way to create request queues; search for any visible references of production/ preview and remove them from the entire article-->

Das Erstellen einer Anfrage-Warteschlange unterscheidet sich je nach verwendeter Umgebung.

### Erstellen einer Anfrage-Warteschlange in der Produktionsumgebung

In diesem Abschnitt wird beschrieben, wie Sie Warteschlangendetails für die folgenden Objekte definieren können:

* Ein Projekt in der Produktionsumgebung
* Eine Vorlage in der Produktions- oder Vorschauumgebung

Wenn Sie ein Projekt als Anfrage-Warteschlange einrichten, muss der Projektstatus Aktuell sein, damit er im Bereich Anfragen von Workfront angezeigt wird.

>[!TIP]
>
>Ihr Workfront- oder Gruppen-Administrator kann Ihnen eine benutzerdefinierte Layout-Vorlage zuweisen, die möglicherweise nicht alle der in den folgenden Schritten beschriebenen Abschnitte enthält.


So erstellen Sie eine Anfrage-Warteschlange:

1. Wechseln Sie zu dem Projekt, das Sie als Anfrage-Warteschlange einrichten möchten.
1. (Optional) Klicken Sie **linken Bereich auf****Projektdetails) und fügen Sie dem Projekt** Bereich **Übersicht** eine Beschreibung hinzu. Diese Informationen werden bei allen neuen Anfragen angezeigt.
1. Klicken Sie **linken Bedienfeld** Warteschlangendetails“. Möglicherweise müssen Sie auf **Weitere anzeigen** und dann auf **Warteschlangendetails** klicken.

   Dadurch wird der Abschnitt Warteschlangendetails geöffnet.

   ![Warteschlangendetails am Anfang des Abschnitts](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Geben Sie die folgenden Informationen an:

   * **Als Warteschlange für Hilfeanfragen veröffentlichen:** Wählen Sie diese Option, um dieses Projekt als Anforderungswarteschlange zu identifizieren. Alle eingehenden Anfragen werden als Anfragen betrachtet.\
     Wenn diese Option nicht ausgewählt ist, verhält sich das Projekt wie ein Standardprojekt in Workfront, und alle eingehenden Probleme sind Probleme.

   * **Wer kann dieser Warteschlange Anforderungen hinzufügen:** Wählen Sie aus, welche Benutzer Zugriff haben, um Anforderungen zu dieser Warteschlange hinzuzufügen. Sie können den folgenden Personengruppen erlauben, die Anfrage-Warteschlange in ihrem Anfragebereich der globalen Navigationsleiste anzuzeigen, wenn sie eine neue Anfrage hinzufügen:

     | Wer Anfragen eingeben kann | Beschreibung |
     |---|---|
     | Jeder | Jeder Workfront-Benutzer mit einem aktiven Konto kann diese Anfrage-Warteschlange einsehen und ihr Anfragen hinzufügen |
     | Benutzer mit Ansichtszugriff auf dieses Projekt | Benutzende mit Anzeigeberechtigungen für das Projekt können Anfragen anzeigen und zu dieser Warteschlange hinzufügen |
     | Personen im Unternehmen dieses Projekts | Benutzer, die zu dem Unternehmen gehören, das mit diesem Projekt verknüpft ist, können Anfragen anzeigen und zu dieser Warteschlange hinzufügen. Wenn dem Projekt eine Firma zugeordnet ist, wird der Name der Firma nach dieser Einstellung in Klammern aufgeführt. |
     | Personen in der Gruppe dieses Projekts | Benutzer, die zu der mit diesem Projekt verknüpften Gruppe gehören, können Anfragen anzeigen und zu dieser Warteschlange hinzufügen. Wenn mit dem Projekt eine Gruppe verknüpft ist, wird der Name der Gruppe nach dieser Einstellung in Klammern in grauer Schriftart aufgeführt. |

     {style="table-layout:auto"}

   * **Über diese Links freigeben** Mit den folgenden Optionen können Sie Benutzern außerhalb von Workfront oder Workfront-Benutzern, die eine externe Seite verwenden, direkten Zugriff auf die Anfrage-Warteschlange und die damit verbundenen Formulare gewähren. Informationen zum Einbetten einer Anfrage-Warteschlange in ein Dashboard als externe Seite finden Sie unter [Anfrage-Warteschlange in ein Dashboard einbetten](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Benutzer müssen bereits über Zugriffsrechte für die Anfrage-Warteschlange verfügen, um direkten Zugriff zu erhalten. Durch die Verwendung einer der hier beschriebenen Optionen wird Benutzenden nicht automatisch Zugriff gewährt.

     >[!TIP]
     >
     >Anwender müssen sich zuerst bei Workfront anmelden, bevor sie Zugriff auf die Anfrage-Warteschlange erhalten, wenn sie von einem anderen Programm aus auf die Seite „Anfrage-Warteschlange“ zugreifen.

      * **Direktzugriff-URL:** Wenn ein Benutzer über einen Browser auf diese URL zugreift, wird der Benutzer direkt zum Abschnitt „Neue Anfrage“ im Bereich „Anfragen“ geleitet und diese Anfrage ist standardmäßig für ihn ausgewählt.

        ![Anfrage-Warteschlange mit direkter URL im Dashboard freigeben](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >Sie können eine Anfrage-Warteschlange in einem Dashboard als externe Seite anzeigen. In diesem Fall ist die Anfragewarteschlange vorausgewählt, Sie können jedoch eine beliebige andere Anfragewarteschlange aus dem Feld Anfragetyp auswählen. Benutzer können den Anfragetyp ändern. Navigationskomponenten der Anfragen werden ebenfalls angezeigt.

      * **Einbettungs-Code:** Verwenden Sie diesen HTML-Code, um das Formular für die Anfrage-Warteschlange als iframe in eine beliebige HTML-Seite einzubetten.\
        Wenn Benutzende nicht bereits bei Workfront authentifiziert sind, wenn sie die Seite aufrufen, auf der der Code eingebettet ist, wird das Workfront-Anmeldedialogfeld angezeigt. Nachdem sich Benutzer angemeldet haben, wird das Formular Anfrage-Warteschlange angezeigt.

        >[!NOTE]
        >
        >Wenn eine Anfrage-Warteschlange in einem IFrame angezeigt wird, wird nur das Anfrage-Formular angezeigt, und der Name der Anfrage ist vorab ausgewählt und abgeblendet. Der Benutzer kann den Anfragetyp nicht ändern. Navigationskomponenten des Bereichs Anfragen werden nicht angezeigt.

        Damit das Formular für die Anfrage-Warteschlange bei Verwendung dieses Einbettungs-Codes angezeigt wird, müssen Sie in Ihrem System-Setup die Einstellung „Einbettung von Workfront in einen iframe zulassen“ aktivieren. Weitere Informationen zum Aktivieren der Einbettung von Workfront in einen iframe finden Sie unter [Systemsicherheitseinstellungen konfigurieren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Wenn diese Einstellung nicht aktiviert ist, wird der IFrame als leer angezeigt.

        Sie können verschiedene Aspekte der Anzeige des eingebetteten Formulars wie folgt anpassen:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funktionalität</strong> </p> </th> 
           <th> <p><strong>Lösung</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Anpassen der Rahmengröße</p> </td> 
           <td> <p>Ändern Sie die Attribute „width“ und „height“.</p> <p>Standardmäßig ist die Breite „500“ und die Höhe „600“</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Benutzer zu einem bestimmten Warteschlangenthema oder einer bestimmten Themengruppe weiterleiten</p> </td> 
           <td> <p>Fügen Sie den Parameter „path“ zur src-URL hinzu. Sie können den Pfadparameter finden, indem Sie zum gewünschten Warteschlangenthema oder zur gewünschten Themengruppe im nicht eingebetteten Formular navigieren und die URL überprüfen.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Anzeigen und Zulassen, dass Benutzer die vorkonfigurierte Dropdown-Liste Themengruppe ändern</p> </td> 
           <td> <p>Verwenden Sie den Parameter „path“, indem Sie dem <code>src URL</code> den Parameter <code>showPreSelectedOptions=true</code> hinzufügen.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Erkennen, wann das Formular gesendet wurde</p> </td> 
           <td> <p>Fügen Sie einen Ereignis-Listener „Nachricht“ zum Fenster Ihrer Web-Seite hinzu und überprüfen Sie, ob <code>event.data.type</code> <code>requestSubmitted</code> ist. <code>event.data.newIssueID</code> wird auf die ID des erstellten Problems gesetzt.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Anfragetypen:** Sie aus den unten stehenden Standardoptionen aus.

     Der Workfront-Administrator kann die Standardanfragetypen umbenennen. Weitere Informationen zum Umbenennen der Anfragetypen finden Sie unter [Anpassen von Standardanfragetypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Fehlerbericht
      * Änderungsanforderung
      * Problem
      * Anfrage

        Dies ist ein Pflichtfeld, und Sie müssen mindestens eine Option auswählen.

     >[!NOTE]
     >
     >Anfragetypen werden nur dann als Auswahl im Bereich Anfragen angezeigt, wenn der Anfragetyp sowohl auf der Seite Warteschlangendetails als auch auf der Seite Warteschlangenthema ausgewählt ist. Informationen zum Einrichten des Bereichs „Warteschlangendetails“ eines Projekts finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Jeder hier ausgewählte Typ ist im Formular verfügbar (Sie können mehrere Typen auswählen). Die Auswahl mehrerer Typen kann dabei helfen, mehrere eingehende Anfragen zu organisieren.\
     Wenn Sie das Formular beispielsweise in einer Anfrage-Warteschlange für ein IT-Projekt verwenden, können die folgenden Anfragetypen in die Warteschlange aufgenommen werden: Hardware, Software, Fehlerbehebungen und Probleme.

   * **Standarddauer:** Die Standarddauer ist die Zeit, die normalerweise zum Beheben eines Problems benötigt wird. Dies wird zur Standardeinstellung für alle eingehenden Probleme und kann manuell geändert werden. Die Dauer wird im Allgemeinen in Stunden, Tagen oder Wochen festgelegt. Die Standarddauer eines Problems entspricht den für das Problem geplanten Stunden. Das geplante Abschlussdatum der Anfrage wird auf Grundlage dieses Felds berechnet.\
     Der Standardwert für die Problemdauer ist 1 Tag oder 8 Stunden. Wenn Ihr Workfront-Administrator die typischen Stunden pro Arbeitstag auf weniger als 8 Stunden festgelegt hat, beträgt die Standarddauer für Probleme weiterhin 8 Stunden. Wenn beispielsweise die typischen Stunden pro Arbeitstag auf 7 Stunden eingestellt sind, beträgt die Standarddauer für Probleme 1,14 Tage oder 8 Stunden. Weitere Informationen zum Einrichten des Systems „Typische Stunden pro Arbeitstag“ finden Sie im Abschnitt „Zeitleistenberechnungen“ im Artikel [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Personen aus demselben Unternehmen erben dieselben Berechtigungen für alle Anfragen.:** Wenn diese Option aktiviert ist, sind alle an die Warteschlange gesendeten Anfragen für Benutzer im selben Unternehmen sichtbar. Benutzer können diese Anfragen im Abschnitt Alle Anfragen anzeigen, der sich im Bereich Anfragen befindet. Zum Zeitpunkt der Aktivierung oder Deaktivierung dieser Einstellung wirkt sich dies nicht rückwirkend auf die Informationen aus, sondern auf alle zukünftigen Anfragen.
   * **Wenn jemand eine Anfrage stellt, automatisch erteilen:** Wenn ein Benutzer eine Anfrage an die Anfrage-Warteschlange sendet, wird dem Benutzer automatisch die Berechtigungsstufe gewährt, die Sie für diese Anfrage auswählen. Wählen Sie aus den folgenden Berechtigungsebenen aus:

      * **Ansichtszugriff**
      * **Beitragszugriff**. Dies ist die Standardauswahl.
      * **Zugriff verwalten**

     Weitere Informationen zum Workfront-Berechtigungsmodell finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Wenn Sie hier Berechtigungen festlegen, sparen Sie Zeit, da Sie nicht für jede einzelne eingehende Anfrage Berechtigungen erteilen müssen. Die Auswahl dieser Option wirkt sich auf alle zukünftigen Anfragen aus, hat jedoch keine rückwirkenden Auswirkungen auf bestehende Anfragen.

   * **Standardgenehmigung**: Verknüpfen Sie einen Genehmigungsprozess mit dieser Anfrage-Warteschlange. In diesem Dropdown-Menü werden nur Problemgenehmigungsprozesse angezeigt. Alle an diese Warteschlange gesendeten Probleme werden mit diesem Genehmigungsprozess verknüpft. Ihr Workfront-Administrator muss Genehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Anfragewarteschlangen verknüpfen können. Benutzende mit administrativem Zugriff auf Genehmigungsprozesse können auch gruppenspezifische Genehmigungsprozesse erstellen.

     >[!IMPORTANT]
     >
     >Wenn sich die Gruppe des Projekts ändert, wird der gruppenspezifische Genehmigungsprozess, der an vorhandene Probleme angehängt ist, zu einem einmaligen Genehmigungsprozess. Weitere Informationen darüber, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter [Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Wenn mehrere Warteschlangenthemen mit einer Anfrage-Warteschlange verknüpft sind, empfehlen wir, stattdessen Genehmigungsprozesse mit den Warteschlangenthemen zu verknüpfen. Weitere Informationen zum Erstellen von Warteschlangenthemen finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Beachten Sie beim Hinzufügen von Genehmigungsprozessen zu Anfrage-Warteschlangen Folgendes:

      * In der Liste werden nur aktive Genehmigungsprozesse angezeigt.
      * In der Liste werden systemweite und gruppenspezifische Genehmigungsprozesse angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt.

   * **Standardroute**: Verknüpfen Sie diese Anfrage-Warteschlange mit einer Routing-Regel. Verwenden Sie Routing-Regeln, um neue Probleme, die an eine Anfrage-Warteschlange gesendet wurden, automatisch der richtigen Ressource (Benutzer, Aufgabengebiet oder Team) und dem richtigen Projekt zuzuweisen. Alle an diese Warteschlange gesendeten Probleme werden dieser Routingregel zugeordnet. Sie müssen Routing-Regeln konfigurieren, bevor sie im Abschnitt Warteschlangendetails angezeigt werden und bevor Sie sie mit der Anfrage-Warteschlange verknüpfen können.\
     Wenn mehrere Warteschlangenthemen mit einer Anfrage-Warteschlange verknüpft sind, empfehlen wir, stattdessen Routing-Regeln mit den Warteschlangenthemen zu verknüpfen. Weitere Informationen zum Erstellen von Routingregeln finden Sie unter [Routingregeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Neue Problemfelder:** Wählen Sie im Abschnitt **Die folgenden ausgewählten Felder für alle Benutzer anzeigen** alle Felder aus, die für alle Benutzer sichtbar sein sollen, die eine Anfrage an das Projekt senden oder ein Problem zum Projekt oder zu den Aufgaben hinzufügen.

     >[!TIP]
     >
     >Neue Anfragefelder, die im Abschnitt Warteschlangendetails ausgewählt sind, sind auch mit allen neuen Anfragen verknüpft, die dem <!--this is confusing: or to the tasks in the Issues section--> hinzugefügt werden.

     Wenn Sie die Felder Zugewiesen an, Aufgabengebiet oder Team aktivieren, werden sie im Anfrageformular immer in Zuweisungen umbenannt, Sie können jedoch nur den hier ausgewählten Zuweisungstyp angeben.

     >[!NOTE]
     >
     >Wenn Sie im Bereich „Warteschlangendetails“ die Option „Zugewiesen an“ ausgewählt haben, können Sie im Anforderungsformular nur Benutzer in das Feld „Zuweisungen“ eingeben. In diesem Fall können Sie keine Aufgabengebiete oder ein Team eingeben.

   * **Dokumente**: Wenn Sie den Abschnitt „Dokumente“ im neuen Anfrageformular anzeigen, wählen Sie aus, wo der Abschnitt „Dokument hochladen“ platziert werden soll. Wählen Sie aus den folgenden Optionen aus:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Nach benutzerdefinierten Formularen</td> 
        <td><span>Der Abschnitt Dokumente wird unten im Anfrageformular angezeigt.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Vor benutzerdefinierten Formularen</td> 
        <td> <p><span>Der Abschnitt Dokumente wird zwischen den Workfront-Feldern und den benutzerdefinierten Feldern des Anfrageformulars angezeigt.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![Neuer Problemfeldbereich mit Dokumenten](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Alle ausgewählten und nicht ausgewählten Felder anzeigen für** Wählen Sie aus, für welche Benutzer alle Felder im neuen Anfrageformular angezeigt werden sollen. Die folgenden Optionen steuern den Zugriff auf die Felder im Formular.

     | Benutzer, die alle Felder im Anfrageformular sehen können | Beschreibung |
     |---|---| 
     | Alle Benutzer (Planlizenzen) | Alle Benutzer, die über eine Planlizenz verfügen, können die ausgewählten sowie die nicht ausgewählten Felder sehen. |
     | Personen mit Ansichtszugriff auf dieses Projekt (Planlizenz) | Benutzer mit einer Planlizenz, die auch über Ansichtsrechte für dieses Projekt verfügen, können die ausgewählten sowie die nicht ausgewählten Felder sehen. Der Rest der Benutzer, die Anfragen an dieses Projekt senden können, kann nur die ausgewählten Felder sehen. |
     | Keine Benutzer | Die nicht ausgewählten Felder können nicht von Benutzenden angezeigt werden. Alle Benutzer, die Anfragen an dieses Projekt senden können, können nur die ausgewählten Felder sehen. |

   * **Benutzerdefinierte Forms**: Wählen Sie ein benutzerdefiniertes Formular aus, das mit der Anfrage-Warteschlange verknüpft werden soll. In diesem Dropdown-Menü stehen nur benutzerdefinierte Forms für Probleme zur Auswahl. Allen Anfragen, die an die Anfrage-Warteschlange gesendet werden, sind die ausgewählten Formulare zugeordnet. Sie müssen benutzerdefinierte Anfrageformulare erstellen, bevor Sie sie im Abschnitt Warteschlangendetails anzeigen können.
Wenn einer Anfrage-Warteschlange mehrere Warteschlangenthemen zugeordnet sind, empfehlen wir, stattdessen benutzerdefinierte Formulare mit den Warteschlangenthemen zu verknüpfen. Weitere Informationen zum Erstellen von Unterabschnitten für die Anfrage-Warteschlange finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Benutzerdefinierte Formulare in Warteschlangendetails](assets/custom-forms-on-queue-details.png)

     Wenn mehrere benutzerdefinierte Formulare mit der Anfrage-Warteschlange verknüpft sind, ziehen Sie die Formulare per Drag-and-Drop, um sie in der gewünschten Reihenfolge zu sortieren, im Abschnitt **Forms neu**.

     >[!TIP]
     >
     >Benutzerdefinierte Formulare, die zum Abschnitt Warteschlangendetails hinzugefügt wurden, sind auch mit allen neuen Problemen verknüpft, die zum <!--this is confusiong: or the tasks in the Issues  section--> hinzugefügt wurden.

1. Wählen Sie weiterhin Informationen für die Einstellungen im Bereich **E-Mail-Warteschlangeneinstellungen** aus, damit Benutzer E-Mail-Anfragen an das Projekt für die Anfrage-Warteschlange senden können.

   Weitere Informationen finden Sie unter [Benutzer können ein Problem per E-Mail an ein Anfrage-Warteschlangenprojekt senden](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Klicken Sie auf **Speichern**.\
   Ihr Projekt wurde jetzt als Anfrage-Warteschlange konfiguriert, und Benutzer können ihm jetzt Anforderungen hinzufügen.

1. (Optional) Um die Funktionalität für die Anfrage-Warteschlange zu verbessern, erstellen Sie zusätzliche Unterabschnitte für Ihre Warteschlange sowie Regeln für die Weiterleitung der eingehenden Anfragen an das richtige Team, den richtigen Verantwortlichen oder das richtige Projekt.

   * Informationen zum Erstellen von Unterabschnitten für die Anfrage-Warteschlange finden Sie in den Artikeln [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) und [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * Weitere Informationen zum Weiterleiten der Anfragen an den entsprechenden Verantwortlichen, das entsprechende Team und das entsprechende Projekt finden Sie unter [Routing-Regeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

<div class="preview">

### Erstellen einer Anfrage-Warteschlange in der Vorschau-Umgebung

Wenn Sie ein Projekt als Anfrage-Warteschlange einrichten, muss der Projektstatus Aktuell sein, damit er im Bereich Anfragen von Workfront angezeigt wird.

>[!TIP]
>
>Ihr Workfront- oder Gruppen-Administrator kann Ihnen eine benutzerdefinierte Layout-Vorlage zuweisen, die möglicherweise nicht alle der in den folgenden Schritten beschriebenen Abschnitte enthält.

So erstellen Sie eine Anfrage-Warteschlange:

1. Wechseln Sie zu dem Projekt, das Sie als Anfrage-Warteschlange einrichten möchten.
1. (Optional) Klicken Sie **linken Bereich auf****Projektdetails) und fügen Sie dem Projekt** Bereich **Übersicht** eine Beschreibung hinzu. Diese Informationen werden bei allen neuen Anfragen angezeigt.
1. Klicken Sie **linken Bedienfeld** Warteschlangendetails“. Möglicherweise müssen Sie auf **Weitere anzeigen** und dann auf **Warteschlangendetails** klicken.

   Dadurch wird der Abschnitt Warteschlangendetails geöffnet.

   ![Abschnitt „Warteschlangentyp“ im Bereich „Warteschlangendetails“](assets/unshimmed-queue-type-section-queue-details-area.png)

1. Geben Sie die folgenden Informationen an:

   * **Als Warteschlange für Hilfeanfragen veröffentlichen**: Wählen Sie diese Option, um dieses Projekt als Anfragewarteschlange zu identifizieren. Alle eingehenden Anfragen werden als Anfragen betrachtet.\
     Wenn diese Option nicht ausgewählt ist, verhält sich das Projekt wie ein Standardprojekt in Workfront, und alle eingehenden Probleme sind Probleme.

   * **Wer kann dieser Warteschlange Anforderungen hinzufügen?**: Wählen Sie aus, welche Benutzer Zugriff haben, um Anfragen zu dieser Warteschlange hinzuzufügen. Sie können den folgenden Personengruppen erlauben, die Anfrage-Warteschlange in ihrem Anfragebereich der globalen Navigationsleiste anzuzeigen, wenn sie eine neue Anfrage hinzufügen:

     | Wer Anfragen eingeben kann | Beschreibung |
     |---|---|
     | Jeder | Jeder Workfront-Benutzer mit einem aktiven Konto kann diese Anfrage-Warteschlange einsehen und ihr Anfragen hinzufügen |
     | Benutzer mit Ansichtszugriff auf dieses Projekt | Benutzende mit Anzeigeberechtigungen für das Projekt können Anfragen anzeigen und zu dieser Warteschlange hinzufügen |
     | Personen im Unternehmen dieses Projekts | Benutzer, die zu dem Unternehmen gehören, das mit diesem Projekt verknüpft ist, können Anfragen anzeigen und zu dieser Warteschlange hinzufügen. Wenn dem Projekt eine Firma zugeordnet ist, wird der Name der Firma nach dieser Einstellung in Klammern aufgeführt. |
     | Personen in der Gruppe dieses Projekts | Benutzer, die zu der mit diesem Projekt verknüpften Gruppe gehören, können Anfragen anzeigen und zu dieser Warteschlange hinzufügen. Wenn mit dem Projekt eine Gruppe verknüpft ist, wird der Name der Gruppe nach dieser Einstellung in Klammern in grauer Schriftart aufgeführt. |

     {style="table-layout:auto"}

   * Verwenden Sie die folgenden Optionen, um Benutzern außerhalb von Workfront oder Workfront-Benutzern mithilfe einer eingebetteten externen Seite direkten Zugriff auf die Anfrage-Warteschlange und die damit verbundenen Formulare bereitzustellen.

   Informationen zum Einbetten einer Anfrage-Warteschlange in ein Dashboard als externe Seite finden Sie unter [Anfrage-Warteschlange in ein Dashboard einbetten](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

   Benutzer müssen zunächst über Berechtigungen für die Anfrage-Warteschlange verfügen, um direkten Zugriff zu erhalten. Durch die Verwendung einer der hier beschriebenen Optionen wird Benutzenden nicht automatisch Zugriff gewährt.

   >[!TIP]
   >
   >Anwender müssen sich zuerst bei Workfront anmelden, bevor sie Zugriff auf die Anfrage-Warteschlange erhalten, wenn sie von einem anderen Programm aus auf die Seite „Anfrage-Warteschlange“ zugreifen.

   * **Direktzugriff-URL:** Wenn ein Benutzer über einen Browser auf diese URL zugreift, wird der Benutzer direkt zum Abschnitt „Neue Anfrage“ im Bereich „Anfragen“ geleitet und diese Anfrage ist standardmäßig für ihn ausgewählt.

     ![Neues Anfragefeld von Direct URL Share](assets/new-request-box-from-direct-url-share.png)

     >[!NOTE]
     >
     >Sie können eine Anfrage-Warteschlange in einem Dashboard als externe Seite anzeigen. In diesem Fall ist die Anfragewarteschlange vorausgewählt, Sie können jedoch eine beliebige andere Anfragewarteschlange aus dem Feld Anfragetyp auswählen. Benutzer, die die Anfrage senden, können einen anderen Anfragetyp auswählen. Themengruppen und Warteschlangenthemen werden ebenfalls angezeigt.

   * **Einbettungs-Code:** Verwenden Sie diesen HTML-Code, um das Formular für die Anfrage-Warteschlange als iframe in eine beliebige HTML-Seite einzubetten.\
     Wenn Benutzende nicht bereits bei Workfront authentifiziert sind, wenn sie die Seite aufrufen, auf der der Code eingebettet ist, wird das Workfront-Anmeldedialogfeld angezeigt. Nachdem sich Benutzer angemeldet haben, wird das Formular Anfrage-Warteschlange angezeigt.

     >[!NOTE]
     >
     >Wenn eine Anfrage-Warteschlange in einem IFrame angezeigt wird, wird nur das Anfrage-Formular angezeigt, und der Name der Anfrage ist vorab ausgewählt und abgeblendet. Der Benutzer kann den Anfragetyp nicht ändern. Navigationskomponenten des Bereichs Anfragen werden nicht angezeigt.

     Damit das Formular für die Anfrage-Warteschlange bei Verwendung dieses Einbettungs-Codes angezeigt wird, muss der Workfront-Administrator die Einstellung „Einbetten von Workfront in einen iframe zulassen“ im Bereich „System-Setup“ aktivieren.

     Weitere Informationen zum Aktivieren der Einbettung von Workfront in einen iframe finden Sie unter [Systemsicherheitseinstellungen konfigurieren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Wenn diese Einstellung nicht aktiviert ist, wird der IFrame als leer angezeigt.

     Sie können verschiedene Aspekte der Anzeige des eingebetteten Formulars wie folgt anpassen:

     <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funktionalität</strong> </p> </th> 
           <th> <p><strong>Lösung</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Anpassen der Rahmengröße</p> </td> 
           <td> <p>Ändern Sie die Attribute „width“ und „height“.</p> <p>Standardmäßig ist die Breite „500“ und die Höhe „600“</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Benutzer zu einem bestimmten Warteschlangenthema oder einer bestimmten Themengruppe weiterleiten</p> </td> 
           <td> <p>Fügen Sie den Parameter „path“ zur src-URL hinzu. Sie können den Pfadparameter finden, indem Sie zum gewünschten Warteschlangenthema oder zur gewünschten Themengruppe im nicht eingebetteten Formular navigieren und die URL überprüfen.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Anzeigen und Zulassen, dass Benutzer die vorkonfigurierte Dropdown-Liste Themengruppe ändern</p> </td> 
           <td> <p>Verwenden Sie den Parameter „path“, indem Sie dem <code>src URL</code> den Parameter <code>showPreSelectedOptions=true</code> hinzufügen.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Erkennen, wann das Formular gesendet wurde</p> </td> 
           <td> <p>Fügen Sie einen Ereignis-Listener „Nachricht“ zum Fenster Ihrer Web-Seite hinzu und überprüfen Sie, ob <code>event.data.type</code> <code>requestSubmitted</code> ist. <code>event.data.newIssueID</code> wird auf die ID des erstellten Problems gesetzt.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Anfragetypen:** Wählen Sie im Abschnitt **Warteschlangeneigenschaften** eine der folgenden Optionen aus:

   * Fehlerbericht
   * Änderungsanforderung
   * Problem
   * Anfrage

   Dies ist ein Pflichtfeld, und Sie müssen mindestens eine Option auswählen.

   Der Workfront-Administrator kann die Standardanfragetypen umbenennen. Weitere Informationen zum Umbenennen der Anfragetypen finden Sie unter [Anpassen von Standardanfragetypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

   >[!NOTE]
   >
   >Wenn Benutzer über den Bereich Anfragen auf die Anfrage-Warteschlange zugreifen, werden die Anfragetypen nur dann als Auswahl angezeigt, wenn der Anfragetyp sowohl auf der Seite Warteschlangendetails als auch auf der Seite Warteschlangenthema ausgewählt ist.
   >
   >Informationen zum Einrichten des Bereichs Warteschlangenthemen eines Projekts finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   Jeder hier ausgewählte Typ ist im Formular verfügbar (Sie können mehrere Typen auswählen). Die Auswahl mehrerer Typen kann dabei helfen, mehrere eingehende Anfragen zu organisieren.\
   Wenn Sie das Formular beispielsweise in einer Anfrage-Warteschlange für ein IT-Projekt verwenden, können die folgenden Anfragetypen in die Warteschlange aufgenommen werden: Hardware, Software, Fehlerbehebungen und Probleme.

   * **Standarddauer:** Sie eine Zahl für die Dauer ein und wählen Sie dann aus dem Dropdown-Menü eine der folgenden Einheiten für die Dauer aus:

      * Tag(e)
      * Stunden
      * Minuten
      * Wochen

   Die Standarddauer ist die Zeit, die normalerweise benötigt wird, um ein an diese Anfrage-Warteschlange gesendetes Problem zu beheben. Dies wird zur Standardeinstellung für alle eingehenden Probleme und kann manuell geändert werden.
Die Standarddauer eines Problems entspricht den für das Problem geplanten Stunden. Das geplante Abschlussdatum der Anfrage wird auf Grundlage dieses Felds berechnet.\
   Wenn sie unverändert gelassen wird, beträgt der Standardwert für die Problemdauer 1 Tag oder 8 Stunden.
Wenn Ihr Workfront-Administrator im Bereich „Setup“ für jeden Arbeitstag einen Wert von unter 8 Stunden festgelegt hat, beträgt die Standarddauer für Probleme weiterhin 8 Stunden.
Wenn beispielsweise die Standardstundenzahl pro Arbeitstag im Bereich Setup von Workfront auf 7 Stunden festgelegt ist, beträgt die Standarddauer für Probleme 1,14 Tage oder 8 Stunden.
Weitere Informationen zum Einrichten des Systems „Typische Stunden pro Arbeitstag“ finden Sie im Abschnitt „Zeitleistenberechnungen“ im Artikel [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Personen aus demselben Unternehmen erben dieselben Berechtigungen für alle Anfragen.**: Wenn diese Option aktiviert ist, sind alle an die Warteschlange gesendeten Anfragen für Benutzer im selben Unternehmen sichtbar. Benutzer können diese Anfragen im Abschnitt Alle Anfragen anzeigen, der sich im Bereich Anfragen befindet. Zum Zeitpunkt der Aktivierung oder Deaktivierung dieser Einstellung wirkt sich dies nicht rückwirkend auf die Informationen aus, sondern auf alle zukünftigen Anfragen.
   * **Wenn jemand eine Anfrage stellt, automatisch erteilen…** Wenn ein Benutzer eine Anfrage an die Anfrage-Warteschlange sendet, wird dem Benutzer automatisch die Berechtigungsstufe gewährt, die Sie für diese Anfrage auswählen. Klicken Sie auf die Schaltfläche Zugriff , um aus den folgenden Berechtigungsebenen auszuwählen:

      * **Ansichtszugriff**
      * **Beitragszugriff**. Dies ist die Standardauswahl und der Name der Schaltfläche „Zugriff“.
      * **Zugriff verwalten**

     Weitere Informationen zum Workfront-Berechtigungsmodell finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Wenn Sie hier Berechtigungen festlegen, sparen Sie Zeit, da Sie für jede eingehende Anfrage nicht einzeln Berechtigungen erteilen müssen. Die Auswahl dieser Option wirkt sich auf alle zukünftigen Anfragen aus, hat jedoch keine rückwirkenden Auswirkungen auf bestehende Anfragen.

   * **Standardgenehmigung**: Klicken Sie auf das Dropdown-Menü, um einen Genehmigungsprozess für diese Anfrage-Warteschlange auszuwählen. In diesem Dropdown-Menü werden nur Problemgenehmigungsprozesse angezeigt. Alle an diese Warteschlange gesendeten Probleme werden mit diesem Genehmigungsprozess verknüpft. Ihr Workfront-Administrator muss Genehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Anfragewarteschlangen verknüpfen können. Benutzende mit administrativem Zugriff auf Genehmigungsprozesse können auch gruppenspezifische Genehmigungsprozesse erstellen.

     >[!IMPORTANT]
     >
     >Wenn sich die Gruppe des Projekts ändert, wird der gruppenspezifische Genehmigungsprozess, der an vorhandene Probleme angehängt ist, zu einem einmaligen Genehmigungsprozess. Weitere Informationen darüber, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter [Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Wenn mehrere Warteschlangenthemen mit einer Anfrage-Warteschlange verknüpft sind, empfehlen wir, stattdessen Genehmigungsprozesse mit den Warteschlangenthemen zu verknüpfen.

     Weitere Informationen zum Erstellen von Warteschlangenthemen finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Beachten Sie beim Hinzufügen von Genehmigungsprozessen zu Anfrage-Warteschlangen Folgendes:

      * In der Liste werden nur aktive Problemgenehmigungsprozesse angezeigt.
      * In der Liste werden systemweite und gruppenspezifische Problemgenehmigungsprozesse angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt.

   * **Standardroute**: Klicken Sie auf das Dropdown-Menü, um eine Routing-Regel für diese Anfrage-Warteschlange auszuwählen. Routing-Regeln weisen automatisch neue Probleme zu, die an eine Anfrage-Warteschlange gesendet wurden, an die richtige Ressource (Benutzer, Aufgabengebiet oder Team) und an das richtige Projekt. Alle an diese Warteschlange gesendeten Probleme werden dieser Routingregel zugeordnet. Sie müssen Routing-Regeln konfigurieren, bevor sie im Abschnitt Warteschlangendetails angezeigt werden und bevor Sie sie mit der Anfrage-Warteschlange verknüpfen können.\
     Wenn mehrere Warteschlangenthemen mit einer Anfrage-Warteschlange verknüpft sind, empfehlen wir, stattdessen Routing-Regeln mit den Warteschlangenthemen zu verknüpfen. Weitere Informationen zum Erstellen von Routingregeln finden Sie unter [Routingregeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Neue Problemfelder:** Wählen Sie im Abschnitt **Die folgenden ausgewählten Felder für alle Benutzer anzeigen** die Felder aus, die für alle Benutzer sichtbar sein sollen, die eine Anfrage an das Projekt senden oder ein Problem zu diesem Projekt oder den Aufgaben des Projekts hinzufügen.

     >[!NOTE]
     >
     >* Wenn Sie eines der Felder Zugewiesen an, Aufgabengebiet oder Team aktivieren, werden sie im Anfrageformular immer in Zuweisungen umbenannt, wenn Benutzer die Anfrage senden. Sie können den Typ der Zuweisung nur im Bereich Warteschlangendetails angeben.
     >
     >* Wenn Sie im Bereich „Warteschlangendetails“ die Option „Zugewiesen an“ ausgewählt haben, können Sie im Anforderungsformular nur Benutzer in das Feld „Zuweisungen“ eingeben. In diesem Fall können Sie keine Aufgabengebiete oder ein Team eingeben.

   * **Dokumente**: Wählen Sie diese Option, um den Abschnitt Dokumente im neuen Anfrageformular anzuzeigen, und wählen Sie dann aus, wo der Abschnitt Dokument hochladen positioniert werden soll. Wählen Sie aus den folgenden Optionen aus:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Nach benutzerdefinierten Formularen</td> 
        <td><span>Der Abschnitt Dokumente wird unten im Anfrageformular angezeigt.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Vor benutzerdefinierten Formularen</td> 
        <td> <p><span>Der Abschnitt Dokumente wird zwischen den Workfront-Feldern und den benutzerdefinierten Feldern des Anfrageformulars angezeigt.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![Neue Problemfelder und Dokumente in Warteschlangendetails](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **Alle ausgewählten und nicht ausgewählten Felder anzeigen für** Wählen Sie aus, welchen Benutzern alle Felder im neuen Anfrageformular angezeigt werden sollen. Die folgenden Optionen steuern den Zugriff auf die Felder im Formular.

     | Benutzer, die alle Felder im Anfrageformular sehen können | Beschreibung |
     |---|---| 
     | Alle Benutzer (Planlizenzen) | Alle Benutzer, die über eine Planlizenz verfügen, können die ausgewählten sowie die nicht ausgewählten Felder sehen. |
     | Personen mit Ansichtszugriff auf dieses Projekt (Planlizenz) | Benutzer mit einer Planlizenz, die auch über Ansichtsrechte für dieses Projekt verfügen, können die ausgewählten sowie die nicht ausgewählten Felder sehen. Der Rest der Benutzer, die Anfragen an dieses Projekt senden können, kann nur die ausgewählten Felder sehen. |
     | Keine Benutzer | Die nicht ausgewählten Felder können nicht von Benutzenden angezeigt werden. Alle Benutzer, die Anfragen an dieses Projekt senden können, können nur die ausgewählten Felder sehen. Dies ist die Standardauswahl. |

   * **Benutzerdefinierte Forms**: Wählen Sie aus dem Dropdown-Menü ein benutzerdefiniertes Formular aus, das mit der Anfrage-Warteschlange verknüpft werden soll. Sie können mehrere Formulare auswählen und sie dann per Drag-and-Drop in der Reihenfolge ablegen, in der sie im Anfrageformular angezeigt werden sollen.
In diesem Dropdown-Menü stehen nur benutzerdefinierte Problemformulare zur Auswahl. Allen Problemen, die an diese Anfrage-Warteschlange gesendet und dem Projekt oder seinen Aufgaben hinzugefügt werden, werden die ausgewählten Formulare zugeordnet.
Sie müssen benutzerdefinierte Anfrageformulare erstellen, bevor Sie sie im Abschnitt Warteschlangendetails anzeigen können.
Wenn mehrere Warteschlangenthemen mit einer Anfrage-Warteschlange verknüpft sind, empfehlen wir, stattdessen benutzerdefinierte Formulare mit den Warteschlangenthemen zu verknüpfen.
Weitere Informationen finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Benutzerdefiniertes Formular-Feld in Warteschlangendetails](assets/custom-forms-box-on-queue-details.png)

1. Wählen Sie weiterhin Informationen für die Einstellungen im Bereich **E-Mail-Warteschlangeneinstellungen** aus, damit Benutzer E-Mail-Anfragen an das Projekt für die Anfrage-Warteschlange senden können.

   Weitere Informationen finden Sie unter [Benutzer können ein Problem per E-Mail an ein Anfrage-Warteschlangenprojekt senden](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Klicken Sie auf **Speichern**.\
   Ihr Projekt wurde jetzt als Anfrage-Warteschlange konfiguriert, und Benutzer können ihm jetzt Anforderungen hinzufügen.

1. (Optional) Um die Funktionalität für die Anfrage-Warteschlange zu verbessern, erstellen Sie zusätzliche Unterabschnitte für Ihre Warteschlange sowie Regeln für die Weiterleitung der eingehenden Anfragen an das richtige Team, den richtigen Verantwortlichen oder das richtige Projekt.

   * Informationen zum Erstellen von Unterabschnitten für die Anfrage-Warteschlange finden Sie in den folgenden Artikeln
   * [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)
   * [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

     Weitere Informationen zum Weiterleiten der Anfragen an den entsprechenden Verantwortlichen, das entsprechende Team und das entsprechende Projekt finden Sie unter [Routing-Regeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

</div>
