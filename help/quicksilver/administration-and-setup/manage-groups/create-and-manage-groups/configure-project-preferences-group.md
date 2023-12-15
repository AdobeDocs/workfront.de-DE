---
title: Konfigurieren von Projektvoreinstellungen für eine Gruppe
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Wenn Sie Gruppenadministrator und Adobe Workfront-Administrator sind und eine Projektvoreinstellung für alle Gruppen im System freischalten, können Sie diese Voreinstellung so konfigurieren, dass sich diese Voreinstellung auf alle nachfolgenden von Ihrer Gruppe erstellten Projekte auswirkt.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '2658'
ht-degree: 2%

---

# Konfigurieren von Projektvoreinstellungen für eine Gruppe

Wenn Sie Gruppenadministrator und Adobe Workfront-Administrator sind und eine Projektvoreinstellung für alle Gruppen im System freischalten, können Sie diese Voreinstellung so konfigurieren, dass sich diese Voreinstellung auf alle nachfolgenden von Ihrer Gruppe erstellten Projekte auswirkt.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>* In der Regel bleibt eine entsperrte Voreinstellung auf unbestimmte Zeit entsperrt. Wenn der Workfront-Administrator sie erneut sperrt, wird die Systemeinstellung erneut wirksam und die Einstellungen für die von den Gruppenadministratoren vorgenommene Voreinstellung gehen verloren.
>* Die Voreinstellungen für die Gruppe, die mit einem Projekt verknüpft ist, haben Vorrang vor den Voreinstellungen, die für die Startseite des Benutzers festgelegt wurden, der das Projekt erstellt.
>* Einige Voreinstellungen auf Gruppenebene wirken sich auf Projektvorlagen aus, die Sie für die Gruppe erstellen. Weitere Informationen finden Sie im Abschnitt . [Anzeigen, Arbeiten mit und Erstellen von Vorlagen für Ihre Gruppe über den Bereich Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) im Artikel [Erstellen und Ändern von Gruppenprojektvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt hat, können Sie sie konfigurieren und dann sperren, um sicherzustellen, dass alle Mitglieder Ihrer Gruppe und ihrer Untergruppen dieselbe Konfiguration verwenden. Dies entspricht der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle Benutzer im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Voreinstellung zum Sperren oder Entsperren eines Projekts, einer Aufgabe oder eines Problems für Untergruppen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

Die Konfiguration auf Gruppenebene ist auch für die Voreinstellungen für Aufgaben und Ausgaben sowie für Zeitblatt- und Stundenvoreinstellungen möglich. Weitere Informationen finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) und [Konfigurieren von Zeitblatt- und Stundeneinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Informationen dazu, wie ein Workfront-Administrator eine Projektvoreinstellung entsperrt, finden Sie unter [Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Konfigurieren einer entsperrten Projektreferenz für eine Gruppe

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie zu Einrichtung > Projekteinstellungen > Projekte navigieren und dann im Feld oben auf der Seite nach dem Gruppennamen suchen.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, deren Projektvoreinstellungen Sie konfigurieren möchten.
1. Klicken Sie im linken Bereich auf **Projektvoreinstellungen**.
1. Fahren Sie auf der angezeigten Seite mit einem der vier unten aufgeführten Abschnitte fort, um die Voreinstellungen für Projektstatus, Zeitpläne, Geschäftsfälle und Lebensdauer nach dem Tod zu konfigurieren.

   >[!TIP]
   >
   >Wenn Sie den Mauszeiger über eine Voreinstellung bewegen und eine QuickInfo angezeigt wird, um Ihnen mitzuteilen, dass sie gesperrt ist, können Sie Ihren Workfront-Administrator bitten, sie für alle Gruppen in der Organisation zu entsperren.

* [Projektstatus](#project-status)
* [Zeitpläne](#timelines)
* [Geschäftsszenarios](#business-cases)
* [Nachdem das Projekt eingestellt wurde](#life-after-death)

### Projektstatus {#project-status}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte, die mit der Gruppe verknüpft sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Benutzern erlauben, Projekte ohne Vorlage zu erstellen</td>
<td><p>Mit dieser Voreinstellung können Benutzer Projekte ohne Verwendung einer Vorlage erstellen, wenn sie ein Projekt aus den folgenden Bereichen erstellen:</p>
<ul>
<li><p>Verwenden der Option "Neues Projekt"in einer Liste von Projekten</p></li>

<li><p>Konvertieren eines Problems von der Seite des Problems in ein Projekt</p></li>
</ul>

<p>Diese Voreinstellung ist standardmäßig auf Systemebene aktiviert.</p>
<p><b>NOTIZ</b></p>
<p>Wenn ein Benutzer mehreren Gruppen mit unterschiedlichen Voreinstellungen angehört, kann er ein Projekt ohne Vorlage erstellen, wenn mindestens eine seiner Gruppen diese Voreinstellung aktiviert hat.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Setzen Sie den Status des neuen Projekts auf</td> 
   <td> <p>Bestimmen Sie den Status neuer Projekte.</p> <p><b>NOTE</b>   
     <ul> 
      <li>Wenn Sie oder ein anderer Workfront-Administrator den hier ausgewählten Status ausblendet, ändert sich der Standardstatus in den ersten Status in der Statusliste.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Für Gruppenprojektvoreinstellungen können Sie nur einen gesperrten Status oder einen erforderlichen Status als Standardstatus auswählen.</li> 
      <li> <p>Wenn ein gesperrtes System oder ein Gruppenstatus als Standardstatus festgelegt ist und später von einem anderen entsperrt wird, versucht das System, es durch einen gesperrten Status des gleichen Statustyps zu ersetzen.</p> <p>Wenn er keinen finden kann, sucht er nach einem erforderlichen Status:</p> 
       <ul> 
        <li>Wenn ein erforderlicher Status vorhanden ist, der dem entsperrten Standardstatus entspricht, wird der erforderliche Status zum Standardstatus, auch wenn er entsperrt ist.</li> 
        <li>Wenn keiner der erforderlichen Status dem entsperrten Standardstatus entspricht, wird der erste erforderliche Status in der Statusliste zum Standardstatus.</li> 
       </ul> <p>Informationen zu den erforderlichen Status finden Sie in den Artikeln . <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemprojektstatus</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemaufgabenstatus</a>, und <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemfehlerstatus</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prozentsatz berechnen Abgeschlossen basierend auf</td> 
   <td> <p>Der prozentuale Abschluss eines Projekts oder einer übergeordneten Aufgabe basiert auf dem Gesamtfortschritt der Aufgaben. Diese Informationen können entweder anhand der Dauer oder der geplanten Stunden der Aufgaben eines Projekts berechnet werden.</p> <p>Wenn Sie "Dauer"auswählen, bestimmt die Dauer jeder Aufgabe in einem Projekt den Gesamtprozentsatz der Abschlüsse für das Projekt und die Dauer jeder Unteraufgabe bestimmt den Gesamtprozentsatz der Abschlüsse für die übergeordnete Aufgabe.</p> <p>Wenn Sie "Dauer"auswählen, stellen Sie sicher, dass Sie die typischen Stunden pro Arbeitstag und die typischen Arbeitstage pro Woche im Abschnitt Zeitpläne angeben. Workfront verwendet diese Informationen bei der Berechnung des prozentualen Abschlusses einer Aufgabe basierend auf der Dauer. </p> <p>Wenn Sie "Geplante Stunden"auswählen, stellen Sie sicher, dass für alle Aufgaben in jedem Projekt die Anzahl der geplanten Stunden definiert ist und dass der Betrag nicht null ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Projektbedingungen je nach Fortschrittstatus automatisch setzen</td> 
   <td> <p>Mit dieser Voreinstellung können Benutzer die Projektbedingung manuell festlegen (On Target, At Risk, In Trouble) oder Workfront die Bedingung (Progress Status) automatisch basierend auf dem Projektfortschritt auf der Timeline festlegen lassen. Weitere Informationen zum Projektzustand finden Sie unter <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Projektbedingung und Bedingungstyp</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Baselines automatisch erstellen</p> </td> 
   <td> <p>Diese Voreinstellung erstellt automatisch eine Grundlinie (Momentaufnahme) der Aufgaben- und Projektdetails, wenn sich der Status des Projekts in "Aktuell"ändert. Informationen zum Erstellen von Grundlinien finden Sie unter <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Erstellen von Projekt-Grundlinien</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Performance-Index-Methode </p> </td> 
   <td> <p>Die Leistungsindex-Methode (PIM) für das Projekt steuert die Methode, die Workfront zur Berechnung von Earned Value-Metriken wie Cost Performance Index (CPI) und Estimate At Completion (EAC) verwendet. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">CPI (Cost Performance Index) berechnen</a>und <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Schätzung nach Abschluss berechnen (EAC)</a></p> 
    <ul> 
     <li><strong>Stundenbasiert</strong>: Workfront verwendet geplante Stunden zur Berechnung von Leistungsmetriken wie EAC und CPI. Wenn die PIM auf der Grundlage von Stunden berechnet wird, wird die EAC als Anzahl von Stunden angezeigt. Stellen Sie sicher, dass Sie einen Wert für "Geplante Stunden"haben, der nicht null ist.</li> 
     <li> <p><strong>Kostenbasiert</strong>: Workfront verwendet geplante Arbeitskosten zur Berechnung von Leistungsmetriken wie EAC und CPI. Stellen Sie sicher, dass Ihre Arbeitsplatzrollen oder -benutzer den Kosten pro Stunde zugeordnet sind. Wenn der PIM auf der Grundlage von Kosten berechnet wird, wird der EAC als Währungswert angezeigt.</p> <p>Der Projektmanager kann diese Einstellung auf Projektebene ändern, indem er den Bereich "Finanzen"in den Projektdetails verwendet. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Informationen im Bereich "Projekt-Finanzen"</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Schätzung bei Fertigstellung </p> </td> 
   <td> <p>Bestimmen Sie, welche Daten Workfront zur Berechnung der Schätzung bei Abschluss (EAC) verwendet, die die voraussichtlichen Gesamtkosten eines Projekts darstellt.</p> 
    <ul> 
     <li><strong>Auf Projektebene berechnen</strong>:EAC für die übergeordnete Aufgabe und das Projekt werden durch Eingabe der tatsächlichen Arbeitszeiten oder tatsächlichen Arbeitskosten in die EAC-Formeln bestimmt. Diese Berechnung schließt tatsächliche Stunden oder Kosten und Ausgaben ein, die direkt der übergeordneten Aufgabe oder dem übergeordneten Projekt hinzugefügt werden.</li> 
     <li> <p><strong>Aufrollen von Aufgaben/Unteraufgaben</strong>: Die EAC für die übergeordnete Aufgabe und das Projekt werden durch Addieren der EAC für jede untergeordnete Aufgabe bestimmt. Diese Berechnung schließt tatsächliche Stunden oder tatsächliche Kosten und Ausgaben aus, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.</p> <p>Der Projektmanager kann diese Einstellung auf Projektebene ändern, indem er den Bereich "Finanzen"in den Projektdetails verwendet. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Informationen im Bereich "Projekt-Finanzen"</a>.</p> </li> 
    </ul> <p>Weitere Informationen zur Berechnung der EAC finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Schätzung nach Abschluss berechnen (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Zeitleisten {#timelines}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte, die mit der Gruppe verknüpft sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Planen ab</td> 
   <td> <p>Bestimmen Sie, ob neue Projekte ab dem Startdatum oder ab dem Abschlussdatum geplant werden, wenn sie erstellt werden.</p> 
    <ul> 
     <li><strong>Startdatum</strong>: Für neue Aufgaben wird standardmäßig die Begrenzung der Aufgaben so bald wie möglich festgelegt, und Projektmanager werden aufgefordert, ein geplantes Startdatum für das Projekt anzugeben.</li> 
     <li><strong>Abschlussdatum</strong>: Für neue Aufgaben wird standardmäßig die Begrenzung der Aufgaben so spät wie möglich festgelegt, und Projektmanager werden aufgefordert, ein geplantes Abschlussdatum für das Projekt anzugeben.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzer-Ausfallzeiten</td> 
   <td> <p>Bestimmen Sie, ob durch die Zeitabstände des Primären Verantwortlichen einer Aufgabe die für diese Aufgabe geplanten Zeitpunkte für ein Projekt angepasst werden.</p> 
    <ul> 
     <li> <p><strong>Benutzerzeitlimit in Aufgabendauern berücksichtigen</strong>: Jede für den Primären Verantwortlichen einer Aufgabe geplante Zeitüberschreitung passt die geplanten Zeitpunkte der Aufgabe an, wenn die Zeitüberschreitung während der Aufgabendauer eintritt. Dies ist die Standardeinstellung. </p> <p>Wenn beispielsweise eine Aufgabe mit der Beschränkung So bald wie möglich am 1. Juni beginnen und am 3. Juni abgeschlossen sein soll und der Primäre Verantwortliche den 2. Juni für "Zeitlimit"markiert hat, werden die geplanten Zeitpunkte der Aufgabe auf den 1. bis 4. Juni angepasst.</p> <p><b>WICHTIG</b>: Die Dauer der Aufgabe ändert sich bei Auswahl dieser Einstellung nicht. Je nach Aufgabenbegrenzung ändern sich nur die geplanten Datumswerte.</p> </li> 
     <li><strong>Ignorieren der Benutzerzeit in der Aufgabendauer</strong>: Die geplanten Termine für jede Aufgabe eines Projekts bleiben wie ursprünglich geplant, auch wenn der Primäre Verantwortliche einer Aufgabe während ihrer Dauer über eine gewisse Zeitspanne verfügt.</li> 
    </ul> <p>Beachten Sie bei der Auswahl der Optionen für diese Einstellung Folgendes:</p> 
    <ul> 
     <li>Wenn Sie diese Einstellung ändern, übernehmen nur die nach der Änderung erstellten Projekte und Vorlagen die aktualisierte Einstellung. </li> 
     <li> <p>Der Wert der Aufgabenbegrenzung bestimmt, welche geplanten Aufgabendaten angepasst werden sollen: </p> 
      <ul> 
       <li>Das geplante Startdatum</li> 
       <li>Das geplante Abschlussdatum</li> 
       <li>Beide Datumsangaben</li> 
       <li>Keines der beiden Datum. </li> 
      </ul> <p>Wenn eine Aufgabe beispielsweise die Begrenzung fester Datumswerte aufweist, werden die Daten nicht angepasst, wenn der Primäre Verantwortliche eine Zeitüberschreitung hat, selbst wenn die Option Benutzerzeitlimit in Aufgabendauer berücksichtigen ausgewählt ist. Weitere Informationen zu Aufgabenbegrenzungen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Aufgabenbegrenzungen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Die Projektzeitpläne werden automatisch neu berechnet</strong> </p> </td> 
   <td> <p>Bestimmen Sie, wann die Timeline eines Projekts neu berechnet wird. Informationen zur Neuberechnung der Projekt-Timeline finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Projektzeitpläne neu berechnen</a>.</p> <p>Die folgenden Optionen sind standardmäßig aktiviert. Sie können eine oder mehrere der folgenden Einstellungen auswählen:</p> 
    <ul> 
     <li> <p><strong>Jeden Tag</strong>: Wählen Sie diese Option aus, um die Projektzeitpläne jede Nacht neu zu berechnen. Änderungen, die Sie am Projekt vornehmen und die sich auf die Timeline auswirken können, sind nicht sofort sichtbar. Workfront ​ ​ ​ die Neuberechnung der Fristen nachts nur für Projekte, bei denen beide der folgenden Bedingungen erfüllt sind:</p> <p> 
       <ul> 
        <li>Der Status Aktuell</li> 
        <li>In den letzten drei Monaten wurde ein Update durchgeführt</li> 
       </ul> </p> </li> 
     <li> <p><strong>Wenn sich der Umfang eines Projekts ändert</strong>: Wählen Sie diese Option aus, um die Projektzeitpläne sofort bei einer Änderung des Projektumfangs neu zu berechnen. Weitere Informationen zu einer Änderung des Projektumfangs finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Projektzeitpläne neu berechnen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Wenn mehrere Benutzer einer Aufgabe zugewiesen sind, verwenden Sie den Zeitplan der</strong> </p> </td> 
   <td> <p>Wenn einem Projekt kein Zeitplan zugewiesen ist oder den Benutzern kein Zeitplan zugewiesen wurde, verwendet Workfront den Standardsystemplan, um die Zeitleiste der Aufgaben zu berechnen.</p> <p>Wenn Sie derselben Aufgabe in einem Projekt mehrere Benutzer zuweisen, denen ein Zeitplan zugewiesen ist - und den den Aufgaben zugewiesenen Benutzern auch ein Zeitplan zugewiesen ist - verwendet Workfront die folgenden Zeitpläne:</p> 
    <ul> 
     <li><strong>Primäre Zuweisung</strong>: Workfront verwendet den Zeitplan der Primären Zuweisung für die Aufgabe zur Berechnung der Zeitpläne.</li> 
     <li><strong>Projekt</strong>: Workfront verwendet den Zeitplan des Projekts zur Berechnung der Zeitleiste jeder Aufgabe.</li> 
    </ul> <p>Weitere Informationen zu Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Zeitplan erstellen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Zeitleistenberechnungen </p> </td> 
   <td> 
    <ul> 
     <li><strong>Typische Stunden pro Arbeitstag</strong>: Legt die Anzahl der Stunden an einem typischen Arbeitstag für die Benutzer fest, die an Projekten arbeiten. Der Standardwert ist 8 Stunden.</li> 
    </ul> 
    <ul> 
     <li><strong>Typische Arbeitstage pro Woche</strong>: Legen Sie die standardmäßige Arbeitswoche für die Benutzer fest, die an Projekten arbeiten werden. Der Standardwert ist 5 Tage.</li> 
    </ul> <p>Diese beiden Optionen konvertieren Tage in Stunden oder Wochen in Tage.</p> <p>Wenn Sie beispielsweise eine Aufgabe mit 8 geplanten Stunden haben und die Dauer auf der Grundlage geplanter Stunden berechnet wird, wandelt Workfront diese Stunden in Tage um, um die Dauer als Tage anzuzeigen.</p> <p>Aus dem Feld Typische Arbeitstage pro Woche berechnet Workfront den Vollzeitäquivalenzwert (FTE) für Ihr System. Dies wird von Workfront bei der Berechnung der Benutzerzuweisungen verwendet.</p> <p>Diese Werte werden verwendet, wenn Sie Zeitpläne für Projekte planen, Ressourcen in den Budgets einplanen oder die Zeit für die Projektabwicklung einplanen. </p> <p>Sie werden nicht verwendet, wenn Sie Timesheets für Benutzer im System erstellen, wie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Zeitblatt- und Stundenvoreinstellungen konfigurieren</a>.</p> <p><b>NOTE</b>: Workfront-Administratoren können die Voreinstellungen für Zeitleistenberechnungen nicht entsperren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Benutzerdefinierte Quartal</strong> </p> </td> 
   <td> <p>Konfigurieren Sie benutzerdefinierte Jahresquartale für die Benutzer, die an Projekten arbeiten werden. Benutzerdefinierte Quartale sind in der Regel Quartale, die nicht mit der herkömmlichen Verteilung der Quartale in einem Kalenderjahr übereinstimmen. Sie können mehrere benutzerdefinierte Quartale hinzufügen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Quartale für Projekte aktivieren</a>.</p> <p><b>NOTE</b>: Workfront-Administratoren können die Voreinstellungen für benutzerdefinierte Quartal nicht entsperren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Business Cases {#business-cases}

Sie können ein Geschäftsbeispiel für neu erstellte Projekte erstellen, die mit der Gruppe verknüpft sind, um Projektanfragen zu senden. Sie können Voreinstellungen definieren, um festzulegen, welche Bereiche auf der **Geschäftsfall** Formular. Es wird empfohlen, diese Optionen zu aktivieren, damit andere Tools wie der Portfolio Optimizer ordnungsgemäß aktualisiert werden. Weitere Informationen dazu, was die einzelnen Felder anzeigen, finden Sie unter [Geschäftsfall definieren: Artikelindex](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Nachdem der Workfront-Administrator die Abschnitte im Geschäftsfall aktiviert hat, kann ein Projekteigentümer auf Projektebene einen Geschäftsfall erstellen. Informationen zum Erstellen eines Geschäftsfalls finden Sie unter [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Nachdem das Projekt eingestellt wurde  {#life-after-death}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte, die mit der Gruppe verknüpft sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Nachdem ein Projekt als abgeschlossen markiert wurde, können Personen weiterhin</strong> </p> </td> 
   <td> <p>Legen Sie die Regeln für Ihre Organisation (oder Gruppe, wenn Sie Projektvoreinstellungen für eine Gruppe konfigurieren) dahingehend fest, ob eine Aufgabe oder ein Problem gelöscht werden kann, nachdem der Projektstatus als Abgeschlossen markiert wurde.</p> 
    <ul> 
     <li><strong>Aufgaben löschen</strong>: Ermöglicht Benutzern das Löschen von Aufgaben aus einem Projekt, nachdem das Projekt als abgeschlossen markiert wurde.<br></li> 
     <li><strong>Probleme löschen</strong>: Ermöglicht Benutzern das Löschen von Problemen aus einem Projekt, nachdem das Projekt als abgeschlossen markiert wurde.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Nachdem ein Projekt als "Abgeschlossen", "Dead"oder "Ausstehende Genehmigung"markiert wurde, können Personen weiterhin</strong> </p> </td> 
   <td> <p>Legen Sie die Regeln für Ihre Organisation (oder Gruppe, wenn Sie Projektvoreinstellungen für eine Gruppe konfigurieren) fest, die festlegen, was mit Aufgaben, Problemen, Dokumenten und anderen Objekten in einem Projekt geschieht, nachdem der Projektstatus markiert wurde. <strong>Fertig</strong>, <strong>Inaktiv</strong>oder ist <strong>Ausstehende Genehmigung</strong>.</p> 
    <ul> 
     <li><strong>Aufgaben hinzufügen und bearbeiten</strong> Benutzer können: 
      <ul> 
       <li>Bearbeiten Sie Aufgaben innerhalb eines Projekts, nachdem das Projekt mit "Abgeschlossen", "Dead"oder "Ausstehende Genehmigung"gekennzeichnet wurde. Dazu gehören das Hinzufügen von Stunden und das Ändern von Ausgabeneinträgen für eine Aufgabe.</li> 
       <li>Aufgaben zu einem Projekt hinzufügen.</li> 
      </ul></li> 
     <li><strong>Hinzufügen und Bearbeiten von Problemen</strong>: Ermöglicht Benutzern Folgendes: 
      <ul> 
       <li>Bearbeiten Sie Probleme innerhalb eines Projekts, nachdem das Projekt als "Abgeschlossen", "Unzulässig"oder "Ausstehende Genehmigung"gekennzeichnet wurde.</li> 
       <li>Fügen Sie einem Projekt Probleme hinzu, nachdem das Projekt als "Fertig"oder "Abgeschlossen"markiert wurde. (Sie können einem Projekt, bei dem die Genehmigung ausstehend ist, keine Probleme hinzufügen.)</li> 
      </ul></li> 
     <li> <p><strong>Hinzufügen von Dokumenten zum Projekt sowie zu seinen Aufgaben und Problemen</strong>: Ermöglicht Benutzern das Hinzufügen von Dokumenten zu einem Projekt (oder das Hinzufügen von Dokumenten zu Aufgaben und Problemen innerhalb des Projekts), nachdem das Projekt als abgeschlossen oder ungültig markiert wurde.</p> <p>Diese Option gilt nicht für Projekte, die noch nicht genehmigt wurden.</p> </li> 
     <li> <p><strong>Vorlagen anhängen</strong>: Ermöglicht Benutzern das Anhängen von Vorlagen an ein Projekt, nachdem das Projekt als abgeschlossen oder ungültig markiert wurde.</p> <p>Diese Option gilt nicht für Projekte, die noch nicht genehmigt wurden.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
