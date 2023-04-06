---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 13
description: Adobe Workfront hat die API-Version 13 am 22. April 2021 veröffentlicht. API Version 13 enthält die folgenden Änderungen gegenüber Version 12.
author: Becky
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 1ea7e1a0435e9d199c3d828723d11ce530a80540
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# Neue Funktionen in API Version 13

Adobe Workfront hat die API-Version 13 am 22. April 2021 veröffentlicht. API Version 13 enthält die folgenden Änderungen gegenüber Version 12.

## Hinzugefügte Ressourcen

Für API Version 13 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API Version 13 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen

Die folgenden Ressourcen wurden für API Version 13 geändert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Gruppe </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Projekt</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">TestversandApproval</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Aufgabe</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Arbeitszeittabelle</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">TimesheetProfile</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelegation</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Arbeit </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

Ein AccessLevel -Objekt ist mit Benutzern verknüpft und beschreibt den Satz von AccessLevelPermissions, der bestimmt, auf welchen Benutzer zugreifen können.

Weitere Informationen zu Zugriffsebenen finden Sie unter [Funktionsweise von Zugriffsstufen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Beschreibung</b> </p> <p>Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass die Länge der Beschreibung nicht mehr als 4000 Zeichen beträgt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

Ein BreadCrumb-Objekt stellt ein Element in der übergeordneten/untergeordneten Hierarchie eines Workfront-Arbeitselements dar. Breadcrumbs zeigen an, wie ein Arbeitselement in die größere Struktur von Portfolios, Projekten, Projekten und Aufgaben passt.

Weitere Informationen zu Breadcrumbs finden Sie unter [Breadcrumbs-Übersicht im neuen Adobe Workfront-Erlebnis](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Objektcodes finden Sie im <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

Ein BurndownEvent -Objekt stellt ein Objekt dar, das das Bundle einer Iteration ändert.

Weitere Informationen zum Burndown finden Sie unter [Niederschlag](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> <p>Die folgenden Felder haben das Flag NOT_GROUPABLE entfernt </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

Ein CustomerPreferences -Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Instanz von Workfront festgelegt hat.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Mögliche Werte wurden hinzugefügt:</p> 
      <ul> 
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.limit.timesheet.edit.owner.admins (config.timesheet.restricted.timesheet.edit.owner.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p>Die folgenden Aktionen wurden der Ressource CustomerPreferences hinzugefügt.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Nimmt das Argument:</p> 
      <ul> 
       <li> <p>Voreinstellungen (map)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Ein DocumentVersion -Objekt stellt eine bestimmte Version einer Datei dar (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

Weitere Informationen zu Dokumentversionen finden Sie unter [Eine neue Version eines Dokuments hochladen](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Möglicher Wert hinzugefügt:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Flag NOT_FILTERABLE hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppe  {#group}

Ein Group -Objekt stellt eine Gruppe von Benutzern und Teams dar. Gruppen stellen oft die Struktur der Abteilungen dar.

Weitere Informationen zu Gruppen finden Sie unter [Gruppen vs. Teams in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Aktionen</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Diese Aktion gibt ein Array der übergeordneten Gruppen der Gruppe zurück (Gruppen, zu denen die angegebene Gruppe gehört).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

Das JournalEntry -Objekt kann so eingerichtet werden, dass bei jeder Änderung dieser Felder Informationen über bestimmte Objektfelder protokolliert werden. Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird bei jeder Änderung dieses Felds ein entsprechender Journaleintrag erstellt.

Die Ressource JournalEntry hat das Flag REPORTABLE hinzugefügt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> <p>Die folgenden Felder haben das Flag NOT_GROUPABLE entfernt:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>Die folgenden Felder haben das Flag NOT_FILTERABLE hinzugefügt:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Adobe Workfront-Administratoren oder Gruppenadministratoren können Vorlagen erstellen, um die Layoutelemente in Adobe Workfront anzupassen. Das LayoutTemplate-Objekt ist spezifisch für Adobe Workfront Classic.

Informationen zu dem Objekt, das Layoutvorlagen im neuen Adobe Workfront-Erlebnis darstellt, finden Sie unter [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Beschreibung</b> </p> <p>Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass die Länge der Beschreibung nicht mehr als 4000 Zeichen beträgt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Ein LinkedFolder-Objekt stellt einen Ordner dar, der von einem externen Dokumentenanbieter wie Google Drive oder Dropbox verknüpft ist.

Weitere Informationen zu verknüpften Ordnern finden Sie unter [Verknüpfen von Dokumenten mit externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Möglicher Wert hinzugefügt:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>Suchfelder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>Direkte Felder</p> </td> 
   <td> <p>Die folgenden Felder wurden zur Ressource Testversand-Genehmigung hinzugefügt.</p> 
    <ul> 
     <li> <p><b>approveStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Ein QueueDef-Objekt stellt eine Warteschlange dar. Hierbei handelt es sich um ein Projekt, das in den Help Desk-Bereich veröffentlicht wurde, damit Benutzer Probleme an dieses Objekt senden können.

Weitere Informationen zu Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Hinzugefügt. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>0 (Nach benutzerdefinierten Formularen)</p> </li> 
       <li> <p>1 (Vor benutzerdefinierten Formularen)</p> </li> 
      </ul> </li> 
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
   <td> <p>Suchfelder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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

### Arbeitszeittabelle {#timesheet}

Ein Timesheet-Objekt stellt eine virtuelle Timecard dar, mit der Benutzer die tatsächlichen Arbeitsstunden für Aufgaben, Projekte und Hochtypen eingeben können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Kernfelder</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Entfernt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TimesheetProfile {#timesheetprofile}

Ein Timesheet-Objekt stellt eine virtuelle Timecard dar, mit der Benutzer die tatsächlichen Arbeitsstunden für Aufgaben, Projekte und Hochtypen eingeben können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Standardfelder</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront-Administratoren oder Gruppenadministratoren können Vorlagen erstellen, um die Layoutelemente in Adobe Workfront anzupassen. Das UITemplate-Objekt ist spezifisch für das neue Adobe Workfront-Erlebnis.

Informationen zu dem Objekt, das Layoutvorlagen in Adobe Workfront Classic darstellt, finden Sie unter [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> <p>Die folgenden Aktionen wurden der Ressource UITemplate hinzugefügt.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Nimmt das Argument:</p> 
      <ul> 
       <li> <p>overrideIfExists (boolean)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Übernimmt die Argumente:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (boolean)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegation {#userdelegation}

Ein UserDelegation -Objekt stellt den Vorgang dar, bei dem die Arbeit von einem Benutzer an einen anderen für einen bestimmten Zeitraum delegiert wird.

Das UserDelegations-Objekt hat das Flag REPORTABLE hinzugefügt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> <p>Die folgenden Felder haben das Flag NOT_GROUPABLE entfernt</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standardfelder</td> 
   <td> <p>Die folgenden Felder wurden hinzugefügt:</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
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
   <td> <p>Suchfelder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
