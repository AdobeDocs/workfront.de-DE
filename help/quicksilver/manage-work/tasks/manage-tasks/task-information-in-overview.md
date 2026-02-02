---
product-area: projects
navigation-topic: manage-tasks
title: Verwalten von Aufgabeninformationen im Bereich „Aufgabendetails - Übersicht“
description: Sie können die Informationen einer Aufgabe anzeigen oder bearbeiten, indem Sie im Abschnitt „Aufgabendetails“ im Bereich „Übersicht“ aufrufen. Es gibt eine begrenzte Anzahl von Feldern, die Sie im Abschnitt Aufgabendetails anzeigen oder bearbeiten können.
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 5%

---

# Verwalten von Aufgabeninformationen im Bereich „Aufgabendetails - Übersicht“

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

Sie können die Informationen einer Aufgabe anzeigen oder bearbeiten, indem Sie im Abschnitt „Aufgabendetails“ im Bereich „Übersicht“ aufrufen. Es gibt eine begrenzte Anzahl von Feldern, die Sie im Abschnitt Aufgabendetails anzeigen oder bearbeiten können.

Informationen zum Bearbeiten aller Informationen für eine Aufgabe finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

In diesem Artikel wird beschrieben, wie Sie Informationen im Bereich Übersicht der Aufgabendetails anzeigen oder bearbeiten. Informationen zum Aktualisieren anderer Bereiche von Aufgabendetails finden Sie in den folgenden Artikeln:

