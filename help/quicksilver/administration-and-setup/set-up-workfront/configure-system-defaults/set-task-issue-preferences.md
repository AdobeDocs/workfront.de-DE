---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Voreinstellungen für systemweite Aufgaben und Probleme konfigurieren
description: Sie können systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren. Diese Voreinstellungen wirken sich auf die Art und Weise aus, wie Ihre Benutzer Aufgaben und Probleme in Workfront erstellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '2074'
ht-degree: 0%

---

# Systemweite Aufgaben- und Problemeinstellungen konfigurieren

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

Als [!DNL Adobe Workfront] -Administrator können Sie systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren. Diese Voreinstellungen wirken sich darauf aus, wie Ihre Benutzer Aufgaben und Probleme in [!DNL Workfront] erstellen.

Standardmäßig sind die Voreinstellungen für Aufgaben und Ausgaben gesperrt und Gruppenadministratoren können sie nicht auf Gruppenebene ändern, es sei denn, Sie entsperren sie für alle Gruppen im System. Weitere Informationen finden Sie im Abschnitt [Voreinstellungen für Aufgaben und Ausgaben für Gruppen sperren](#lock-task-and-issue-preferences-for-groups) in diesem Artikel.


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   oder
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren von Aufgaben- und Problemeinstellungen für alle in [!DNL Workfront]

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Projekteinstellungen]** >**[!UICONTROL Aufgaben und Probleme].**

