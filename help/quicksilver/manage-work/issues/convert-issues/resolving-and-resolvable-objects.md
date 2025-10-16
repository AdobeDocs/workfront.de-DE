---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: Übersicht über das Auflösen und das Auflösen von Objekten
description: Ein lösbares Objekt ist ein Problem, dessen Auflösung an ein Lösungsobjekt gebunden ist. Ein Lösungsobjekt ist ein Projekt, eine Aufgabe oder ein anderes Problem.
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1760'
ht-degree: 2%

---

# Übersicht über das Auflösen und das Auflösen von Objekten

<!-- Audited: 08/2025 -->

Ein lösbares Objekt ist ein Problem, dessen Auflösung an ein Lösungsobjekt gebunden ist. Ein Lösungsobjekt ist ein Projekt, eine Aufgabe oder ein anderes Problem.

Wenn Sie ein Problem in eine Aufgabe oder ein Projekt konvertieren, wird das Problem zum lösbaren Objekt der Aufgabe oder des Projekts.

Sie können ein Problem auch manuell mit einem Lösungsobjekt verknüpfen, bei dem es sich um eine Aufgabe, ein Projekt oder ein Problem handeln kann. Weitere Informationen finden Sie unter [Manuelles Verknüpfen der Lösung eines Problems mit anderen Problemen, Aufgaben oder Projekten](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md).

In diesem Szenario wird das ursprüngliche Problem zum lösbaren Objekt der Aufgabe, des Projekts oder des Problems.

## Einrichten von Adobe Workfront für die Verarbeitung auflösbarer Objekte {#set-up-adobe-workfront-to-handle-resolvable-objects}

Als Workfront-Administrator oder Gruppenadministrator können Sie entscheiden, wie Sie die lösbaren Objekte in Ihrem System oder für Ihre Gruppe verarbeiten möchten.

Sie können auswählen, ob das auflösbare Objekt beim Konvertieren in eine Aufgabe oder ein Projekt beibehalten oder gelöscht werden soll, sobald die Aufgabe oder das Projekt erstellt wurde. Sie können auswählen, ob diese Einstellungen während der Konvertierung von Problemen geändert werden können. Dadurch kann der/die Benutzende, der/die die Probleme konvertiert, auswählen, ob das Problem während der Konvertierung beibehalten oder gelöscht werden soll.

>[!NOTE]
>
>Lösbare Objekte sind immer Probleme, deren Auflösung und Status von der Auflösung und dem Status des Lösungsobjekts abhängen können, mit dem sie verknüpft sind. Das Auflösen von Objekten kann Probleme, Aufgaben oder Projekte sein.

Informationen zum Einrichten von Voreinstellungen für die Verarbeitung von lösbaren Objekten finden Sie unter [Systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: drafted and just pointed the user to the article linked above)&nbsp;</p>
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to Workfront as a Workfront administrator <span>or group administrator.</span></li>
<li value="2"> <p>  From the main menu, click <strong>Setup</strong>. </p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x521.png" style="width: 350;height: 521;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <strong>Project Preferences</strong>.</li>
<li value="4">Click <strong>Tasks & Issues</strong>.</li>
<li value="5">Go to the <strong>Issues</strong> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><strong>Automatically update Resolvable Issue status when the status of the Resolving Object changes:</strong> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <strong>Keep the original issue and tie its resolution to the task</strong> or<strong>project</strong> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><strong>When converting an issue to a TASK...:</strong> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><strong>Keep the original issue and tie its resolution to the task:</strong> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><strong>Allow Primary Contact to have access to the task:</strong> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><strong>When converting an issue to a PROJECT...:</strong> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><strong>Keep the original issue and tie its resolution to the project:</strong> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><strong>Allow Primary Contact to have access to the project:</strong> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Behandeln des lösbaren Objekts während der Konvertierung in ein Projekt oder eine Aufgabe

Je nachdem, wie der Workfront- oder Gruppen-Administrator die Problemeinstellungen auf System- oder Gruppenebene konfiguriert hat, können Sie das lösbare Objekt während der Konvertierung eines Problems in ein Projekt oder eine Aufgabe verarbeiten.

Die folgenden Szenarien sind vorhanden:

