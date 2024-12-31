---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 13
description: Adobe Workfront hat API Version 13 am 22. April 2021 veröffentlicht. Die API-Version 13 enthält die folgenden Änderungen gegenüber Version 12.
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 2%

---

# Neue Funktionen in der API-Version 13

Adobe Workfront hat API Version 13 am 22. April 2021 veröffentlicht. Die API-Version 13 enthält die folgenden Änderungen gegenüber Version 12.

## Ressourcen hinzugefügt

Für API-Version 13 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API-Version 13 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen

Die folgenden Ressourcen wurden für die API-Version 13 geändert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">Zugriffsebene</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">Kundenpräferenzen</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref"></a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Projekt</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">TestversandValidierung</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Aufgabe</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Arbeitszeittabelle</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">Arbeitszeittabellen-Profil</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelegation</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref"></a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Zugriffsebene {#accesslevel}

Ein AccessLevel-Objekt ist Benutzern zugeordnet und beschreibt den Satz von AccessLevelPermissions, die bestimmen, auf was Benutzer zugreifen können.

Weitere Informationen zu Zugriffsebenen finden Sie unter [ von Zugriffsebenen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Beschreibung</b> </p> <p>Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass die Beschreibung nicht länger als 4.000 Zeichen ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Brotkrume {#breadcrumb}

Ein BreadCrumb-Objekt stellt ein Element in der übergeordneten/untergeordneten Hierarchie eines Workfront-Arbeitselements dar. Breadcrumbs geben an, wie ein Arbeitselement in die größere Struktur von Portfolios, Projekten, Projekten und Aufgaben passt.

Weitere Informationen zu Breadcrumbs finden Sie unter [Breadcrumbs - Übersicht in der neuen Adobe Workfront-Version](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

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

Ein BurndownEvent -Objekt, das ein Objekt darstellt, das den Bunddown einer Iteration ändert.

Weitere Informationen zum Burndown finden Sie unter [Burndown](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

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

### Kundenpräferenzen {#customerpreferences}

Ein CustomerPreferences-Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Workfront-Instanz festgelegt hat.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Hinzugefügte mögliche Werte:</p> 
      <ul> 
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> Kennwort: aemAADomain (config.general.aem.adomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">Arbeitszeittabelle:default.timesheet.restriction.timesheet.edit.owners.admins (config.timesheet.restriction.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p>Die folgenden Aktionen wurden der Ressource „Kundeneinstellungen“ hinzugefügt.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Nimmt das Argument:</p> 
      <ul> 
       <li> <p>Voreinstellungen (Karte)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

Ein DocumentVersion-Objekt stellt eine bestimmte Version einer Datei dar (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

Weitere Informationen zu Dokumentversionen finden Sie unter [Hochladen einer neuen Version eines Dokuments](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Zusätzlicher möglicher Wert:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Das Flag NOT_FILTERABLE wurde hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppe  {#group}

Ein Gruppenobjekt steht für eine Gruppe von Benutzern und Teams. Gruppen repräsentieren oft die Abteilungsstruktur.

Weitere Informationen zu Gruppen finden Sie unter [Gruppen im Vergleich zu Teams in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Aktionen</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>Diese Aktion gibt ein Array der übergeordneten Gruppen der Gruppe zurück (Gruppen, von denen die angegebene Gruppe eine Untergruppe ist).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Tagebucheintrag {#journalentry}

Das JournalEntry-Objekt kann so eingerichtet werden, dass Informationen zu bestimmten Objektfeldern jedes Mal protokolliert werden, wenn diese Felder geändert werden. Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird jedes Mal, wenn dieses Feld geändert wird, ein entsprechender Journaleintrag erstellt.

Die JournalEntry-Ressource hat das Flag REPORTABLE hinzugefügt.

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

### Layout-Vorlage {#layouttemplate}

Adobe Workfront-Administratoren oder Gruppenadministratoren können Vorlagen erstellen, um die Layout-Elemente in Adobe Workfront anzupassen. Das LayoutTemplate-Objekt ist spezifisch für Adobe Workfront Classic.

Das -Objekt, das Layout-Vorlagen in der neuen Adobe Workfront-Version darstellt, finden Sie unter [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Beschreibung</b> </p> <p>Der Validator MAX_LENGTH wurde hinzugefügt, der angibt, dass die Beschreibung nicht länger als 4.000 Zeichen ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

Ein LinkedFolder-Objekt stellt einen Ordner dar, der über einen externen Dokumentanbieter verknüpft ist, z. B. Google Drive oder Dropbox.

Weitere Informationen zu verknüpften Ordnern finden Sie unter [Verknüpfen von Dokumenten aus externen Anwendungen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Zusätzlicher möglicher Wert:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>Suchfelder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>Direkte Felder</p> </td> 
   <td> <p>Die folgenden Felder wurden der Ressource Testversandvalidierung hinzugefügt.</p> 
    <ul> 
     <li> <p><b>ApproverStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

Ein QueueDef -Objekt stellt eine Warteschlange dar. Dabei handelt es sich um ein Projekt, das im Helpdesk-Bereich veröffentlicht wurde, um Benutzenden die Übermittlung von Problemen zu ermöglichen.

Weitere Informationen zu Anfrage-Warteschlangen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>hinzugefügt. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>0 (nach benutzerdefinierten Formularen)</p> </li> 
       <li> <p>1 (Vor benutzerdefinierten Formularen)</p> </li> 
      </ul> </li> 
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

### Arbeitszeittabelle {#timesheet}

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

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
     <li> <p><b>objCode</b> </p> <p>entfernt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbeitszeittabellen-Profil {#timesheetprofile}

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

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

Adobe Workfront-Administratoren oder Gruppenadministratoren können Vorlagen erstellen, um die Layout-Elemente in Adobe Workfront anzupassen. Das UITemplate-Objekt ist spezifisch für das neue Adobe Workfront-Erlebnis.

Das -Objekt, das Layout-Vorlagen in Adobe Workfront Classic darstellt, finden Sie unter [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> <p>Die folgenden Aktionen wurden der UITemplate-Ressource hinzugefügt.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Nimmt das Argument:</p> 
      <ul> 
       <li> <p>overrideIfExists (boolesch)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Nimmt die Argumente:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (boolesch)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Benutzerdelegierung {#userdelegation}

Ein UserDelegation-Objekt stellt den Vorgang dar, bei dem Arbeit von einem Benutzer an einen anderen für einen bestimmten Zeitraum delegiert wird.

Das UserDelegation-Objekt hat das Flag REPORTABLE hinzugefügt.

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

Ein Arbeitsobjekt ist eine gemeinsame Schnittstelle, die sowohl von Task als auch von OpTask erbt wird und gemeinsamen Code zwischen den beiden verwendet.

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
