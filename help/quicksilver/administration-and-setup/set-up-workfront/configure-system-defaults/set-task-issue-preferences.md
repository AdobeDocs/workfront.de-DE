---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren
description: Sie können systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren. Diese Voreinstellungen beeinflussen die Art und Weise, wie Ihre Benutzerinnen und Benutzer Aufgaben und Probleme in Workfront erstellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 3f2cc191c316d107f16a12160cb126203b05387c
workflow-type: tm+mt
source-wordcount: '2251'
ht-degree: 0%

---

# Systemweite Aufgaben- und Problemvoreinstellungen konfigurieren

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Als [!DNL Adobe Workfront] können Sie systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren. Diese Voreinstellungen beeinflussen die Art und Weise, wie Ihre Benutzerinnen und Benutzer Aufgaben und Probleme in [!DNL Workfront] erstellen.

Standardmäßig sind die Voreinstellungen für Aufgaben und Probleme gesperrt und können von Gruppenadministratoren nur dann auf Gruppenebene geändert werden, wenn sie sie für alle Gruppen im System entsperrt werden. Weitere Informationen finden Sie im Abschnitt [Sperren von Aufgaben- und Problemeinstellungen für Gruppen](#lock-task-and-issue-preferences-for-groups) in diesem Artikel.


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   oder
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einstellungen für Aufgaben und Probleme für alle in [!DNL Workfront] konfigurieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Aufgaben und Probleme].**