1. Fahren Sie auf der angezeigten Seite mit einem der fünf unten aufgeführten Abschnitte fort, um die Einstellungen für [!UICONTROL Neue Aufgabenstandardwerte], [!UICONTROL Probleme], [!UICONTROL Löschung], [!UICONTROL Tatsächliche Datumswerte] und [!UICONTROL Zugriff] zu konfigurieren:

   * [[!UICONTROL Neue Aufgabenstandardwerte]](#new-task-defaults)
   * [[!UICONTROL Probleme]](#issues)
   * [[!UICONTROL Löschen]](#deletion)
   * [[!UICONTROL Tatsächliche Datumswerte]](#actual-dates)
   * [[!UICONTROL Delegation]](#delegation)

   <!--
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Bearbeiten Sie es</a> </li>
  --&gt;

* [[!UICONTROL Zugriff]](#access)

### [!UICONTROL Neue Aufgabenstandardwerte] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Startdatum]</td> 
    <td> <p>Legt das standardmäßige Startdatum für neue Aufgaben für Projektmanager fest. Das Startdatum für neue Aufgaben kann entweder das geplante Startdatum des Projekts oder der Tag sein, an dem die Aufgabe erstellt wird.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Duration Type] </p> </td> 
    <td> <p>Bestimmt die Beziehung zwischen der Anzahl der Ressourcen (und ihrem Zuordnungsprozentsatz) und der Dauer oder dem Gesamtaufwand für die Aufgabe. Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Aufgabendauer und -dauer </a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Umsatz]</td> 
    <td> <p>Berechnet geplante und tatsächliche Einnahmenschätzungen für eine Aufgabe. Wenn <strong>[!UICONTROL Umsatz]</strong> auf <strong>[!UICONTROL Nicht abrechenbar]</strong> gesetzt ist, generieren die geplanten und die tatsächlichen aufgezeichneten Stunden keine Umsatzschätzung für die Aufgabe und die Arbeit an der Aufgabe trägt nicht zum Umsatz auf Projektebene bei.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Kostentyp]</td> 
    <td> <p>Berechnet geplante und tatsächliche Kostenschätzungen für eine Aufgabe. Wenn der Wert auf <strong>[!UICONTROL No Cost]</strong> gesetzt ist, generieren die geplanten und die tatsächlichen aufgezeichneten Stunden keine geplante oder tatsächliche Kostenschätzung für die Aufgabe und die Arbeit an der Aufgabe trägt nicht zu den Kosten auf Projektebene bei.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Probleme {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Status von gelösten Problemen automatisch aktualisieren, wenn sich der Status des aufgelösten Objekts ändert]</td> 
    <td> <p>Wenn ein Problem in ein Projekt oder eine Aufgabe konvertiert wird, werden sowohl das ursprüngliche Problem als auch das konvertierte Projekt oder die konvertierte Aufgabe zu auflösenden Objekten. Mit dieser Einstellung können Sie die Auflösung des ursprünglichen Problems mit der Auflösung des auflösbaren Objekts korrelieren. Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und Auflösen von Objekten </a>.</p> <p>Damit diese Einstellung irgendwelche Auswirkungen haben kann, muss die Option <strong>[!UICONTROL Das ursprüngliche Problem beibehalten"ausgewählt und seine Auflösung mit der Aufgabe</strong> verknüpft werden.</p> 
      <ul> 
      <li>Wenn diese Einstellung aktiviert ist, können Sie benutzerdefinierte Status mit demselben Schlüssel für Probleme und Projekte oder Aufgaben erstellen. Wenn das Projekt oder die Aufgabe (als auflösbares Objekt) in den benutzerdefinierten Status umgewandelt wird, spiegelt die Änderung auch den Status des Problems wider. Der Statusschlüssel muss für das Problem und den Projekt- oder Aufgabenstatus identisch sein.</li> 
      <li>Wenn diese Einstellung deaktiviert ist, wird beim Auflösen des Objektstatus automatisch der Standardstatus anstelle der benutzerdefinierten festgelegt. Weitere Informationen zu den Standardstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemfehlerstatus</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Beim Konvertieren eines Problems in eine Aufgabe]</td> 
    <td> <p>Die Einstellungen in diesem Abschnitt bestimmen, was während des Konvertierungsprozesses von Problem zu Aufgabe geschieht:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Behalten Sie das ursprüngliche Problem bei und binden Sie seine Lösung an die Aufgabe]</strong>: Wenn Sie das Problem konvertieren, bleibt es als Problem sichtbar, bis die Aufgabe abgeschlossen ist. Der Status des Problems ändert sich automatisch in [!UICONTROL Geschlossen] , wenn die Aufgabe abgeschlossen ist. Wenn diese Option deaktiviert ist, wird das Problem gelöscht.</p> <p><b>NOTE</b>:  <p>Benutzer ohne Zugriff oder Berechtigung zum Löschen von Problemen können das Problem beim Konvertieren nicht löschen, unabhängig vom Status dieser Einstellung. Informationen zum Zugriff auf und zu Berechtigungen für Probleme finden Sie unter:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Gewähren des Zugriffs auf Probleme</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Primären Kontakt erlauben, Zugriff auf die Aufgabe zu haben]</strong>: Gibt dem Hauptkontakt (Ersteller von Problemen) Zugriff auf die Aufgabe, um sie zu überprüfen, über ihren Fortschritt auf dem Laufenden zu bleiben und Kommentare zum Abschnitt "Aktualisierungen"der Aufgabe abzugeben.</li> 
      <li> <p><strong>[!UICONTROL Änderungen dieser Einstellungen während der Konvertierung zulassen]</strong>: Ermöglicht dem Benutzer, der das Problem konvertiert, diese Optionen während der Konvertierung eines Problems in eine Aufgabe zu ändern.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Beim Konvertieren eines Problems in ein Projekt]</td> 
    <td> <p>Die Einstellungen in diesem Abschnitt bestimmen, was während des Konvertierungsprozesses von einem Problem zum Projekt geschieht:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Das ursprüngliche Problem beibehalten und seine Lösung mit dem Projekt verknüpfen]</strong>: Wenn Sie das Problem konvertieren, bleibt es als Problem sichtbar, bis das Projekt abgeschlossen ist. Der Status des Problems ändert sich automatisch in [!UICONTROL Geschlossen] , wenn das Projekt abgeschlossen ist. Wenn diese Option deaktiviert ist, wird das Problem gelöscht. </p> <p><b>NOTE</b>:  <p>Benutzer ohne Zugriff oder Berechtigung zum Löschen von Problemen können das Problem beim Konvertieren nicht löschen, unabhängig vom Status dieser Einstellung. Informationen zum Zugriff auf und zu Berechtigungen für Probleme finden Sie unter:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Gewähren des Zugriffs auf Probleme</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Primären Kontakt erlauben, Zugriff auf das Projekt zu haben]</strong>: Gibt dem Hauptkontakt (Ersteller von Problemen) Zugriff auf das Projekt, um es zu überprüfen, über den Fortschritt auf dem Laufenden zu bleiben und Kommentare zum Abschnitt "Aktualisierungen"des Projekts abzugeben.</li> 
      <li><strong>[!UICONTROL Änderungen dieser Einstellungen während der Konvertierung zulassen]</strong>: Ermöglicht dem Benutzer, der das Problem konvertiert, die aufgeführten Optionen während der Konvertierung eines Problems in ein Projekt zu ändern.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Löschen] {#deletion}

**[!UICONTROL Ermöglichen Sie Benutzern, Aufgaben und Probleme mit angemeldeten Stunden zu löschen]**: Ermöglicht Ihnen, festzulegen, ob Sie das Löschen von Aufgaben oder Problemen, bei denen Stunden protokolliert werden, zulassen. Diese Option ist standardmäßig ausgewählt.

>[!TIP]
>
>Diese Einstellung gilt auch für das Löschen von Projekten, bei denen Aufgaben oder Probleme mit Stunden protokolliert sind. Diese Einstellung gilt nicht für das Löschen von Projekten, bei denen die Zeit direkt für das Projekt protokolliert wird.

* Wenn diese Option ausgewählt ist, erhalten Sie eine Informationswarnung, wenn Sie eine Aufgabe oder ein Problem löschen. Die Warnung weist Sie darauf hin, dass Aufgaben oder Probleme, die Stunden protokolliert haben, entweder in das Projekt verschoben oder gelöscht werden. Sie können konfigurieren, ob die Stunden gelöscht oder in das Projekt verschoben werden, und zwar im Bereich [!UICONTROL Voreinstellungen für das Timesheet und die Stunden] im Bereich [!UICONTROL Setup] . Nachdem Sie bestätigt haben, dass Sie die Warnung gesehen haben, wird die Aufgabe oder das Problem gelöscht. Weitere Informationen zum Konfigurieren der Voreinstellungen für das Zeitblatt und die Stunden finden Sie unter [Voreinstellungen für das Zeitblatt und die Stunde konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  >[!TIP]
  >
  >Wenn Sie ein Projekt mit Aufgaben und Problemen löschen, die Stunden protokolliert haben, werden die protokollierten Stunden entweder gelöscht oder gemäß den Einstellungen im Bereich &quot;[!UICONTROL Voreinstellungen für Zeitblatt und Stunden]&quot;von [!UICONTROL Setup] beibehalten. Die Warnmeldung wird beim Löschen eines Projekts nicht angezeigt.

* Wenn Sie diese Option deaktivieren, erhalten Sie eine unzulässige Warnung, wenn Sie eine Aufgabe löschen oder ein Problem mit angemeldeten Stunden beheben oder wenn Sie ein Projekt löschen, für das Stunden für die Aufgaben oder Probleme protokolliert wurden. Der Warnhinweis weist darauf hin, dass der Administrator das Löschen von Aufgaben oder Problemen mit angemeldeten Stunden nicht zulässt. Die Aufgaben, Probleme oder Projekte, bei denen Stunden für Aufgaben und Probleme protokolliert wurden, können nicht gelöscht werden.

### [!UICONTROL Tatsächliche Datumswerte] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Wenn eine Aufgabe oder ein Problem von "Neu"zu "In Bearbeitung"geht, setzen Sie das tatsächliche Startdatum auf]</td> 
    <td> <p>Wählen Sie eine der folgenden Optionen aus, wenn das tatsächliche Startdatum in [!DNL Workfront] aufgezeichnet wird, wenn eine Aufgabe oder ein Problem von <strong>[!UICONTROL New]</strong> in <strong>[!UICONTROL In Bearbeitung]</strong> übergeht:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> Das tatsächliche Startdatum wird auf das aktuelle Datum festgelegt.</li> 
      <li><strong>[!UICONTROL Das geplante Startdatum]:</strong> Das tatsächliche Startdatum wird auf das geplante Startdatum der Aufgabe oder des Problems gesetzt.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Wenn eine Aufgabe oder ein Problem abgeschlossen ist, setzen Sie das tatsächliche Abschlussdatum auf]</td> 
    <td> <p>Wählen Sie eine der folgenden Optionen aus, wenn das tatsächliche Abschlussdatum in [!DNL Workfront] aufgezeichnet wird, wenn eine Aufgabe oder ein Problem abgeschlossen ist:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> Das tatsächliche Abschlussdatum wird auf das aktuelle Datum festgelegt.</li> 
      <li> <p><strong>[!UICONTROL Das geplante Abschlussdatum]:</strong> Das tatsächliche Abschlussdatum wird auf das geplante Abschlussdatum der Aufgabe oder des Problems gesetzt.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Delegierung

Durch Aktivierung der Einstellung **[!UICONTROL Delegieren von Aufgaben und Problemen durch Benutzer zulassen]** können alle Benutzer in vorübergehend ihre Arbeit an andere delegieren.

Wenn diese Einstellung aktiviert ist, sehen Benutzer Folgendes:

* Der Link [!UICONTROL Delegieren] in ihrem Bereich [!UICONTROL Home]. Von hier aus können sie Genehmigungen oder Aufgaben- und Problemzuweisungen delegieren.
* Ein Hinweis darauf, dass eine Aufgabe oder ein Problem einem anderen Benutzer im Bereich [!UICONTROL Zuweisungen und Delegationen] in der Aufgaben- oder Problemüberschrift zugewiesen wird.

  Wenn Sie die Einstellung [!UICONTROL Erlauben, dass Benutzer ihre Aufgaben und Probleme delegieren] deaktivieren, werden die aktuell geplanten Delegationen beendet und die delegierten Benutzer erhalten eine E-Mail-Benachrichtigung, dass die Zuweisung beendet wurde.

Informationen zur Übertragung von Arbeiten an andere finden Sie in den folgenden Artikeln:

* [Delegieren von Arbeiten - Übersicht](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Verwalten der Zuweisung von Aufgaben und Ausgaben](../../../manage-work/delegate-work/how-to-delegate-work.md)

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
    <td role="rowheader">[!UICONTROL Wenn jemand einer Aufgabe zugewiesen ist]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Zugriff auf eine Aufgabe gewähren]</strong>: Definiert die Standardberechtigung, die ein Benutzer für die Aufgabe hat, der er zugewiesen ist. Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</li> 
      <li> <p><strong>[!UICONTROL Gewähren Sie ihnen ... Zugriff auf das Projekt]</strong>: Definiert die Standardberechtigung, die ein Benutzer für das Projekt hat, dem er eine Aufgabe zugewiesen hat. Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektanvoreinstellungen konfigurieren</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Wenn einem Problem ein Benutzer zugewiesen ist]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Zugriff auf eine Aufgabe gewähren]</strong>: Definiert die Standardberechtigung, die ein Benutzer für die Aufgabe hat, der er zugewiesen ist. Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</li> 
      <li> <p><strong>[!UICONTROL Gewähren Sie ihnen ... Zugriff auf das Projekt]</strong>: Definiert die Standardberechtigung, die ein Benutzer für das Projekt hat, dem er eine Aufgabe zugewiesen hat. Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektanvoreinstellungen konfigurieren</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Wenn jemand eine Anforderung sendet]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Erteilen Sie ihnen ... Zugriff auf das Problem]</strong>: Definiert die Standardberechtigung, die ein Benutzer für eine von ihm gesendete Anfrage hat. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Ein Problem freigeben </a>.</li> 
      <li> <p><strong>[!UICONTROL Personen desselben Unternehmens erben dieselben Berechtigungen für alle Anforderungen]</strong>: Ermöglicht Benutzern das Anzeigen von Anforderungen, die von anderen Benutzern aus demselben Unternehmen gesendet wurden. Sie haben dieselben Berechtigungen für diese Anforderungen wie für ihre eigenen gesendeten Anforderungen.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Voreinstellungen für Aufgaben und Probleme sperren {#lock-task-and-issue-preferences-for-groups}

Wenn Gruppen in Ihrem Unternehmen eine Aufgabe oder eine Voreinstellung für ein Problem benötigen, die für ihre individuellen Workflows unterschiedlich konfiguriert ist, können Sie die Voreinstellung für alle Gruppen in der Organisation entsperren, damit sie sie selbst konfigurieren können. Wenn eine Voreinstellung entsperrt ist und der Gruppenadministrator sie ändert, werden die mit der Gruppe verbundenen Aufgaben oder Probleme durch die Gruppenebeneneinstellung für die Voreinstellung und nicht durch die Einstellung auf Systemebene beeinflusst.

Informationen dazu, wie ein Gruppenadministrator Aufgaben- und Ausgabevoreinstellungen für eine Gruppe konfiguriert, finden Sie unter [Konfigurieren von Aufgaben- und Ausgabevoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Nachdem ein [!DNL Workfront] -Administrator eine Voreinstellung auf Systemebene entsperrt hat, kann jeder Gruppenadministrator sie konfigurieren und sie dann sperren, um sicherzustellen, dass alle Mitglieder ihrer Gruppe und der unten stehenden Untergruppen dieselbe Konfiguration verwenden. Dies entspricht der Möglichkeit, dass ein [!DNL Workfront] -Administrator eine Voreinstellung für alle Benutzer im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Konfigurieren von Projekteigenschaften für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) und [Sperren oder Entsperren von Projekten, Aufgaben oder Problemeinstellungen für Untergruppen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

So sperren oder entsperren Sie eine Aufgabe oder eine Voreinstellung für ein Problem, damit Gruppen sie konfigurieren können:

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Projekteinstellungen]** > **[!UICONTROL Aufgaben und Probleme]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Administratoren von Gruppen unter Ihrer Gruppe eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie ![](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass Ihre Gruppe und alle darunter stehenden Gruppen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie gesperrt ist (dies ist die Standardeinstellung).

     >[!IMPORTANT]
     >
     >Es wird empfohlen, mit den Administratoren und Benutzern in Gruppen im gesamten System zu kommunizieren, um sicherzustellen, dass alle Anforderungen so berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird Ihre Konfiguration für sie von allen Gruppen im System übernommen. Wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Einstellungen, die von Gruppenadministratoren vorgenommen wurden.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
