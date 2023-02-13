---
title: Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe
user-type: administrator
product-area: system-administration;user-management;setup
keywords: group,Preferences,task,issue,unlock
navigation-topic: create-and-manage-groups
description: Wenn Gruppen in Ihrem Unternehmen eine Aufgabe oder eine Aufgabenvorgabe unabhängig von der Konfiguration auf Systemebene konfigurieren müssen, kann ein Adobe Workfront-Administrator die Voreinstellung entsperren. Als Gruppenadministrator können Sie dann die Voreinstellung für Ihre Gruppe konfigurieren und sie wirkt sich auf alle Aufgaben oder Probleme aus, die mit Ihrer Gruppe verbunden sind.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 2%

---

# Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe

Wenn Gruppen in Ihrem Unternehmen eine Aufgabe oder eine Aufgabenvorgabe unabhängig von der Konfiguration auf Systemebene konfigurieren müssen, kann ein Adobe Workfront-Administrator die Voreinstellung entsperren. Als Gruppenadministrator können Sie dann die Voreinstellung für Ihre Gruppe konfigurieren und sie wirkt sich auf alle Aufgaben oder Probleme aus, die mit Ihrer Gruppe verbunden sind.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Informationen dazu, wie der Workfront-Administrator Voreinstellungen entsperrt, finden Sie unter [Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>Die Konfiguration auf Gruppenebene ist auch für Projektvoreinstellungen möglich. Weitere Informationen finden Sie unter [Konfigurieren von Projektvoreinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* In der Regel bleibt eine entsperrte Voreinstellung auf unbestimmte Zeit entsperrt. Wenn der Workfront-Administrator sie erneut sperrt, wird die Systemeinstellung erneut wirksam und die Einstellungen für die von den Gruppenadministratoren vorgenommene Voreinstellung gehen verloren.
>* Die Voreinstellungen für die Gruppe, die mit einem Projekt verknüpft ist, haben Vorrang vor den Voreinstellungen, die für die Startseite des Benutzers festgelegt wurden, der das Projekt erstellt.
>* Einige Voreinstellungen auf Gruppenebene wirken sich auf Projektvorlagen aus, die Sie für die Gruppe erstellen. Weitere Informationen finden Sie im Abschnitt . [Anzeigen, Arbeiten mit und Erstellen von Vorlagen für Ihre Gruppe über den Bereich &quot;Gruppen&quot;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) im Artikel [Erstellen und Ändern von Gruppenprojektvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt hat, können Sie sie konfigurieren und dann sperren, um sicherzustellen, dass alle Mitglieder Ihrer Gruppe und ihrer Untergruppen dieselbe Konfiguration verwenden. Dies entspricht der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle Benutzer im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Voreinstellung zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder eines Problems für Untergruppen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Konfigurieren von entsperrten Aufgaben und Problemeinstellungen für eine Gruppe der obersten Ebene

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie zu Einrichtung > Projekteinstellungen > Aufgaben und Probleme navigieren und dann im Feld oben auf der Seite nach dem Gruppennamen suchen.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie die entsperrte Aufgabe und die Ausgabevoreinstellungen konfigurieren möchten.
1. Klicken Sie auf der Seite, die für die Gruppe angezeigt wird, im linken Bereich auf **Voreinstellungen für Aufgaben und Probleme**.
1. Fahren Sie auf der angezeigten Seite mit einem der fünf Abschnitte fort, die unter diesen Schritten aufgeführt sind, um die Einstellungen für die Bereiche &quot;Neue Aufgabenstandardwerte&quot;, &quot;Probleme&quot;, &quot;Löschen&quot;, &quot;Tatsächliche Datumswerte&quot;und &quot;Zugriff&quot;zu konfigurieren. Klicken Sie dann auf **Speichern**.

   Wenn Sie den Mauszeiger über das Sperrsymbol bewegen ![](assets/lock-toggle-button-dimmed.png) Wenn Sie eine Voreinstellung wünschen, die Sie konfigurieren müssen, und eine QuickInfo angezeigt wird, die Sie darüber informiert, dass gesperrt ist, können Sie Ihren Workfront-Administrator bitten, sie für alle Gruppen in der Organisation zu entsperren.

   Wenn sie entsperrt ist, können Sie und andere Gruppenadministratoren sie für Ihre eigenen Gruppen separat konfigurieren. Sie können sie auch für Ihre Gruppe und alle Untergruppen unterhalb Ihrer Gruppe sperren.

   * [Voreinstellungen für neue Aufgabe](#new-task-defaults)
   * [Probleme](#issues)
   * [Löschung](#deletion)
   * [Tatsächliche Termine](#actual-dates)

      <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [Zugriff](#access)

### Voreinstellungen für neue Aufgabe {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Startdatum für neue Aufgaben</td> 
      <td> <p>Legt das standardmäßige Startdatum für neue Aufgaben für Projektmanager fest. Das Startdatum für neue Aufgaben kann entweder das geplante Startdatum des Projekts oder der Tag sein, an dem die Aufgabe erstellt wird.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Dauertyp </p> </td> 
      <td> <p>Bestimmt die Beziehung zwischen der Anzahl der Ressourcen (und ihrem Zuordnungsprozentsatz) und der Dauer oder dem Gesamtaufwand für die Aufgabe. Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Aufgabendauer und -dauer</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Umsatztyp</td> 
      <td> <p>Berechnet geplante und tatsächliche Einnahmenschätzungen für eine Aufgabe. Wenn die <strong>Umsatztyp</strong> auf<strong>Nicht abrechenbar</strong>, generieren die geplanten und die tatsächlichen aufgezeichneten Stunden keine Umsatzschätzung für die Aufgabe und die Arbeit an der Aufgabe trägt nicht zum Umsatz auf Projektebene bei.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kostenart</td> 
      <td> <p>Berechnet geplante und tatsächliche Kostenschätzungen für eine Aufgabe. Wenn auf <strong>Keine Kosten</strong>, generieren die geplanten und die tatsächlichen aufgezeichneten Stunden keine geplante oder tatsächliche Kostenschätzung für die Aufgabe und die Arbeit an der Aufgabe trägt nicht zu den Kosten auf Projektebene bei.</p> </td> 
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
      <td> <p>Wenn ein Problem in ein Projekt oder eine Aufgabe konvertiert wird, werden sowohl das ursprüngliche Problem als auch das konvertierte Projekt oder die konvertierte Aufgabe zu auflösenden Objekten. Mit dieser Einstellung können Sie die Auflösung des ursprünglichen Problems mit der Auflösung des auflösbaren Objekts korrelieren. Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und Auflösen von Objekten </a>.</p> <p>Damit diese Einstellung Auswirkungen haben kann, muss die Option <strong>Behalten Sie das ursprüngliche Problem bei und binden Sie die Lösung an die Aufgabe</strong> ausgewählt sein.</p> 
       <ul> 
        <li>Wenn diese Einstellung aktiviert ist, können Sie benutzerdefinierte Status mit demselben Schlüssel für Probleme und Projekte oder Aufgaben erstellen. Wenn das Projekt oder die Aufgabe (als auflösbares Objekt) in den benutzerdefinierten Status umgewandelt wird, spiegelt die Änderung auch den Status des Problems wider. Der Statusschlüssel muss für das Problem und den Projekt- oder Aufgabenstatus identisch sein.</li> 
        <li>Wenn diese Einstellung deaktiviert ist, wird beim Auflösen des Objektstatus automatisch der Standardstatus anstelle der benutzerdefinierten festgelegt. Weitere Informationen zu den Standardstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemfehlerstatus</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beim Konvertieren eines Problems in eine Aufgabe</td> 
      <td> <p>Die Einstellungen in diesem Abschnitt bestimmen, was während des Konvertierungsprozesses von Problem zu Aufgabe geschieht:</p> 
       <ul> 
        <li><strong>Behalten Sie das ursprüngliche Problem bei und binden Sie die Lösung an die Aufgabe</strong>: Wenn Sie das Problem konvertieren, bleibt es als Problem sichtbar, bis die Aufgabe abgeschlossen ist. Der Status des Problems ändert sich automatisch in Geschlossen , wenn die Aufgabe abgeschlossen ist.</li> 
        <li><strong>Zugriff auf die Aufgabe durch Primären Kontakt zulassen</strong>: Ermöglicht dem Hauptkontakt (Problemersteller) Zugriff auf die Aufgabe, die Aufgabe zu überprüfen, Aktualisierungen vorzunehmen und über ihren Fortschritt auf dem Laufenden zu bleiben</li> 
        <li> <p><strong>Zulassen, dass diese Einstellungen während der Konvertierung geändert werden</strong>: Ermöglicht dem Benutzer, der das Problem konvertiert, diese Optionen während der Konvertierung eines Problems in eine Aufgabe zu ändern.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beim Konvertieren eines Problems in ein Projekt</td> 
      <td> <p>Die Einstellungen in diesem Abschnitt bestimmen, was während des Konvertierungsprozesses von einem Problem zum Projekt geschieht:</p> 
       <ul> 
        <li><strong>Behalten Sie das ursprüngliche Problem bei und binden Sie die Lösung an das Projekt</strong>: Wenn Sie das Problem konvertieren, bleibt es als Problem sichtbar, bis das Projekt abgeschlossen ist. Der Status des Problems ändert sich automatisch in Geschlossen , wenn das Projekt abgeschlossen ist.</li> 
        <li><strong>Primären Kontakt Zugriff auf das Projekt gewähren</strong>: Ermöglicht dem Hauptansprechpartner (Problemersteller) Zugriff auf das Projekt, das Projekt zu überprüfen, zu aktualisieren und über den Fortschritt auf dem Laufenden zu bleiben.</li> 
        <li><strong>Zulassen, dass diese Einstellungen während der Konvertierung geändert werden</strong>: Ermöglicht dem Benutzer, der das Problem konvertiert, die aufgelisteten Optionen während der Konvertierung eines Problems in ein Projekt zu ändern.</li> 
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
      <td role="rowheader">Benutzern das Löschen von Aufgaben und Anfragen mit protokollierten Stunden ermöglichen</td> 
      <td> <p> Ermöglicht Ihnen zu bestimmen, ob Sie das Löschen von Aufgaben oder Problemen, bei denen Stunden protokolliert werden, zulassen. Diese Option ist standardmäßig ausgewählt.</p> 
       <div> 
        <p><b>Tipp</b>: Diese Einstellung gilt auch für das Löschen von Projekten, bei denen Aufgaben oder Probleme mit Stunden protokolliert sind. Diese Einstellung gilt nicht für das Löschen von Projekten, bei denen die Zeit direkt für das Projekt protokolliert wird. </p> 
        <p>Beachten Sie Folgendes:</p> 
        <ul> 
         <li> <p>Wenn diese Option aktiviert ist, erhalten Sie beim Löschen einer Aufgabe oder eines Problems eine Informationswarnung. Die Warnung weist Sie darauf hin, dass Aufgaben oder Probleme, die Stunden protokolliert haben, entweder in das Projekt verschoben oder gelöscht werden. Sie können konfigurieren, ob die Stunden gelöscht oder in das Projekt verschoben werden, und zwar im Bereich "Voreinstellungen"unter "Planung". Nachdem Sie bestätigt haben, dass Sie die Warnung gesehen haben, wird die Aufgabe oder das Problem gelöscht. Weitere Informationen zum Konfigurieren der Voreinstellungen für das Zeitblatt und die Stunden finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Zeitblatt- und Stundenvoreinstellungen konfigurieren</a>. </p> <p>Tipp: <span>Wenn Sie ein Projekt mit Aufgaben und Problemen löschen, die Stunden protokolliert haben, werden die protokollierten Stunden entweder gelöscht oder gemäß den Einstellungen im Bereich "Voreinstellungen"unter "Einrichtung"im Bereich "Zeitblatt &amp; Stunden"beibehalten</span>. </p> </li> 
         <li><span>Wenn Sie diese Option deaktivieren, erhalten Sie eine unzulässige Warnung, wenn Sie eine Aufgabe löschen oder ein Problem mit angemeldeten Stunden beheben oder wenn Sie ein Projekt löschen, bei dem Stunden für seine Aufgaben oder Probleme protokolliert wurden</span> <span>.</span> In der Warnung wird angegeben, dass der Administrator das Löschen von Aufgaben oder Problemen mit angemeldeten Stunden nicht zulässt. Aufgaben, Probleme<span>oder Projekten, bei denen Stunden für Aufgaben und Probleme protokolliert wurden</span> kann nicht gelöscht werden. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### Tatsächliche Termine {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wenn eine Aufgabe oder ein Problem von "Neu"zu "In Bearbeitung"übergeht, setzen Sie das tatsächliche Startdatum auf</td> 
      <td> <p>Wählen Sie eine der folgenden Optionen aus, wenn das tatsächliche Startdatum in Workfront aufgezeichnet wird, wenn eine Aufgabe oder ein Problem von <strong>Neu</strong> nach <strong>In Bearbeitung</strong>:</p> 
       <ul> 
        <li><strong>Jetzt:</strong> Das tatsächliche Startdatum wird auf das aktuelle Datum festgelegt.</li> 
        <li><strong>Das geplante Startdatum:</strong> Das tatsächliche Startdatum ist auf das geplante Startdatum der Aufgabe oder des Problems eingestellt.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn eine Aufgabe oder ein Problem abgeschlossen ist, setzen Sie das tatsächliche Abschlussdatum auf</td> 
      <td> <p>Wählen Sie eine der folgenden Optionen aus, wenn das tatsächliche Abschlussdatum in Workfront aufgezeichnet wird, wenn eine Aufgabe oder ein Problem abgeschlossen ist:</p> 
       <ul> 
        <li><strong>Jetzt:</strong> Das tatsächliche Abschlussdatum wird auf das aktuelle Datum festgelegt.</li> 
        <li> <p><strong>Das geplante Abschlussdatum:</strong> Das tatsächliche Abschlussdatum wird auf das geplante Abschlussdatum der Aufgabe oder des Problems festgelegt.</p> </li> 
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

### Zugriff {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wenn jemand einer Aufgabe zugewiesen ist</td> 
      <td> 
       <ul> 
        <li><strong>Gewähren Sie ihnen Zugriff auf eine Aufgabe.</strong>: Definiert die Standardberechtigung, die ein Benutzer für die Aufgabe hat, der er zugewiesen ist. Weitere Informationen zu Aufgabenberechtigungen finden Sie unter<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Benutzern Zugriff gewähren</a>.</li> 
        <li> <p><strong>Gewähren Sie ihnen auch ... Zugriff auf das Projekt.</strong>: Definiert die Standardberechtigung, die ein Benutzer für das Projekt hat, dem ihm eine Aufgabe zugewiesen ist. Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn jemand einem Problem zugewiesen ist</td> 
      <td> 
       <ul> 
        <li><strong>Gewähren Sie ihnen Zugriff auf eine Aufgabe.</strong>: Definiert die Standardberechtigung, die ein Benutzer für die Aufgabe hat, der er zugewiesen ist. Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</li> 
        <li> <p><strong>Gewähren Sie ihnen auch ... Zugriff auf das Projekt.</strong>: Definiert die Standardberechtigung, die ein Benutzer für das Projekt hat, dem ihm eine Aufgabe zugewiesen ist. Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn jemand eine Anforderung sendet</td> 
      <td> 
       <ul> 
        <li><strong>Gewähren Sie ihnen Zugriff auf das Problem.</strong>: Definiert die Standardberechtigung, die ein Benutzer für eine von ihm gesendete Anfrage hat. Weitere Informationen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben</a>.</li> 
        <li> <p><strong>Personen desselben Unternehmens erben dieselben Berechtigungen für alle Anforderungen</strong>: Ermöglicht Benutzern das Anzeigen von Anforderungen, die von anderen Benutzern aus demselben Unternehmen gesendet wurden. Sie haben dieselben Berechtigungen für diese Anforderungen wie für ihre eigenen gesendeten Anforderungen.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
