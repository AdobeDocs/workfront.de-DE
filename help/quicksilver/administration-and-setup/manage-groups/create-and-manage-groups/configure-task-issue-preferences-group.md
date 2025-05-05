---
title: Konfigurieren der Voreinstellungen für Aufgaben und Probleme für eine Gruppe
user-type: administrator
product-area: system-administration;user-management;setup
keywords: Gruppe,Voreinstellungen,Aufgabe,Problem,Entsperren
navigation-topic: create-and-manage-groups
description: Wenn Gruppen in Ihrem Unternehmen eine Aufgaben- oder Problem-Voreinstellung unabhängig von der Konfiguration auf Systemebene konfigurieren müssen, kann ein Adobe Workfront-Administrator die Voreinstellung entsperren. Als Gruppenadministrator können Sie dann die Voreinstellung für Ihre Gruppe konfigurieren. Dies wirkt sich auf alle Aufgaben oder Probleme Ihrer Gruppe aus.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2189'
ht-degree: 2%

---

# Konfigurieren der Voreinstellungen für Aufgaben und Probleme für eine Gruppe

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Wenn Gruppen in Ihrem Unternehmen eine Aufgaben- oder Problem-Voreinstellung unabhängig von der Konfiguration auf Systemebene konfigurieren müssen, kann ein Adobe Workfront-Administrator die Voreinstellung entsperren. Als Gruppenadministrator können Sie dann die Voreinstellung für Ihre Gruppe konfigurieren. Dies wirkt sich auf alle Aufgaben oder Probleme Ihrer Gruppe aus.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Informationen dazu, wie Workfront-Admins Voreinstellungen entsperren, finden Sie unter [Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>Die Konfiguration auf Gruppenebene ist auch für Projektvoreinstellungen möglich. Weitere Informationen finden Sie [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* In der Regel bleibt eine entsperrte Voreinstellung auf unbestimmte Zeit entsperrt. Wenn der Workfront-Administrator sie erneut sperrt, wird die Systemeinstellung erneut wirksam und die Einstellungen für die von den Gruppenadministratoren vorgenommenen Voreinstellungen gehen verloren.
>* Die Voreinstellungen, die für die mit einem Projekt verknüpfte Gruppe festgelegt wurden, haben Vorrang vor den Voreinstellungen, die für die Hauptgruppe des Benutzers festgelegt wurden, der das Projekt erstellt.
>* Einige Voreinstellungen auf Gruppenebene wirken sich auf Projektvorlagen aus, die Sie für die Gruppe erstellen. Weitere Informationen finden Sie im Abschnitt [Anzeigen, Arbeiten mit und Erstellen von Vorlagen für Ihre Gruppe im Bereich Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) im Artikel [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt hat, können Sie sie konfigurieren und dann sperren, um sicherzustellen, dass alle Personen in Ihrer Gruppe und ihren Untergruppen dieselbe Konfiguration verwenden. Dies geschieht parallel zu der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Projekt, Aufgabe oder Problem für Untergruppen sperren oder entsperren](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren der Einstellungen für entsperrte Aufgaben und Probleme für eine Gruppe auf oberster Ebene

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie zu Einrichtung > Projektvoreinstellungen > Aufgaben und Probleme wechseln und dann im Feld oben auf der Seite nach dem Namen der Gruppe suchen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![Symbol „Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie die Voreinstellungen für entsperrte Aufgaben und Probleme konfigurieren möchten.
1. Klicken Sie auf der Seite, die für die Gruppe angezeigt wird, im linken Bereich auf **Voreinstellungen für Aufgaben und Probleme**.
1. Fahren Sie auf der angezeigten Seite mit einem der fünf unten aufgeführten Abschnitte fort, um die Einstellungen für die Bereiche Standardeinstellungen für neue Aufgaben, Probleme, Löschen, Tatsächliche Termine und Zugriff zu konfigurieren, und klicken Sie dann auf **Speichern**.

   Wenn Sie den Mauszeiger über das Sperrsymbol ![Sperrsymbol](assets/lock-toggle-button-dimmed.png) für eine Voreinstellung bewegen, die Sie konfigurieren müssen, und eine QuickInfo angezeigt wird, die Ihnen mitteilt, dass gesperrt ist, können Sie Ihren Workfront-Administrator bitten, diese für alle Gruppen im Unternehmen zu entsperren.

   Wenn er entsperrt ist, können Sie und andere Gruppenadministratoren ihn separat für Ihre eigenen Gruppen konfigurieren. Sie können sie auch für Ihre Gruppe und alle Untergruppen unter Ihrer Gruppe sperren.

   * [Standardeinstellungen für neue Aufgaben](#new-task-defaults)
   * [Probleme](#issues)
   * [Löschen](#deletion)
   * [Verschieben](#move)
   * [Tatsächliche Termine](#actual-dates)
   * [Delegierung](#delegation)
   * [Zugriff](#access)

### Voreinstellungen für neue Aufgabe {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Startdatum neuer Aufgaben</td> 
      <td> <p>Legt das standardmäßige Startdatum für neue Aufgaben für Projektmanager fest. Das Startdatum für neue Aufgaben kann entweder das geplante Startdatum des Projekts oder der Tag sein, an dem die Aufgabe erstellt wird.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Dauertyp </p> </td> 
      <td> <p>Bestimmt das Verhältnis zwischen der Anzahl der Ressourcen (und ihrem jeweiligen Prozentsatz) und der Dauer des Gesamtaufwands für die Aufgabe. Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Aufgabendauer und -dauertypen: Artikelindex</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Umsatztyp</td> 
      <td> <p>Berechnet den geplanten und tatsächlichen Umsatz einer Aufgabe. Wenn der <strong>Umsatztyp</strong> auf "<strong> fakturierbar“ </strong> ist, generieren die geplanten Stunden und die aufgezeichneten tatsächlichen Stunden keine Umsatzschätzung für die Aufgabe, und die Arbeit an der Aufgabe trägt nicht zum Umsatz auf Projektebene bei.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kostenart</td> 
      <td> <p>Berechnet die geplanten Kosten und Istkosten für eine Aufgabe. Bei Festlegung <strong>Keine Kosten</strong> erzeugen die geplanten Stunden und die erfassten Ist-Stunden keine geplanten oder Ist-Kostenschätzungen für die Aufgabe, und die Arbeit an der Aufgabe trägt nicht zu den Kosten auf Projektebene bei.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### Probleme {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status für "Lösbares Problem" automatisch aktualisieren, wenn sich der Status für "Problemlösendes Objekt" ändert</td> 
      <td> <p>Wenn jemand ein Problem in ein Projekt oder eine Aufgabe konvertiert, werden sowohl das ursprüngliche Problem als auch das konvertierte Projekt oder die konvertierte Aufgabe zu Lösungsobjekten. Mit dieser Einstellung können Sie die Lösung des ursprünglichen Problems mit der Lösung des lösbaren Objekts korrelieren. Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und das Auflösen von Objekten </a>.</p> <p>Damit diese Einstellung wirksam wird, muss die Option "<strong> ursprüngliche Anfrage beibehalten und deren Lösung mit der Aufgabe verknüpft</strong> ausgewählt werden.</p> 
       <ul> 
        <li>Wenn diese Einstellung aktiviert ist, können Sie benutzerdefinierte Status mit demselben Schlüssel für sowohl Probleme als auch Projekte oder Aufgaben erstellen. Wenn das Projekt oder die Aufgabe (als lösbares Objekt) in den benutzerdefinierten Status übergeht, spiegelt die Änderung auch den Status des Problems wider. Der Statusschlüssel muss für den Problem- und Projekt- oder Aufgabenstatus identisch sein.</li> 
        <li>Wenn diese Einstellung deaktiviert ist, werden für die Auflösung von Objektstatus automatisch der Standardstatus anstelle der benutzerdefinierten festgelegt. Weitere Informationen zu den Standardstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemanfragestatus</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bei der Konvertierung eines Problems in eine Aufgabe</td> 
      <td> <p>Die Einstellungen in diesem Abschnitt bestimmen, was während des Konvertierungsprozesses von einem Problem zu einer Aufgabe geschieht:</p> 
       <ul> 
        <li><strong>Ursprüngliches Problem beibehalten und seine Lösung mit der Aufgabe verknüpfen</strong>: Wenn Sie das Problem konvertieren, bleibt es als Problem sichtbar, bis die Aufgabe abgeschlossen ist. Der Status des Problems ändert sich automatisch in Geschlossen , wenn die Aufgabe abgeschlossen ist.</li> 
        <li><strong>Primären Kontakt Zugriff auf die Aufgabe gewähren</strong>: Ermöglicht dem primären Kontakt (dem Problemersteller) Zugriff auf die Aufgabe, die Aufgabe zu überprüfen, Aktualisierungen vorzunehmen und über den Fortschritt auf dem Laufenden zu bleiben</li> 
        <li> <p><strong>Ändern dieser Einstellungen während der Konvertierung zulassen</strong>: Ermöglicht dem Benutzer, der das Problem konvertiert, diese Optionen während der Konvertierung eines Problems in eine Aufgabe zu ändern.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beim Konvertieren eines Problems in ein Projekt</td> 
      <td> <p>Die Einstellungen in diesem Abschnitt bestimmen, was während des Konvertierungsprozesses von einem Problem in ein Projekt geschieht:</p> 
       <ul> 
        <li><strong>Ursprüngliches Problem beibehalten und seine Lösung mit dem Projekt verknüpfen</strong>: Wenn Sie das Problem konvertieren, bleibt es als Problem sichtbar, bis das Projekt abgeschlossen ist. Der Status des Problems ändert sich nach Abschluss des Projekts automatisch in Geschlossen .</li> 
        <li><strong>Primären Kontakt Zugriff auf das Projekt gewähren</strong>: Ermöglicht dem primären Kontakt (dem Problemersteller) Zugriff auf das Projekt, um das Projekt zu überprüfen, Aktualisierungen vorzunehmen und über den Fortschritt des Projekts auf dem Laufenden zu bleiben.</li> 
        <li><strong>Ändern dieser Einstellungen während der Konvertierung zulassen</strong>: Ermöglicht dem Benutzer, der das Problem konvertiert, die aufgelisteten Optionen während der Konvertierung eines Problems in ein Projekt zu ändern.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Löschung {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Benutzenden das Löschen von Aufgaben und Problemen mit protokollierten Stunden erlauben</td> 
      <td> <p> Hiermit können Sie bestimmen, ob Sie das Löschen von Aufgaben oder Problemen zulassen, bei denen Stunden protokolliert werden. Diese Option ist standardmäßig ausgewählt.</p> 
       <div> 
        <p><b>Tipp</b>: Diese Einstellung gilt auch für das Löschen von Projekten, in denen Aufgaben oder Probleme mit Stunden protokolliert wurden. Diese Einstellung gilt nicht für das Löschen von Projekten, bei denen die Zeit direkt für das Projekt protokolliert wird. </p> 
        <p>Beachten Sie Folgendes:</p> 
        <ul> 
         <li> <p>Bei Auswahl dieser Option erhalten Sie eine informative Warnung, wenn Sie eine Aufgabe oder ein Problem löschen. Die Warnung erinnert Sie daran, dass Aufgaben oder Probleme, die Stunden protokolliert haben, entweder in das Projekt verschoben oder gelöscht werden. Sie können im Bereich Arbeitszeittabelle und Stundeneinstellungen des Setups konfigurieren, ob die Stunden gelöscht oder in das Projekt verschoben werden. Nachdem Sie bestätigt haben, dass Sie die Warnung gesehen haben, wird die Aufgabe oder das Problem gelöscht. Weitere Informationen zum Konfigurieren der Einstellungen für Arbeitszeittabellen und Stunden finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen</a>. </p> <p>Tipp: <span>Wenn Sie ein Projekt mit Aufgaben und Problemen löschen, in denen Stunden protokolliert wurden, werden die protokollierten Stunden entweder gelöscht oder gemäß den Einstellungen im Bereich „Arbeitszeittabellen- und Stunden-Voreinstellungen“ unter Setup beibehalten</span>. </p> </li> 
         <li><span>Wenn Sie diese Option deaktivieren, erhalten Sie eine unzulässige Warnung, wenn Sie eine Aufgabe oder ein Problem mit protokollierten Stunden löschen oder wenn Sie ein Projekt löschen, für dessen Aufgaben oder Probleme Stunden protokolliert wurden</span> <span>.</span> Die Warnung gibt an, dass der Administrator nicht zulässt, dass Aufgaben oder Probleme mit protokollierten Stunden gelöscht werden. Die Aufgaben, Probleme <span> Projekte, in denen Stunden für Aufgaben und Probleme protokolliert wurden</span> können nicht gelöscht werden. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>


### Verschieben

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Benutzenden das Verschieben von Aufgaben und Problemen mit protokollierten Stunden erlauben</td> 
      <td> <p> Hiermit können Sie bestimmen, ob Sie das Verschieben von Aufgaben oder Problemen zulassen, bei denen Stunden protokolliert werden. Diese Option ist standardmäßig ausgewählt.</p> 
       <p>Beachten Sie Folgendes:</p> 
        <ul> 
         <li> Wenn es ausgewählt ist, können Sie Aufgaben und Probleme verschieben, für die Zeit protokolliert wurde. Die Stunden werden auch mit den Aufgaben oder Problemen verschoben. </li>
      <li>Wenn Sie diese Option deaktivieren, erhalten Sie eine unzulässige Warnung, wenn Sie eine Aufgabe oder ein Problem mit protokollierten Stunden verschieben. Die Warnung gibt an, dass der Administrator nicht zulässt, dass Aufgaben oder Probleme mit protokollierten Stunden verschoben werden. Die Aufgaben oder Probleme, für die Stunden protokolliert wurden, können nicht in ein anderes Projekt verschoben werden. Sie können Aufgaben mit protokollierten Stunden innerhalb desselben Projekts verschieben, selbst wenn diese Option deaktiviert ist.  </li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

### Tatsächliche Termine {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wenn sich der Status einer Aufgabe oder eines Problems von „Neu“ in „In Bearbeitung“ ändert, das tatsächliche Startdatum auf Folgendes setzen</td> 
      <td> <p>Wählen Sie eine der folgenden Optionen aus, um festzulegen, wann das tatsächliche Startdatum in Workfront aufgezeichnet wird, wenn eine Aufgabe oder ein Problem von <strong>Neu</strong> zu <strong>In Bearbeitung</strong> wechselt:</p> 
       <ul> 
        <li><strong>Jetzt</strong> Das tatsächliche Startdatum wird auf das aktuelle Datum festgelegt.</li> 
        <li><strong>Das geplante Startdatum:</strong> Das tatsächliche Startdatum wird auf das geplante Startdatum der Aufgabe oder Anfrage festgelegt.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nach vollständiger Bearbeitung einer Aufgabe oder Anfrage das tatsächliche Abschlussdatum auf Folgendes setzen</td> 
      <td> <p>Wählen Sie eine der folgenden Optionen für den Fall aus, dass das tatsächliche Abschlussdatum nach Abschluss einer Aufgabe oder eines Problems in Workfront aufgezeichnet wird:</p> 
       <ul> 
        <li><strong>Jetzt</strong> Das tatsächliche Abschlussdatum wird auf das aktuelle Datum festgelegt.</li> 
        <li> <p><strong>Das geplante Abschlussdatum:</strong> Das tatsächliche Abschlussdatum wird auf das geplante Abschlussdatum der Aufgabe oder Anfrage festgelegt.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### Delegierung

Wenn die Einstellung **[!UICONTROL Erlauben Sie Benutzern, ihre Aufgaben und Probleme zu delegieren]** aktiviert ist, können alle Benutzer in der Gruppe ihre Arbeit vorübergehend an andere delegieren.

Wenn diese Einstellung aktiviert ist, können Gruppenbenutzer Folgendes sehen:

* Die [!UICONTROL **Delegieren**] in ihren Widgets [!UICONTROL Meine &#x200B;]), [!UICONTROL Meine Aufgaben] oder [!UICONTROL Meine Probleme] im Bereich [!UICONTROL Home]. Dort können sie Aufgaben- und Problemzuweisungen delegieren.

  >[!NOTE]
  >
  >  Der [!UICONTROL **Genehmigungen delegieren**] ist immer im Bereich [!UICONTROL Startseite] aktiviert.

* Ein Hinweis darauf, dass eine Aufgabe oder ein Problem an einen anderen Benutzer im Bereich [!UICONTROL Zuweisungen und Zuweisungen] in der Aufgaben- oder Problem-Kopfzeile delegiert wurde.
* Ein Hinweis darauf, dass eine Aufgabe oder ein Problem an einen anderen Benutzer in seinem Widget [!UICONTROL Meine Arbeit] in [!UICONTROL Startseite] delegiert wurde.

  Wenn Sie die Einstellung [!UICONTROL Erlauben Sie Benutzern, ihre Aufgaben und Probleme zu delegieren] deaktivieren, werden die aktuell geplanten Delegierungen beendet und die delegierten Benutzer erhalten eine E-Mail-Benachrichtigung, dass die Delegierung gestoppt wurde.

Informationen zum Delegieren von Arbeit an andere finden Sie in den folgenden Artikeln:

* [Delegieren von Arbeit - Übersicht](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Delegieren von Aufgaben und Problemen](../../../manage-work/delegate-work/how-to-delegate-work.md)

### Zugriff {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wenn jemand einer Aufgabe zugewiesen wird</td> 
      <td> 
       <ul> 
        <li><strong>Zugriff auf eine Aufgabe erteilen</strong>: Legt die Standardberechtigung fest, die ein Benutzer für die Aufgabe hat, der er zugewiesen ist. Weitere Informationen zu Aufgabenberechtigungen finden Sie unter<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Gewähren des Zugriffs für Benutzer</a>.</li> 
        <li> <p><strong>Ihnen auch Zugriff auf das Projekt gewähren</strong>: Definiert die Standardberechtigung, die ein Benutzer für das Projekt hat, dem er eine Aufgabe zugewiesen hat. Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn jemand einem Problem zugewiesen wird</td> 
      <td> 
       <ul> 
        <li><strong>Zugriff auf eine Aufgabe erteilen</strong>: Legt die Standardberechtigung fest, die ein Benutzer für die Aufgabe hat, der er zugewiesen ist. Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</li> 
        <li> <p><strong>Ihnen auch Zugriff auf das Projekt gewähren</strong>: Definiert die Standardberechtigung, die ein Benutzer für das Projekt hat, dem er eine Aufgabe zugewiesen hat. Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn jemand eine Anfrage einreicht</td> 
      <td> 
       <ul> 
        <li><strong>Zugriff auf das Problem erteilen: </strong> die Standardberechtigung, die ein Benutzer für eine von ihm gesendete Anfrage hat. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Freigeben eines Problems</a>.</li> 
        <li> <p><strong>Benutzer aus derselben Firma erben dieselben Berechtigungen für alle Anfragen</strong>: Ermöglicht Benutzern das Anzeigen von Anfragen, die von anderen Benutzern aus derselben Firma gesendet wurden. Sie verfügen über dieselben Berechtigungen für diese Anfragen wie für ihre eigenen gesendeten Anfragen.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
