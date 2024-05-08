---
product-area: projects
navigation-topic: convert-issues
title: Übersicht über Konvertierungsprobleme in Adobe Workfront
description: Wenn nach dem Absenden des Problems noch mehr Arbeit erforderlich ist, können Sie das Problem in ein Projekt oder eine Aufgabe konvertieren.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 2%

---

# Übersicht über Konvertierungsprobleme in Adobe Workfront

Wenn nach dem Absenden des Problems noch mehr Arbeit erforderlich ist, können Sie das Problem in ein Projekt oder eine Aufgabe konvertieren.

Informationen zum Konvertieren von Problemen in Aufgaben finden Sie unter [Konvertieren eines Problems in eine Aufgabe in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md).

Informationen zum Konvertieren von Problemen in Projekte finden Sie unter [Konvertieren eines Problems in ein Projekt in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Überlegungen beim Konvertieren von Problemen

* Beim Konvertieren von Problemen in Aufgaben oder Projekte werden die meisten Informationen aus dem Problem an die Aufgabe oder das Projekt übertragen, sofern in diesem Artikel nichts anderes angegeben ist.
* Ihr Workfront-Administrator oder -Gruppenadministrator hat bereits die Voreinstellungen für das Auftreten eines Problems, dessen Lösung und den Zugriff seines Primären Kontakts bei der Konvertierung in ein Projekt oder eine Aufgabe festgelegt, wie in [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Workfront entfernt alle Genehmigungen, die mit Problemen während der Konvertierung verbunden sind.
* Workfront überschreibt das Auflösungsobjekt des Problems, wenn Sie es in eine Aufgabe oder ein Projekt konvertieren. Die neue Aufgabe oder das neue Problem wird nach der Konvertierung zum neuen Auflösungsobjekt des Problems.
* Beachten Sie Folgendes:

   * Während der Konvertierung werden Sie möglicherweise gefragt, ob Sie das Problem und seine Lösung an das Projekt oder die Aufgabe, die Sie erstellen, binden möchten.
   * Wenn Sie das Problem beibehalten, aktualisieren der Status und der Prozentsatz am Ende des Projekts oder der Aufgabe automatisch den Status und den Prozentsatz des Abschlusses des Problems, wenn Änderungen am Projekt, der Aufgabe oder dem Problem auftreten oder wenn die Workfront die Timeline neu berechnet.

* Beim Konvertieren eines Problems in eine Aufgabe oder ein Projekt wird das Problem aus dem Startbereich des dem Problem zugewiesenen Benutzers entfernt.

* Beim Konvertieren eines Problems werden die Berechtigungen für die ursprünglichen Probleme nicht an das konvertierte Objekt (Aufgabe oder Projekt) übertragen.

* Beim Konvertieren eines Problems in ein Projekt mithilfe einer Vorlage werden die meisten Informationen aus der Vorlage an das neue Projekt übertragen. Einige Informationen aus dem Problem können jedoch auch an das neue Projekt übertragen werden. Weitere Informationen finden Sie unter [Übersicht über die Projektfelder bei der Konvertierung eines Problems in ein Projekt mithilfe einer Vorlage](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) in diesem Artikel beschrieben.
* Beim Konvertieren eines Problems werden nicht alle Dokumente oder deren Informationen in das neue Objekt verschoben, in das das Problem konvertiert wird. Die folgenden Elemente sind enthalten, wenn Sie ein Problem konvertieren, an das Dokumente oder Dokumentlinks angehängt sind:

   * Dokument
   * Dokumentieren Sie Links zu Drittanbieterdiensten, z. B. Google Drive oder SharePoint.
   * Versionen
   * Testsendungen werden nur einbezogen, wenn die Option **Behalten Sie das ursprüngliche Problem bei und binden Sie die Lösung an diese Aufgabe** deaktiviert ist.
   * Dokumentgenehmigungen sind nicht enthalten, wenn Sie ein Problem konvertieren, an das Dokumente und Dokumentverknüpfungen angehängt sind.

* Wenn Sie beschlossen haben, das Problem in der Konvertierung beizubehalten und Dokumente angehängt sind, werden das Dokument und seine Versionen in das Projekt oder die Aufgabe kopiert. Die Testsendungen und Dokumentgenehmigungen werden nicht in das Projekt oder die Aufgabe kopiert.
* Wenn Sie beschlossen haben, das Problem nicht in der Konvertierung zu belassen und Dokumente angehängt sind, werden das Dokument, die Versionen und die Testsendungen an das Projekt oder die Aufgabe übertragen. Die Dokumentgenehmigungen werden nicht an das Projekt oder die Aufgabe übertragen.
* Wenn Sie Dokumente und Ordner haben, die mit dem ursprünglichen Problem von Drittanbieterdiensten wie Google Drive verknüpft sind, unabhängig davon, ob Sie das Problem während der Konvertierung beibehalten oder nicht, werden diese Links in das neue Objekt kopiert.
* Problemkommentare werden auch in die Aufgabe oder das Projekt kopiert, die/das aus dem Problem konvertiert wurde, aber getaggte Benutzer werden nicht übertragen.
* Wenn Sie benutzerdefinierte Formulardaten von einem Problem an das Projekt oder die Aufgabe übertragen möchten, in das/die Sie konvertieren, stellen Sie sicher, dass Sie über ein benutzerdefiniertes Projekt- oder Aufgabenformular verfügen, das dieselben Felder enthält, die Sie von dem Problem übertragen möchten. Weitere Informationen finden Sie unter [Übertragen benutzerdefinierter Formulardaten beim Konvertieren eines Objekts](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## Übersicht über die Projektfelder bei der Konvertierung eines Problems in ein Projekt mithilfe einer Vorlage {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

Beim Konvertieren eines Problems in ein Projekt können Sie es entweder in ein leeres Projekt konvertieren oder eine Vorlage verwenden.

Weitere Informationen finden Sie unter [Konvertieren eines Problems in ein Projekt in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

Bei Verwendung einer Vorlage werden einige Felder, die in der Vorlage ausgefüllt sind, an das aus dem konvertierten Problem erstellte Projekt übertragen. Andere Felder werden vom konvertierten Problem an das Projekt übertragen.

In der folgenden Tabelle sind die Projektinformationen aufgeführt und ob sie von der Vorlage oder aus dem Problem übertragen werden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Beschreibung</td> 
   <td> <p>Die Beschreibung der Ausgabe wird an das neue Projekt übertragen. </p> <p> Wenn es keine Beschreibung zum Problem gibt, wird die Beschreibung aus der Vorlage an das Projekt übertragen. </p> <p>Wenn das Feld Beschreibung sowohl für das Problem als auch für die Vorlage leer ist, ist das Feld im Projekt leer. </p> </td> 
  </tr> 
  <tr> 
   <td>Status</td> 
   <td>Standardstatus, der für die Gruppe in der Vorlage ausgewählt wird. Wenn die Vorlage nicht mit der Gruppe verknüpft ist, wird der Projektstatus vom Workfront-Administrator im Bereich "Projekteinstellungen"des Setups auf den Standardstatus festgelegt. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</td> 
  </tr> 
  <tr> 
   <td>Priorität</td> 
   <td><p>Übertragungen aus dem Problem.</p>
   <p>Wenn Sie eine Vorlage für das konvertierte Projekt verwenden, können Sie die Priorität manuell ändern. Wenn Sie es nicht ändern möchten, wird die Priorität des Problems an das Projekt übertragen. 
    </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>Die URL aus dem Problem wird an das neue Projekt übertragen. </p> <p> Wenn für das Problem keine URL angegeben ist, wird die URL aus der Vorlage an das Projekt übertragen. </p> <p>Wenn das Feld URL sowohl für das Problem als auch für die Vorlage leer ist, ist das Feld im Projekt leer. </p> </td> 
  </tr> 
  <tr> 
   <td>Projektbedingungstyp</td> 
   <td>Übertragungen aus der Vorlage.</td> 
  </tr> 
  <tr> 
   <td>Projektbedingung</td> 
   <td>Entspricht den Standardeinstellungen auf Systemebene, die vom Workfront-Administrator im Bereich "Setup"festgelegt wurden. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte</a></td> 
  </tr> 
  <tr> 
   <td>Planen ab</td> 
   <td>Übertragungen aus der Vorlage.</td> 
  </tr> 
  <tr> 
   <td>Projekttermine</td> 
   <td> 
    <ul> 
     <li> <p><b>Geplantes Startdatum</b>: Die nächstgelegene Arbeitszeit, die auf der Arbeitszeit des Vorlagenzeitplans basiert, sollte entsprechend der Zeitzone des Zeitplans der Vorlage vorausgewählt werden. Dieses Feld ist deaktiviert, wenn im Feld Planen von die Option Aus Abschluss ausgewählt ist. </p> </li> 
     <li> <p><b>Geplantes Abschlussdatum</b>: Die nächstgelegene Arbeitszeit, die auf der Arbeitszeit des Vorlagenzeitplans basiert, sollte entsprechend der Zeitzone des Zeitplans der Vorlage vorausgewählt werden. Dieses Feld ist deaktiviert, wenn im Feld Planung von die Option Von Start ausgewählt ist. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td> 
  </tr> 
  <tr> 
   <td>Programm</td> 
   <td>Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td> 
  </tr> 
  <tr> 
   <td>Gruppe</td> 
   <td><p> Die folgenden Szenarien existieren:</p>
     <ul><li>Wenn während der Konvertierung eine Gruppe angegeben wird, wird dies zur Gruppe des Projekts</li>
     <li>Wenn Sie mithilfe einer Vorlage in ein Projekt konvertieren und sich in der Vorlage eine Gruppe befindet und während der Konvertierung keine Gruppe angegeben wird, wird die Gruppe der Vorlage zur Gruppe des neuen Projekts</li>
      <li> Wenn keine Gruppe in der Vorlage vorhanden ist und Sie während der Konvertierung keine Gruppe angeben, wird die Gruppe des Projekts des ursprünglichen Problems zur Gruppe des neuen Projekts</li> </ul>
      </td> 
  </tr> 
  <tr> 
   <td>Firma</td>    
   <td>  Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td>

</tr> 
  <tr> 
   <td>Projektbesitzer</td> 
   <td>Übertragungen aus dem Feld Vorlageneigentümer in der Vorlage. Andernfalls wird er auf den angemeldeten Benutzer festgelegt, der die Konvertierung durchführt. </td> 
  </tr> 
  <tr> 
   <td>Projektsponsor</td> 
   <td>Übertragungen aus dem Feld "Vorlagen-Sponsor"auf der Vorlage. Andernfalls ist dieses Feld leer.</td> 
  </tr> 
  <tr> 
   <td>Ressourcenmanager</td> 
   <td>Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td> 
  </tr> 
  <tr> 
   <td>Einstellungen für die Aufgabe</td> 
   <td>Aus der Vorlage übertragen.</td> 
  </tr> 
  <tr> 
   <td>Problemeinstellungen</td> 
   <td>Aus der Vorlage übertragen. </td> 
  </tr> 
  <tr> 
   <td>Zugriff</td> 
   <td> <p>Übertragungen aus dem Bereich Zugriff auf der Vorlage. </p> </td> 
  </tr> 
  <tr> 
   <td>Genehmigungen</td> 
   <td>Aus der Vorlage übertragen. Die mit dem Problem verknüpften Genehmigungen werden während der Konvertierung entfernt. </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p>  </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p>  </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## Originalinformationen zu Problemen in Projekten und Aufgaben anzeigen {#view-original-issue-information-on-projects-and-tasks}

Sie können die ursprünglichen Probleminformationen in Projekt- und Aufgabenlisten und Berichten oder im Bereich Projektdetails anzeigen. Informationen zum Erstellen von Berichten finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Die folgende Tabelle zeigt, welche Problemfelder in den konvertierten Projekten und Aufgaben sichtbar sind.

| Problemfelder | Projekt- oder Aufgabenfeld | Projektliste oder Bericht | Bereich &quot;Projektdetails&quot; | Aufgabenliste oder Bericht | Bereich &quot;Aufgabendetails&quot; |
|---|---|---|---|---|---|
| Name des Problems | Name des konvertierten Problems | ms | ms | ms | ms |
| Hauptansprechpartner | Name des konvertierten Emittenten | ms | `✔` | ms |  |
| Eingabedatum | Problem-Eingabedatum konvertiert | ms |  | ms |  |


>[!CAUTION]
>
>Wenn sich der Primäre Kontakt eines Problems ändert oder wenn die Verknüpfung des Problems mit dem Projekt oder der Aufgabe aufgehoben wird, nachdem das Problem konvertiert wurde, wird der Name des konvertierten Emittenten nicht aktualisiert und der ursprüngliche Primäre Kontakt des Problems wird zum Zeitpunkt der Konvertierung des Problems angezeigt.
