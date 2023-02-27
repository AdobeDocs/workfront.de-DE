---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 12
description: Workfront hat die API-Version 12 am 12. November 2020 veröffentlicht. API Version 12 enthält die folgenden Änderungen gegenüber Version 11
author: Becky
feature: Workfront API
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 2%

---

# Neue Funktionen in API Version 12

Workfront hat die API-Version 12 am 12. November 2020 veröffentlicht. API Version 12 enthält die folgenden Änderungen gegenüber Version 11

## Hinzugefügte Ressourcen

Die folgenden Ressourcen sind in Workfront API Version 12 neu.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

Ein BreadCrumb-Objekt stellt ein Element in der übergeordneten/untergeordneten Hierarchie eines Adobe Workfront-Arbeitselements dar. Breadcrumbs zeigen an, wie ein Arbeitselement in die größere Struktur von Portfolios, Projekten, Projekten und Aufgaben passt.

Weitere Informationen zu Breadcrumbs in Workfront finden Sie unter [Breadcrumbs-Übersicht im neuen Adobe Workfront-Erlebnis](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Aktion</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

Rich-Text-Felder sind jetzt für weitere Objekte verfügbar. Das RichTextParameterValue -Objekt wurde zu Workfront hinzugefügt, um diese Verfügbarkeit zu unterstützen.

Weitere Informationen finden Sie unter [Rich-Text-Felder in der Adobe Workfront-API](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## Entfernte Ressourcen

Für API Version 12 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen

Die folgenden Ressourcen wurden für die Workfront API Version 12 geändert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnnouncementAttachment</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Genehmigung</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">CalendarSection</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Firma</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Kunde</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Dokument</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Gruppe </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Parameter</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Programm</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Aufgabe</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TemplateTask</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Arbeitszeittabelle</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">Benutzer</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Arbeit </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

Ein AccessLevel -Objekt ist mit Benutzern verknüpft und beschreibt den Satz von AccessLevelPermissions, der bestimmt, auf welchen Benutzer zugreifen können.

Weitere Informationen zu Zugriffsebenen finden Sie unter [Funktionsweise von Zugriffsstufen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

Ein AccessLevelPermissions -Objekt stellt eine spezifische Berechtigung zum Zugreifen auf, Erstellen oder Ändern eines Workfront-Objekts dar. Diese Berechtigungen können dann einer Zugriffsebene zugeordnet werden.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Ein Benutzer mit einer Zugriffsstufe, die diese Berechtigung enthält, kann geplante Stunden im Arbeitslastausgleich aktualisieren.</p> <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuordnungen im Lastenausgleich</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Benutzer mit einer Zugriffsebene, die diese Berechtigung enthält, können benutzerdefinierte Formulare um Felder erweitern.</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Ein Benutzer mit einer Zugriffsstufe, die diese Berechtigung enthält, kann ein benutzerdefiniertes Feld systemweit für den Löschzugriff freigeben.</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
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
     <li> <p style="font-weight: bold;">action</p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Ein Benutzer mit einer Zugriffsstufe, die diese Berechtigung enthält, kann geplante Stunden im Arbeitslastausgleich aktualisieren.</p> <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuordnungen im Lastenausgleich</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Benutzer mit einer Zugriffsebene, die diese Berechtigung enthält, können benutzerdefinierte Formulare um Felder erweitern.</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Ein Benutzer mit einer Zugriffsstufe, die diese Berechtigung enthält, kann ein benutzerdefiniertes Feld systemweit für den Löschzugriff freigeben.</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets</a>.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Ein Benutzer mit einer Zugriffsstufe, die diese Berechtigung enthält, kann geplante Stunden im Arbeitslastausgleich aktualisieren.</p> <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuordnungen im Lastenausgleich</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Benutzer mit einer Zugriffsebene, die diese Berechtigung enthält, können benutzerdefinierte Formulare um Felder erweitern.</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Ein Benutzer mit einer Zugriffsstufe, die diese Berechtigung enthält, kann ein benutzerdefiniertes Feld systemweit für den Löschzugriff freigeben.</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

Ein ActivityLog-Objekt ist eine vollständige Liste aller Aktivitäten, die in einem bestimmten Workfront-Testkonto stattgefunden haben.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Vorgänge</p> </td> 
   <td> <p>Der folgende Vorgang wurde aus dem ActivityLog-Objekt entfernt:</p> 
    <ul> 
     <li> <p><strong>HINZUFÜGEN</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnnouncementAttachment {#announcementattachment}

Ein AnnouncementAttachment -Objekt stellt eine Datei dar, die an eine Workfront-Ankündigung angehängt wurde.

Weitere Informationen zu Ankündigungsanlagen finden Sie unter [Mitteilungen senden](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Mögliche Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslide (enum.fileextension.qslide)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Die folgenden Flags wurden entfernt:</p> 
      <ul> 
       <li> <p>DYNAMISCH,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Die folgenden Flags wurden hinzugefügt</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMISCH,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Dieses Feld wurde hinzugefügt. Es zeigt an, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand für die Ausführung einer Aufgabe benötigt. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>1 (Klein)</p> </li> 
       <li> <p>2 (Mittel)</p> </li> 
       <li> <p>3 (groß)</p> </li> 
      </ul> <p>Weitere Informationen zu den Arbeitsbemühungen in Workfront finden Sie unter <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Übersicht über den Arbeitsaufwand</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CalendarSection {#calendarsection}

Ein Kalenderabschnitt ist ein Kalenderbericht.

Weitere Informationen zu Kalenderberichten finden Sie unter [Kalenderberichte - Übersicht](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p style="font-weight: normal;">Die folgenden Felder wurden zum CalendarSection -Objekt hinzugefügt, um die neue Funktion zur Verwendung benutzerdefinierter Datumswerte in Kalenderberichten zu unterstützen. </p> <p style="font-weight: normal;">Weitere Informationen finden Sie unter <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Firma {#company}

Ein Unternehmensobjekt stellt eine Organisation dar, die aus einer Personensammlung besteht.

Weitere Informationen zu Unternehmen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Die Kennung der Gruppe, mit der das Unternehmen verknüpft ist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Gruppe</p> <p style="font-weight: normal;">Die Gruppe, mit der das Unternehmen verbunden ist. Wenn Sie ein Unternehmen mit einer Gruppe verknüpfen, kann der Gruppenadministrator den Gruppenzugriff und die Gruppenberechtigungen auf das Unternehmen erweitern.</p> </li> 
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
  <tr> 
   <td>Aktionen</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">Diese Aktion akzeptiert ein CustomerProductTypeEnum -Argument und gibt einen booleschen Wert zurück, der angibt, ob dieser Kunde über ein Konto für dieses Produkt verfügt. </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled (Zoom-Integration im Aktualisierungsstream aktivieren)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
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
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Mögliche Werte wurden entfernt:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aktionen</td> 
   <td> <p>Die folgenden Aktionen wurden dem Dokumentobjekt hinzugefügt.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">Diese Aktion akzeptiert das documentVersonID-Argument (Zeichenfolge) und gibt eine Zuordnung zurück, die die Entscheidung des Validierers angibt.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">Diese Aktion akzeptiert die folgenden Argumente:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (string)</p> </li> 
       <li> <p>reviewerDecision (Zeichenfolge)</p> </li> 
       <li> <p>comment (string)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppe  {#group}

Ein Group -Objekt stellt eine Gruppe von Benutzern und Teams dar. Gruppen stellen oft die Struktur der Abteilungen dar.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">Die Kennung des der Gruppe zugewiesenen Business Leaders.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">Der der Gruppe zugewiesene Business Leader. Ein Business Leader ist jemand, der Geschäftsentscheidungen für die Gruppe trifft.</p> <p style="font-weight: normal;">Weitere Informationen zu Unternehmensführern finden Sie unter <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Übersicht über Business Leader</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>Diese Aktion akzeptiert die folgenden Argumente:</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID (Zeichenfolge)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>Diese Aktion akzeptiert die folgenden Argumente:</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Mögliche Werte wurden entfernt:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Ein OpTask-Objekt wird häufig als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise anzeigt, dass ein Problem vorliegt, das die Fertigstellung einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungen bei Bestellungen, Anforderungen und Fehlern sind ebenfalls Probleme.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Die Reihenfolge gibt die Position einer Aufgabe oder Geschichte im Agile-Backlog an.</p> <p>In diesem Feld wurden die folgenden Flags entfernt:
       <ul>
        <li>DYNAMISCH,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> <p>Mit diesen Aktionen wurde der Argumentstatus hinzugefügt, um die neue Schaltfläche Start zu unterstützen, die den Status eines Arbeitselements ändert, wenn ein Benutzer auf die Schaltfläche klickt, um anzuzeigen, dass er mit der Bearbeitung des Elements begonnen hat.</p> <p>Weitere Informationen finden Sie unter <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche Start</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

Ein Parameter -Objekt ist ein benutzerdefiniertes Feld.

Die Ressource Parameter hat das Flag SHARABLE hinzugefügt.

Weitere Informationen zu benutzerdefinierten Feldern finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Möglicher Wert hinzugefügt:</p> 
      <ul> 
       <li> <p>RICH (Rich Text)</p> <p>Weitere Informationen finden Sie unter <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich-Text-Felder in der Adobe Workfront-API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Möglicher Wert hinzugefügt:</p> 
      <ul> 
       <li> <p>RICH (Textfeld mit Formatierung)</p> <p>Weitere Informationen finden Sie unter <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich-Text-Felder in der Adobe Workfront-API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>label</strong> </p> <p>Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standardfelder</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>label</strong> </p> <p>Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

Ein Portfolio-Objekt ist eine Sammlung von Projekten, die um die gleichen Ressourcen konkurrieren, in der Regel um Geld oder Personen, um sie zu vervollständigen.

Weitere Informationen zu Portfolios finden Sie unter [Übersicht über Portfolio in Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Die Kennung der Gruppe, mit der das Portfolio verknüpft ist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Gruppe</p> <p style="font-weight: normal;">Die Gruppe, mit der das Portfolio verknüpft ist. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Programm {#program}

Ein Programmobjekt ist eine Teilmenge von Projekten in einem Portfolio, in dem ähnliche Projekte gruppiert werden können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Die Kennung der Gruppe, mit der das Programm verknüpft ist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Gruppe</p> <p style="font-weight: normal;">Die Gruppe, mit der das Programm verknüpft ist. </p> </li> 
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
     <li><strong>requestorCoreAction</strong> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Ein Benutzer mit einer Zugriffsstufe, die diese Berechtigung enthält, kann geplante Stunden im Arbeitslastausgleich aktualisieren.</p> <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuordnungen im Lastenausgleich</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Benutzer mit einer Zugriffsebene, die diese Berechtigung enthält, können benutzerdefinierte Formulare um Felder erweitern.</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Ein Benutzer mit einer Zugriffsstufe, die diese Berechtigung enthält, kann ein benutzerdefiniertes Feld systemweit für den Löschzugriff freigeben.</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

Ein ScheduledReport -Objekt stellt einen Bericht dar, der für die Bereitstellung konfiguriert wurde.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>format</strong> </p> <p>Mögliche Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslide (enum.fileextension.qslide)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Ein ScoreCardQuestion -Objekt stellt eine Frage dar, die einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfolio-Manager bestimmt und ihre Antworten ermöglichen es dem Manager zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

Weitere Informationen zu Scorecard-Fragen finden Sie unter [Scorecard erstellen](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Der mögliche Wert RICH (Textfeld mit Formatierung) wurde hinzugefügt. </p> <p style="font-weight: normal;">Weitere Informationen finden Sie unter <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich-Text-Felder in der Adobe Workfront-API</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aufgabe {#task}

Ein Task -Objekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (zum Abschließen eines Projekts) ausgeführt werden muss.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Dieses Feld wurde hinzugefügt. Es zeigt an, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand für die Ausführung einer Aufgabe benötigt. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>1 (Klein)</p> </li> 
       <li> <p>2 (Mittel)</p> </li> 
       <li> <p>3 (groß)</p> </li> 
      </ul> <p>Weitere Informationen zu den Arbeitsbemühungen in Workfront finden Sie unter <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Übersicht über den Arbeitsaufwand</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> <p>Mit diesen Aktionen wurde der Argumentstatus hinzugefügt, um die neue Schaltfläche Start zu unterstützen, die den Status eines Arbeitselements ändert, wenn ein Benutzer auf die Schaltfläche klickt, um anzuzeigen, dass er mit der Bearbeitung des Elements begonnen hat.</p> <p>Weitere Informationen finden Sie unter <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche Start</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

Ein Team-Objekt ist eine Sammlung von Benutzern, die einem Arbeitselement zugewiesen werden können.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> <p>Die folgenden Felder wurden der Ressource Team hinzugefügt:</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Dieses Feld gibt die Anzahl der Tage an, die eine ausgefüllte Karte auf dem Kanban-Board verbleibt.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>In diesem Feld wird ein Team mit einer Gruppe verknüpft. Dadurch wird das Team als Teil der Gruppe identifiziert und der Gruppenadministrator kann die Teams verwalten.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Dies ist ein boolescher Parameter, der anzeigt, ob die Schaltfläche "Arbeit an diesem Team"als Schaltfläche "Start"konfiguriert wurde. Wenn ein Mitglied des Teams auf die Schaltfläche Starten klickt, um mit der Arbeit an einem Arbeitselement zu beginnen, ändert sich der Status des Elements von Neu in einen in den Teameinstellungen konfigurierten Status.</p> </li> 
     <li> <p>Mit den folgenden Feldern können Sie benutzerdefinierte Status für die Schaltfläche Start für die einzelnen Arbeitselemente angeben.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>Weitere Informationen zur Schaltfläche Start finden Sie unter <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche Start</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referenzfelder</td> 
   <td> <p>Das folgende Feld wurde der Ressource Team hinzugefügt:</p> 
    <ul> 
     <li> <p><strong>Gruppe</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

Ein TemplateTask -Objekt stellt eine Aufgabe dar, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, in dem die Vorlage verwendet wird.

Weitere Informationen zu Vorlagenaufgaben finden Sie unter [Vorlagenaufgabe bearbeiten](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Dieses Feld wurde hinzugefügt. Es zeigt an, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand für die Ausführung einer Aufgabe benötigt. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>1 (Klein)</p> </li> 
       <li> <p>2 (Mittel)</p> </li> 
       <li> <p>3 (groß)</p> </li> 
      </ul> <p>Weitere Informationen zu den Arbeitsbemühungen in Workfront finden Sie unter <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Übersicht über den Arbeitsaufwand</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbeitszeittabelle {#timesheet}

Ein Timesheet-Objekt stellt eine virtuelle Timecard dar, mit der Benutzer die tatsächlichen Arbeitsstunden für Aufgaben, Projekte und Hochtypen eingeben können.

Weitere Informationen zu Timesheets finden Sie unter [Timesheets - Übersicht](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Kernfelder</td> 
   <td> <p>Das folgende Feld wurde aus der Timesheet-Ressource entfernt:</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aktualisieren

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Weitere Informationen zu Initiativen finden Sie unter <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Übersicht über Initiativen im Szenario-Planer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Benutzer {#user}

Ein User -Objekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> <p>Die folgenden Felder wurden der Ressource Benutzer hinzugefügt:</p> 
    <ul> 
     <li> <p><strong>effectiveDeactivationDate</strong> </p> <p>Dies stellt das Datum und die Uhrzeit dar, zu der ein Benutzer deaktiviert wurde.</p> <p>Weitere Informationen zu deaktivierten Benutzern finden Sie unter <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Benutzer deaktivieren oder reaktivieren</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>In diesem Feld wird der Zugriff des Benutzers auf Workfront-Ziele angezeigt. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>Kein Zugriff</p> </li> 
       <li> <p>Anzeigen</p> </li> 
       <li> <p>Bearbeiten</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> <p>Die folgende Aktion wurde der Ressource Benutzer hinzugefügt:</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>Diese Aktion akzeptiert die folgenden Argumente</p> 
      <ul> 
       <li> <p>id (string)</p> </li> 
       <li> <p>objCode (Zeichenfolge)</p> </li> 
      </ul> </li> 
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
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Die Reihenfolge gibt die Position einer Aufgabe oder Geschichte im Agile-Backlog an.</p> <p>In diesem Feld wurden die folgenden Flags entfernt:</p> 
      <ul> 
       <li> <p>DYNAMISCH,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>In diesem Feld wurden die folgenden Flags hinzugefügt:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMISCH,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Dieses Feld wurde hinzugefügt. Es zeigt an, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand für die Ausführung einer Aufgabe benötigt. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>1 (Klein)</p> </li> 
       <li> <p>2 (Mittel)</p> </li> 
       <li> <p>3 (groß)</p> </li> 
      </ul> <p>Weitere Informationen zu den Arbeitsbemühungen in Workfront finden Sie unter <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Übersicht über den Arbeitsaufwand</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
