---
product-area: projects
navigation-topic: convert-issues
title: Übersicht über Konvertierungsprobleme in Adobe Workfront
description: Wenn nach dem Übermitteln eines Problems weitere Arbeit zum Abschließen des Problems erforderlich ist, können Sie das Problem in ein Projekt oder eine Aufgabe konvertieren.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1497'
ht-degree: 2%

---

# Übersicht über die Konvertierung von Problemen in Adobe Workfront

<!--Audited: 08/2025-->

Wenn nach dem Übermitteln eines Problems weitere Arbeit zum Abschließen des Problems erforderlich ist, können Sie das Problem in ein Projekt oder eine Aufgabe konvertieren.

Informationen zum Konvertieren von Problemen in Aufgaben finden Sie unter [Konvertieren eines Problems in eine Aufgabe](../../../manage-work/issues/convert-issues/convert-issue-to-task.md).

Informationen zum Konvertieren von Problemen in Projekte finden Sie unter [Konvertieren eines Problems in ein Projekt](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Überlegungen beim Konvertieren von Problemen

* Wenn Probleme in Aufgaben oder Projekte konvertiert werden, werden die meisten Informationen aus dem Problem an die Aufgabe oder das Projekt übertragen, sofern in diesem Artikel nichts anderes festgelegt ist.
* Ihr Workfront-Administrator oder Gruppenadministrator hat bereits die Voreinstellungen für ein Problem, seine Lösung und den Zugriff seines Primären Kontakts bei der Konvertierung in ein Projekt oder eine Aufgabe festgelegt, wie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) beschrieben.
* Workfront entfernt alle Genehmigungen, die mit Problemen während der Konvertierung verbunden sind.
* Workfront überschreibt das Lösungsobjekt des Problems, wenn Sie es in eine Aufgabe oder ein Projekt konvertieren. Die neue Aufgabe oder das neue Problem wird nach der Konvertierung zum neuen Lösungsobjekt des Problems.
* Beachten Sie Folgendes:

   * Während der Konvertierung werden Sie möglicherweise gefragt, ob Sie das Problem und seine Lösung an das Projekt oder die Aufgabe binden möchten, das bzw. die Sie erstellen.
   * Wenn Sie das Problem beibehalten, werden der Status und der abgeschlossene Prozentsatz des Projekts oder der Aufgabe automatisch aktualisiert, wenn Änderungen am Projekt, an der Aufgabe oder an dem Problem auftreten oder wenn Workfront die Timeline neu berechnet.

  >[!NOTE]
  >
  >   Nachdem der Status des Problems zu Geschlossen wird (infolge des Schließens der Aufgabe oder des Projekts), und zwar unabhängig davon, in welchen Status sich die Aufgabe oder das Projekt nach dem Schließen ändert, bleibt das Problem geschlossen.


* Beim Konvertieren eines Problems in eine Aufgabe oder ein Projekt wird das Problem aus dem Bereich „Startseite“ des Benutzers entfernt, der dem Problem zugewiesen wurde.

* Beim Konvertieren eines Problems werden die Berechtigungen für die ursprünglichen Probleme nicht an das konvertierte Objekt (Aufgabe oder Projekt) übertragen.

* Wenn ein Problem mithilfe einer Vorlage in ein Projekt konvertiert wird, werden die meisten Informationen aus der Vorlage an das neue Projekt übertragen. Einige Informationen aus dem Problem können jedoch auch auf das neue Projekt übertragen werden. Weitere Informationen finden Sie im Abschnitt [Übersicht über Projektfelder beim Konvertieren eines Problems in ein Projekt mithilfe einer Vorlage](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) in diesem Artikel.
* Beim Konvertieren eines Problems werden nicht alle Dokumente oder deren Informationen in das neue Objekt verschoben, in das das Problem konvertiert wird. Die folgenden Elemente sind enthalten, wenn Sie ein Problem konvertieren, an das Dokumente oder Dokument-Links angehängt sind:

   * Dokument
   * Dokument-Links zu Services von Drittanbietern, wie Google Drive oder SharePoint.
   * Versionen
   * Korrekturabzüge werden nur einbezogen, wenn die Option **Ursprüngliches Problem beibehalten und seine Lösung mit dieser Aufgabe verknüpfen** nicht ausgewählt ist.
   * Dokumentgenehmigungen werden nicht einbezogen, wenn Sie ein Problem konvertieren, an das Dokumente und Dokument-Links angehängt sind.