1. Fahren Sie auf der angezeigten Seite mit einem der folgenden sechs Abschnitte fort, um die Einstellungen für [!UICONTROL Neue Aufgabenstandardwerte], [!UICONTROL Probleme], [!UICONTROL Löschung], [!UICONTROL Tatsächliche Termine] und [!UICONTROL Zugriff]:

   * [[!UICONTROL Standardeinstellungen für neue Aufgaben]](#new-task-defaults)
   * [[!UICONTROL Probleme]](#issues)
   * [[!UICONTROL Löschen]](#deletion)
   * [Verschieben](#move)
   * [[!UICONTROL Tatsächliche Daten]](#actual-dates)
   * [[!UICONTROL Delegation]](#delegation)
   * [[!UICONTROL Zugriff]](#access)


### [!UICONTROL Standardeinstellungen für neue Aufgaben] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Startdatum]</td> 
    <td> <p>Legt das standardmäßige Startdatum für neue Aufgaben für Projektmanager fest. Das Startdatum für neue Aufgaben kann entweder das geplante Startdatum des Projekts oder der Tag sein, an dem die Aufgabe erstellt wird.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Dauertyp] </p> </td> 
    <td> <p>Bestimmt das Verhältnis zwischen der Anzahl der Ressourcen (und ihrem jeweiligen Prozentsatz) und der Dauer des Gesamtaufwands für die Aufgabe. Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Aufgabendauer und Dauertypen</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Umsatztyp]</td> 
    <td> <p>Berechnet den geplanten und tatsächlichen Umsatz einer Aufgabe. Wenn der <strong>[!UICONTROL Revenue Type]</strong> auf <strong>[!UICONTROL Not Billable]</strong> festgelegt ist, erzeugen die geplanten Stunden und die tatsächlich aufgezeichneten Stunden keine Umsatzschätzung für die Aufgabe, und die Arbeit an der Aufgabe trägt nicht zum Umsatz auf Projektebene bei.</p>
         <p>Informationen zu den verschiedenen Umsatztypen finden Sie unter <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md">Übersicht über Abrechnung und Umsatz</a>.</p></td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Kostentyp]</td> 
    <td> <p>Berechnet die geplanten Kosten und Istkosten für eine Aufgabe. Bei Festlegung auf <strong>[!UICONTROL Keine Kosten]</strong> erzeugen die geplanten Stunden und die aufgezeichneten tatsächlichen Stunden keine Schätzung der geplanten oder tatsächlichen Kosten für die Aufgabe, und die Arbeit an der Aufgabe trägt nicht zu den Kosten auf Projektebene bei.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Probleme {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL aktualisiert automatisch den Status „Lösbares Problem“, wenn sich der Status des Lösungsobjekts ändert]</td> 
    <td> <p>Wenn jemand ein Problem in ein Projekt oder eine Aufgabe konvertiert, werden sowohl das ursprüngliche Problem als auch das konvertierte Projekt oder die konvertierte Aufgabe zu Lösungsobjekten. Mit dieser Einstellung können Sie die Lösung des ursprünglichen Problems mit der Lösung des lösbaren Objekts korrelieren. Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und das Auflösen von Objekten </a>.</p> <p>Damit diese Einstellung wirksam wird, muss die Option zum <strong>[!UICONTROL Ursprüngliches Problem beibehalten und seine Lösung mit der Aufgabe verknüpfen]</strong> ausgewählt werden.</p> 
      <ul> 
      <li>Wenn diese Einstellung aktiviert ist, können Sie benutzerdefinierte Status mit demselben Schlüssel für sowohl Probleme als auch Projekte oder Aufgaben erstellen. Wenn das Projekt oder die Aufgabe (als lösbares Objekt) in den benutzerdefinierten Status übergeht, spiegelt die Änderung auch den Status des Problems wider. Der Statusschlüssel muss für den Problem- und Projekt- oder Aufgabenstatus identisch sein.</li> 
      <li>Wenn diese Einstellung deaktiviert ist, werden für die Auflösung von Objektstatus automatisch der Standardstatus anstelle der benutzerdefinierten festgelegt. Weitere Informationen zu den Standardstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemanfragestatus</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL beim Konvertieren eines Problems in eine Aufgabe]</td> 
    <td> <p>Die Einstellungen in diesem Abschnitt bestimmen, was während des Konvertierungsprozesses von einem Problem zu einer Aufgabe geschieht:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Ursprüngliches Problem beibehalten und seine Lösung mit der Aufgabe verknüpfen]</strong>: Wenn Sie das Problem konvertieren, bleibt es als Problem sichtbar, bis die Aufgabe abgeschlossen ist. Der Status des Problems ändert sich nach Abschluss der Aufgabe automatisch in [!UICONTROL Closed]. Wenn diese Option deaktiviert ist, wird das Problem gelöscht.</p> <p><b>HINWEIS</b>:  <p>Benutzende ohne Zugriff oder Berechtigung zum Löschen von Problemen können das Problem während der Konvertierung nicht löschen, unabhängig vom Status dieser Einstellung. Informationen zu Zugriff und Berechtigungen für Probleme finden Sie unter:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Anfragen gewähren</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problemfreigabe </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Primären Kontakten Zugriff auf die Aufgabe erteilen]</strong>: Ermöglicht dem Hauptkontakt (dem Problemersteller), die Aufgabe anzuzeigen, um die Aufgabe zu überprüfen, über den Fortschritt auf dem Laufenden zu bleiben und Kommentare zum Abschnitt „Aktualisierungen“ der Aufgabe abzugeben.</li> 
      <li> <p><strong>[!UICONTROL Zulassen, dass diese Einstellungen während der Konvertierung geändert werden]</strong>: Ermöglicht dem Benutzer, der das Problem konvertiert, diese Optionen während der Konvertierung eines Problems in eine Aufgabe zu ändern.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL beim Konvertieren eines Problems in ein Projekt]</td> 
    <td> <p>Die Einstellungen in diesem Abschnitt bestimmen, was während des Konvertierungsprozesses von einem Problem in ein Projekt geschieht:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Ursprüngliches Problem beibehalten und seine Lösung mit dem Projekt verknüpfen]</strong>: Wenn Sie das Problem konvertieren, bleibt es als Problem sichtbar, bis das Projekt abgeschlossen ist. Der Status des Problems ändert sich nach Abschluss des Projekts automatisch in [!UICONTROL Closed]. Wenn diese Option deaktiviert ist, wird das Problem gelöscht. </p> <p><b>HINWEIS</b>:  <p>Benutzende ohne Zugriff oder Berechtigung zum Löschen von Problemen können das Problem während der Konvertierung nicht löschen, unabhängig vom Status dieser Einstellung. Informationen zu Zugriff und Berechtigungen für Probleme finden Sie unter:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Anfragen gewähren</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problemfreigabe </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Primären Kontakten Zugriff auf das Projekt erteilen]</strong>: Ermöglicht dem Hauptkontakt (dem Problemersteller), Zugriff auf das Projekt zu erhalten, um das Projekt zu überprüfen, über den Fortschritt auf dem Laufenden zu bleiben und den Abschnitt „Aktualisierungen“ des Projekts zu kommentieren.</li> 
      <li><strong>[!UICONTROL Zulassen, dass diese Einstellungen während der Konvertierung geändert werden]</strong>: Ermöglicht dem Benutzer, der das Problem konvertiert, die aufgelisteten Optionen während der Konvertierung eines Problems in ein Projekt zu ändern.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Löschen] {#deletion}

**[!UICONTROL Erlauben Sie Benutzern das Löschen von Aufgaben und Problemen mit protokollierten Stunden]**: Ermöglicht Ihnen zu bestimmen, ob Sie das Löschen von Aufgaben oder Problemen zulassen, bei denen Stunden protokolliert werden. Diese Option ist standardmäßig ausgewählt.

>[!TIP]
>
>Diese Einstellung gilt auch für das Löschen von Projekten, für die Aufgaben oder Probleme mit Stunden protokolliert wurden. Diese Einstellung gilt nicht für das Löschen von Projekten, bei denen die Zeit direkt für das Projekt protokolliert wird.

* Bei Auswahl dieser Option erhalten Sie eine informative Warnung, wenn Sie eine Aufgabe oder ein Problem löschen. Die Warnung erinnert Sie daran, dass Aufgaben oder Probleme, die Stunden protokolliert haben, entweder in das Projekt verschoben oder gelöscht werden. Sie können konfigurieren, ob die Stunden gelöscht oder in das Projekt verschoben werden[!UICONTROL  indem Sie im Bereich „Arbeitszeittabelle und ]&quot; von [!UICONTROL Setup“ ]. Nachdem Sie bestätigt haben, dass Sie die Warnung gesehen haben, wird die Aufgabe oder das Problem gelöscht. Weitere Informationen zum Konfigurieren der Einstellungen für Arbeitszeittabellen und Stunden finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  >[!TIP]
  >
  >Wenn Sie ein Projekt mit Aufgaben und Problemen löschen, in denen Stunden protokolliert wurden, werden die protokollierten Stunden entweder gelöscht oder gemäß den Einstellungen im Bereich „Arbeitszeittabelle [!UICONTROL  Stundeneinstellungen] von [!UICONTROL Setup] beibehalten. Beim Löschen eines Projekts wird keine Warnmeldung angezeigt.

* Wenn Sie diese Option deaktivieren, erhalten Sie eine unzulässige Warnung, wenn Sie eine Aufgabe oder ein Problem mit protokollierten Stunden löschen oder wenn Sie ein Projekt löschen, für dessen Aufgaben oder Probleme Stunden protokolliert wurden. Die Warnung gibt an, dass der Administrator nicht zulässt, dass Aufgaben oder Probleme mit protokollierten Stunden gelöscht werden. Die Aufgaben, Probleme oder Projekte, für die Stunden für Aufgaben und Probleme protokolliert wurden, können nicht gelöscht werden.

### Verschieben

**[!UICONTROL Erlauben Sie Benutzern, Aufgaben und Probleme mit protokollierten Stunden zu verschieben]**: Ermöglicht Ihnen zu bestimmen, ob Sie das Verschieben von Aufgaben oder Problemen zulassen, bei denen Stunden protokolliert werden. Diese Option ist standardmäßig ausgewählt.

* Wenn es ausgewählt ist, können Sie Aufgaben und Probleme verschieben, für die Zeit protokolliert wurde. Die Stunden werden auch mit den Aufgaben oder Problemen verschoben.

* Wenn Sie diese Option deaktivieren, erhalten Sie eine unzulässige Warnung, wenn Sie eine Aufgabe oder ein Problem mit protokollierten Stunden in ein anderes Projekt verschieben. Die Warnung gibt an, dass der Administrator nicht zulässt, dass Aufgaben oder Probleme mit protokollierten Stunden verschoben werden. Die Aufgaben oder Probleme, für die Stunden protokolliert wurden, können nicht verschoben werden. Sie können Aufgaben innerhalb desselben Projekts verschieben, selbst wenn diese Option deaktiviert ist.

### [!UICONTROL Tatsächliche Daten] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Wenn sich der Status einer Aufgabe oder eines Problems von „Neu“ in „In Bearbeitung“ ändert, das tatsächliche Startdatum auf] setzen</td> 
    <td> <p>Wählen Sie eine der folgenden Optionen aus, um festzulegen, wann das tatsächliche Startdatum in [!DNL Workfront] aufgezeichnet wird, wenn eine Aufgabe oder ein Problem von <strong>[!UICONTROL Neu]</strong> zu <strong>[!UICONTROL In Bearbeitung]</strong>:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> Das tatsächliche Startdatum wird auf das aktuelle Datum gesetzt.</li> 
      <li><strong>[!UICONTROL Das geplante Startdatum]:</strong> Das tatsächliche Startdatum wird auf das geplante Startdatum der Aufgabe oder des Problems festgelegt.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Nach vollständiger Bearbeitung einer Aufgabe oder eines Problems das tatsächliche Abschlussdatum auf] setzen</td> 
    <td> <p>Wählen Sie eine der folgenden Optionen für den Fall aus, dass das tatsächliche Abschlussdatum nach Abschluss einer Aufgabe oder eines Problems in [!DNL Workfront] aufgezeichnet wird:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> Das tatsächliche Abschlussdatum wird auf das aktuelle Datum gesetzt.</li> 
      <li> <p><strong>[!UICONTROL Das geplante Abschlussdatum]:</strong> Das tatsächliche Abschlussdatum wird auf das geplante Abschlussdatum der Aufgabe oder des Problems festgelegt.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Delegierung

