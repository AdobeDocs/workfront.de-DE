---
content-type: overview
product-area: templates
keywords: überschreiben,Feld,überschrieben
navigation-topic: templates-navigation-topic
title: Überblick über das Anhängen einer Vorlage an ein Projekt
description: Wenn Sie eine Vorlage an ein vorhandenes Projekt anhängen, ändern Sie einige Informationen im Projekt entsprechend der Vorlage. Einige Informationen über das Projekt bleiben unverändert.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 7%

---

# Überblick über das Anhängen einer Vorlage an ein Projekt

Wenn Sie eine Vorlage an ein vorhandenes Projekt anhängen, ändern Sie einige Informationen im Projekt entsprechend der Vorlage. Einige Informationen über das Projekt bleiben unverändert.

Informationen zum Anhängen einer Vorlage an ein Projekt finden Sie unter [Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Überlegungen beim Hinzufügen von Vorlagen zu Projekten

Beachten Sie beim Hinzufügen von Vorlagen zu Projekten Folgendes:

* Sie können nur aktive Vorlagen an Projekte anhängen.
* Sie können eine Vorlage nur dann an ein Projekt anhängen, wenn sich das Projekt im Status „Abgeschlossen“, „Eingestellt“ oder „Ausstehende Genehmigung“ befindet, wenn diese Funktion von Ihrem Adobe Workfront-Administrator oder einem Gruppenadministrator im Bereich „Projektvoreinstellungen“ aktiviert wurde. Informationen zum Festlegen von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Alle Vorlagenaufgaben werden dem vorhandenen Projekt hinzugefügt, es sei denn, Sie schließen bestimmte Vorlagenaufgaben davon aus, dass sie im Anfügeprozess hinzugefügt werden.
* Die meisten Vorlageneinstellungen werden dem Projekt hinzugefügt. Einige Projekteinstellungen werden beibehalten. Weitere Informationen finden Sie im Abschnitt [Grundlegendes zu Änderungen an Projektfeldern beim Anhängen einer Vorlage](#understand-changes-to-project-fields-when-attaching-a-template) in diesem Artikel.

## Grundlegendes zu Änderungen an Projektfeldern beim Anhängen einer Vorlage {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Das Anhängen einer Vorlage an ein Projekt ist nicht dasselbe wie das Erstellen eines Projekts aus einer Vorlage. Wenn Sie ein Projekt über eine Vorlage erstellen, werden alle Vorlagenfelder in das neue Projekt übertragen. Beim Anhängen einer Vorlage bleiben einige der vorhandenen Projektfelder unverändert.

Einige Vorlageneinstellungen werden automatisch in das Projekt übertragen, es sei denn, Sie markieren sie ausdrücklich, um während des Vorlagenanfügevorgangs ausgeschlossen zu werden. Wenn Sie sie zum Ausschluss markieren, werden die Feldwerte des Projekts beibehalten.

Es stehen jedoch nicht alle Projektfelder zur Verfügung, die verwaltet werden können, wenn eine Vorlage an ein Projekt angehängt wird. Weitere Informationen finden Sie unter [Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

In der folgenden Tabelle wird beschrieben, was standardmäßig mit Projektfeldern geschieht, wenn eine Vorlage angehängt wird, und welche Felder Sie während des Anfügevorgangs verwalten können, um das Standardverhalten zu überschreiben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Feld</td> 
   <td>Was passiert standardmäßig beim Anhängen einer Vorlage?</td> 
   <td>Möglichkeit, die Feldaktualisierungen im Anlagenprozess zu verwalten </td> 
  </tr> 
  <tr> 
   <td>Beschreibung</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Status</p> </td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>Von Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Priorität</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bedingungstyp</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Zeitplanmodus</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Geplante Daten</td> 
   <td>Kann sich je nach den hinzugefügten Aufgaben ändern</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tatsächliche Termine</td> 
   <td>Kann sich je nach den hinzugefügten Aufgaben ändern</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programm</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppe</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Firma</td> 
   <td>Von Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Geplante Stunden</td> 
   <td>Kann sich je nach den hinzugefügten Aufgaben ändern</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projektbesitzer</td> 
   <td>Von Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projektsponsor</td> 
   <td>Von Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ressourcenmanager</td> 
   <td>Der Liste der im Projekt vorhandenen Ressourcenmanager hinzugefügt</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Formulare</td> 
   <td>Dem Projekt hinzugefügt, zusätzlich zu Formularen, die sich bereits im Projekt befinden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Budget</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Währung</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>PIM</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Geplanter Gewinn</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tatsächlicher Gewinn</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Meilensteinpfad</td> 
   <td>Von Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fertigstellungsmodus</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Zusammenfassung - Fertigstellungsmodus</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Update-Typ</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Zeitplan</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benutzer-Ausfallzeiten</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Abgleichsmodus für Ressourcen</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risiko (Projektfeld)</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ressourcenpools</td> 
   <td>Wurde zur Liste der vorhandenen Ressourcenpools im Projekt hinzugefügt</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Stundentypen</td> 
   <td> <p>Wenn diese Option während des Anfügevorgangs deaktiviert ist, bleibt die Einstellung „Stundentypen“ für das Projekt unverändert. </p> <p>Wenn diese Option ausgewählt ist, wird die Vorlageneinstellung auf das Projekt übertragen. Wenn die Stundentypfilterung sowohl für das Projekt als auch für die Vorlage auf Ja festgelegt ist, werden die Stundentypen aus der Vorlage zu den im Projekt enthaltenen Stundentypen hinzugefügt.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Erinnerungsnachrichten</td> 
   <td> <p>Wurde zur Liste der vorhandenen Erinnerungen für das Projekt hinzugefügt. </p> <p>Wenn diese Option während des Anfügevorgangs deaktiviert ist, bleiben die Projekterinnerungsbenachrichtigungen unverändert. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Aufgabe – Standardgenehmigungsprozess</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Aufgabe – Benutzerdefiniertes Standardformular</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Work Effort</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Benutzenden erlauben, Probleme inline hinzuzufügen</span> </td> 
   <td><span>Projektinformationen werden beibehalten</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Alle Einstellungen</td> 
   <td>Vorlageneinstellungen überschreiben die des Projekts</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgaben</td> 
   <td>Am Ende der Aufgabenliste hinzugefügt, zusätzlich zu den vorhandenen Projektaufgaben</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dokumente</td> 
   <td>Dem Projekt zusätzlich zu vorhandenen Projektdokumenten hinzugefügt</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risiken (Objekte im Risikobereich des Projekts)</td> 
   <td>Dem Projekt hinzugefügt, zusätzlich zu vorhandenen Projektrisiken </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Genehmigungsprozess</td> 
   <td>Aus Vorlage übertragen</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Abrechnungssätze</td> 
   <td> <p>Von der Vorlage zusätzlich zu den vorhandenen Abrechnungssätzen für das Projekt übertragen. </p> <p>Wenn sowohl für das Projekt als auch für die Vorlage ein unterschiedlicher Satz für dasselbe Aufgabengebiet vorhanden ist, bleibt der Satz für das Projekt unverändert. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Abrechnungseinträge</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ausgaben</td> 
   <td>Von Vorlage zusätzlich zu den bestehenden Aufwendungen für das Projekt übertragen</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Finanzinformationen</td> 
   <td> <p>Wenn dies im Anlagenprozess ausgewählt wird, werden die folgenden Felder entweder übertragen oder zum Projekt hinzugefügt: </p> 
    <ul> 
     <li> <p>Fixkosten</p> <p>Wenn die Option ausgewählt ist, werden die aktualisierten Fixkosten des Projekts anhand der folgenden Formel berechnet:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Festeinnahmen</p> <p>Wenn die Option ausgewählt ist, wird der aktualisierte feste Umsatz des Projekts anhand der folgenden Formel berechnet:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Kostentyp für Aufgaben</p> <p>Aus Vorlage übertragen</p> </li> 
     <li> <p>Umsatztyp für Aufgaben</p> <p>Aus Vorlage übertragen</p> </li> 
    </ul> <p>Wenn die Auswahl dieses Felds während des Anfügevorgangs aufgehoben wird, geschieht Folgendes:</p> 
    <ul> 
     <li> <p>Die Festkosten und Festeinnahmen für das Projekt werden beibehalten.</p> </li> 
     <li> <p>Die Kosten- und Umsatztypen für die über die Vorlage hinzugefügten Aufgaben sind auf „Keine Kosten“ und „Nicht fakturierbar“ festgelegt</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Stunden</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Warteschlangendetails, Themengruppen, Warteschlangenthemen, Routing-Regeln</td> 
   <td> <p>Aus Vorlage übertragen</p> <p>Wenn Sie die Option <strong>Warteschlangeneigenschaften und Problem-Setup</strong> während des Anfügevorgangs auswählen, überschreiben die Warteschlangendetails der Vorlage die des Projekts. In diesem Fall werden die Routing-Regeln, Warteschlangenthemen und Themengruppen der Vorlage zu denen des Projekts hinzugefügt. <br>Wenn das Projekt als Anforderungswarteschlange eingerichtet ist und die dem Projekt angehängte Vorlage nicht als Anforderungswarteschlange eingerichtet ist, werden die Warteschlangeninformationen des Projekts entfernt, wenn Sie das Kontrollkästchen <strong>Warteschlangeneigenschaften und Problemeinstellungen</strong> aktiviert lassen. <br>Wenn Sie das Kontrollkästchen <strong>Warteschlangeneigenschaften und Problem-Setup</strong> deaktivieren, bleiben alle Warteschlangeneinstellungen des Projekts erhalten und es werden keine Warteschlangeneinstellungen aus der Vorlage angehängt.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabenbeschränkungen</td> 
   <td> <p>Aus Vorlage übertragen </p> <p>Wenn diese Option während des Anfügevorgangs deaktiviert ist, werden die Aufgabenbeschränkungen auf „So bald wie möglich“ oder „So spät wie möglich“ festgelegt, je nach der Einstellung von „Projektzeitplan ab“. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabenvorgänger</td> 
   <td> <p>Aus Vorlage übertragen</p> <p>Wenn diese Option während des Anfügevorgangs deaktiviert ist, werden alle Vorgängerverbindungen zwischen den Vorlagenaufgaben entfernt.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Freigabeoptionen</td> 
   <td> <p>Wenn diese Option während des Anfügevorgangs deaktiviert wird, bleiben die Projektberechtigungen unverändert.</p> <p>Wenn diese Option während des Anfügevorgangs ausgewählt wird, werden die Vorlagenberechtigungen dem Projekt hinzugefügt bzw. überschrieben. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Benutzer A über Anzeigeberechtigungen für das Projekt verfügt, aber Verwaltungsberechtigungen für die Vorlage hat, erhält Benutzer A nach dem Anhängen der Vorlage Verwaltungszugriff auf das Projekt.</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>



<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom Forms</b>: Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p> </p>
</div>
-->


