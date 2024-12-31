---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 11
description: ReportBudgedHour wurde zur Adobe Workfront-API als Ressource für das Reporting hinzugefügt. Es enthält Referenzfelder, Kernfelder und Standardfelder, die in BudgetedHour nicht vorhanden sind.
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '3573'
ht-degree: 2%

---

# Neue Funktionen in der API-Version 11

* [Ressourcen hinzugefügt](#added-resources)
* [Entfernte Ressourcen](#removed-resources)
* [Geänderte Ressourcen](#modified-resources)

## Ressourcen hinzugefügt {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableBudgetedHour](#reportablebudgetedhour)

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
     <li style="font-weight: bold;">Kunde</li> 
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
     <li style="font-weight: bold;">Kunde  </li> 
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
     <li style="font-weight: bold;">restrictionsLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">Kunde  </li> 
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

### ReportableBudgetedHour {#reportablebudgetedhour}

ReportBudgedHour wurde zur Adobe Workfront-API als Ressource für das Reporting hinzugefügt. Es enthält Referenzfelder, Kernfelder und Standardfelder, die in BudgetedHour nicht vorhanden sind.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>Das Zuteilungsdatum ist der erste Tag (ein Sonntag) der Woche, für die Sie die Stunden im Ressourcenplaner budgetiert haben.</p> </li> 
     <li> <p style="font-weight: bold;">budgetierte Stunden </p> <p>Budgetierte Stunden sind Stunden, die der Ressourcen-Manager für die Arbeit budgetiert, die Ressourcen für Projekte ausführen müssen</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>Die eindeutige Workfront-ID, die einem bestimmten berichtspflichtigen budgetierten Stundenobjekt zugewiesen ist.</p> </li> 
     <li style="font-weight: bold;">geplante budgetierte Stunden </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>Die eindeutige Workfront-ID, die einem bestimmten Projekt zugewiesen ist.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>Die eindeutige Workfront-ID, die einem bestimmten Aufgabengebiet zugewiesen ist.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>Die eindeutige Workfront-ID, die einem bestimmten Benutzer zugewiesen ist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">Projekt</p> <p>Das Projekt, dem eine ReportBudgetedHour zugeordnet ist.</p> </li> 
     <li> <p style="font-weight: bold;">Rolle</p> <p>Das Aufgabengebiet, dem eine ReportBudgetedHour zugeordnet ist.</p> </li> 
     <li> <p style="font-weight: bold;">Benutzer</p> <p>Der Benutzer, dem eine ReportBudgetedHour zugeordnet ist.</p> </li> 
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
     <li style="font-weight: bold;">ANZAHL</li> 
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
     <li><a href="#accesslevelpermissions" class="MCXref xref">Zugriffsberechtigungen</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">Zugriffsregel</a> </li> 
     <li><a href="#approval" class="MCXref xref">Genehmigung</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">Genehmigungsprozess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Zuweisung</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">BaselineTask</a> </li> 
     <li><a href="#category" class="MCXref xref">Kategorie</a> </li> 
     <li><a href="#company" class="MCXref xref">Firma</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Kunde</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">Kundenpräferenzen</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Dokument</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Iteration</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Layoutvorlage</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">Hinweis</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parameter</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio </a> </li> 
     <li><a href="#program" class="MCXref xref">Programm</a> </li> 
     <li><a href="#project" class="MCXref xref">Projekt</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">TestversandValidierung</a> </li> 
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
     <li><a href="#work" class="MCXref xref"></a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### ZugriffsebeneBerechtigungen {#accesslevelpermissions}

Ein AccessLevelPermissions-Objekt stellt einen Berechtigungssatz dar. Dieser Berechtigungssatz kann dann mit einer Zugriffsebene verknüpft werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder haben den möglichen Wert BUDGETING_INFORMATION hinzugefügt. Dies ermöglicht es Benutzenden mit der Berechtigung, Prioritäten und Budgetstunden im Planer zu bearbeiten.</p> 
    <ul> 
     <li style="font-weight: bold;">CoreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">sekundäre Aktionen  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Zugriffsanforderung {#accessrequest}

Wenn ein(e) Benutzende(r) keinen Zugriff auf ein Objekt in Workfront hat, das er/sie benötigt, kann er/sie Zugriff auf dieses Objekt anfordern. Das AccessRequest-Objekt stellt diese Anforderung dar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">Handlung</p> <p>Der mögliche Wert BUDGETING_INFORMATION wurde hinzugefügt. Dies ermöglicht es Benutzenden mit der Berechtigung, Prioritäten und Budgetstunden im Planer zu bearbeiten.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Zugriffsregel {#accessrule}

Ein AccessRule-Objekt stellt einen Regelsatz in benutzerdefinierten Zugriffsebenen dar, der bestimmt, wie Benutzer erstellte Projekte freigeben können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder haben den möglichen Wert BUDGETING_INFORMATION hinzugefügt. Dies ermöglicht es Benutzenden mit der Berechtigung, Prioritäten und Budgetstunden im Planer zu bearbeiten.</p> 
    <ul> 
     <li style="font-weight: bold;">CoreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">sekundäre Aktionen  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Genehmigung {#approval}

Für ein bestimmtes Arbeitselement, z. B. eine Aufgabe, ein Dokument oder eine Arbeitszeittabelle, kann es erforderlich sein, dass ein Verantwortlicher oder ein anderer Benutzer das Arbeitselement abzeichnet. Ein Validierungsobjekt stellt die Aktion des Abzeichnens eines Arbeitselements dar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">Die folgenden Felder haben die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Validatoren geben an, dass Datumsangaben für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zur öffentlichen API hinzugefügt, um die Berechnung der BK (Schätzung bei Abschluss) transparenter zu gestalten.</p>
    <ul>
     <li><p style="font-weight: bold;">BCWP</p><p style="font-weight: normal;">Die budgetierten Kosten der geleisteten Arbeit (BCWP), auch als Ertragswert bezeichnet, sind eine Projektleistungskennzahl, die die budgetierten Kosten des Betrags der Aufgabe darstellt, der zum Zeitpunkt der Berechnung dieser Kennzahl tatsächlich abgeschlossen wurde. Für Aufgaben: SKAA = Tatsächlicher Prozentsatz der Fertigstellung x Aufgabenbudget. Für Projekte: BCWP = SUM(BCWP-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
     <li><p style="font-weight: bold;">BCWS</p><p style="font-weight: normal;">Die budgetierten Kosten der geplanten Arbeit (BCWS), auch als Geplanter Wert bezeichnet, sind eine Projektleistungskennzahl, die die budgetierten Kosten des Betrags der Aufgabe darstellt, der zum Zeitpunkt der Berechnung dieser Kennzahl hätte abgeschlossen sein sollen. Für Aufgaben: BCWS = Geplanter Prozentsatz der Fertigstellung x Aufgabenbudget. Für Projekte: BCWS = SUM(BCWS-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
    </ul><p style="font-weight: normal;">Die folgenden Felder haben den möglichen Wert ET hinzugefügt. Dieser Wert stellt die Einheit der verstrichenen Zeit in Monaten dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">WorkUnit</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder haben das Flag WÄHRUNG hinzugefügt</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden aus dem Genehmigungsobjekt entfernt.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde zum Genehmigungsobjekt hinzugefügt.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservierteZeit</p> <p style="font-weight: normal;">Aus dem Genehmigungsobjekt entfernt  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">hat zum Genehmigungsobjekt hinzugefügt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

Ein ApprovalPath-Objekt ist eine Verzweigung innerhalb eines Genehmigungsprozesses. Genehmigungspfade basieren auf dem Status des Objekts, mit dem der Genehmigungsprozess verknüpft ist.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Hinzugefügt den möglichen Wert ET. Dieser Wert stellt die Einheit der verstrichenen Zeit in Monaten dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Genehmigungsprozess {#approvalprocess}

Ein Validierungsprozess-Objekt ist eine mehrstufige Validierung, die mit einem Projekt, einer Aufgabe oder einem Problem verknüpft werden kann.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt aktiv ist, und „false“, wenn dies nicht der Fall ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden. Objekte, für die nicht „Aktiv“ festgelegt ist, werden nicht in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt, um sie an andere Objekte anzuhängen.  </p> </li> 
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
     <li style="font-weight: bold;"> <p>WorkUnit </p> <p style="font-weight: normal;">Hinzugefügt den möglichen Wert ET. Dieser Wert stellt die Einheit der verstrichenen Zeit in Monaten dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Baseline-Aufgabe {#baselinetask}

Baselines sind Momentaufnahmen der Leistung eines Projekts zu einem bestimmten Zeitpunkt. Sie speichern wichtige Informationen über das Projekt, wie wichtige Daten, Fortschritt, Kosten und Umsatzwerte. Wenn Sie eine Baseline erstellen, werden die Aufgabeninformationen auch in den Baseline-Aufgaben dieser Baseline erfasst.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Hinzugefügt den möglichen Wert ET. Dieser Wert stellt die Einheit der verstrichenen Zeit in Monaten dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kategorie {#category}

Ein Kategorieobjekt ist ein benutzerdefiniertes Formular. Sie können Berichte für dieses Objekt erstellen und sie auch in anderen Objektberichten anzeigen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt aktiv ist, und „false“, wenn dies nicht der Fall ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden. Objekte, für die nicht „Aktiv“ festgelegt ist, werden nicht in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt, um sie an andere Objekte anzuhängen.  </p> </li> 
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

Ein Unternehmensobjekt stellt eine Organisation dar, die aus einer Sammlung von Personen besteht. Firmen sind mit einem Benutzer oder einem Projekt verknüpft.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt aktiv ist, und „false“, wenn dies nicht der Fall ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden. Objekte, für die nicht „Aktiv“ festgelegt ist, werden nicht in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt, um sie an andere Objekte anzuhängen.  </p> </li> 
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

### Benutzerdefinierte Enumeration {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p style="font-weight: normal;">Die folgenden Aktionen wurden zum CustomEnum-Objekt hinzugefügt</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Abfragen</td> 
   <td> <p>Die folgenden Abfragen wurden zum CustomEnum-Objekt hinzugefügt</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kunde {#customer}

Ein Customer-Objekt stellt eine Organisation dar, die eine Instanz von Workfront verwendet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Hinzugefügte mögliche Werte: </p> 
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
   <td> <p style="font-weight: normal;">Die folgenden Aktionen wurden zum Customer-Objekt hinzugefügt</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kundenpräferenzen {#customerpreferences}

Ein CustomerPreferences-Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Workfront-Instanz festgelegt hat.

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
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Hinzugefügte mögliche Werte:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Anforderungen an die Kennwortkomplexität)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (Mindestlänge des Kennworts)</li> 
       <li style="font-weight: normal;">password:mobile Sitzungszeitüberschreitung (Zeitüberschreitung bei mobilen Sitzungen)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (Benutzer-Ausfallzeit)</li> 
       <li style="font-weight: normal;">Arbeitszeittabelle:default.timesheet.manualrole (manuelle Kontrollrolle)</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole (config.proofhq.defaultNonRecipientRole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole (config.proofhq.defaultNonRecipientGuestRole)  </li> 
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

Ein Dokumentobjekt, das eine Datei darstellt (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p>Die folgenden Aktionen wurden zum Dokumentobjekt hinzugefügt.</p> 
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

Ein Iterationsobjekt stellt eine einzelne Agile-Iteration dar. Iterationen sind diskrete Zeiträume, in denen agile Storys geplant und abgeschlossen werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder wurden zum Iterationsobjekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">Abgeschlossene Punkte</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Layoutvorlage {#layout-template}

Ein Layout-Vorlagenobjekt stellt eine bestimmte Anordnung von Layout-Elementen dar, z. B. das Hauptmenü, den Navigationsbereich oder den Home-Bereich. Layout-Vorlagen können Benutzern, Teams, Gruppen oder Aufgabengebieten zugewiesen werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und ist ein boolescher Parameter mit dem Wert „true“, wenn eine Layout-Vorlage so eingestellt ist, dass Zeitstempel für Fälligkeitsdaten in der Arbeitsliste und im Kalender angezeigt werden, und „false“, wenn Zeitstempel ausgeblendet werden sollen.  </p> </li> 
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

### Meilensteinpfad {#milestonepath}

Ein Meilenstein ist eine Markierung auf einer Aufgabe, die darauf hinweist, dass es sich um einen Schlüsselpunkt im Projekt handelt. Wird im Allgemeinen verwendet, um ein wichtiges Ereignis zu kennzeichnen, z. B. den Abschluss einer Projektphase oder einer Reihe kritischer Aktivitäten. Ein MilestonePath-Objekt ist eine Sammlung von Meilensteinen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt aktiv ist, und „false“, wenn dies nicht der Fall ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden. Objekte, für die nicht „Aktiv“ festgelegt ist, werden nicht in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt, um sie an andere Objekte anzuhängen.  </p> </li> 
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

Ein Notizobjekt ist ein Kommentar oder eine Aktualisierung eines Workfront-Objekts.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder wurden zum Notizobjekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">Korrekturabzug-ID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>„Likes“</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Ein OpTask-Objekt wird im Allgemeinen als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise darauf hinweist, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungsanforderungen, -anfragen und -fehler sind ebenfalls Probleme.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">Die folgenden Felder haben die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Validatoren geben an, dass Datumsangaben für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zu OpTask hinzugefügt.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">Die eindeutige Workfront-ID eines Kanban-Board-Objekts.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Prozent abgeschlossen ist ein Parameter, der den abgeschlossenen Betrag eines Problems in Prozent zurückgibt.</p></li>
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
     <li style="font-weight: bold;"> <p>Arbeit</p> <p style="font-weight: normal;">entfernt</p> </li> 
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
   <td> <p>Die folgenden Aktionen wurden zum OpTask-Objekt hinzugefügt</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">Anfrage kopieren</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

Ein Parameter-Objekt ist ein benutzerdefiniertes Feld.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Der mögliche Wert wurde TYAH (typeahead) hinzugefügt.</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und verweist auf den Objekt-Code eines referenzierten Objekts. Objektcodes für alle Objekte finden Sie im <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Ein Portfolio-Objekt ist eine Sammlung von Projekten, die um dieselben Ressourcen konkurrieren, normalerweise Geld oder Personen, um sie abzuschließen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Beschreibung</p> <p style="font-weight: normal;">Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass die Beschreibung nicht länger als 4.000 Zeichen ist.</p> </li> 
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
     <li style="font-weight: bold;"> <p>Beschreibung</p> <p style="font-weight: normal;">Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass die Beschreibung nicht länger als 4.000 Zeichen ist.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt aktiv ist, und „false“, wenn dies nicht der Fall ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden. Objekte, für die nicht „Aktiv“ festgelegt ist, werden nicht in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt, um sie an andere Objekte anzuhängen.  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass der Name nicht länger als 255 Zeichen ist.  </p> </li> 
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

Projekte sind Arbeitselemente innerhalb von Workfront und ein wichtiger Baustein in der Art und Weise, wie Workfront Menschen bei der Arbeit unterstützt. Ein Project-Objekt stellt eine Gruppe von Aufgaben mit einem gemeinsamen, spezifischen Ziel dar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">Die folgenden Felder haben die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Validatoren geben an, dass Datumsangaben für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zur öffentlichen API hinzugefügt, um die Berechnung der BK (Schätzung bei Abschluss) transparenter zu gestalten.</p>
    <ul>
     <li><p style="font-weight: bold;">BCWP</p><p style="font-weight: normal;">Die budgetierten Kosten der geleisteten Arbeit (BCWP), auch als Ertragswert bezeichnet, sind eine Projektleistungskennzahl, die die budgetierten Kosten des Betrags der Aufgabe darstellt, der zum Zeitpunkt der Berechnung dieser Kennzahl tatsächlich abgeschlossen wurde. Für Aufgaben: SKAA = Tatsächlicher Prozentsatz der Fertigstellung x Aufgabenbudget. Für Projekte: BCWP = SUM(BCWP-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
     <li><p style="font-weight: bold;">BCWS</p><p style="font-weight: normal;">Die budgetierten Kosten der geplanten Arbeit (BCWS), auch als Geplanter Wert bezeichnet, sind eine Projektleistungskennzahl, die die budgetierten Kosten des Betrags der Aufgabe darstellt, der zum Zeitpunkt der Berechnung dieser Kennzahl hätte abgeschlossen sein sollen. Für Aufgaben: BCWS = Geplanter Prozentsatz der Fertigstellung x Aufgabenbudget. Für Projekte: BCWS = SUM(BCWS-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
    </ul><p style="font-weight: normal;">Die folgenden Felder haben das Flag WÄHRUNG hinzugefügt</p>
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

### Testversandvalidierung {#proofapproval}

Ein ProofApproval-Objekt stellt eine Genehmigung dar, die direkt mit einem Korrekturabzug verbunden ist.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitDecision</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und ist ein boolescher Parameter mit dem Wert „true“, wenn ein Korrekturabzug auf eine Entscheidung wartet, und „false“, wenn dies nicht der Fall ist.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Ein QueueDef -Objekt stellt eine Warteschlange dar. Dabei handelt es sich um ein Projekt, das im Helpdesk-Bereich veröffentlicht wurde, um Benutzenden die Übermittlung von Problemen zu ermöglichen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder haben den möglichen Wert BUDGETING_INFORMATION hinzugefügt. Dies ermöglicht es Benutzenden mit der Berechtigung, Prioritäten und Budgetstunden im Planer zu bearbeiten.</p> 
    <ul> 
     <li style="font-weight: bold;">RequestorCoreAction</li> 
     <li style="font-weight: bold;">RequestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

Ein ReservedTime -Objekt stellt Tage dar, die für die persönliche Zeit eines Benutzers angegeben sind, was bedeutet, dass der Benutzer nicht für Arbeiten zur Verfügung steht.

Die ReservedTime -Ressource hat das Flag REPORTABLE hinzugefügt.

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
     <li style="font-weight: bold;"> <p>Aufgabe</p> <p style="font-weight: normal;">entfernt  </p> </li> 
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

Ein ResourcePlannerFilter-Objekt ist ein Regelsatz, der bestimmt, welche Elemente im Ressourcenplaner angezeigt werden.

Die ResourcePlannerFilter-Ressource hat das Flag SHARABLE hinzugefügt. Andere Änderungen am Objekt wurden nicht vorgenommen.

### Risiko {#risk}

Ein Risikoobjekt stellt ein mögliches Ereignis dar, das verhindern kann, dass ein Projekt termingerecht oder innerhalb des Budgets abgeschlossen wird. Projekte werden in der Planungsphase mit Risiken versehen, um potenzielle Hindernisse vor der Genehmigung von Arbeiten zu identifizieren.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p>Die folgenden Felder wurden zum Objekt Risiko hinzugefügt:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">Die ID des Benutzers, der das Objekt ursprünglich erstellt hat.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>Das Datum, an dem ein Objekt von einem Benutzer in Workfront übermittelt wurde.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Der Parameter Letztes Aktualisierungsdatum gibt das Datum zurück, an dem die letzte Aktualisierung an einem Objekt vorgenommen wurde.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>„Zuletzt aktualisiert von ID“ ist ein Parameter, der die Benutzer-ID des letzten Benutzers zurückgibt, der das Objekt aktualisiert hat.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> <p style="font-weight: normal;">Die folgenden Referenzfelder wurden zum Risikoobjekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Geplanter Bericht {#scheduledreport}

Ein ScheduledReport-Objekt stellt einen Bericht dar, der für die Bereitstellung geplant wurde.

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

Ein ScoreCardQuestion-Objekt stellt eine Frage dar, die zu einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfoliomanager bestimmt und ihre Antworten geben dem Portfolio die Möglichkeit zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Der mögliche Wert wurde hinzugefügt: TAH (typeahead)  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aufgabe {#task}

Ein Aufgabenobjekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (Fertigstellen eines Projekts) ausgeführt werden muss.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">Die folgenden Felder haben die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Validatoren geben an, dass Datumsangaben für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zur öffentlichen API hinzugefügt, um die Berechnung der BK (Schätzung bei Abschluss) transparenter zu gestalten.</p>
    <ul>
     <li><p style="font-weight: bold;">BCWP</p><p style="font-weight: normal;">Die budgetierten Kosten der geleisteten Arbeit (BCWP), auch als Ertragswert bezeichnet, sind eine Projektleistungskennzahl, die die budgetierten Kosten des Betrags der Aufgabe darstellt, der zum Zeitpunkt der Berechnung dieser Kennzahl tatsächlich abgeschlossen wurde. Für Aufgaben: SKAA = Tatsächlicher Prozentsatz der Fertigstellung x Aufgabenbudget. Für Projekte: BCWP = SUM(BCWP-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
     <li><p style="font-weight: bold;">BCWS</p><p style="font-weight: normal;">Die budgetierten Kosten der geplanten Arbeit (BCWS), auch als Geplanter Wert bezeichnet, sind eine Projektleistungskennzahl, die die budgetierten Kosten des Betrags der Aufgabe darstellt, der zum Zeitpunkt der Berechnung dieser Kennzahl hätte abgeschlossen sein sollen. Für Aufgaben: BCWS = Geplanter Prozentsatz der Fertigstellung x Aufgabenbudget. Für Projekte: BCWS = SUM(BCWS-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
    </ul><p style="font-weight: normal;">Die folgenden Felder haben den möglichen Wert ET hinzugefügt. Dieser Wert stellt die Einheit der verstrichenen Zeit in Monaten dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">WorkUnit</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde aus dem Objekt Aufgabe entfernt.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde zum Objekt Aufgabe hinzugefügt.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservierteZeit</p> <p style="font-weight: normal;">entfernt  </p> </li> 
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
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">Dieses Feld wurde dem Team -Objekt hinzugefügt. Der Agile-Schätztyp bestimmt, wie die Arbeitslast einer Story geschätzt wird. Bei einer Schätzung in Stunden ist dies die Anzahl der geplanten Stunden, die der Story hinzugefügt werden. Bei einer Schätzung in Punkten addiert jeder Punkt die Anzahl der geplanten Stunden zur Story, je nachdem, wie die Punkte festgelegt sind (der Standardwert ist 8 Stunden). Mögliche Werte für den Agile-Schätzungstyp sind:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (Story-Punkte)</li> 
       <li style="font-weight: normal;">STUNDEN (hours)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (Stunden als Punkte)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Vorlage {#template}

Ein Vorlagenobjekt stellt ein Muster für ein Projekt dar. Projekte können aus Vorlagen erstellt werden, um Zeit zu sparen. Eine Vorlage enthält ein Team und Aufgaben, die bei Verwendung der Vorlage in ein Projekt kopiert werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Dieses Feld wurde hinzugefügt und ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt aktiv ist, und „false“, wenn dies nicht der Fall ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden. Objekte, für die nicht „Aktiv“ festgelegt ist, werden nicht in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt, um sie an andere Objekte anzuhängen.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Alle Prioritäten</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
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

### Vorlagenzuweisung {#templateassignment}

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
     <li style="font-weight: bold;"> <p>WorkUnit</p> <p style="font-weight: normal;">Hinzugefügt den möglichen Wert ET. Dieser Wert stellt die Einheit der verstrichenen Zeit in Monaten dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Vorlagenaufgabe {#templatetask}

Ein TemplateTask-Objekt stellt eine Aufgabe dar, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, in dem die Vorlage verwendet wird.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p style="font-weight: normal;">Die folgenden Felder haben den möglichen Wert ET hinzugefügt. Dieser Wert stellt die Einheit der verstrichenen Zeit in Monaten dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">WorkUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Alle Prioritäten</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbeitszeittabelle {#timesheet}

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Kernfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">entfernt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aktualisieren {#update}

Arbeitselemente in Workfront können aktualisiert werden, um Benutzende über den aktuellen Status zu informieren. Ein Update -Objekt stellt eine dieser Aktualisierungen dar. Aktualisierungen können von Benutzenden eingegeben oder vom Workfront-System erstellt werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Der mögliche Wert referenceObjectCustomData (enum.updateTypeEnum.referenceObjectCustomData) wurde hinzugefügt.  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Abfragen</td> 
   <td> <p style="font-weight: normal;">Die folgenden Abfragen wurden zum Aktualisierungsobjekt hinzugefügt.</p> 
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
   <td> <p style="font-weight: normal;">Die folgenden Aktionen wurden zum Benutzerobjekt hinzugefügt.</p> 
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
   <td> <p style="font-weight: normal;">Die folgenden Aktionen wurden zum Benutzerobjekt hinzugefügt.</p> 
    <ul> 
     <li style="font-weight: bold;">confirmMyNotifications</li> 
     <li style="font-weight: bold;">unknownAllObjectsTypeCount  </li> 
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

Ein Arbeitsobjekt ist eine gemeinsame Schnittstelle, die sowohl von Task als auch von OpTask erbt wird und gemeinsamen Code zwischen den beiden verwendet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direkte Felder<p style="font-weight: normal;">Die folgenden Felder haben die Validatoren AT_DATE_BEFORE_YEAR und AT_DATE_AFTER_YEAR hinzugefügt. Diese Validatoren geben an, dass Datumsangaben für verknüpfte Objekte nicht vor dem Jahr 1900 oder nach 2200 festgelegt werden können.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">scheduledCompletionDate</li>
     <li style="font-weight: bold;">scheduledStartDate</li>
    </ul><p style="font-weight: normal;">Die folgenden Felder wurden zur öffentlichen API hinzugefügt, um die Berechnung der BK (Schätzung bei Abschluss) transparenter zu gestalten.</p>
    <ul>
     <li><p style="font-weight: bold;">BCWP</p><p style="font-weight: normal;">Die budgetierten Kosten der geleisteten Arbeit (BCWP), auch als Ertragswert bezeichnet, sind eine Projektleistungskennzahl, die die budgetierten Kosten des Betrags der Aufgabe darstellt, der zum Zeitpunkt der Berechnung dieser Kennzahl tatsächlich abgeschlossen wurde. Für Aufgaben: SKAA = Tatsächlicher Prozentsatz der Fertigstellung x Aufgabenbudget. Für Projekte: BCWP = SUM(BCWP-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
     <li><p style="font-weight: bold;">BCWS</p><p style="font-weight: normal;">Die budgetierten Kosten der geplanten Arbeit (BCWS), auch als Geplanter Wert bezeichnet, sind eine Projektleistungskennzahl, die die budgetierten Kosten des Betrags der Aufgabe darstellt, der zum Zeitpunkt der Berechnung dieser Kennzahl hätte abgeschlossen sein sollen. Für Aufgaben: BCWS = Geplanter Prozentsatz der Fertigstellung x Aufgabenbudget. Für Projekte: BCWS = SUM(BCWS-Werte aller übergeordneten und einzelnen Aufgaben).</p></li>
    </ul><p style="font-weight: normal;">Die folgenden Felder haben den möglichen Wert ET hinzugefügt. Dieser Wert stellt die Einheit der verstrichenen Zeit in Monaten dar, die sich auf Monate ohne Berücksichtigung von Wochenenden oder Feiertagen bezieht.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">WorkUnit</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde aus dem Arbeitsobjekt entfernt.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">Das folgende Feld wurde zum Arbeitsobjekt hinzugefügt.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservierteZeit</p> <p style="font-weight: normal;">entfernt  </p> </li> 
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
