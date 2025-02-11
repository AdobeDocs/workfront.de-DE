---
title: Konfigurieren von Projektvoreinstellungen für eine Gruppe
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Wenn Sie Gruppenadministrator sind und ein Adobe Workfront-Administrator eine Projektvoreinstellung für alle Gruppen im System freischaltet, können Sie diese Voreinstellung für Ihre Gruppe so konfigurieren, dass sie sich auf alle nachfolgenden Projekte auswirkt, die Ihre Gruppe erstellt.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2767'
ht-degree: 2%

---

# Projektvoreinstellungen für eine Gruppe konfigurieren


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Wenn Sie Gruppenadministrator sind und ein Adobe Workfront-Administrator eine Projektvoreinstellung für alle Gruppen im System freischaltet, können Sie diese Voreinstellung für Ihre Gruppe so konfigurieren, dass sie sich auf alle nachfolgenden Projekte auswirkt, die Ihre Gruppe erstellt.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>* In der Regel bleibt eine entsperrte Voreinstellung auf unbestimmte Zeit entsperrt. Wenn der Workfront-Administrator sie erneut sperrt, wird die Systemeinstellung erneut wirksam und die Einstellungen für die von den Gruppenadministratoren vorgenommenen Voreinstellungen gehen verloren.
>* Die Voreinstellungen, die für die mit einem Projekt verknüpfte Gruppe festgelegt wurden, haben Vorrang vor den Voreinstellungen, die für die Hauptgruppe des Benutzers festgelegt wurden, der das Projekt erstellt.
>* Einige Voreinstellungen auf Gruppenebene wirken sich auf Projektvorlagen aus, die Sie für die Gruppe erstellen. Weitere Informationen finden Sie im Abschnitt [Anzeigen, Arbeiten mit und Erstellen von Vorlagen für Ihre Gruppe im Bereich Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) im Artikel [Erstellen und Ändern der Projektvorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Nachdem ein Workfront-Administrator eine Voreinstellung auf Systemebene entsperrt hat, können Sie sie konfigurieren und dann sperren, um sicherzustellen, dass alle Personen in Ihrer Gruppe und ihren Untergruppen dieselbe Konfiguration verwenden. Dies geschieht parallel zu der Möglichkeit, dass ein Workfront-Administrator eine Voreinstellung für alle im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Projekt, Aufgabe oder Problem für Untergruppen sperren oder entsperren](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

Die Konfiguration auf Gruppenebene ist auch für Voreinstellungen für Aufgaben und Probleme sowie für Arbeitszeittabellen- und Stundeneinstellungen möglich. Weitere Informationen finden Sie unter [Aufgaben- und Problemeinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) und [Arbeitszeittabellen- und Stundeneinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Informationen dazu, wie Workfront-Admins eine Projektvoreinstellung entsperren, finden Sie unter [Projektvoreinstellungen für alle Gruppen im System sperren oder entsperren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## Konfigurieren von Voreinstellungen für entsperrte Projekte für eine Gruppe

>[!TIP]
>
>Wenn Sie Workfront-Administrator sind, können Sie die Schritte 1 bis 4 umgehen, indem Sie zu Einrichtung > Projektvoreinstellungen > Projekte wechseln und dann im Feld oben auf der Seite nach dem Namen der Gruppe suchen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![Symbol „Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, deren Projektvoreinstellungen Sie konfigurieren möchten.
1. Klicken Sie im linken Bedienfeld auf **Projektvoreinstellungen**.
1. Fahren Sie auf der angezeigten Seite mit einem der vier unten aufgeführten Abschnitte fort, um Voreinstellungen für den Projektstatus, Timelines, Business Cases und die Lebensdauer nach dem Tod zu konfigurieren.

   >[!TIP]
   >
   >Wenn Sie den Mauszeiger über eine Voreinstellung bewegen und eine QuickInfo angezeigt wird, die Ihnen mitteilt, dass sie gesperrt ist, können Sie Ihren Workfront-Administrator bitten, sie für alle Gruppen im Unternehmen zu entsperren.

* [Projektstatus](#project-status)
* [Timelines](#timelines)
* [Business Cases](#business-cases)
* [Nachdem das Projekt eingestellt wurde](#life-after-death)

### Projektstatus {#project-status}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte, die mit der Gruppe verknüpft sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>Benutzern erlauben, Projekte ohne Vorlage zu erstellen</td>
<td><p>Diese Einstellung ermöglicht es Benutzenden, Projekte ohne Vorlage zu erstellen, wenn sie ein Projekt aus den folgenden Bereichen erstellen:</p>
<ul>
<li><p>Verwenden der Option Neues Projekt in einer Projektliste</p></li>

<li><p>Konvertieren eines Problems in ein Projekt über die Problemseite</p></li>
</ul>

<p>Diese Einstellung ist standardmäßig auf Systemebene aktiviert.</p>
<p><b>NOTIZ</b></p>
<p>Wenn ein(e) Benutzende(r) mehreren Gruppen mit unterschiedlichen Voreinstellungen angehört, kann er/sie ein Projekt ohne Vorlage erstellen, wenn diese Voreinstellung für mindestens eine der Gruppen aktiviert ist.</p>
</td></tr>
  <tr> 
   <td role="rowheader">Status des neuen Projekts auf festlegen</td> 
   <td> <p>Status neuer Projekte ermitteln.</p> <p><b>HINWEIS</b>   
     <ul> 
      <li>Wenn Sie oder ein anderer Workfront-Administrator bzw. eine andere Administratorin den hier ausgewählten Status ausblendet, ändert sich der Standardstatus in den ersten Status in der Statusliste.</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">Für die Voreinstellungen für Gruppenprojekte können Sie nur einen gesperrten Status oder einen erforderlichen Status als Standardstatus auswählen.</li> 
      <li> <p>Wenn ein gesperrter System- oder Gruppenstatus als Standardstatus festgelegt ist und später von jemandem entsperrt wird, versucht das System, ihn durch einen gesperrten Status desselben Statustyps zu ersetzen.</p> <p>Wenn er keinen finden kann, sucht er nach dem erforderlichen Status:</p> 
       <ul> 
        <li>Wenn ein erforderlicher Status vorhanden ist, der dem entsperrten Standardstatus entspricht, wird der erforderliche Status zum Standardstatus, selbst wenn er entsperrt ist.</li> 
        <li>Wenn keiner der erforderlichen Status dem entsperrten Standardstatus entspricht, wird der erste erforderliche Status in der Statusliste zum Standardstatus.</li> 
       </ul> <p>Informationen zu erforderlichen Status finden Sie in den Artikeln <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemprojektstatus</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der </a> und <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">Zugriff auf die Liste der Systemanfragestatus</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prozent abgeschlossen berechnen auf Basis von</td> 
   <td> <p>Der Prozentsatz der Fertigstellung eines Projekts oder einer übergeordneten Aufgabe basiert auf dem Gesamtfortschritt der Aufgaben. Diese Informationen können entweder anhand der Dauer oder der geplanten Stunden der Aufgaben in einem Projekt berechnet werden.</p> <p>Wenn Sie Dauer auswählen, bestimmt die Dauer jeder Aufgabe in einem Projekt den Gesamtprozentsatz der Fertigstellung für das Projekt und die Dauer jeder Teilaufgabe den Gesamtprozentsatz der Fertigstellung für die übergeordnete Aufgabe.</p> <p>Wenn Sie „Dauer“ auswählen, stellen Sie sicher, dass Sie die typischen Stunden pro Arbeitstag und typische Arbeitstage pro Woche im Abschnitt „Timelines“ angeben. Workfront verwendet diese Informationen, wenn der Prozentsatz der Fertigstellung einer Aufgabe auf der Grundlage der Dauer berechnet wird. </p> <p>Wenn Sie „Geplante Stunden“ auswählen, stellen Sie sicher, dass für alle Aufgaben in jedem Projekt die Anzahl der geplanten Stunden definiert ist und dass der Betrag nicht null ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Projektbedingungen je nach Fortschrittstatus automatisch setzen</td> 
   <td> <p>Diese Einstellung ermöglicht es Benutzenden, die Bedingung eines Projekts manuell festzulegen (am Ziel, gefährdet, in Schwierigkeiten) oder Workfront die Bedingung (Fortschrittsstatus) automatisch auf der Grundlage des Projektfortschritts auf der Timeline festlegen zu lassen. Weitere Informationen über den Zustand von Projekten finden Sie unter <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Projektbedingung und Bedingungstyp</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Baselines automatisch erstellen</p> </td> 
   <td> <p>Diese Voreinstellung erstellt automatisch eine Baseline (Momentaufnahme) der Aufgaben- und Projektdetails, wenn der Status des Projekts in „Aktuell“ geändert wird. Informationen zum Erstellen von Baselines finden Sie unter <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">Erstellen von Projekt-Baselines</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Performance-Index-Methode </p> </td> 
   <td> <p>Die Performance-Index-Methode (PIM) für das Projekt steuert die Methode, die Workfront verwendet, um Earned Value-Metriken wie Cost Performance Index (CPI) und Estimate at Completion (EAC) zu berechnen. Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">Calculate Cost Performance Index (CPI)</a> und <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Calculate Estimate at Completion (EAC)</a></p> 
    <ul> 
     <li><strong>Stundenbasiert</strong>: Workfront verwendet die geplanten Stunden zur Berechnung von Leistungsmetriken wie EAC und CPI. Wenn das PIM auf der Grundlage von Stunden berechnet wird, wird die EAC als Anzahl von Stunden angezeigt. Stellen Sie sicher, dass Sie einen anderen Wert für Geplante Stunden als null haben.</li> 
     <li> <p><strong>Kostenbasiert</strong>: Workfront verwendet geplante Arbeitskosten, um Leistungsmetriken wie EAC und CPI zu berechnen. Stellen Sie sicher, dass Ihre Aufgabengebiete oder Benutzer den Stundensätzen „Kosten pro Stunde“ zugeordnet sind. Wenn die PIM auf der Grundlage von Kosten berechnet wird, wird die EAC als Währungswert angezeigt.</p> <p>Der Projekt-Manager kann diese Einstellung auf Projektebene ändern, indem er den Bereich Finanzen in den Projektdetails verwendet. Weitere Informationen finden Sie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Informationen im Bereich Projektfinanzierung</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Schätzung bei Fertigstellung </p> </td> 
   <td> <p>Legen Sie fest, welche Daten Workfront für die Schätzung der Kosten bis zur Fertigstellung verwendet, d. h. die erwarteten Gesamtkosten eines Projekts.</p> 
    <ul> 
     <li><strong>Auf Projektebene berechnen</strong>: Die BK für die übergeordnete Aufgabe und das übergeordnete Projekt wird bestimmt, indem in die BK-Formeln die Ist-Stunden oder die Ist-Lohnkosten eingegeben werden. Diese Berechnung enthält die tatsächlichen Stunden oder Kosten und Ausgaben, die der übergeordneten Aufgabe oder dem übergeordneten Projekt direkt hinzugefügt werden.</li> 
     <li> <p><strong>Rollup aus Aufgaben/Teilaufgaben</strong>: Die LGR für die übergeordnete Aufgabe und das übergeordnete Projekt wird bestimmt, indem die LGR für jede untergeordnete Aufgabe zusammengefasst werden. Diese Berechnung schließt tatsächliche Stunden oder Istkosten und Ausgaben aus, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.</p> <p>Der Projekt-Manager kann diese Einstellung auf Projektebene ändern, indem er den Bereich Finanzen in den Projektdetails verwendet. Weitere Informationen finden Sie <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Informationen im Bereich Projektfinanzierung</a>.</p> </li> 
    </ul> <p>Weitere Informationen zur EAC-Berechnung finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">Berechnete Schätzung bei Abschluss berechnen (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Timelines {#timelines}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte, die mit der Gruppe verknüpft sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Planen ab</td> 
   <td> <p>Legen Sie fest, ob neue Projekte ab dem Startdatum oder ab dem Abschlussdatum geplant werden, wenn sie erstellt werden.</p> 
    <ul> 
     <li><strong>Startdatum</strong>: Für neue Aufgaben wird die Option „Sobald wie möglich“ ausgewählt, und die Projektverantwortlichen werden aufgefordert, ein geplantes Startdatum für das Projekt anzugeben.</li> 
     <li><strong>Abschlussdatum</strong>: Für neue Aufgaben wird standardmäßig die Einschränkung So spät wie möglich verwendet, und die Projektverantwortlichen werden aufgefordert, ein geplantes Abschlussdatum für das Projekt anzugeben.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Benutzer-Ausfallzeiten</td> 
   <td> <p>Legen Sie fest, ob die Ausfallzeit des Primären Verantwortlichen für eine Aufgabe die geplanten Termine für diese Aufgabe in einem Projekt anpasst.</p> 
    <ul> 
     <li> <p><strong>Auszeiten von Benutzern in Aufgabendauer berücksichtigen</strong>: Jede für den Primären Beauftragten einer Aufgabe geplante Auszeit passt die geplanten Termine der Aufgabe an, wenn die Auszeit während der Aufgabendauer eintritt. Dies ist die Standardeinstellung. </p> <p>Wenn beispielsweise eine Aufgabe mit der Einschränkung So bald wie möglich am 1. Juni beginnen und am 3. Juni abgeschlossen werden soll und der Primäre Verantwortliche für den 2. Juni eine Ausfallzeit markiert hat, werden die Termine für die Aufgabe auf den 1. Juni bis zum 4. Juni festgelegt.</p> <p><b>WICHTIG</b>: Die Dauer der Aufgabe ändert sich nicht, wenn Sie diese Einstellung auswählen. Je nach Aufgabenbeschränkung ändern sich nur die geplanten Termine.</p> </li> 
     <li><strong>Benutzer-Ausfallzeit in Aufgabendauer ignorieren</strong>: Die geplanten Termine jeder Aufgabe in einem Projekt bleiben wie ursprünglich geplant, auch wenn der Primäre Verantwortliche einer Aufgabe während ihrer Laufzeit Ausfallzeiten hat.</li> 
    </ul> <p>Beachten Sie bei der Auswahl von Optionen für diese Einstellung Folgendes:</p> 
    <ul> 
     <li>Wenn Sie diese Einstellung ändern, erben nur die Projekte und Vorlagen, die nach der Änderung erstellt wurden, die aktualisierte Einstellung. </li> 
     <li> <p>Der Wert der Aufgabenbeschränkung der Aufgabe bestimmt, welche geplanten Aufgabendaten angepasst werden sollen: </p> 
      <ul> 
       <li>Das geplante Startdatum</li> 
       <li>Das geplante Abschlussdatum</li> 
       <li>Beide Daten</li> 
       <li>Kein Datum. </li> 
      </ul> <p>Wenn beispielsweise eine Aufgabe eine Beschränkung für feste Termine aufweist, werden die Termine nicht angepasst, wenn der Primäre Verantwortliche Ausfallzeiten hat, auch wenn die Option Benutzer-Ausfallzeiten in Aufgabendauer berücksichtigen ausgewählt ist. Informationen zu Aufgabenbeschränkungen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Aufgabenbeschränkungen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Projektzeitleisten werden automatisch neu berechnet</strong> </p> </td> 
   <td> <p>Legen Sie fest, wann die Zeitleiste eines Projekts neu berechnet wird. Informationen zur Neuberechnung der Projekt-Zeitleiste finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Neuberechnen von Projekt-Zeitleisten</a>.</p> <p>Die folgenden Optionen sind standardmäßig aktiviert. Sie können eine oder mehrere der folgenden Einstellungen auswählen:</p> 
    <ul> 
     <li> <p><strong>Jede Nacht</strong>: Wählen Sie diese Option, um die Projektzeitleisten jede Nacht neu zu berechnen. Alle Änderungen, die Sie am Projekt vornehmen und die sich auf die Zeitleiste auswirken könnten, sind nicht sofort sichtbar. Workfront​​​ berechnet Timelines nur bei Nacht neu für Projekte, bei denen die beiden folgenden Bedingungen erfüllt sind:</p> <p> 
       <ul> 
        <li>den Status „Aktuell“ haben</li> 
        <li>In den letzten 3 Monaten ein Update erhalten haben</li> 
       </ul> </p> </li> 
     <li> <p><strong>Wenn sich der Projektumfang ändert</strong>: Wählen Sie diese Option, um die Projektzeitleisten sofort nach einer Änderung des Projektumfangs neu zu berechnen. Informationen dazu, was eine Änderung des Projektumfangs ausmacht, finden Sie unter <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">Neuberechnen von Projektzeitleisten</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Wenn mehrere Benutzer einer Aufgabe zugewiesen sind, verwenden Sie den Zeitplan von …</strong> </p> </td> 
   <td> <p>Wenn einem Projekt kein Zeitplan zugewiesen ist oder den Benutzern, die seinen Aufgaben zugewiesen sind, kein Zeitplan zugewiesen ist, berechnet Workfront mithilfe des Systemstandardzeitplans den Zeitplan der Aufgaben.</p> <p>Wenn Sie derselben Aufgabe in einem Projekt mehrere Benutzer zuweisen und den Benutzern dieser Aufgaben ebenfalls ein Zeitplan zugewiesen ist, verwendet Workfront die folgenden Zeitpläne:</p> 
    <ul> 
     <li><strong>Primäre Zuweisung</strong>: Workfront verwendet den Zeitplan der Primären Zuweisung für die Aufgabe, um die Zeitleisten zu berechnen.</li> 
     <li><strong>Projekt</strong>: Workfront verwendet den Zeitplan des Projekts, um die Zeitleiste jeder Aufgabe zu berechnen.</li> 
    </ul> <p>Weitere Informationen zu Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Erstellen eines Zeitplans</a>.</p> </td> 
  </tr> 
 <tr> 
   <td role="rowheader"> <p><strong>Wenn ein(e) Benutzende(r) einer Aufgabe zugewiesen wird, den Zeitplan verwenden von…</strong> </p> </td> 
   <td> <p>Wenn einem Projekt kein Zeitplan zugewiesen ist oder den Benutzern, die seinen Aufgaben zugewiesen sind, kein Zeitplan zugewiesen ist, berechnet [!DNL Workfront] anhand des Systemstandardzeitplans den Zeitplan der Aufgaben.</p>

<p>Wenn Sie einer Aufgabe in einem Projekt einen Benutzer zuweisen und sowohl dem Projekt als auch dem Benutzer ein Zeitplan zugeordnet ist, verwendet [!UICONTROL Workfront] die folgenden Zeitpläne:</p> 
    <ul> 
     <li><strong>[!UICONTROL User]</strong>: Der Zeitplan des zugewiesenen Benutzers für die Aufgabe, um die Zeitleisten zu berechnen.</li> 
     <li><strong>[!UICONTROL Project]</strong>: Der Zeitplan des Projekts zur Berechnung der Zeitleiste der Aufgabe.</li> 
    </ul> <p>Weitere Informationen zu Zeitplänen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">Erstellen eines Zeitplans</a>.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Timeline-Berechnungen </p> </td> 
   <td> 
    <ul> 
     <li><strong>Typische Stunden pro Arbeitstag</strong>: Legen Sie die Anzahl der Stunden in einem typischen Arbeitstag für die Benutzer fest, die an Projekten arbeiten werden. Der Standardwert ist 8 Stunden.</li> 
    </ul> 
    <ul> 
     <li><strong>Typische Arbeitstage pro Woche</strong>: Legen Sie die Standard-Arbeitswoche für die Benutzer fest, die an Projekten arbeiten werden. Der Standardwert ist 5 Tage.</li> 
    </ul> <p>Diese zwei Optionen konvertieren Tage in Stunden bzw. Wochen in Tage.</p> <p>Wenn beispielsweise ein Vorgang mit acht geplanten Stunden vorhanden ist und die Dauer auf der Grundlage der geplanten Stunden berechnet wird, wandelt Workfront diese Stunden in Tage um, um die Dauer als Tage anzuzeigen.</p> <p>Aus dem Feld Typische Arbeitstage pro Woche berechnet Workfront den Vollzeitäquivalentwert (VZÄ) für Ihr System. Dies wird von Workfront bei der Berechnung der Zuweisungen für -Benutzer verwendet.</p> <p>Diese Werte werden verwendet, wenn Sie Projektzeitleisten planen, Ressourcen budgetieren oder Zeit für Projekte protokollieren. </p> <p>Sie werden nicht verwendet, wenn Sie Arbeitszeittabellen für Benutzende im System erstellen, wie in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen</a> beschrieben.</p> <p><b>HINWEIS</b>: Workfront-Administratoren können die Voreinstellungen für Zeitleistenberechnungen nicht entsperren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>Benutzerdefinierte Quartale</strong> </p> </td> 
   <td> <p>Konfigurieren Sie benutzerdefinierte jährliche Quartale für die Benutzer, die an Projekten arbeiten werden. Benutzerdefinierte Quartale sind in der Regel Quartale, die nicht der herkömmlichen Aufschlüsselung von Quartalen während eines Kalenderjahres entsprechen. Sie können mehrere benutzerdefinierte Quartale hinzufügen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Quartale für Projekte </a>.</p> <p><b>HINWEIS</b>: Workfront-Administratoren können die Voreinstellungen für benutzerdefinierte Quartale nicht entsperren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Business Cases {#business-cases}

Sie können einen Business Case für neu erstellte Projekte erstellen, die mit der Gruppe verknüpft sind, um Projektanfragen zu senden. Sie können Voreinstellungen definieren, um zu bestimmen, welche Bereiche im Formular **Business Case** sichtbar sind. Es wird empfohlen, diese Optionen zu aktivieren, damit andere Tools, wie z. B. Portfolio Optimizer, ordnungsgemäß aktualisiert werden. Weitere Informationen zu den einzelnen Feldern finden Sie unter [Definieren eines Business-Case: Artikelindex](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Nachdem der Workfront-Administrator die Abschnitte zum Business Case aktiviert hat, kann ein Projektinhaber dann einen Business Case auf Projektebene erstellen. Informationen zum Erstellen eines Business-Case finden Sie [Erstellen eines Business-Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### Nachdem das Projekt eingestellt wurde  {#life-after-death}

Konfigurieren Sie eine der folgenden Voreinstellungen für neu erstellte Projekte, die mit der Gruppe verknüpft sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>Nachdem ein Projekt als Abgeschlossen gekennzeichnet wurde, können Benutzer weiterhin</strong> </p> </td> 
   <td> <p>Legen Sie die Regeln für Ihre Organisation (oder Gruppe, wenn Sie Projektvoreinstellungen für eine Gruppe konfigurieren) fest, die festlegen, ob eine Aufgabe oder ein Problem gelöscht werden kann, nachdem der Projektstatus als „Abgeschlossen“ markiert wurde.</p> 
    <ul> 
     <li><strong>Aufgaben löschen</strong>: Ermöglicht Benutzern das Löschen von Aufgaben aus einem Projekt, nachdem das Projekt als „Abgeschlossen“ markiert wurde.<br></li> 
     <li><strong>Anfragen löschen</strong>: Ermöglicht Benutzern das Löschen von Anfragen aus einem Projekt, nachdem das Projekt als „Abgeschlossen“ markiert wurde.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>Nachdem ein Projekt als Abgeschlossen, Eingestellt oder mit dem Hinweis Ausstehende Genehmigungen, gekennzeichnet wurde, können Benutzer weiterhin</strong> </p> </td> 
   <td> <p><strong> Legen Sie die Regeln für Ihre Organisation (oder Gruppe, wenn Sie Projektvoreinstellungen für eine Gruppe konfigurieren) fest, was mit Aufgaben, Problemen, Dokumenten und anderen Objekten in einem Projekt geschieht, nachdem der Projektstatus als „Abgeschlossen</strong>, <strong>Eingestellt</strong> gekennzeichnet wurde oder <strong>Genehmigung steht</strong>.</p> 
    <ul> 
     <li><strong>Aufgaben hinzufügen und bearbeiten</strong> Ermöglicht Benutzern Folgendes: 
      <ul> 
       <li>Aufgaben innerhalb eines Projekts bearbeiten, nachdem das Projekt als „Abgeschlossen“, „Eingestellt“ oder „Genehmigung steht aus“ gekennzeichnet wurde. Dazu gehören das Hinzufügen von Stunden und das Ändern von Kosteneinträgen für eine Aufgabe.</li> 
       <li>Aufgaben zu einem Projekt hinzufügen.</li> 
      </ul></li> 
     <li><strong>Probleme hinzufügen und bearbeiten</strong>: Ermöglicht Benutzern Folgendes: 
      <ul> 
       <li>Probleme innerhalb eines Projekts bearbeiten, nachdem das Projekt als „Abgeschlossen“, „Eingestellt“ oder „Genehmigung steht aus“ gekennzeichnet wurde.</li> 
       <li>Probleme zu einem Projekt hinzufügen, nachdem das Projekt als „Abgeschlossen“ oder „Eingestellt“ gekennzeichnet wurde. (Sie können keine Probleme zu einem Projekt hinzufügen, für das die Genehmigung aussteht.)</li> 
      </ul></li> 
     <li> <p><strong>Dokumente zum Projekt sowie zu seinen Aufgaben und Problemen hinzufügen</strong>: Ermöglicht Benutzern das Hinzufügen von Dokumenten zu einem Projekt (oder das Hinzufügen von Dokumenten zu Aufgaben und Problemen innerhalb des Projekts), nachdem das Projekt als Abgeschlossen oder Eingestellt markiert wurde.</p> <p>Diese Option gilt nicht für Projekte, die noch nicht genehmigt wurden.</p> </li> 
     <li> <p><strong>Vorlagen anhängen</strong>: Ermöglicht Benutzern, Vorlagen an ein Projekt anzuhängen, nachdem das Projekt als „Abgeschlossen“ oder „Eingestellt“ gekennzeichnet wurde.</p> <p>Diese Option gilt nicht für Projekte, die noch nicht genehmigt wurden.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