* Wenn der Workfront- oder Gruppenadministrator die Option „Ursprüngliches Problem beibehalten“ hat und seine Lösung mit der Aufgabe verknüpfen und die Option „Ursprüngliches Problem beibehalten“ hat und seine Lösung mit dem ausgewählten Projekt verknüpft ist und die Option „Zulassen, dass diese Einstellungen während der Konvertierung geändert werden“ deaktiviert ist, können Sie diese Einstellungen beim Konvertieren von Problemen in Aufgaben oder Projekte nicht ändern.\
  ![Bereich „Projektvoreinstellungen - Probleme“](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* Wenn der Workfront- oder Gruppen-Administrator bzw. die Gruppenadministratorin die Option Ursprüngliches Problem beibehalten und seine Lösung mit der Aufgabe verknüpfen sowie das ursprüngliche Problem beibehalten und seine Lösung mit dem ausgewählten oder nicht ausgewählten Projekt verknüpfen kann und die Option Zulassen, dass diese Einstellungen während der Konvertierung geändert werden ausgewählt ist, können Sie diese Einstellungen ändern, während Sie Probleme in Aufgaben oder Projekte konvertieren.\
  ![Option zum Beibehalten des Problems](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

Weitere Informationen zum Konvertieren von Problemen in Aufgaben und Projekte finden Sie unter [Übersicht über das Konvertieren von Problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Tie the resolution of an issue to a project, task or </h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: created new article for this section; draft when the article is live and see if you need to make a link from this one to the new article) </p>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p>  </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form,  click in the <strong>Resolved By</strong> field,  and select from the following types of resolving objects:
<ul>
<li><strong>Project</strong></li>
<li><strong>Task</strong></li>
<li><p><strong>Issue</strong></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <strong>Save</strong>&nbsp;<strong>Changes</strong>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## Synchronisieren Sie den Status des auflösbaren Objekts mit dem des auflösenden Objekts {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [Status synchronisieren, wenn das anfragelösende Objekt ein Problem ist](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [Synchronisieren von Status, wenn das Lösungsobjekt eine Aufgabe oder ein Projekt ist](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### Synchronisieren von Status, wenn das anfragelösende Objekt ein Problem ist {#synchronize-statuses-when-the-resolving-object-is-an-issue}

Wenn ein Problem manuell mit einem anderen Problem verknüpft wird, ändert der Status des zweiten Problems (Lösungsobjekt) den Status des ersten Problems (lösbares Objekt) Trigger. Der Status des ersten Problems entspricht dem Status, in den das zweite Problem geändert wird. Dies gilt sowohl für den standardmäßigen als auch für den benutzerdefinierten Problemstatus.

### Synchronisieren von Status, wenn das Lösungsobjekt eine Aufgabe oder ein Projekt ist {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

Wenn ein Problem das lösbare Objekt einer Aufgabe oder eines Projekts ist, ändern sich der Status der Aufgaben und der Projektstatus im Trigger des Problems. Standardstatus werden in diesem Fall anders ausgelöst als benutzerdefinierter Status.

Wenn der benutzerdefinierte Status eines Projekts einem Standardstatus entspricht, der keine Änderung des Problemstatus Trigger, wird durch die Änderung des Projektstatus keine Statusänderung für das Problem Trigger.

* [Synchronisieren Sie den Standardstatus des Lösungsobjekts mit dem Standardstatus des lösbaren Objekts](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [Synchronisieren Sie den benutzerdefinierten Status des Lösungsobjekts mit dem benutzerdefinierten Status des lösbaren Objekts.](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### Synchronisieren Sie den Standardstatus des Lösungsobjekts mit dem Standardstatus des lösbaren Objekts. {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

Unabhängig davon, ob die Option Status „Lösbares Problem automatisch aktualisieren“ aktiviert ist, wenn sich der Status des Lösungsobjekts ändert, ändert sich der Status des lösbaren Objekts (Probleme) entsprechend, wenn sich der Standardstatus für die Lösungsobjekte (Projekte oder Aufgaben) ändert. Nur Standardstatus sind bereits Triggern wie dieser zugeordnet.

Der Trigger der folgenden Standardaufgabe ändert die Standardanfragestatus, wenn das Problem als Lösungsobjekt der Aufgabe festgelegt wird:

| **AUFGABENSTATUS** | **PROBLEMSTATUS** |
|---|---|
| Neu | Neu |
| In Arbeit | In Arbeit |
| Abgeschlossen | Geschlossen |

Der folgende Trigger des Standardprojekts zeigt die folgenden Änderungen am Standardproblemstatus an, wenn das Problem als lösbares Objekt eines Projekts festgelegt wird. Bei einigen Projektstatus werden keine Trigger-Änderungen an den Problemstatus vorgenommen. Die Probleme verbleiben in dem Status, in dem sie sich befanden, bevor das Projekt in einen der folgenden Status umgewandelt wurde:

| **PROJEKTSTATUS** | **PROBLEMSTATUS** |
|---|---|
| In Planung | Neu |
| Aktuell | In Arbeit |
| Zurückgestellt | Zurückgestellt |
| Angefordert | Ändert den Problemstatus nicht in einen Trigger |
| Genehmigt | Ändert den Problemstatus nicht in einen Trigger |
| Abgelehnt | Ändert den Problemstatus nicht in einen Trigger |
| Idee | Ändert den Problemstatus nicht in einen Trigger |
| Eingestellt | Geschlossen |
| Abgeschlossen | Geschlossen |

>[!NOTE]
>
>Nachdem der Anfragestatus zu Geschlossen wird (infolge des Schließens der Aufgabe oder des Projekts), und zwar unabhängig davon, wie sich der Aufgaben- oder Projektstatus nach dem Schließen ändert, bleibt das Problem geschlossen.

#### Synchronisieren Sie den benutzerdefinierten Status des Lösungsobjekts mit dem benutzerdefinierten Status des lösbaren Objekts. {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

Wenn Sie den Status der Aufgabe oder des Projekts in einen benutzerdefinierten Status ändern, ändert sich der Problemstatus nur dann in einen benutzerdefinierten Problemstatus, wenn die folgenden zwei Bedingungen erfüllt sind:

* Die Option Problemstatus automatisch aktualisieren, wenn der Status des Lösungsobjekts sich ändert ausgewählt ist. Weitere Informationen finden Sie unter [Einrichten von Adobe Workfront für die Verarbeitung von lösbaren Objekten](#set-up-adobe-workfront-to-handle-resolvable-objects).

* Der benutzerdefinierte Status des Projekts oder der Aufgabe hat denselben aus drei Buchstaben bestehenden Code wie der benutzerdefinierte Status des Problems.

Sie können benutzerdefinierte Status mit demselben Schlüssel sowohl für Probleme als auch für Projekte oder Aufgaben erstellen. Wenn das Projekt oder die Aufgabe (als Lösungsobjekt) in den benutzerdefinierten Status geändert wird, spiegelt die Änderung auch den Problemstatus wider. Der Statusschlüssel muss für den Problem- und Projekt- oder Aufgabenstatus identisch sein.

Angenommen, Sie erstellen ein benutzerdefinierter Projektstatus mit dem Namen „Launch“ mit dem aus drei Buchstaben bestehenden LCD-Code, was dem aktuellen entspricht. Als Nächstes erstellen Sie einen benutzerdefinierten Problemstatus mit dem Namen „Projekt gestartet“, auch mit dem Buchstaben-Code-LCD, der mit „In Bearbeitung“ übereinstimmt. Wenn Sie das Projekt als gestartet markieren, ändert das Problem automatisch den Status in Projekt gestartet. Wenn der Status „Lösbares Problem automatisch aktualisieren“ nicht aktiviert ist, wenn der Status des Lösungsobjekts sich ändert, ändert sich stattdessen der Problemstatus in „In Bearbeitung“.

Weitere Informationen zum Erstellen eines benutzerdefinierten Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Synchronisieren Sie den Prozentwert der Fertigstellung eines Lösungsobjekts mit dem des lösbaren Objekts.

Wenn ein Problem durch eine Aufgabe oder ein Projekt gelöst wird, wird der Prozentsatz der Fertigstellung des Problems auf dem lösbaren Problem aktualisiert, wenn eine der folgenden Situationen eintritt:

* Wenn jemand eine Änderung an der Aufgabe oder dem Projekt speichert.
* Wenn die Zeitleiste des Projekts neu berechnet wird.

Wenn ein Problem durch ein anderes Problem behoben wird, wird der Prozentsatz der abgeschlossenen Probleme aktualisiert, wenn eines der Probleme aktualisiert wird.

## Suchen des lösbaren Objekts in einer Aufgabe oder einem Projekt

>[!NOTE]
>
>Um die Schritte in diesem Abschnitt ausführen zu können, müssen Sie mindestens über Anzeigezugriff auf Aufgaben und Projekte sowie über Anzeigeberechtigungen für die Aufgabe oder das Projekt verfügen, die bzw. das das auflösbare Objekt enthält, das Sie anzeigen möchten.

Das Auffinden des Lösungsobjekts ist für Aufgaben und Projekte identisch.

1. Navigieren Sie zu einem Projekt oder einer Aufgabe, das/die Sie durch Konvertieren eines Problems erstellt haben.
1. Wählen Sie links auf der Seite die Registerkarte **Aufgabendetails** oder **Projektdetails** aus.
1. Suchen Sie unten im Abschnitt **Übersicht** das Feld **Dies löst**, in dem das lösbare Objekt der Aufgabe oder des Projekts angezeigt wird.

   ![Dieses Feld wird aufgelöst](assets/this-resolves-field.png)

   >[!NOTE]
   >
   >Probleme können nicht in andere Probleme konvertiert werden, sie können jedoch manuell mit einem Problem verknüpft werden, das gelöst wird. Ein Projekt, eine Aufgabe oder ein Problem kann mehrere Probleme als lösbare Objekte haben. Wenn das Projekt, die Aufgabe oder das Problem aufgelöst wird, wird auch das lösbare Objekt (Problem) aufgelöst. Das lösbare Problem bleibt auch dann geschlossen, wenn das Projekt, die Aufgabe oder das Problem, das bzw. das es gelöst hat, erneut geöffnet wird.

## Identifizieren eines Problems mit einem Lösungsobjekt in einer Liste

In einer Liste von Problemen können Sie Probleme, die als Lösungsobjekte gekennzeichnet sind, über Statussymbole identifizieren, indem Sie dieses Symbol in den Spalten **Statussymbole** oder **Flags** suchen:

![Problemlösendes Objekt](assets/resolving-icon.png)

## Anzeigen von Informationen zu auflösbaren und auflösenden Objekten in einem Bericht

Sie können Informationen zu den lösbaren oder auflösenden Objekten in der Ansicht oder im Bericht für Projekte, Aufgaben oder Probleme anzeigen.

Die folgende Tabelle zeigt, welche Felder angezeigt werden können und in welchen Ansichten sie angezeigt werden können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Feld in der Ansicht</strong> </th> 
   <th><strong>Anfrageansicht</strong> </th> 
   <th><strong>Aufgabenansicht</strong> </th> 
   <th><strong>Projektansicht</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Hat lösbare Probleme</strong>: Zeigt einen Wert „True“ an, wenn dem Projekt oder der Aufgabe lösbare Probleme zugeordnet sind, und einen Wert „False“, wenn dies nicht der Fall ist.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>Name des ursprünglichen Problems, ursprüngliches Problem-Eingabedatum, Name des Absenders</strong>: Zeigt den Namen und das Eingabedatum des ursprünglichen Problems sowie den Namen des Benutzers an, der das Problem in einer benutzerdefinierten Textmodus-Ansicht erstellt hat.<br>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">Anzeigen: ursprüngliche Probleminformationen in Aufgaben- oder Projektlisten anzeigen</a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lösbare Objekte:</strong> Zeigt eine Liste aller lösbaren Objekte in einer benutzerdefinierten Textmodusansicht für einen Projekt- oder Aufgabenbericht oder eine Liste an.</p> <p>Weitere Informationen finden Sie unter <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">Ansicht: Auflösbare Objekte in einem Aufgaben- oder Projektbericht</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong>Urheber eines konvertierten Problems</strong>: Zeigt Informationen zu dem Benutzer an, der das Problem ursprünglich protokolliert hat, das später in die Aufgabe konvertiert wurde. </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Projekt auflösen</strong>: Zeigt Informationen zum auflösenden Projekt an, das entweder aus der ursprünglichen Anfrage konvertiert wurde oder manuell als auflösendes Objekt einer Anfrage bezeichnet wurde.</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Aufgabe auflösen</strong>: Zeigt Informationen zur auflösenden Aufgabe an, die entweder aus dem ursprünglichen Problem konvertiert oder manuell als Lösungsobjekt für ein Problem ausgewiesen wurde.</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>Problem beheben</strong>: Zeigt Informationen zum Problem an, das gelöst wurde und manuell als Lösungsobjekt eines Problems angegeben wurde.</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
