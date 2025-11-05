---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 12
description: Workfront hat API Version 12 am 12. November 2020 veröffentlicht. API Version 12 enthält die folgenden Änderungen gegenüber Version 11
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '2421'
ht-degree: 2%

---

# Neue Funktionen in der API-Version 12

Workfront hat API Version 12 am 12. November 2020 veröffentlicht. API Version 12 enthält die folgenden Änderungen gegenüber Version 11

## Ressourcen hinzugefügt

Die folgenden Ressourcen sind neu in der Workfront-API-Version 12.

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### Brotkrume {#breadcrumb}

Ein BreadCrumb-Objekt stellt ein Element in der übergeordneten/untergeordneten Hierarchie eines Adobe Workfront-Arbeitselements dar. Breadcrumbs geben an, wie ein Arbeitselement in die größere Struktur von Portfolios, Projekten, Projekten und Aufgaben passt.

Weitere Informationen zu Breadcrumbs in Workfront finden Sie unter [Breadcrumbs - Übersicht in der neuen Adobe Workfront-Version](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

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

Rich-Text-Felder sind jetzt für mehr Objekte verfügbar. Das RichTextParameterValue-Objekt wurde zu Workfront hinzugefügt, um diese Verfügbarkeit zu unterstützen.

Weitere Informationen finden Sie unter [Rich-Textfelder in der Adobe Workfront-API](../../wf-api/general/rich-text-field-api.md).

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

Für API-Version 12 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen

Die folgenden Ressourcen wurden für die Workfront-API-Version 12 geändert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">Zugriffsebene</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">Zugriffsberechtigungen</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">Zugriffsregel</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnkündigungAnhang</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Genehmigung</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">CalendarSection</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Firma</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Kunde</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">Kundenpräferenzen</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Dokument</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref"></a> </p> </li> 
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
     <li> <p><a href="#work" class="MCXref xref"></a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### Zugriffsebene {#accesslevel}

Ein AccessLevel-Objekt ist Benutzern zugeordnet und beschreibt den Satz von AccessLevelPermissions, die bestimmen, auf was Benutzer zugreifen können.

Weitere Informationen zu Zugriffsebenen finden Sie unter [&#x200B; von Zugriffsebenen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

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

### ZugriffsebeneBerechtigungen {#accesslevelpermissions}

Ein AccessLevelPermissions-Objekt stellt eine bestimmte Berechtigung zum Zugreifen auf, Erstellen oder Ändern eines Workfront-Objekts dar. Diese Berechtigungen können dann mit einer Zugriffsebene verknüpft werden.

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
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Benutzende mit einer Zugriffsebene, die diese Berechtigung enthält, können geplante Stunden im Workload-Balancer aktualisieren.</p> <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aktualisieren der geplanten Stunden bei der Verwaltung von Benutzerzuweisungen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuweisungen im Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Ein Benutzer mit einer Zugriffsebene, die diese Berechtigung enthält, kann benutzerdefinierten Formularen Felder hinzufügen.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Erstellen oder Bearbeiten eines benutzerdefinierten Formulars</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Benutzende mit einer Zugriffsebene, die diese Berechtigung enthält, können ein benutzerdefiniertes Feld systemweit für den Löschzugriff freigeben.</p> </li> 
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
     <li> <p style="font-weight: bold;">Aktion</p> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Benutzende mit einer Zugriffsebene, die diese Berechtigung enthält, können geplante Stunden im Workload-Balancer aktualisieren.</p> <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aktualisieren der geplanten Stunden bei der Verwaltung von Benutzerzuweisungen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuweisungen im Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Ein Benutzer mit einer Zugriffsebene, die diese Berechtigung enthält, kann benutzerdefinierten Formularen Felder hinzufügen.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Erstellen oder Bearbeiten eines benutzerdefinierten Formulars</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Benutzende mit einer Zugriffsebene, die diese Berechtigung enthält, können ein benutzerdefiniertes Feld systemweit für den Löschzugriff freigeben.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Benutzende mit einer Zugriffsebene, die diese Berechtigung enthält, können geplante Stunden im Workload-Balancer aktualisieren.</p> <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aktualisieren der geplanten Stunden bei der Verwaltung von Benutzerzuweisungen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuweisungen im Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Ein Benutzer mit einer Zugriffsebene, die diese Berechtigung enthält, kann benutzerdefinierten Formularen Felder hinzufügen.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Erstellen oder Bearbeiten eines benutzerdefinierten Formulars</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Benutzende mit einer Zugriffsebene, die diese Berechtigung enthält, können ein benutzerdefiniertes Feld systemweit für den Löschzugriff freigeben.</p> </li> 
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

Ein ActivityLog-Objekt ist eine vollständige Liste aller Aktivitäten, die in einem bestimmten Workfront Proof-Konto stattgefunden haben.

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

### Anhang für die Ankündigung {#announcementattachment}

Ein Ankündigungs-Attachment-Objekt stellt eine Datei dar, die an eine Workfront-Ankündigung angehängt wurde.

Weitere Informationen zu Ankündigungs-Anhängen finden Sie unter [Ankündigungen senden](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Hinzugefügte mögliche Werte:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileExtension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileExtension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileExtension.qsheet)</p> </li> 
      </ul> </li> 
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
     <li> <p><strong>workEffort</strong> </p> <p>Dieses Feld wurde hinzugefügt und gibt an, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand benötigt, um eine Aufgabe abzuschließen. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>1 (Klein)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Groß)</p> </li> 
      </ul> <p>Weitere Informationen zum Work Effort in Workfront finden Sie unter <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort - Übersicht</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kalenderabschnitt {#calendarsection}

Ein Kalenderabschnitt ist ein Kalenderbericht.

Weitere Informationen zu Kalenderberichten finden Sie unter [Übersicht über Kalenderberichte](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> <p style="font-weight: normal;">Die folgenden Felder wurden zum CalendarSection -Objekt hinzugefügt, um die neue Funktionalität der Verwendung benutzerdefinierter Datumsangaben in Kalenderberichten zu unterstützen. </p> <p style="font-weight: normal;">Weitere Informationen finden Sie unter <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht</a>.</p> 
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

Ein Unternehmensobjekt stellt eine Organisation dar, die aus einer Sammlung von Personen besteht.

Weitere Informationen zu Unternehmen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Die ID der Gruppe, mit der die Firma verknüpft ist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Gruppe</p> <p style="font-weight: normal;">Die Gruppe, mit der die Firma verknüpft ist. Durch das Verknüpfen einer Firma mit einer Gruppe kann der Gruppenadministrator den Gruppenzugriff und die Gruppenberechtigungen für die Firma erweitern.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kundin bzw. Kunde {#customer}

Ein Customer-Objekt stellt eine Organisation dar, die eine Instanz von Workfront verwendet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Aktionen</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">Bei dieser Aktion wird ein CustomerProductTypeEnum-Argument verwendet und ein boolescher Wert zurückgegeben, der angibt, ob dieser Kunde über ein Konto für dieses Produkt verfügt. </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled (Zoom-Integration im Aktualisierungsverlauf aktivieren)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
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
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Entfernte möglichen Wert:</p> 
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
   <td> <p>Die folgenden Aktionen wurden zum Dokumentobjekt hinzugefügt.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">Diese Aktion verwendet das documentVersionID-Argument (Zeichenfolge) und gibt eine Zuordnung zurück, die die Entscheidung der Überprüfenden angibt.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">Diese Aktion verwendet die folgenden Argumente:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (Zeichenfolge)</p> </li> 
       <li> <p>reviewerDecision (Zeichenfolge)</p> </li> 
       <li> <p>Kommentar (Zeichenfolge)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppe  {#group}

Ein Gruppenobjekt steht für eine Gruppe von Benutzern und Teams. Gruppen repräsentieren oft die Abteilungsstruktur.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">Die ID des Business Leaders, der der Gruppe zugewiesen wurde.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Business Leader</p> <p style="font-weight: normal;">Der der Gruppe zugewiesene Business Leader. Ein Business Leader ist jemand, der geschäftliche Entscheidungen für die Gruppe trifft.</p> <p style="font-weight: normal;">Weitere Informationen über Business Leader finden Sie unter <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader - Übersicht</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>Diese Aktion verwendet die folgenden Argumente:</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (Zeichenfolge[])</p> </li> 
       <li> <p>teamID (Zeichenfolge)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>Diese Aktion verwendet die folgenden Argumente:</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (Zeichenfolge[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Entfernte möglichen Wert:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

Ein OpTask-Objekt wird im Allgemeinen als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise darauf hinweist, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungsanforderungen, -anfragen und -fehler sind ebenfalls Probleme.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Reihenfolge gibt die Position einer Aufgabe oder Story im Agile-Rückstand an.</p> <p>Dieses Feld entfernte die folgenden Flags:
       <ul>
        <li>DYNAMISCH,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> <p>Diese Aktionen haben den Argumentstatus hinzugefügt, um die neue Funktion der Schaltfläche Starten zu unterstützen. Damit wird der Status eines Arbeitselements geändert, wenn ein Benutzer auf die Schaltfläche klickt, um anzugeben, dass er mit der Bearbeitung des Elements begonnen hat.</p> <p>Weitere Informationen finden Sie unter <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Starten“ </a>.</p> 
    <ul> 
     <li> <p><strong>acceptedWork</strong> </p> </li> 
     <li> <p><strong>unacceptedWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

Ein Parameter-Objekt ist ein benutzerdefiniertes Feld.

Die Parameterressource hat das Flag SHARABLE hinzugefügt.

Weitere Informationen zu benutzerdefinierten Feldern finden Sie unter [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md) in [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Zusätzlicher möglicher Wert:</p> 
      <ul> 
       <li> <p>RICH (Rich Text)</p> <p>Weitere Informationen finden Sie unter <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich-Textfelder in der Adobe Workfront-API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Zusätzlicher möglicher Wert:</p> 
      <ul> 
       <li> <p>RICH (Textfeld mit Formatierung)</p> <p>Weitere Informationen finden Sie unter <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich-Textfelder in der Adobe Workfront-API</a>.</p> </li> 
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

Ein Portfolio-Objekt ist eine Sammlung von Projekten, die um dieselben Ressourcen konkurrieren, normalerweise Geld oder Personen, um sie abzuschließen.

Weitere Informationen zu Portfolios finden Sie unter Übersicht über Portfolio in Adobe Workfront [&#128279;](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Die ID der Gruppe, mit der das Portfolio verknüpft ist.</p> </li> 
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

Ein Programmobjekt ist eine Teilmenge von Projekten innerhalb eines Portfolios, in dem ähnliche Projekte gruppiert werden können.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Die ID der Gruppe, mit der das Programm verknüpft ist.</p> </li> 
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
     <li><strong>RequestorCoreAction</strong> <p>Die folgenden möglichen Werte wurden hinzugefügt:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>Benutzende mit einer Zugriffsebene, die diese Berechtigung enthält, können geplante Stunden im Workload-Balancer aktualisieren.</p> <p>Weitere Informationen finden Sie unter <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Aktualisieren der geplanten Stunden bei der Verwaltung von Benutzerzuweisungen</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Verwalten von Benutzerzuweisungen im Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>Ein Benutzer mit einer Zugriffsebene, die diese Berechtigung enthält, kann benutzerdefinierten Formularen Felder hinzufügen.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Erstellen oder Bearbeiten eines benutzerdefinierten Formulars</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>Benutzende mit einer Zugriffsebene, die diese Berechtigung enthält, können ein benutzerdefiniertes Feld systemweit für den Löschzugriff freigeben.</p> </li>
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Geplanter Bericht {#scheduledreport}

Ein ScheduledReport-Objekt stellt einen Bericht dar, der für die Bereitstellung geplant wurde.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>format</strong> </p> <p>Hinzugefügte mögliche Werte:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileExtension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileExtension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileExtension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

Ein ScoreCardQuestion-Objekt stellt eine Frage dar, die zu einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfolio-Manager bestimmt, und die Antworten geben dem Manager die Möglichkeit zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

Weitere Informationen zu Scorecard-Fragen finden Sie unter [Erstellen einer Scorecard](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Zusätzlicher möglicher Wert: RICH (Textfeld mit Formatierung) </p> <p style="font-weight: normal;">Weitere Informationen finden Sie unter <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich-Textfelder in der Adobe Workfront-API</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Aufgabe {#task}

Ein Aufgabenobjekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (Fertigstellen eines Projekts) ausgeführt werden muss.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Dieses Feld wurde hinzugefügt und gibt an, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand benötigt, um eine Aufgabe abzuschließen. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>1 (Klein)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Groß)</p> </li> 
      </ul> <p>Weitere Informationen zum Work Effort in Workfront finden Sie unter <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort - Übersicht</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> <p>Diese Aktionen haben den Argumentstatus hinzugefügt, um die neue Funktion der Schaltfläche Starten zu unterstützen. Damit wird der Status eines Arbeitselements geändert, wenn ein Benutzer auf die Schaltfläche klickt, um anzugeben, dass er mit der Bearbeitung des Elements begonnen hat.</p> <p>Weitere Informationen finden Sie unter <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Starten“ </a>.</p> 
    <ul> 
     <li> <p><strong>acceptedWork</strong> </p> </li> 
     <li> <p><strong>unacceptedWork</strong> </p> </li> 
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
   <td> <p>Die folgenden Felder wurden der Team-Ressource hinzugefügt:</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>Dieses Feld gibt die Anzahl der Tage an, die eine ausgefüllte Karte auf dem Kanban-Board verbleibt.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Dieses Feld verknüpft ein Team mit einer Gruppe. Dadurch wird das Team als Teil der Gruppe identifiziert und der Gruppenadministrator kann die Teams verwalten.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>Dies ist ein boolescher Parameter, der angibt, ob die Schaltfläche „Bearbeiten“ des Teams als Schaltfläche „Starten“ konfiguriert wurde. Wenn ein Mitglied des Teams auf die Schaltfläche Starten klickt, um mit der Arbeit an einem Arbeitselement zu beginnen, ändert sich der Status des Elements von Neu in einen in den Team-Einstellungen konfigurierten Status.</p> </li> 
     <li> <p>In den folgenden Feldern können Sie benutzerdefinierte Status für die Schaltfläche „Starten“ für die einzelnen Arbeitselemente angeben.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>Weitere Informationen über die Schaltfläche „Starten“ finden Sie <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Ersetzen der Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Starten“</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referenzfelder</td> 
   <td> <p>Das folgende Feld wurde der Team-Ressource hinzugefügt:</p> 
    <ul> 
     <li> <p><strong>group</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Vorlagenaufgabe {#templatetask}

Ein TemplateTask-Objekt stellt eine Aufgabe dar, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, in dem die Vorlage verwendet wird.

Weitere Informationen zu Vorlagenaufgaben finden Sie unter [Vorlagenaufgaben bearbeiten](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>Dieses Feld wurde hinzugefügt und gibt an, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand benötigt, um eine Aufgabe abzuschließen. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>1 (Klein)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Groß)</p> </li> 
      </ul> <p>Weitere Informationen zum Work Effort in Workfront finden Sie unter <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort - Übersicht</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Arbeitszeittabelle {#timesheet}

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

Weitere Informationen zu Arbeitszeittabellen finden Sie unter [Arbeitszeittabellen - Übersicht](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Kernfelder</td> 
   <td> <p>Das folgende Feld wurde aus der Arbeitszeittabellen-Ressource entfernt:</p> 
    <ul> 
     <li> <p><strong>objCode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Update

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
       <li> <p>initiativeAdd (enum.updateTypeEnum.initiativeAdd)</p> </li> 
       <li> <p>initiativeEdit (enum.updateTypeEnum.initiativeEdit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Weitere Informationen zu Initiativen finden Sie unter <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Initiativen - Übersicht im Szenario-Planer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Benutzerin bzw. Benutzer {#user}

Ein Benutzerobjekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> <p>Die folgenden Felder wurden der Benutzerressource hinzugefügt:</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>Dies stellt das Datum und die Uhrzeit dar, zu der ein Benutzer deaktiviert wurde.</p> <p>Weitere Informationen zu deaktivierten Benutzern finden Sie unter <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren eines Benutzers</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>In diesem Feld wird der Zugriff der Benutzenden auf Workfront-Ziele angezeigt. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>Kein Zugriff</p> </li> 
       <li> <p>Ansicht</p> </li> 
       <li> <p>Bearbeiten</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> <p>Die folgende Aktion wurde zur Benutzerressource hinzugefügt:</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjectCode</strong> </p> <p>Diese Aktion verwendet die folgenden Argumente</p> 
      <ul> 
       <li> <p>IDs (Zeichenfolge)</p> </li> 
       <li> <p>objCode (Zeichenfolge)</p> </li> 
      </ul> </li> 
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
   <td>Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Reihenfolge gibt die Position einer Aufgabe oder Story im Agile-Rückstand an.</p> <p>Dieses Feld entfernte die folgenden Flags:</p> 
      <ul> 
       <li> <p>DYNAMISCH,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Dieses Feld fügte die folgenden Flags hinzu:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMISCH,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>Dieses Feld wurde hinzugefügt und gibt an, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand benötigt, um eine Aufgabe abzuschließen. Mögliche Werte sind:</p> 
      <ul> 
       <li> <p>1 (Klein)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Groß)</p> </li> 
      </ul> <p>Weitere Informationen zum Work Effort in Workfront finden Sie unter <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort - Übersicht</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
