---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 14
description: Adobe Workfront hat API Version 14 am 9. September 2021 veröffentlicht. Die API-Version 14 enthält die folgenden Änderungen gegenüber Version 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---

# Neue Funktionen in der API-Version 14

Adobe Workfront hat API Version 14 am 9. September 2021 veröffentlicht. Die API-Version 14 enthält die folgenden Änderungen gegenüber Version 14.

## Ressourcen hinzugefügt

Für API-Version 14 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API-Version 14 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen

Die folgenden Ressourcen wurden für die API-Version 14 geändert.

* [BillingRecord (BILL)](#billingrecord-bill)
* [Kategorie (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Kunde (CUST)](#customer-cust)
* [Kundenvoreinstellungen (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Gruppe (GRUPPE)](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [Projekt (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Ressourcenzuweisung (RSALLO)](#resource-allocation-rsallo)
* [Rolle (ROLE)](#role-role)
* [Vorlage (TMPL)](#template-tmpl)
* [Arbeitszeittabelle (TABELLE)](#timesheet-tshet)

### Rechnungsnachweis (BILL) {#billingrecord-bill}

Ein BillingRecord-Objekt zeichnet die Einnahmen, Stunden oder Ausgaben auf, die in Rechnung gestellt werden können. Diese Informationen können zur Erstellung von Rechnungen in einem externen Buchhaltungssystem verwendet werden.

Weitere Informationen zu Rechnungsnachweisen finden Sie unter [Rechnungsnachweise erstellen](../../manage-work/projects/project-finances/create-billing-records.md).

Das BillingRecord-Objekt hat das Flag **DATA_EXTENDIBLE** hinzugefügt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Direkte Felder</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>hinzugefügt. Eine Kategorie ist ein benutzerdefiniertes Formular. Dieser Parameter wurde hinzugefügt, um das Hinzufügen benutzerdefinierter Forms zu BillingRecord-Objekten zu unterstützen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referenzfelder</td> 
   <td> 
    <ul> 
     <li> <p><b>Kategorie</b> </p> <p>hinzugefügt. Eine Kategorie ist ein benutzerdefiniertes Formular. Dieser Parameter wurde hinzugefügt, um das Hinzufügen benutzerdefinierter Formulare zu BillingRecord-Objekten zu unterstützen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sammlungsfelder</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>hinzugefügt. Dies stellt eine Auflistung von Kategorien (benutzerdefinierte Formulare) dar, die mit dem BillingRecord-Objekt verknüpft sind.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>hinzugefügt. Diese Aktion berechnet die Ausdrücke in benutzerdefinierten Formularfeldern neu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kategorie (CTG) {#category-ctgy}

Ein Kategorieobjekt ist ein benutzerdefiniertes Formular.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Zusätzlicher möglicher Wert:</p> 
      <ul> 
       <li> <p> BILL (Billing Record)</p> </li> 
      </ul> <p>Dieser Wert wurde hinzugefügt, um das Hinzufügen benutzerdefinierter Formulare zu BillingRecord-Objekten zu unterstützen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Diese Aktion übernimmt die Parameter objID und objCode und gibt einen booleschen Wert zurück.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

Das CustomEnum-Objekt unterstützt Sie beim Konvertieren von Status-Codes in für Menschen lesbaren Text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Abfragen</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>hinzugefügt. Diese Abfrage unterstützt die Möglichkeit, Status für Gruppen und Untergruppen zu erstellen und zu verwalten. </p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Verwalten von Gruppenstatus</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kunde (CUST) {#customer-cust}

Ein Customer-Objekt stellt eine Organisation dar, die eine Instanz von Workfront verwendet.

Dies ist ein internes -Objekt.

### Kundenvoreinstellungen (CUSTPR) {#customerpreferences-custpr}

Ein CustomerPreferences-Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Workfront-Instanz festgelegt hat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Zusätzlicher möglicher Wert:</p> 
      <ul> 
       <li> <p>Benutzern erlauben, Bilder in Aktualisierungen hinzuzufügen (updates:images.toggle)</p> </li> 
      </ul> <p>Dieser Parameter unterstützt die Möglichkeit, Bilder zu Arbeitselementaktualisierungen hinzuzufügen. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Arbeit aktualisieren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Ein DocumentVersion-Objekt stellt eine bestimmte Version einer Datei dar (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

Weitere Informationen zu Dokumentversionen finden Sie unter [Hochladen einer neuen Version eines Dokuments](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>hinzugefügt. In diesem Feld werden Datum und Uhrzeit des letzten Rückrufs von Workfront Proof aufgezeichnet, wenn die Version mit einem Korrekturabzug verknüpft ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Gruppe (GROUP) {#group-group}

Ein Gruppenobjekt steht für eine Gruppe von Benutzern und Teams. Gruppen repräsentieren oft die Abteilungsstruktur.

Weitere Informationen zu Gruppen finden Sie unter [Gruppen im Vergleich zu Teams in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>hinzugefügt. Diese Aktion verwendet ein Array von groupIDs und fügt diese Gruppen als Untergruppen zur angegebenen Gruppe hinzu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Notiz-Tag (NTAG) {#notetag-ntag}

Ein NoteTag -Objekt stellt den Vorgang des Taggens eines Benutzers oder Teams in einer Aktualisierung eines Arbeitselements dar.

Weitere Informationen zum Tagging in Aktualisierungen finden Sie unter [Andere in Aktualisierungen taggen](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Vorgänge</td> 
   <td> <p>Die folgenden Vorgänge wurden zum NoteTag -Objekt hinzugefügt:</p> 
    <ul> 
     <li> <p><b>ANZAHL</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>BERICHT</b> </p> </li> 
     <li> <p><b>SUCHE</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projekt (PROJ) {#project-proj}

Projekte sind Arbeitselemente innerhalb von Workfront und ein wichtiger Baustein in der Art und Weise, wie Workfront Menschen bei der Arbeit unterstützt. Ein Project-Objekt stellt eine Gruppe von Aufgaben mit einem gemeinsamen, spezifischen Ziel dar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>hinzugefügt.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Ein QueueDef -Objekt stellt eine Warteschlange dar. Dabei handelt es sich um ein Projekt, das im Helpdesk-Bereich veröffentlicht wurde, um Benutzenden die Übermittlung von Problemen zu ermöglichen.

Weitere Informationen zu Anfrage-Warteschlangen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aktionen</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>hinzugefügt. Diese Aktion unterstützt die Möglichkeit, Anfragen mithilfe des Pfads über die Anfragewarteschlange und Themengruppen zu finden.</p> <p>Weitere Informationen zum Suchen von Anfrage-Warteschlangen nach Pfad finden Sie unter <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Erstellen von Anfragen und Generieren von Entwürfen in der Workfront-Web</a>App) in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Erstellen und Senden von Adobe Workfront-Anfragen</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Ressourcenzuteilung (RSALLO) {#resource-allocation-rsallo}

Ein Ressourcenzuordnungsobjekt stellt die Schätzung der für ein bestimmtes Projekt benötigten Ressourcen dar. Dieses Objekt wird nur im alten Ressourcenplaner verwendet. Verwenden Sie für das entsprechende Feld im neuen Ressourcenplaner die Option Budgetierte Stunde (BGHR).

Das Ressourcenzuordnungsobjekt hat das Flag &quot;**&quot;**.

### Rolle (ROLE) {#role-role}

Ein Rollenobjekt (Aufgabengebiet) stellt eine funktionale Kapazität oder eine Qualifikation dar, die ein Benutzer ausfüllen kann, z. B. Designer oder Product Manager.

Informationen zu Aufgabengebieten finden Sie unter [Aufgabengebiet - Übersicht](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">hinzugefügt. Dies ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt „Active“ ist, und den Wert „false“, wenn es nicht ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden.</p> </li> 
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

Ein Vorlagenobjekt stellt ein Muster für ein Projekt dar. Projekte können aus Vorlagen erstellt werden, um Zeit zu sparen. Eine Vorlage enthält ein Team und Aufgaben, die in jedes aus der Vorlage erstellte Projekt kopiert werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direkte Felder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">hinzugefügt. Dieses Feld wurde hinzugefügt, um die Zuordnung von Gruppen zu Vorlagen zu unterstützen.</p> <p style="font-weight: normal;">Weitere Informationen finden Sie unter <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Projektvorlagen bearbeiten</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Referenzfelder</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Gruppe</p> <p style="font-weight: normal;">hinzugefügt. Dieses Feld wurde hinzugefügt, um die Zuordnung von Gruppen zu Vorlagen zu unterstützen.</p> <p style="font-weight: normal;">Weitere Informationen finden Sie unter <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Projektvorlagen bearbeiten</a>.</p> </li> 
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
