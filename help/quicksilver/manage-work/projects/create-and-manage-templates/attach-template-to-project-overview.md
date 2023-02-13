---
content-type: overview
product-area: templates
keywords: overwrite,field,overwrite
navigation-topic: templates-navigation-topic
title: Übersicht über das Anhängen einer Vorlage an ein Projekt
description: Wenn Sie eine Vorlage an ein vorhandenes Projekt anhängen, ändern Sie einige Informationen im Projekt entsprechend der Vorlage. Einige der Angaben zum Projekt bleiben unverändert.
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 5%

---

# Übersicht über das Anhängen einer Vorlage an ein Projekt

Wenn Sie eine Vorlage an ein vorhandenes Projekt anhängen, ändern Sie einige Informationen im Projekt entsprechend der Vorlage. Einige der Angaben zum Projekt bleiben unverändert.

Informationen zum Anhängen einer Vorlage an ein Projekt finden Sie unter [Eine Vorlage an ein Projekt anhängen](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Überlegungen zum Hinzufügen von Vorlagen zu Projekten

Beachten Sie beim Hinzufügen von Vorlagen zu Projekten Folgendes:

* Sie können nur aktive Vorlagen an Projekte anhängen.
* Sie können eine Vorlage nur dann an ein Projekt anhängen, wenn der Status des Projekts &quot;Abgeschlossen&quot;, &quot;Unbeendet&quot;oder &quot;Ausstehende Genehmigung&quot;lautet, wenn der Adobe Workfront-Administrator oder ein Gruppenadministrator diese Funktion im Bereich &quot;Projekteinstellungen&quot;aktiviert hat. Weitere Informationen zum Festlegen von Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Sofern Sie bestimmte Vorlagenaufgaben nicht aus dem Anlagenprozess ausschließen, werden alle Vorlagenaufgaben zum vorhandenen Projekt hinzugefügt.
* Die meisten Vorlageneinstellungen werden dem Projekt hinzugefügt. Einige Projekteinstellungen bleiben erhalten. Weitere Informationen finden Sie im Abschnitt . [Grundlegendes zu Änderungen an Projektfeldern beim Anhängen einer Vorlage](#understand-changes-to-project-fields-when-attaching-a-template) in diesem Artikel.

## Grundlegendes zu Änderungen an Projektfeldern beim Anhängen einer Vorlage {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>Das Anhängen einer Vorlage an ein Projekt entspricht nicht dem Erstellen eines Projekts aus einer Vorlage. Wenn Sie ein Projekt aus einer Vorlage erstellen, werden alle Vorlagenfelder in das neue Projekt übertragen. Beim Anhängen einer Vorlage bleiben einige der vorhandenen Projektfelder unverändert.

Einige Vorlageneinstellungen werden automatisch in das Projekt übertragen, es sei denn, Sie markieren sie explizit, damit sie während des Vorlagenanlagenanlagenprozesses ausgeschlossen werden. Wenn Sie sie zum Ausschließen markieren, bleiben die Projektfeldwerte erhalten.

Es sind jedoch nicht alle Projektfelder verfügbar, die beim Anhängen einer Vorlage an ein Projekt verwaltet werden können. Weitere Informationen finden Sie unter [Eine Vorlage an ein Projekt anhängen](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

In der folgenden Tabelle wird beschrieben, wie die Standardeinstellungen für die Arbeit mit Projektfeldern beim Anhängen einer Vorlage und die Felder, die Sie während des Anlagenprozesses verwalten können, angewendet werden, um das Standardverhalten zu überschreiben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Feld</td> 
   <td>Was geschieht standardmäßig beim Anhängen einer Vorlage?</td> 
   <td>Möglichkeit zur Verwaltung der Feldaktualisierungen im Anlagenprozess </td> 
  </tr> 
  <tr> 
   <td>Beschreibung</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Status</p> </td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>Aus Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Priorität</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bedingungstyp</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Zeitplanmodus</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Geplante Daten</td> 
   <td>Kann sich basierend auf den hinzugefügten Aufgaben ändern</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tatsächliche Datumswerte</td> 
   <td>Kann sich basierend auf den hinzugefügten Aufgaben ändern</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programm</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppe</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Firma</td> 
   <td>Aus Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Geplante Stunden</td> 
   <td>Kann sich basierend auf den hinzugefügten Aufgaben ändern</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projektbesitzer</td> 
   <td>Aus Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projektsponsor</td> 
   <td>Aus Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ressourcenmanager</td> 
   <td>Zur Liste der vorhandenen Ressourcen-Manager im Projekt hinzugefügt</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Forms</td> 
   <td>Zum Projekt hinzugefügt, zusätzlich zu den Formularen, die sich bereits im Projekt befinden</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Budget</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Währung</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>PIM</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Geplanter Gewinn</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tatsächlicher Gewinn</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Meilensteinpfad</td> 
   <td>Aus Vorlage übertragen, wenn das Feld im Projekt leer ist</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fertigstellungsmodus</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modus für Zusammenfassungsabschluss</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Update-Typ</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Zeitplan</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Zeitlimit für Benutzer</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Abgleichsmodus für Ressourcen</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risiko (Projektfeld)</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ressourcenpools</td> 
   <td>Zur Liste der vorhandenen Ressourcen-Pools im Projekt hinzugefügt</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Stundentypen</td> 
   <td> <p>Wenn die Auswahl während des Anlagenprozesses aufgehoben wird, bleibt die Einstellung "Stündungstypen"im Projekt unverändert. </p> <p>Wenn diese Option aktiviert ist, wird die Vorlageneinstellung an das Projekt übertragen. Wenn die Filterfunktion "Stündentyp"sowohl im Projekt als auch in der Vorlage auf Ja gesetzt ist, werden die Stundentypen aus der Vorlage den im Projekt vorhandenen hinzugefügt.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Erinnerungsnachrichten</td> 
   <td> <p>Zur Liste der vorhandenen Erinnerungen zum Projekt hinzugefügt. </p> <p>Wenn die Projekterinnerungsbenachrichtigungen während des Anlagenvorgangs deaktiviert werden, bleiben sie unverändert. </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Aufgabe – Standardgenehmigungsprozess</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierter Forms für Aufgaben</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Arbeitsaufwand</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Benutzern erlauben, Probleme inline hinzuzufügen</span> </td> 
   <td><span>Projektinformationen werden beibehalten</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Alle Einstellungen</td> 
   <td>Die Vorlageneinstellungen überschreiben die des Projekts</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgaben</td> 
   <td>Zum Ende der Aufgabenliste hinzugefügt, zusätzlich zu den vorhandenen Projektaufgaben</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dokumente</td> 
   <td>Zum Projekt hinzugefügt, zusätzlich zu vorhandenen Projektdokumenten</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risiken (Objekte im Bereich "Risiken"des Projekts)</td> 
   <td>Zum Projekt hinzugefügt, zusätzlich zu den bestehenden Projektrisiken </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Genehmigungsprozess</td> 
   <td>Aus Vorlage übertragen</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Abrechnungssätze</td> 
   <td> <p>Wird von der Vorlage zusätzlich zu den bestehenden Abrechnungskursen für das Projekt übertragen. </p> <p>Wenn es für dieselbe Rolle im Auftrag sowohl für das Projekt als auch für die Vorlage eine andere Rate gibt, bleibt die Projektquote unverändert. </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Rechnungsnachweise</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ausgaben</td> 
   <td>Aus Vorlage zusätzlich zu den bestehenden Projektausgaben übertragen</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Finanzinformationen</td> 
   <td> <p>Wenn dies im Anlagenprozess ausgewählt wird, werden die folgenden Felder entweder übertragen oder zum Projekt hinzugefügt: </p> 
    <ul> 
     <li> <p>Fixkosten</p> <p>Wenn die Option ausgewählt ist, wird die aktualisierte Festkosten des Projekts mit der folgenden Formel berechnet:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>Festeinnahmen</p> <p>Wenn die Option ausgewählt ist, wird der aktualisierte feste Umsatz des Projekts mit der folgenden Formel berechnet:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>Kostentyp für Aufgaben</p> <p>Aus Vorlage übertragen</p> </li> 
     <li> <p>Umsatztyp bei Aufgaben</p> <p>Aus Vorlage übertragen</p> </li> 
    </ul> <p>Wenn dieses Feld während des Anlagenvorgangs deaktiviert wird, geschieht Folgendes:</p> 
    <ul> 
     <li> <p>Feste Kosten und fester Umsatz im Projekt bleiben erhalten.</p> </li> 
     <li> <p>Die Kosten- und Umsatztypen der aus der Vorlage hinzugefügten Aufgaben sind auf "Keine Kosten und nicht abrechenbar"eingestellt</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Stunden</td> 
   <td>Projektinformationen werden beibehalten</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Warteschlangendetails, Themengruppen, Warteschlangenthemen, Routing-Regeln</td> 
   <td> <p>Aus Vorlage übertragen</p> <p>Wenn Sie die <strong>Einrichten von Warteschlangeneigenschaften und Problemen</strong> während des Anlagenvorgangs überschreiben die Queue Details der Vorlage die des Projekts. In diesem Fall werden die Routing-Regeln, Warteschlangenthemen und Themengruppen der Vorlage zu denen des Projekts hinzugefügt. <br>Wenn das Projekt als Anforderungswarteschlange eingerichtet ist und die dem Projekt angehängte Vorlage nicht als Anforderungswarteschlange eingerichtet ist, werden die Warteschlangeninformationen des Projekts entfernt, wenn Sie das Projekt verlassen <strong>Einrichten von Warteschlangeneigenschaften und Problemen</strong> aktiviert. <br>Wenn Sie die <strong>Warteschlangeneigenschaften und Problemeinrichtung</strong> bleiben alle Einstellungen für die Warteschlangeneinstellungen des Projekts erhalten und es werden keine Einstellungen für die Warteschlangeneinrichtung aus der Vorlage angehängt.</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabenbegrenzungen</td> 
   <td> <p>Aus Vorlage übertragen </p> <p>Wenn die Aufgabenbegrenzungen während des Anlagenvorgangs deaktiviert werden, werden sie je nach Einstellung des Projektplans so bald wie möglich oder so spät wie möglich festgelegt. </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabenvorgänger</td> 
   <td> <p>Aus Vorlage übertragen</p> <p>Wenn diese Option während des Anlagenvorgangs deaktiviert wird, werden alle Vorgängerverbindungen zwischen den Vorlagenaufgaben entfernt.</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Freigabeoptionen</td> 
   <td> <p>Wenn die Projektberechtigungen während des Anlagenprozesses deaktiviert werden, bleiben sie unverändert.</p> <p>Wenn diese Option während des Anlagenvorgangs ausgewählt wird, werden die Vorlagenberechtigungen dem Projekt hinzugefügt oder es werden diese überschrieben. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Benutzer A über Ansichtsberechtigungen für das Projekt verfügt, aber über Verwaltungsberechtigungen für die Vorlage verfügt, erhält Benutzer A nach dem Anhängen der Vorlage Zugriff auf das Projekt verwalten .</p> </td> 
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
<li> <p><b>Custom&nbsp;Forms</b>:&nbsp;Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start&nbsp;From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project&nbsp;Sponsor</p> </li>
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
<p>&nbsp;</p>
</div>
-->

 