* [Verwalten der Aufgabenfinanzen im Abschnitt „Aufgabendetails“](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [Verwalten benutzerdefinierter Formulare, die an Objekte angehängt sind](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Paket</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz </p> </td> 
   <td><p>Standard</p> 
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Hochladen des Zugriffs auf Projekte und Aufgaben</p> <p>Wenn Sie die richtige Zugriffsebene haben, aber den Abschnitt „Details“ der Aufgabe immer noch nicht bearbeiten können, fragen Sie Ihren Adobe Workfront, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen</p> </td> 
   <td> <p>Mitwirken an oder höhere Berechtigungen für das Projekt</p> <p>Zeigen Sie die Berechtigungen für die Aufgabe an, um Informationen im Abschnitt Details anzuzeigen. </p> 
   <p>Tragen Sie Berechtigungen für die Aufgabe bei, um die folgenden Informationen im Abschnitt Details zu aktualisieren:</p>

<ul>
   <li>Beschreibung</li>
   <li>Status</li>
   </ul>

<p>Verwalten Sie die Berechtigungen für die Aufgabe, um alle Informationen im Abschnitt Details zu aktualisieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> plan*</b> </p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> license*</b> </p> </td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher access to Projects and Tasks</p> <p>If you have the correct access level but still can't edit the Details  section  of the task, ask your Adobe Workfront if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Contribute or higher permissions for the project</p> <p>View permissions for the task to view information in the Details section. </p> 
   <p>Contribute permissions for the task to update the following information  in the Details section:</p>

   <ul>
   <li>Description</li>
   <li>Status</li>
   </ul>
   
   <p>Manage permissions for the task to update all information in the Details section.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Bearbeiten von Aufgabeninformationen im Abschnitt „Aufgabendetails - Übersicht“

1. Wechseln Sie zu einer Aufgabe, die Sie anzeigen oder bearbeiten möchten.
1. Klicken Sie **linken** auf Aufgabendetails .
1. Wechseln Sie zum Bereich **Übersicht**, um weitere Informationen zur Aufgabe anzuzeigen.

   Standardmäßig ist Überblick der erste Bereich im Abschnitt „Aufgabendetails“ und wird erweitert.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator Ihre Layout-Vorlage einrichtet, werden die Felder im Abschnitt Aufgabendetails möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png) in der oberen rechten Ecke des Abschnitts Details und dann auf **Übersicht**.

   >[!TIP]
   >
   >Sie können keine Felder bearbeiten, die automatisch von Workfront generiert wurden oder für die Sie keine Bearbeitungsberechtigung haben.

1. Bearbeiten Sie alle Felder, die bearbeitet werden können, indem Sie einfach auf das Feld klicken oder auf **+Hinzufügen** klicken, um einem leeren Feld Informationen hinzuzufügen.
1. Zeigt eines der folgenden aufgelisteten Felder an oder bearbeitet es.

   Nicht alle Felder können bearbeitet werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td> <p>Zusätzliche Informationen zur Aufgabe</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Referenznummer</td> 
      <td>Dies ist ein eindeutiger Wert für die von Workfront generierte Aufgabe für alle Objekte im System. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Benutzer mit der Berechtigung Verwalten für eine Aufgabe können in diesem Feld einen Link zu einer internen oder externen Seite angeben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Wählen Sie den Status der Aufgabe aus, der angibt, in welchem Entwicklungsstadium sich die Aufgabe befindet.</p> <p>Tipp: Sie können den Aufgabenstatus in der Aufgabenkopfzeile aktualisieren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorität</td> 
      <td> <p>Dies ist eine visuelle Markierung, mit der Sie Ihre Aufgaben priorisieren können. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p> Keine</p> </li> 
        <li> <p> Niedrig </p> </li> 
        <li> <p>Normal </p> </li> 
        <li> <p>Hoch </p> </li> 
        <li> <p> Dringend </p> </li> 
       </ul> <p>Je nach den vom Workfront-Administrator ausgewählten Projektvoreinstellungen können die Namen der Prioritäten für Sie unterschiedlich sein. Informationen zu Aufgabenprioritäten finden Sie unter <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Aufgabenpriorität aktualisieren</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dauertyp</td> 
      <td> <p>Dadurch wird die Beziehung zwischen folgenden Elementen identifiziert: </p> 
       <ul> 
        <li> <p>Die Anzahl der Ressourcen, die einer Aufgabe zugewiesen sind </p> </li> 
        <li> <p>Der Gesamtaufwand, der zum Abschließen der Aufgabe erforderlich ist </p> </li> 
        <li> <p> Die Gesamtdauer der Aufgabe. </p> </li> 
       </ul> <p>Ihr Workfront-Administrator <span> oder ein Gruppenadministrator </span> die Standardeinstellung für den Dauertyp für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Informationen zum Festlegen von Projektstandards finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurieren von systemweiten Projektvoreinstellungen</a>. </p> <p>Mit Dauertypen können Sie konsistente Ressourcenzuweisungen auf der Grundlage der Anforderungen der Aufgabe festlegen. Weitere Informationen zum Dauertyp einer Aufgabe finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die Aufgabendauer und den Dauertyp</a>. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p>Berechnete Zuweisung </p> </li> 
        <li> <p> Berechnete Arbeit </p> </li> 
        <li> <p>Leistungsgesteuert </p> </li> 
        <li> <p>Einfach</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dauer</td> 
      <td> 
       <div> 
        <div> 
         <p>Dies ist der Zeitraum, den Sie einer Aufgabe erlauben, offen zu bleiben, bevor sie abgeschlossen ist. </p> 
         <p>Wichtig: Da die Aufgabendauer normalerweise die Zeit zwischen dem geplanten Start- und dem geplanten Abschlussdatum ist, wirkt sich dies auf die Zeitleiste des Projekts aus.</p> 
         <p>Gehen Sie wie folgt vor, um die Dauer der Aufgabe und die Zeiteinheit anzugeben:</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Geben Sie die Zeitdauer ein und wählen Sie aus den verfügbaren Zeiteinheiten im Dropdown-Menü aus.</p> </li> </ul>

   <p><strong>TIPP</strong></p> <p> Wenn Sie die Dauer von Aufgaben in einer Aufgabenliste aktualisieren, können Sie die Abkürzung für die Zeiteinheit verwenden. </p>      <p> In der folgenden Tabelle können Sie zwischen den Optionen „Reguläre Zeit“ und „Verstrichene Zeit“ wählen: </p> 
         <table style="table-layout:auto"> 
          <col> 
          <col data-mc-conditions=""> 
          <tbody> 
           <tr> 
            <td>Zeiteinheit</td> 
            <td>Abkürzung</td> 
           </tr> 
           <tr> 
            <td>Minutes</td> 
            <td>M</td> 
           </tr> 
           <tr> 
            <td>Stunden</td> 
            <td>H</td> 
           </tr> 
           <tr> 
            <td>Tage. Dies ist der Standardwert. </td> 
            <td>D</td> 
           </tr> 
           <tr> 
            <td>Weeks</td> 
            <td>W</td> 
           </tr> 
           <tr> 
            <td>Months</td> 
            <td>T</td> 
           </tr> 
           <tr> 
            <td>Verstrichene Minuten</td> 
            <td>EM</td> 
           </tr> 
           <tr> 
            <td>Verstrichene Stunden</td> 
            <td>EH</td> 
           </tr> 
           <tr> 
            <td>Verstrichene Tage</td> 
            <td>ED</td> 
           </tr> 
           <tr> 
            <td>Verstrichene Wochen</td> 
            <td>EW</td> 
           </tr> 
           <tr> 
            <td>Verstrichene Monate</td> 
            <td>ET</td> 
           </tr> 
          </tbody> 
         </table> 
         <p><strong>HINWEIS</strong> </p>
         <p> Verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und Ausfallzeiten umfasst. Mit anderen Worten: Verstrichene Zeit ist der Ablauf von Kalendertagen. Die reguläre Zeit berücksichtigt Feiertage, Wochenenden und Auszeiten und schließt sie von der Dauer der Aufgabe aus. Weitere Informationen zur Aufgabendauer finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über die Aufgabendauer und den </a>). </p> 
         <p> 
         <!--You cannot specify the Duration of a task when the Duration Type of the task is Simple, or when the Task Constraint is Fixed Dates. (NOTE: Anna said this is now possible for all duration types in the Assignments area. It's not here, but to clear confusion, I am drafting this out of here.)--></p> 
        </div> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projizierte Dauer</td> 
      <td> <p>Die Differenz in Tagen zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliche Dauer</td> 
      <td> <p>Die Differenz in Tagen zwischen dem tatsächlichen Startdatum und dem tatsächlichen Abschlussdatum. So lange hat es tatsächlich gedauert, die Arbeit zu Ende zu bringen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Stunden</td> 
      <td> <p>Anzahl der geplanten Stunden für die Aufgabe angeben (in Stunden) Dies ist die tatsächliche Zeit, die die Verantwortlichen für die Aufgabe benötigen würden, um diese abzuschließen. Sie können den Betrag der geplanten Stunden für eine Aufgabe nur angeben, wenn als Dauertyp Berechnete Zuweisung festgelegt ist. Weitere Informationen zu Dauertypen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über Aufgabendauer und Dauertyp</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliche Stunden</td> 
      <td>Von Benutzern für die Aufgabe protokollierte Stunden </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Work Effort </td> 
      <td> 
       <div> 
        <p>Der erforderliche Aufwand zum Abschließen der Aufgabe. Möglicherweise verwendet der Projektmanager dieses Feld anstelle der geplanten Stunden, um den für die Erfüllung einer Aufgabe erforderlichen Arbeitsaufwand einzuschätzen. Dieses Feld ist nur sichtbar, wenn die folgenden Bedingungen erfüllt sind:</p> 
        <ul> 
         <li> <p>Die Aufgabe hat einen einfachen Dauertyp. </p> <p>Tipp: Wenn Sie den Dauertyp der Aufgabe ändern, wird dieses Feld abgeblendet. </p> </li> 
         <li>Ihr Projektmanager hat das Feld „Arbeitsaufwand verwenden“ zur automatischen Berechnung der geplanten Stunden für die Aufgabe im Projekt aktiviert. </li> 
        </ul> 
        <p>Wählen Sie aus den folgenden Optionen aus:</p> 
        <ul> 
         <li>Klein</li> 
         <li>Medium <span style="font-weight: normal;">(dies ist der Standardwert für eine neue Aufgabe)</span></li> 
         <li>Groß</li> 
        </ul> 
        <p><strong>NOTIZ</strong></p> 
        <p> Durch die Aktualisierung des Aufwands kann die geplante Arbeitszeit der Aufgabe aktualisiert werden. Die Aktualisierung erfolgt sofort, wenn der Projektaktualisierungstyp Automatisch ist. Wenn der Projektaktualisierungstyp „Manuell“ ist, müssen Sie die Zeitleiste neu berechnen, um die aktualisierten geplanten Stunden anzuzeigen. </p> 
        <p>Informationen zur Verwendung des Work Effort anstelle der geplanten Stunden zur Schätzung des Task Effort finden Sie <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort Overview</a>. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aufgabenbeschränkung</td> 
      <td> <p>Legen Sie durch Angabe einer Aufgabenbeschränkung fest, wann die Aufgabe abgeschlossen werden muss. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p><span>Feste Daten</span> </p> <p>Geben Sie <strong>Geplanter Start</strong> und ein <strong>Geplantes Abschlussdatum</strong> an. </p> </li> 
        <li> <p><span>Muss beginnen am</span> </p> <p>Geben Sie <strong>Geplantes Startdatum“ </strong>. </p> </li> 
        <li> <p><span>Muss beendet werden am</span> </p> <p>Geben Sie <strong> „Geplantes Abschlussdatum“ </strong>. </p> </li> 
       </ul> 
       <ul> 
        <li> <p><span>So bald wie möglich</span></p> </li> 
        <li> <p><span>So spät wie möglich</span></p> </li> 
        <li> <p><span>Frühestmögliche Zeit</span></p> </li> 
        <li> <p> <span>Letzte verfügbare Zeit</span></p> </li> 
        <li> <p><span>Start spätestens</span> </p> </li> 
        <li> <p>Geplantes Startdatum angeben</p> </li> 
        <li> <p><span>Start nicht früher als</span> </p> <p>Geben Sie <strong>Geplantes Startdatum“ </strong>. </p> </li> 
        <li> <p> Beenden <span>spätestens</span></p> <p>Geben Sie <strong> „Geplantes Abschlussdatum“ </strong>. </p> </li> 
        <li> <p> Beenden <span>nicht früher als</span></p> <p>Geben Sie <strong>Geplantes Abschlussdatum“ </strong></p> </li> 
       </ul> <p>Weitere Informationen zur Aufgabenbeschränkung finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Aufgabenbeschränkung - Übersicht</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplantes Startdatum</td> 
      <td> <p>Wann die Aufgabe geplant ist. Das geplante Startdatum einer Aufgabe wird durch eine Reihe von Faktoren festgelegt und beeinflusst:</p> 
       <ul> 
        <li>Je nach der systemweiten Voreinstellung für das geplante Startdatum der Aufgabe kann das Startdatum einer neuen Aufgabe für ein Projekt standardmäßig entweder heute oder das Startdatum des Projekts sein. <span>Der Gruppenadministrator bzw. die Gruppenadministratorin für die mit dem Projekt verknüpfte Gruppe kann diese Einstellung auch für die Gruppe festlegen.</span> Weitere Informationen zu den Voreinstellungen für Aufgaben auf Systemebene oder Gruppenebene finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Systemweite Voreinstellungen für Aufgaben und Probleme konfigurieren</a>.</li> 
        <li>Abhängig von den Vorgängern der Aufgabe wählt Workfront das geplante Startdatum als nächstes verfügbares Datum nach dem Ende der Vorgänger oder als Startdatum, je nach der Vorgängerbeziehung. Weitere Informationen zu Vorgängerbeziehungen finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Übersicht über Aufgabenvorgänger</a>.</li> 
        <li>Der Projektmanager oder Aufgabenbesitzer kann das geplante Startdatum manuell festlegen, wenn die Aufgabenbeschränkung entweder Feste Termine oder Muss beginnen am lautet. Weitere Informationen zu Aufgabenbeschränkungen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voraussichtlicher Starttermin</td> 
      <td> <p>Das „reale“ Datum, an dem die Aufgabe beginnen soll, basierend auf dem Fortschritt und dem Abschluss vorheriger Aufgaben. Dies ist ein berechnetes Feld, das nicht manuell bearbeitet werden kann.</p> <p> Das voraussichtliche Startdatum und das geplante Startdatum sind identisch, wenn zum ersten Mal ein Projekt geplant wird. Das voraussichtliche Startdatum kann vom geplanten Startdatum weg verschoben werden, wenn sich das Projekt weiterentwickelt und die Aufgabe noch nicht gestartet wurde. Weitere Informationen über das voraussichtliche Startdatum finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Übersicht über das voraussichtliche Startdatum des Projekts</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliches Startdatum</td> 
      <td> <p>Geben Sie ein tatsächliches Startdatum für die Aufgabe an. Der Standardwert wird normalerweise automatisch ausgefüllt, wenn Sie den Status der Aufgabe in „In Bearbeitung“ ändern. Das tatsächliche Startdatum kann auch manuell vom Projektmanager oder dem Aufgabenbesitzer geändert werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplantes Abschlussdatum</td> 
      <td> <p>Das voraussichtliche Abschlussdatum, wie es bei der Planung der Aufgabe angezeigt wird. Das geplante Abschlussdatum kann durch eine Reihe von Faktoren festgelegt werden:</p> 
       <ul> 
        <li>Das geplante Abschlussdatum wird anhand des geplanten Startdatums berechnet, indem die Dauer der Aufgabe zum geplanten Startdatum hinzugefügt wird. Wenn der Projekt-Manager oder die Workfront die Dauer der Aufgabe angibt, wird dadurch eine Aktualisierung des geplanten Abschlussdatums Trigger. Wenn sich das geplante Datum ändert, liegt das oft daran, dass die Dauer des s aktualisiert wurde.</li> 
        <li>Der Projektmanager oder Aufgabenbesitzer kann das geplante Abschlussdatum manuell festlegen, wenn die Aufgabenbeschränkung entweder Feste Termine oder Muss abgeschlossen sein muss. Weitere Informationen zu Aufgabenbeschränkungen finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen</a>.</li> 
        <li>Wenn sich der Dauertyp der Aufgabe ändert und sich gleichzeitig die Anzahl der Ressourcen für die Aufgaben ändert, ändert sich auch das geplante Abschlussdatum. Weitere Informationen zu Dauertypen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Übersicht über Aufgabendauer und Dauertyp</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Voraussichtliches Abschlussdatum</td> 
      <td> <p>Das „reale“ Datum, an dem die Aufgabe abgeschlossen wird, basierend auf dem Fortschritt vorheriger Aufgaben und den Fortschrittsaktualisierungen, die der Beauftragte bei der Aufgabe vorgenommen hat. Dies ist ein berechnetes Feld, das nicht manuell bearbeitet werden kann.</p> <p> Das voraussichtliche Abschlussdatum und das geplante Abschlussdatum beginnen bei der ersten Planung eines Projekts damit. Das voraussichtliche Abschlussdatum kann von der geplanten Fertigstellung weggehen, wenn das Projekt weiterentwickelt wird und die Aufgabe noch nicht gestartet wurde. Weitere Informationen zu voraussichtlichen Abschlussdaten finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliches Abschlussdatum</td> 
      <td> <p>Geben Sie Datum und Uhrzeit des tatsächlichen Abschlusses der Aufgabe an. Der standardmäßige Zeitpunkt (Datum und Uhrzeit), zu dem eine Aufgabe abgeschlossen wird, entspricht immer dem tatsächlichen Zeitpunkt, zu dem der Status zu „Abgeschlossen“ wird. Das tatsächliche Abschlussdatum kann auch manuell vom Projektmanager oder dem Aufgabenbesitzer geändert werden. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Verpflichtungsdatum</td> 
      <td> <p>Dies ist das Datum, zu dem sich der Benutzer, der der Aufgabe zugewiesen wurde, verpflichtet, sie abzuschließen. Dies kann vom geplanten Abschlussdatum abweichen. Nur Beauftragte können dieses Feld bearbeiten. Informationen zu Commit-Daten in Workfront finden Sie unter <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Übersicht über Commit-Datum</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Eingabedatum</td> 
      <td>Das Datum, an dem die Aufgabe erstellt wurde</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eingegeben von</td> 
      <td>Person, die die Aufgabe erstellt hat.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Datum der letzten Aktualisierung</td> 
      <td> <p>Das Datum, an dem die Aufgabe zuletzt aktualisiert wurde </p> <p>Tipp: Workfront zeichnet jedes Mal, wenn jemand eine Aufgabe bearbeitet und speichert, ein aktualisiertes Datum auf.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zuletzt aktualisiert von</td> 
      <td> <p>Person, die die Aufgabe zuletzt aktualisiert hat.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Intervallfrequenz</td> 
      <td> <p>Wird nur für das übergeordnete Element der wiederkehrenden Aufgaben angezeigt. Dies ist die Häufigkeit, mit der die Aufgaben in der Wiederholung auftreten. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Wiederkehrende Aufgaben erstellen</a>. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Dauer pro Termin</td> 
      <td> <p>Wird nur für das übergeordnete Element der wiederkehrenden Aufgaben angezeigt. Angezeigt wird die Dauer jeder wiederkehrenden Aufgabe. Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Wiederkehrende Aufgaben erstellen</a>. </p> <p><strong>NOTIZ</strong></p> <p> In einzelnen wiederkehrenden Aufgaben geänderte Dauer zeigt nicht den in diesem Feld angegebenen Wert an. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted, to keep it focused JUST on the Overview section and not others.) </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Custom Forms</strong> to add or forms or edit information on the existing custom forms. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand any of the existing custom forms to edit them, or start typing in the <strong>Add custom form</strong> box in the upper-right corner to add a new form. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding or editing custom forms, see the following articles:</p>
   -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md" class="MCXref xref">Add a custom form to an object</a> </li>   
     -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md" class="MCXref xref">Manage custom forms attached to objects</a> </li>   
     -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Finance</strong>, then <strong>Edit Finance</strong> to view or edit financial information for the task. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand the <strong>Finance</strong> area in the Details section, then double-click any editable field to update it. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about editing financial information for a task, see <a href="../../../manage-work/tasks/manage-tasks/task-finances-in-details.md" class="MCXref xref">Manage task finances in the Task Details section</a>. </p>
   -->

1. Klicken Sie auf **Änderungen speichern**.
