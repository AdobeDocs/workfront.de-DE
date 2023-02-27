---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 14
description: Adobe Workfront hat am 9. September 2021 die API-Version 14 veröffentlicht. API Version 14 enthält die folgenden Änderungen gegenüber Version 14.
author: Becky
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# Neue Funktionen in API Version 14

Adobe Workfront hat am 9. September 2021 die API-Version 14 veröffentlicht. API Version 14 enthält die folgenden Änderungen gegenüber Version 14.

## Hinzugefügte Ressourcen

Für API Version 14 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API Version 14 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen

Die folgenden Ressourcen wurden für API Version 14 geändert.

* [BillingRecord (BILL)](#billingrecord-bill)
* [Kategorie (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Kunde (CUST)](#customer-cust)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Gruppe (GRUPPE)](#group-group)
* [HinweisTag (NTAG)](#notetag-ntag)
* [Projekt (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Ressourcenzuweisung (RSALLO)](#resource-allocation-rsallo)
* [Rolle (ROLE)](#role-role)
* [Vorlage (TMPL)](#template-tmpl)
* [Datenblatt (TSHET)](#timesheet-tshet)

### BillingRecord (BILL) {#billingrecord-bill}

Ein BillingRecord -Objekt zeichnet die Einnahmen, Stunden oder Ausgaben auf, die abgerechnet werden können. Diese Informationen können zur Erstellung von Rechnungen in einem externen Buchführungssystem verwendet werden.

Weitere Informationen zu Rechnungsdatensätzen finden Sie unter [Rechnungsdatensätze erstellen](../../manage-work/projects/project-finances/create-billing-records.md).

Das BillingRecord -Objekt hat die Markierung hinzugefügt **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Hinzugefügt. Eine Kategorie ist ein benutzerdefiniertes Formular. Dieser Parameter wurde hinzugefügt, um die Möglichkeit zu unterstützen, benutzerdefinierte Forms zu BillingRecord -Objekten hinzuzufügen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referenzfelder</td> 
   <td> 
    <ul> 
     <li> <p><b>category</b> </p> <p>Hinzugefügt. Eine Kategorie ist ein benutzerdefiniertes Formular. Dieser Parameter wurde hinzugefügt, um die Möglichkeit zum Hinzufügen benutzerdefinierter Formulare zu BillingRecord -Objekten zu unterstützen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Hinzugefügt. Dies stellt eine Sammlung von Kategorien (benutzerdefinierten Formularen) dar, die mit dem BillingRecord -Objekt verknüpft sind.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Hinzugefügt. Durch diese Aktion werden die Ausdrücke in benutzerdefinierten Formularfeldern neu berechnet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kategorie (CTGY) {#category-ctgy}

Ein Category -Objekt ist ein benutzerdefiniertes Formular.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Möglicher Wert hinzugefügt:</p> 
      <ul> 
       <li> <p> BILL (BillingRecord)</p> </li> 
      </ul> <p>Dieser Wert wurde hinzugefügt, um die Möglichkeit zum Hinzufügen benutzerdefinierter Formulare zu BillingRecord -Objekten zu unterstützen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Diese Aktion akzeptiert die Parameter objID und objCode und gibt einen booleschen Wert zurück.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

Das CustomEnum -Objekt unterstützt die Konvertierung von Status-Codes in für Menschen lesbaren Text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Abfragen</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>Hinzugefügt. Diese Abfrage unterstützt die Erstellung und Verwaltung von Status für Gruppen und Untergruppen. </p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Verwalten von Gruppenstatus</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kunde (CUST) {#customer-cust}

Ein Kundenobjekt stellt eine Organisation dar, die eine Instanz von Workfront verwendet.

Dies ist ein internes Objekt.

### CustomerPreferences (CUSTPR) {#customerpreferences-custpr}

Ein CustomerPreferences -Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Instanz von Workfront festgelegt hat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Möglicher Wert hinzugefügt:</p> 
      <ul> 
       <li> <p>Benutzer können Bilder in Aktualisierungen hinzufügen (updates:images.toggle)</p> </li> 
      </ul> <p>Dieser Parameter unterstützt die Möglichkeit, Bilder zu Arbeitselementaktualisierungen hinzuzufügen. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update der Arbeit</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Ein DocumentVersion -Objekt stellt eine bestimmte Version einer Datei dar (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

Weitere Informationen zu Dokumentversionen finden Sie unter [Eine neue Version eines Dokuments hochladen](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Hinzugefügt. In diesem Feld werden das Datum und die Uhrzeit des letzten Rückrufs aus Workfront Testversand aufgezeichnet, wenn die Version mit einem Testversand verknüpft ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppe (GRUPPE) {#group-group}

Ein Group -Objekt stellt eine Gruppe von Benutzern und Teams dar. Gruppen stellen oft die Struktur der Abteilungen dar.

Weitere Informationen zu Gruppen finden Sie unter [Gruppen vs. Teams in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Hinzugefügt. Diese Aktion akzeptiert ein Array von groupIDs und fügt diese Gruppen als Untergruppen zur angegebenen Gruppe hinzu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### HinweisTag (NTAG) {#notetag-ntag}

Ein NoteTag -Objekt stellt den Akt des Taggings eines Benutzers oder Teams bei einer Aktualisierung eines Arbeitselements dar.

Weitere Informationen zum Tagging in Aktualisierungen finden Sie unter [Tagging anderer Benutzer auf Updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Vorgänge</td> 
   <td> <p>Die folgenden Vorgänge wurden dem NoteTag-Objekt hinzugefügt:</p> 
    <ul> 
     <li> <p><b>COUNT</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>BERICHT</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projekt (PROJ) {#project-proj}

Projekte sind Arbeitselemente in Workfront und stellen einen Hauptbaustein dar, wie Workfront Menschen bei der Arbeit unterstützt. Ein Projektobjekt stellt eine Gruppe von Aufgaben mit einem gemeinsamen, spezifischen Ziel dar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Hinzugefügt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Ein QueueDef-Objekt stellt eine Warteschlange dar. Hierbei handelt es sich um ein Projekt, das in den Help Desk-Bereich veröffentlicht wurde, um Benutzern die Möglichkeit zu geben, Probleme an sie zu senden.

Weitere Informationen zu Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Hinzugefügt. Diese Aktion unterstützt die Möglichkeit, Anforderungen mithilfe des Pfads über die Anforderungswarteschlange und die Themengruppen zu finden.</p> <p>Weitere Informationen zum Durchsuchen von Anforderungswarteschlangen nach Pfad finden Sie unter <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Erstellen von Anforderungen und Generieren von Entwürfen in der Workfront-Webanwendung</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Erstellen und Senden von Adobe Workfront-Anforderungen</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Ressourcenzuweisung (RSALLO) {#resource-allocation-rsallo}

Ein Resource Allocation -Objekt stellt die Schätzung der Ressourcen dar, die für ein bestimmtes Projekt benötigt werden. Dieses Objekt wird nur im Legacy-Ressourcen-Planer verwendet. Verwenden Sie für das entsprechende Feld im neuen Ressourcenplaner Budgeted Hour (BGHR).

Das Resource Allocation -Objekt hat das Flag entfernt **REPORTABLE**.

### Rolle (ROLE) {#role-role}

Ein Rollenobjekt (Auftragsrolle) steht für eine funktionale Kapazität oder eine Fachkompetenz, die ein Benutzer ausfüllen kann, z. B. Designer oder Produkt-Manager.

Informationen zu Auftragsrollen finden Sie unter [Übersicht über die Auftragsrolle](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Hinzugefügt. Dies ist ein boolescher Parameter mit dem Wert true , wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Standardfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Hinzugefügt</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Vorlage (TMPL) {#template-tmpl}

Ein Template -Objekt stellt ein Muster für ein Projekt dar. Projekte können aus Vorlagen erstellt werden, um Zeit zu sparen. Eine Vorlage enthält ein Team und Aufgaben, die in jedes aus der Vorlage erstellte Projekt kopiert werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Hinzugefügt. Dieses Feld wurde hinzugefügt, um die Möglichkeit der Zuordnung von Gruppen zu Vorlagen zu unterstützen.</p> <p style="font-weight: normal;">Weitere Informationen finden Sie unter <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Bearbeiten von Projektvorlagen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Gruppe</p> <p style="font-weight: normal;">Hinzugefügt. Dieses Feld wurde hinzugefügt, um die Möglichkeit der Zuordnung von Gruppen zu Vorlagen zu unterstützen.</p> <p style="font-weight: normal;">Weitere Informationen finden Sie unter <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Bearbeiten von Projektvorlagen</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