* Beim Konvertieren eines Problems gibt es ein Verarbeitungslimit von 5 Minuten. Wenn an das Problem eine große Anzahl von Dokumenten angehängt ist und es nicht konvertiert werden kann, müssen Sie möglicherweise einige der Dokumente entfernen und erneut versuchen.
* Wenn Sie sich entschieden haben, das Problem bei der Konvertierung zu belassen und ihm Dokumente beigefügt sind, werden das Dokument und seine Versionen in das Projekt oder die Aufgabe kopiert. Die Korrekturabzüge und Dokumentgenehmigungen werden nicht in das Projekt oder die Aufgabe kopiert.
* Wenn Sie sich dafür entschieden haben, das Problem nicht in der Konvertierung zu belassen und ihm Dokumente beigefügt sind, werden das Dokument, seine Versionen und die Korrekturabzüge an das Projekt oder die Aufgabe übertragen. Die Dokumentengenehmigungen werden nicht auf das Projekt oder die Aufgabe übertragen.
* Wenn Sie Dokumente und Ordner haben, die mit dem ursprünglichen Problem von Drittanbieterdiensten wie Google Drive verknüpft sind, unabhängig davon, ob Sie das Problem während der Konvertierung beibehalten oder nicht, werden diese Links in das neue Objekt kopiert.
* Problemkommentare werden auch in die Aufgabe oder das Projekt kopiert, die bzw. das aus dem Problem konvertiert wurde, getaggte Benutzende werden jedoch nicht übertragen.
* Wenn Sie benutzerdefinierte Formularinformationen von dem Problem an das Projekt oder die Aufgabe übertragen möchten, in das bzw. die Sie sie konvertieren, stellen Sie sicher, dass Sie über ein benutzerdefiniertes Projekt oder eine Aufgabe verfügen, das bzw. die dieselben Felder enthält, die Sie auch von dem Problem übertragen möchten. Weitere Informationen finden Sie unter [Übertragen von benutzerdefinierten Formulardaten beim Konvertieren eines Objekts](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## Übersicht über Projektfelder beim Konvertieren eines Problems in ein Projekt mithilfe einer Vorlage {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

Wenn Sie ein Problem in ein Projekt konvertieren, können Sie es entweder in ein leeres Projekt konvertieren oder eine Vorlage verwenden.

Weitere Informationen finden Sie unter [Problem in ein Projekt konvertieren](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

Wenn Sie eine Vorlage verwenden, werden einige Felder, die in der Vorlage ausgefüllt sind, an das aus dem konvertierten Problem erstellte Projekt übertragen. Andere Felder werden von dem konvertierten Problem an das Projekt übertragen.

In der folgenden Tabelle sind die Projektinformationen aufgeführt und es wird angegeben, ob sie von der Vorlage oder von der Anfrage übertragen werden:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Beschreibung</td> 
   <td> <p>Die Beschreibung des Problems wird auf das neue Projekt übertragen. </p> <p> Wenn keine Beschreibung des Problems vorhanden ist, wird die Beschreibung aus der Vorlage in das Projekt übertragen. </p> <p>Wenn das Beschreibungsfeld sowohl für das Problem als auch für die Vorlage leer ist, ist das Feld im Projekt leer. </p> </td> 
  </tr> 
  <tr> 
   <td>Status</td> 
   <td>Für die Gruppe in der Vorlage ausgewählter Standardstatus. Wenn die Vorlage nicht mit der Gruppe verknüpft ist, wird der Projektstatus auf den Standardstatus gesetzt, den der Workfront-Administrator im Bereich Projektvoreinstellungen von Setup festgelegt hat. Weitere Informationen finden <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> unter „Systemweite Projektvoreinstellungen konfigurieren</a>.</td> 
  </tr> 
  <tr> 
   <td>Priorität</td> 
   <td><p>Übertragungen aus dem Problem.</p>
   <p>Wenn Sie eine Vorlage für das konvertierte Projekt verwenden, haben Sie die Möglichkeit, die Priorität manuell zu ändern. Wenn Sie die Anfrage nicht ändern möchten, wird die Priorität der Anfrage auf das Projekt übertragen. 
    </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>Die URL des Problems wird an das neue Projekt übertragen. </p> <p> Wenn für das Problem keine URL angegeben ist, wird die URL von der Vorlage an das Projekt übertragen. </p> <p>Wenn das URL-Feld sowohl für das Problem als auch für die Vorlage leer ist, ist das Feld im Projekt leer. </p> </td> 
  </tr> 
  <tr> 
   <td>Projektbedingungstyp</td> 
   <td>Übertragungen aus der Vorlage.</td> 
  </tr> 
  <tr> 
   <td>Projektbedingung</td> 
   <td>Entspricht der vom Workfront-Administrator im Bereich Setup festgelegten Standardeinstellung auf Systemebene. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte</a></td> 
  </tr> 
  <tr> 
   <td>Planen ab</td> 
   <td>Übertragungen aus der Vorlage.</td> 
  </tr> 
  <tr> 
   <td>Projekttermine</td> 
   <td> 
    <ul> 
     <li> <p><b>Geplantes Startdatum</b>: Die auf der Arbeitszeit des Vorlagenplans basierende nächstgelegene Arbeitszeit sollte entsprechend der Zeitzone des Vorlagenplans vorab ausgewählt werden. Dieses Feld ist deaktiviert, wenn das Feld Zeitplan ab auf „Von Fertigstellung“ gesetzt ist. </p> </li> 
     <li> <p><b>Geplantes Abschlussdatum</b>: Die auf der Arbeitszeit des Vorlagenplans basierende nächstgelegene Arbeitszeit sollte entsprechend der Zeitzone des Vorlagenplans vorausgewählt werden. Dieses Feld ist deaktiviert, wenn das Feld „Zeitplan ab“ auf „Von Start“ gesetzt ist. </p> </li> 
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
   <td><p> Die folgenden Szenarien sind vorhanden:</p>
     <ul><li>Wenn während der Konvertierung eine Gruppe angegeben wird, wird diese zur Gruppe des Projekts</li>
     <li>Wenn Sie mithilfe einer Vorlage in ein Projekt konvertieren und die Vorlage eine Gruppe enthält und Sie während der Konvertierung keine Gruppe angeben, wird die Gruppe der Vorlage zur Gruppe des neuen Projekts</li>
      <li> Wenn in der Vorlage keine Gruppe vorhanden ist und Sie während der Konvertierung keine Gruppe angeben, wird die Gruppe des Projekts der ursprünglichen Anfrage zur Gruppe des neuen Projekts</li> </ul>
      </td> 
  </tr> 
  <tr> 
   <td>Firma</td>    
   <td>  Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td>

</tr> 
  <tr> 
   <td>Projektbesitzer</td> 
   <td>Übertragungen aus dem Feld Vorlagenbesitzer in der Vorlage. Andernfalls wird sie auf den angemeldeten Benutzer festgelegt, der die Konvertierung durchführt. </td> 
  </tr> 
  <tr> 
   <td>Projektsponsor</td> 
   <td>Übertragungen aus dem Feld Vorlagen-Sponsor auf der Vorlage. Andernfalls ist dieses Feld leer.</td> 
  </tr> 
  <tr> 
   <td>Ressourcenmanager</td> 
   <td>Übertragungen aus der Vorlage. Andernfalls ist dieses Feld leer.</td> 
  </tr> 
  <tr> 
   <td>Einstellungen für die Aufgabe</td> 
   <td>Übertragung aus der Vorlage.</td> 
  </tr> 
  <tr> 
   <td>Problemeinstellungen</td> 
   <td>Übertragung aus der Vorlage. </td> 
  </tr> 
  <tr> 
   <td>Zugriff</td> 
   <td> <p>Übertragungen aus dem Abschnitt Zugriff auf die Vorlage. </p> </td> 
  </tr> 
  <tr> 
   <td>Genehmigungen</td> 
   <td>Übertragung aus der Vorlage. Die mit dem Problem verbundenen Genehmigungen werden während der Konvertierung entfernt. </td> 
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

## Anzeigen der ursprünglichen Anfrageinformationen zu Projekten und Aufgaben {#view-original-issue-information-on-projects-and-tasks}

Sie können die ursprünglichen Anfrageinformationen in Projekt- und Aufgabenlisten und Berichten oder im Bereich Projektdetails anzeigen. Informationen zum Erstellen von Berichten finden Sie [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Die folgende Tabelle zeigt, welche Problemfelder in den konvertierten Projekten und Aufgaben sichtbar sind.

| Problemfelder | Projekt- oder Aufgabenfeld | Projektliste oder Bericht | Bereich „Projektdetails“ | Aufgabenliste oder Bericht | Aufgabendetailbereich |
|---|---|---|---|---|---|
| Name des Problems | Name des konvertierten Problems | ✔ | ✔ | ✔ | ✔ |
| Hauptansprechpartner | Name des Urhebers des konvertierten Problems | ✔ | `✔` | ✔ |  |
| Eingabedatum | Problem-Eingabedatum konvertiert | ✔ |  | ✔ |  |


>[!CAUTION]
>
>Wenn sich der Primäre Kontakt eines Problems ändert oder die Verknüpfung des Problems mit dem Projekt oder der Aufgabe nach der Konvertierung des Problems aufgehoben wird, wird der Name des konvertierten Problemverursachers nicht aktualisiert und der ursprüngliche Primäre Kontakt des Problems zum Zeitpunkt der Konvertierung des Problems wird angezeigt.