Wenn die Einstellung **[!UICONTROL Zulassen, dass Benutzer ihre Aufgaben und Probleme delegieren]** aktiviert ist, können alle Benutzer im System ihre Arbeit vorübergehend an andere delegieren.

Wenn diese Einstellung aktiviert ist, können Benutzer Folgendes sehen:

* Die [!UICONTROL **Delegieren**] in ihren Widgets [!UICONTROL Meine ]), [!UICONTROL Meine Aufgaben] oder [!UICONTROL Meine Probleme] im Bereich [!UICONTROL Home]. Dort können sie Aufgaben- und Problemzuweisungen delegieren.

  >[!NOTE]
  >
  >  Der [!UICONTROL **Genehmigungen delegieren**] ist immer im Bereich [!UICONTROL Startseite] aktiviert.

* Ein Hinweis darauf, dass eine Aufgabe oder ein Problem an einen anderen Benutzer im Bereich [!UICONTROL Zuweisungen und Zuweisungen] in der Aufgaben- oder Problem-Kopfzeile delegiert wurde.
* Ein Hinweis darauf, dass eine Aufgabe oder ein Problem an einen anderen Benutzer in seinem Widget [!UICONTROL Meine Arbeit] in [!UICONTROL Startseite] delegiert wurde.

  Wenn Sie die Einstellung [!UICONTROL Erlauben Sie Benutzern, ihre Aufgaben und Probleme zu delegieren] deaktivieren, werden die aktuell geplanten Delegierungen beendet und die delegierten Benutzer erhalten eine E-Mail-Benachrichtigung, dass die Delegierung gestoppt wurde.

