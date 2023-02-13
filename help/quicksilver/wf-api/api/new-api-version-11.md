---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 11
description: ReportBudgedHour wurde zur Adobe Workfront-API als Berichtsressource hinzugefügt. Es enthält Referenzfelder, Kernfelder und Standardfelder, die in BudgetedHour fehlen.
author: John
feature: Workfront API
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 2%

---

# Neue Funktionen in API Version 11

* [Hinzugefügte Ressourcen](#added-resources)
* [Entfernte Ressourcen](#removed-resources)
* [Geänderte Ressourcen](#modified-resources)

## Hinzugefügte Ressourcen {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [REportableBudgetedHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">Accessor</li> 
     <li style="font-weight: bold;">customer</li> 
     <li style="font-weight: bold;">Benutzer  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customer  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customer  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### REportableBudgetedHour {#reportablebudgetedhour}

ReportBudgedHour wurde zur Adobe Workfront-API als Berichtsressource hinzugefügt. Es enthält Referenzfelder, Kernfelder und Standardfelder, die in BudgetedHour fehlen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>Das Zuordnungsdatum ist der erste Tag (ein Sonntag) der Woche, für den Sie die Stunden im Ressourcenplaner in den Haushaltsplan eingesetzt haben.</p> </li> 
     <li> <p style="font-weight: bold;">budgetHours </p> <p>Budgetierte Stunden sind Stunden, die der Ressourcen-Manager für die Arbeit einplant, die Ressourcen für Projekte durchführen müssen</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>Die eindeutige Workfront-ID, die einem bestimmten meldepflichtigen Budgeting Hour-Objekt zugewiesen ist.</p> </li> 
     <li style="font-weight: bold;">scheduledBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>Die eindeutige Workfront-ID, die einem bestimmten Projekt zugewiesen ist.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>Die eindeutige Workfront-ID, die einer bestimmten Auftragsrolle zugewiesen ist.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>Die eindeutige Workfront-ID, die einem bestimmten Benutzer zugewiesen ist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">Projekt</p> <p>Das Projekt, mit dem eine ReportableBudgetedHour verknüpft ist.</p> </li> 
     <li> <p style="font-weight: bold;">Funktion</p> <p>Die Auftragsrolle, mit der eine reportableBudgetedHour verknüpft ist.</p> </li> 
     <li> <p style="font-weight: bold;">Benutzer</p> <p>Der Benutzer, mit dem eine ReportableBudgetedHour verknüpft ist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Vorgänge</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">COUNT</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">BERICHT </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Entfernte Ressourcen {#removed-resources}

Für API v11 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">Genehmigung</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Zuweisung</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">BaselineTask</a> </li> 
     <li><a href="#category" class="MCXref xref">Kategorie</a> </li> 
     <li><a href="#company" class="MCXref xref">Firma</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Kunde</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Dokument</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Wiederholung</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Layoutvorlage</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">Notiz</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parameter</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Programm</a> </li> 
     <li><a href="#project" class="MCXref xref">Projekt</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">TestversandApproval</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">Risiko</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Aufgabe</a> </li> 
     <li><a href="#team" class="MCXref xref">Team</a> </li> 
     <li><a href="#template" class="MCXref xref">Vorlage</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Arbeitszeittabelle</a> </li> 
     <li><a href="#update" class="MCXref xref">Aktualisieren</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">Arbeit </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

Ein AccessLevelPermissions -Objekt stellt einen Berechtigungssatz dar. Dieser Berechtigungssatz kann dann einer Zugriffsebene zugeordnet werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>In den folgenden Feldern wurde der mögliche Wert BUDGETING_INFORMATION hinzugefügt. Dadurch können Benutzer mit der Berechtigung Prioritäten und Budgetzeiten im Planer bearbeiten.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Wenn ein Benutzer keinen Zugriff auf ein Objekt in Workfront hat, das er benötigt, kann er den Zugriff auf dieses Objekt anfordern. Das AccessRequest -Objekt stellt diese Anforderung dar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">action</p> <p>Der mögliche Wert BUDGETING_INFORMATION wurde hinzugefügt. Dadurch können Benutzer mit der Berechtigung Prioritäten und Budgetzeiten im Planer bearbeiten.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

Ein AccessRule -Objekt stellt einen Regelsatz in benutzerdefinierten Zugriffsebenen dar, der bestimmt, wie Benutzer von ihnen erstellte Projekte freigeben können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>In den folgenden Feldern wurde der mögliche Wert BUDGETING_INFORMATION hinzugefügt. Dadurch können Benutzer mit der Berechtigung Prioritäten und Budgetzeiten im Planer bearbeiten.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Genehmigung {#approval}

Ein bestimmtes Arbeitselement, wie z. B. eine Aufgabe, ein Dokument oder ein Timesheet, kann vorschreiben, dass ein Supervisor oder ein anderer Benutzer das Arbeitselement abzeichnet. Ein Approval-Objekt stellt die Aktion zum Abmelden eines Arbeitselements dar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">In den folgenden Feldern wurden die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Validatoren legen fest, dass Datumsangaben für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach dem Jahr 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">IststartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zur öffentlichen API hinzugefügt, um Transparenz bei der Berechnung von EAC (Schätzung bei Abschluss) zu gewährleisten.</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Die auch als Earned Value (Earned Value, Earned Value, Budgeted Cost of Work Performed, BCWP) bezeichnete Metrik zur Projektleistung, die die budgetierten Kosten der zum Zeitpunkt der Berechnung dieser Metrik tatsächlich abgeschlossenen Aufgabe darstellt. Bei Aufgaben: BCWP = Tatsächlicher Prozentsatz der Vollständigkeit x Aufgabenbudget. Bei Projekten: BCWP = SUM(BCWP-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Die auch als "Geplanter Wert"bekannten budgetierten Kosten für geplante Arbeit (BCWS) sind eine Metrik zur Projektleistung, die die geplanten Kosten der Aufgabenmenge darstellt, die zum Zeitpunkt der Berechnung dieser Metrik abgeschlossen sein sollten. Für Aufgaben: BCWS = Geplanter Prozentsatz Abgeschlossen x Aufgabenbudget. Bei Projekten BCWS = SUM(BCWS-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
    </ul><p style="font-weight: normal;">Die folgenden Felder haben den möglichen Wert ET hinzugefügt. Dieser Wert stellt die Zeiteinheit der verstrichenen Monate dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">In den folgenden Feldern wurde die Markierung WÄHRUNG hinzugefügt</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden aus dem Objekt Genehmigung entfernt.</p>
    <ul>
     <li style="font-weight: bold;">preserveTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde dem Objekt Genehmigung hinzugefügt.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>preserveTime</p> <p style="font-weight: normal;">Aus dem Objekt "Genehmigung"entfernt  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Zum Objekt Genehmigung hinzugefügt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Ein ApprovalPath -Objekt ist eine Verzweigung innerhalb eines Genehmigungsprozesses. Validierungspfade basieren auf dem Status des Objekts, mit dem der Validierungsprozess verknüpft ist.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Der mögliche Wert ET wurde hinzugefügt. Dieser Wert stellt die Zeiteinheit der verstrichenen Monate dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

Ein ApprovalProcess -Objekt ist eine mehrstufige Genehmigung, die mit einem Projekt, einer Aufgabe oder einem Problem verknüpft werden kann.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt. Es ist ein boolescher Parameter, der den Wert true hat, wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden. Objekte, die nicht auf "Aktiv"gesetzt sind, sind nicht in Dropdown-Menüs und Typvorlagenfeldern sichtbar, die an andere Objekte angehängt werden sollen.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Zuweisung {#assignment}

Ein Zuweisungsobjekt stellt die Verbindung zwischen einem Arbeitselement und dem Benutzer, Team oder der Gruppe dar, der bzw. die für die Bearbeitung zugewiesen ist.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">Der mögliche Wert ET wurde hinzugefügt. Dieser Wert stellt die Zeiteinheit der verstrichenen Monate dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BaselineTask {#baselinetask}

Grundlinien sind Momentaufnahmen davon, wie die Leistung eines Projekts zu einem bestimmten Zeitpunkt aussah. Sie speichern wichtige Informationen zum Projekt, wie z. B. Schlüsseldaten, Fortschritt, Kosten und Umsatzwerte. Wenn Sie eine Grundlinie erstellen, werden die Aufgabeninformationen auch in den Grundaufgaben dieser Grundlinie erfasst.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Der mögliche Wert ET wurde hinzugefügt. Dieser Wert stellt die Zeiteinheit der verstrichenen Monate dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kategorie {#category}

Ein Category -Objekt ist ein benutzerdefiniertes Formular. Sie können Berichte für dieses Objekt erstellen und es auch in anderen Objektberichten anzeigen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt. Es ist ein boolescher Parameter, der den Wert true hat, wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden. Objekte, die nicht auf "Aktiv"gesetzt sind, sind nicht in Dropdown-Menüs und Typvorlagenfeldern sichtbar, die an andere Objekte angehängt werden sollen.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Firma {#company}

Ein Unternehmensobjekt stellt eine Organisation dar, die aus einer Personensammlung besteht. Unternehmen sind mit einem Benutzer oder einem Projekt verknüpft.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt. Es ist ein boolescher Parameter, der den Wert true hat, wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden. Objekte, die nicht auf "Aktiv"gesetzt sind, sind nicht in Dropdown-Menüs und Typvorlagenfeldern sichtbar, die an andere Objekte angehängt werden sollen.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p style="font-weight: normal;">Die folgenden Aktionen wurden dem CustomEnum-Objekt hinzugefügt</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Abfragen</td> 
   <td> <p>Die folgenden Abfragen wurden dem CustomEnum-Objekt hinzugefügt</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kunde {#customer}

Ein Kundenobjekt stellt eine Organisation dar, die eine Instanz von Workfront verwendet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Mögliche Werte wurden hinzugefügt: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (Projektbedingungen)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (Aufgabenbedingungen)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (Problembedingungen)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p style="font-weight: normal;">Dem Kundenobjekt wurden die folgenden Aktionen hinzugefügt</p> 
    <ul> 
     <li style="font-weight: bold;">targetsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

Ein CustomerPreferences -Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Instanz von Workfront festgelegt hat.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Mögliche Werte wurden hinzugefügt:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Anforderungen an die Kennwortkomplexität)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (Mindestlänge des Kennworts)</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout (Zeitlimit für mobile Sitzungen)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (User Time Off)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.manualrole (manuelle Kontrollrolle)</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientGuestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Aktionen</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Dokument {#document}

Ein Dokumentobjekt stellt eine Datei dar (z. B. schriftliches Material, Bilder oder andere Informationsformen).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p>Die folgenden Aktionen wurden dem Dokumentobjekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Wiederholung {#iteration}

Ein Iteration -Objekt stellt eine einzelne Agile Iteration dar. Iterationen sind diskrete Zeiträume, die zur Planung und Ergänzung von Agile-Geschichten verwendet werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder wurden dem Iteration-Objekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">Abgeschlossene Punkte</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Layoutvorlage {#layout-template}

Ein Layout-Vorlagenobjekt stellt eine bestimmte Anordnung von Layoutelementen dar, z. B. das Hauptmenü, das Navigationsfenster oder den Startbereich. Layoutvorlagen können Benutzern, Teams, Gruppen oder Auftragseingaben zugewiesen werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt. Es ist ein boolescher Parameter, der den Wert true hat, wenn eine Layout-Vorlage für die Anzeige von Zeitstempeln für Fälligkeitsdaten in der Arbeitsliste und im Kalender festgelegt ist, und false, wenn Zeitstempel ausgeblendet werden.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### MilestonePath {#milestonepath}

Ein Meilenstein ist ein Marker für eine Aufgabe, der angibt, dass es sich um einen Schlüsselpunkt im Projekt handelt. Wird im Allgemeinen dazu verwendet, ein wichtiges Ereignis zu kennzeichnen, z. B. den Abschluss einer Phase des Projekts oder eine Reihe kritischer Aktivitäten. Ein MilestonePath -Objekt ist eine Sammlung von Meilensteinen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt. Es ist ein boolescher Parameter, der den Wert true hat, wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden. Objekte, die nicht auf "Aktiv"gesetzt sind, sind nicht in Dropdown-Menüs und Typvorlagenfeldern sichtbar, die an andere Objekte angehängt werden sollen.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Notiz {#note}

Ein Hinweis -Objekt ist ein Kommentar oder eine Aktualisierung, die an einem Workfront-Objekt vorgenommen wird.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder wurden dem Notizobjekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>lies</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Ein OpTask-Objekt wird häufig als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise anzeigt, dass ein Problem vorliegt, das die Fertigstellung einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungen bei Bestellungen, Anforderungen und Fehlern sind ebenfalls Probleme.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">In den folgenden Feldern wurden die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Werte geben an, dass Daten für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach dem Jahr 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">IststartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zu OpTask hinzugefügt.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">Die eindeutige Workfront-ID eines Kanban-Board-Objekts.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Percent Complete ist ein Parameter, der den abgeschlossenen Betrag eines Problems in Prozent zurückgibt.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">Arbeit  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Suchfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Arbeit</p> <p style="font-weight: normal;">Entfernt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p>Die folgenden Aktionen wurden dem OpTask-Objekt hinzugefügt</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

Ein Parameter -Objekt ist ein benutzerdefiniertes Feld.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Mögliche Werte vom Typ TYAH (Typahead) hinzugefügt.</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und verweist auf den Objektcode eines referenzierten Objekts. Objektcodes für alle Objekte finden Sie im <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Ein Portfolio-Objekt ist eine Sammlung von Projekten, die um die gleichen Ressourcen konkurrieren, in der Regel um Geld oder Personen, um sie zu vervollständigen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass die Länge der Beschreibung nicht mehr als 4000 Zeichen beträgt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programm {#program}

Ein Programmobjekt ist eine Teilmenge innerhalb eines Portfolios, in der ähnliche Projekte gruppiert werden können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass die Länge der Beschreibung nicht mehr als 4000 Zeichen beträgt.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt. Es ist ein boolescher Parameter, der den Wert true hat, wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden. Objekte, die nicht auf "Aktiv"gesetzt sind, sind nicht in Dropdown-Menüs und Typvorlagenfeldern sichtbar, die an andere Objekte angehängt werden sollen.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass der Name maximal 255 Zeichen lang ist.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projekt {#project}

Projekte sind Arbeitselemente in Workfront und stellen einen Hauptbaustein dar, wie Workfront Menschen bei der Arbeit unterstützt. Ein Projektobjekt stellt eine Gruppe von Aufgaben mit einem gemeinsamen, spezifischen Ziel dar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">In den folgenden Feldern wurden die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Werte geben an, dass Daten für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach dem Jahr 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">IststartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zur öffentlichen API hinzugefügt, um Transparenz bei der Berechnung von EAC (Schätzung bei Abschluss) zu gewährleisten.</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Die auch als Earned Value (Earned Value, Earned Value, Budgeted Cost of Work Performed, BCWP) bezeichnete Metrik zur Projektleistung, die die budgetierten Kosten der zum Zeitpunkt der Berechnung dieser Metrik tatsächlich abgeschlossenen Aufgabe darstellt. Bei Aufgaben: BCWP = Tatsächlicher Prozentsatz der Vollständigkeit x Aufgabenbudget. Bei Projekten: BCWP = SUM(BCWP-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Die auch als "Geplanter Wert"bekannten budgetierten Kosten für geplante Arbeit (BCWS) sind eine Metrik zur Projektleistung, die die geplanten Kosten der Aufgabenmenge darstellt, die zum Zeitpunkt der Berechnung dieser Metrik abgeschlossen sein sollten. Für Aufgaben: BCWS = Geplanter Prozentsatz Abgeschlossen x Aufgabenbudget. Bei Projekten BCWS = SUM(BCWS-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
    </ul><p style="font-weight: normal;">In den folgenden Feldern wurde die Markierung WÄHRUNG hinzugefügt</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde aus dem Projektobjekt entfernt.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TestversandApproval {#proofapproval}

Ein Objekt vom Typ Testversand-Validierung stellt eine Validierung dar, die direkt mit einem Testversand verbunden ist.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitDecision</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt. Es ist ein boolescher Parameter mit dem Wert true , wenn ein Testversand auf eine Entscheidung wartet, und false , wenn dies nicht der Fall ist.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Ein QueueDef-Objekt stellt eine Warteschlange dar. Hierbei handelt es sich um ein Projekt, das in den Help Desk-Bereich veröffentlicht wurde, damit Benutzer Probleme an dieses Objekt senden können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>In den folgenden Feldern wurde der mögliche Wert BUDGETING_INFORMATION hinzugefügt. Dadurch können Benutzer mit der Berechtigung Prioritäten und Budgetzeiten im Planer bearbeiten.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

Ein ReservedTime -Objekt stellt Tage dar, die in der persönlichen Zeit eines Benutzers angegeben sind und angeben, dass der Benutzer nicht zur Arbeit verfügbar sein wird.

Die Ressource ReservedTime hat das Flag REPORTABLE hinzugefügt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder haben das Flag NOT_GROUPABLE entfernt.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>Das folgende Feld wurde aus dem ReservedTime -Objekt entfernt.</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Aufgabe</p> <p style="font-weight: normal;">Entfernt  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Vorgänge</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>BEARBEITEN</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

Ein ResourcePlannerFilter -Objekt ist ein Regelsatz, der bestimmt, welche Elemente im Ressourcenplaner angezeigt werden.

Die Ressource ResourcePlannerFilter hat das Flag SHARABLE hinzugefügt. Es wurden keine anderen Änderungen am Objekt vorgenommen.

### Risiko {#risk}

Ein Risikoobjekt stellt ein mögliches Ereignis dar, das verhindern kann, dass ein Projekt rechtzeitig oder innerhalb des Budgets beendet wird. In der Planungsphase werden den Projekten Risiken hinzugefügt, um potenzielle Hindernisse vor der Genehmigung von Arbeiten zu ermitteln.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Dem Risikoobjekt wurden die folgenden Felder hinzugefügt:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enterByID</p> <p style="font-weight: normal;">Die ID des Benutzers, der das Objekt ursprünglich erstellt hat.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Das Datum, an dem ein Objekt von einem Benutzer in Workfront übermittelt wurde.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Der Parameter Letztes Aktualisierungsdatum gibt das Datum zurück, an dem die letzte Aktualisierung an einem Objekt vorgenommen wurde.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>"Zuletzt aktualisiert von ID"ist ein Parameter, der die Benutzer-ID des letzten Benutzers zurückgibt, der das Objekt aktualisiert hat.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> <p style="font-weight: normal;">Die folgenden Referenzfelder wurden dem RIsk-Objekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">enterBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Ein ScheduledReport -Objekt stellt einen Bericht dar, der für die Bereitstellung konfiguriert wurde.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Ein ScoreCardQuestion -Objekt stellt eine Frage dar, die einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfolio-Manager bestimmt und ihre Antworten ermöglichen es dem Manager zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Möglicher Wert TYAH (Typahead) hinzugefügt  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aufgabe {#task}

Ein Task -Objekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (zum Abschließen eines Projekts) ausgeführt werden muss.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">In den folgenden Feldern wurden die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Werte geben an, dass Daten für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach dem Jahr 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">IststartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zur öffentlichen API hinzugefügt, um Transparenz bei der Berechnung von EAC (Schätzung bei Abschluss) zu gewährleisten.</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Die auch als Earned Value (Earned Value, Earned Value, Budgeted Cost of Work Performed, BCWP) bezeichnete Metrik zur Projektleistung, die die budgetierten Kosten der zum Zeitpunkt der Berechnung dieser Metrik tatsächlich abgeschlossenen Aufgabe darstellt. Bei Aufgaben: BCWP = Tatsächlicher Prozentsatz der Vollständigkeit x Aufgabenbudget. Bei Projekten: BCWP = SUM(BCWP-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Die auch als "Geplanter Wert"bekannten budgetierten Kosten für geplante Arbeit (BCWS) sind eine Metrik zur Projektleistung, die die geplanten Kosten der Aufgabenmenge darstellt, die zum Zeitpunkt der Berechnung dieser Metrik abgeschlossen sein sollten. Für Aufgaben: BCWS = Geplanter Prozentsatz Abgeschlossen x Aufgabenbudget. Bei Projekten BCWS = SUM(BCWS-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
    </ul><p style="font-weight: normal;">Die folgenden Felder haben den möglichen Wert ET hinzugefügt. Dieser Wert stellt die Zeiteinheit der verstrichenen Monate dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde aus dem Task-Objekt entfernt.</p>
    <ul>
     <li style="font-weight: bold;">preserveTimeID</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde dem Task-Objekt hinzugefügt.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>preserveTime</p> <p style="font-weight: normal;">Entfernt  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

Ein Team-Objekt ist eine Sammlung von Benutzern, die einem Arbeitselement zugewiesen werden können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Dieses Feld wurde dem Team-Objekt hinzugefügt. Der Agile Estimate-Typ bestimmt, wie die Arbeitslast einer Geschichte geschätzt wird. Wenn die Anzahl in Stunden geschätzt wird, dann ist dies die Anzahl der geplanten Stunden, die der Story hinzugefügt werden. Wenn der Wert in Punkte geschätzt wird, fügt jeder Punkt eine Anzahl von geplanten Stunden zur Story hinzu, basierend darauf, wie die Punkte festgelegt werden (standardmäßig 8 Stunden). Mögliche Werte für den Agile Estimate Type sind:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (Story Points)</li> 
       <li style="font-weight: normal;">STUNDEN (Stunden)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (Stunden als Punkte)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Vorlage {#template}

Ein Template -Objekt stellt ein Muster für ein Projekt dar. Projekte können aus Vorlagen erstellt werden, um Zeit zu sparen. Eine Vorlage enthält ein Team und Aufgaben , die bei Verwendung der Vorlage in ein Projekt kopiert werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt. Es ist ein boolescher Parameter, der den Wert true hat, wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden. Objekte, die nicht auf "Aktiv"gesetzt sind, sind nicht in Dropdown-Menüs und Typvorlagenfeldern sichtbar, die an andere Objekte angehängt werden sollen.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPrioritäten</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateAssignment {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">Der mögliche Wert ET wurde hinzugefügt. Dieser Wert stellt die Zeiteinheit der verstrichenen Monate dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Ein TemplateTask -Objekt stellt eine Aufgabe dar, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, in dem die Vorlage verwendet wird.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p style="font-weight: normal;">Die folgenden Felder haben den möglichen Wert ET hinzugefügt. Dieser Wert stellt die Zeiteinheit der verstrichenen Monate dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPrioritäten</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbeitszeittabelle {#timesheet}

Ein Timesheet-Objekt stellt eine virtuelle Timecard dar, mit der Benutzer die tatsächlichen Arbeitsstunden für Aufgaben, Projekte und Hochtypen eingeben können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Kernfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">Entfernt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aktualisieren {#update}

Arbeitselemente in Workfront können aktualisiert werden, um die Benutzer über den aktuellen Status auf dem Laufenden zu halten. Ein Update -Objekt stellt eine dieser Aktualisierungen dar. Aktualisierungen können von Benutzern eingegeben oder vom Workfront-System erstellt werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Der mögliche Wert referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata) wurde hinzugefügt.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Abfragen</td> 
   <td> <p style="font-weight: normal;">Die folgenden Abfragen wurden dem Update -Objekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p style="font-weight: normal;">Dem User -Objekt wurden die folgenden Aktionen hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Abfragen</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p style="font-weight: normal;">Dem User -Objekt wurden die folgenden Aktionen hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledged.</li> 
     <li style="font-weight: bold;">unacknowledged  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Abfragen</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbeit  {#work}

Ein Work-Objekt ist eine gemeinsame Schnittstelle, die sowohl von Task als auch von OpTask übernommen wird und gemeinsamen Code für beide verwendet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">In den folgenden Feldern wurden die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Werte geben an, dass Daten für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach dem Jahr 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">effectiveCompletionDate</li>
     <li style="font-weight: bold;">IststartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zur öffentlichen API hinzugefügt, um Transparenz bei der Berechnung von EAC (Schätzung bei Abschluss) zu gewährleisten.</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Die auch als Earned Value (Earned Value, Earned Value, Budgeted Cost of Work Performed, BCWP) bezeichnete Metrik zur Projektleistung, die die budgetierten Kosten der zum Zeitpunkt der Berechnung dieser Metrik tatsächlich abgeschlossenen Aufgabe darstellt. Bei Aufgaben: BCWP = Tatsächlicher Prozentsatz der Vollständigkeit x Aufgabenbudget. Bei Projekten: BCWP = SUM(BCWP-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Die auch als "Geplanter Wert"bekannten budgetierten Kosten für geplante Arbeit (BCWS) sind eine Metrik zur Projektleistung, die die geplanten Kosten der Aufgabenmenge darstellt, die zum Zeitpunkt der Berechnung dieser Metrik abgeschlossen sein sollten. Für Aufgaben: BCWS = Geplanter Prozentsatz Abgeschlossen x Aufgabenbudget. Bei Projekten BCWS = SUM(BCWS-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
    </ul><p style="font-weight: normal;">Die folgenden Felder haben den möglichen Wert ET hinzugefügt. Dieser Wert stellt die Zeiteinheit der verstrichenen Monate dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde aus dem Work -Objekt entfernt.</p>
    <ul>
     <li style="font-weight: bold;">preserveTimeID</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde dem Work-Objekt hinzugefügt.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>preserveTime</p> <p style="font-weight: normal;">Entfernt  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