Informationen zum Delegieren von Arbeit an andere finden Sie in den folgenden Artikeln:

* [Delegieren von Arbeit - Übersicht](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Delegieren von Aufgaben und Problemen](../../../manage-work/delegate-work/how-to-delegate-work.md)


<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL Zugriff] {#access}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Wenn jemand einer Aufgabe zugewiesen wird]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Ihnen Zugriff auf eine Aufgabe erteilen]</strong>: Definiert die Standardberechtigung, die ein Benutzer für die Aufgabe hat, der er zugewiesen ist. Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</li> 
      <li> <p><strong>[!UICONTROL Auch ihnen Zugriff auf das Projekt gewähren]</strong>: Definiert die Standardberechtigung, die ein Benutzer dem Projekt hat, dem er eine Aufgabe zugewiesen hat. Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Wenn jemand einem Problem zugewiesen wird]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Ihnen Zugriff auf eine Aufgabe erteilen]</strong>: Definiert die Standardberechtigung, die ein Benutzer für die Aufgabe hat, der er zugewiesen ist. Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</li> 
      <li> <p><strong>[!UICONTROL Auch ihnen Zugriff auf das Projekt gewähren]</strong>: Definiert die Standardberechtigung, die ein Benutzer dem Projekt hat, dem er eine Aufgabe zugewiesen hat. Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Wenn jemand eine Anfrage sendet]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Diesen Benutzern … Zugriff auf das Problem geben]</strong>: Definiert die Standardberechtigung, die ein Benutzer für eine von ihm gesendete Anfrage hat. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Freigeben eines </a>.</li> 
      <li> <p><strong>[!UICONTROL Personen aus derselben Firma erben dieselben Berechtigungen für alle Anfragen]</strong>: Ermöglicht Benutzern das Anzeigen von Anfragen, die von anderen Benutzern aus derselben Firma gesendet werden. Sie verfügen über dieselben Berechtigungen für diese Anfragen wie für ihre eigenen gesendeten Anfragen.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Voreinstellungen für Aufgaben und Probleme für Gruppen sperren {#lock-task-and-issue-preferences-for-groups}

Wenn Gruppen in Ihrer Organisation eine Aufgaben- oder Problem-Voreinstellung benötigen, die für ihre eindeutigen Workflows anders konfiguriert ist, können Sie die Voreinstellung für alle Gruppen im gesamten Unternehmen entsperren, damit sie sie selbst konfigurieren können. Wenn eine Voreinstellung entsperrt wird und der Gruppenadministrator sie ändert, werden die mit der Gruppe verbundenen Aufgaben oder Probleme von der Einstellung auf Gruppenebene für die Voreinstellung und nicht auf Systemebene beeinflusst.

Informationen dazu, wie Gruppenadministratoren Aufgaben- und Problemeinstellungen für eine Gruppe konfigurieren, finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Nachdem ein [!DNL Workfront] eine Voreinstellung auf Systemebene entsperrt hat, kann sie jeder Gruppenadministrator konfigurieren und dann sperren, um sicherzustellen, dass alle Benutzer in seiner Gruppe und den Untergruppen unten dieselbe Konfiguration verwenden. Dies geschieht parallel zu der Möglichkeit, dass ein [!DNL Workfront]-Administrator eine Voreinstellung für alle im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Sperren oder Entsperren eines Projekts, einer Aufgabe oder einer Problemvoreinstellung für Untergruppen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

So sperren oder entsperren Sie eine Aufgaben- oder Problem-Voreinstellung, damit Gruppen sie konfigurieren können:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Projektvoreinstellungen]** > **[!UICONTROL Aufgaben und Probleme]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Administratoren von Gruppen unter Ihrer Gruppe eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie ![Umschalter Entsperren](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass Ihre Gruppe und alle darunter liegenden Gruppen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie gesperrt ist (dies ist die Standardeinstellung).

     >[!IMPORTANT]
     >
     >Es wird empfohlen, mit den Administratoren und Benutzern in Gruppen im gesamten System zu kommunizieren, um sicherzustellen, dass alle Anforderungen in der Art und Weise berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie ihn sperren, wird die entsprechende Konfiguration von allen Gruppen im System übernommen. Und wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Konfigurationen, die Gruppenadministratoren möglicherweise vorgenommen haben.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
