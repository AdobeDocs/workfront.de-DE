---
product-area: projects
navigation-topic: manage-projects
title: Projektzeitpläne neu berechnen
description: Durch die Neuberechnung von Zeitleisten können Manager sehen, wie verschiedene mit dem Projekt verbundene Faktoren die Zeitleiste des Projekts beeinflussen. Der Zeitrahmen eines Projekts bezieht sich auf geplante und geplante Daten.
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 0%

---

# Projektzeitpläne neu berechnen

Durch die Neuberechnung von Zeitleisten können Manager sehen, wie verschiedene mit dem Projekt verbundene Faktoren die Zeitleiste des Projekts beeinflussen. Der Zeitrahmen eines Projekts bezieht sich auf geplante und geplante Daten.

Änderungen an Zeitplänen, Zeitlimits für Mitarbeiter und anderen Elementen außerhalb des Projektbereichs wirken sich nicht sofort auf die Projektzeitleiste aus. Die Projekt-Timeline wird bei der Neuberechnung der Timeline beeinflusst. Externe Einflüsse wirken sich erst dann auf Ihr Projekt aus, wenn die Neuberechnung erfolgt.

In diesem Artikel wird beschrieben, wie die Timeline-Neuberechnung erfolgt.

## Zugriffsanforderungen

<!--drafted for P&P: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Die automatische Timeline-Neuberechnung erfolgt ohne speziellen Zugriff für alle Benutzer, die an der Arbeit am Projekt beteiligt sind.

Sie müssen jedoch über den folgenden Zugriff verfügen, um die Timeline eines Projekts manuell neu zu berechnen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Systemadministrator zur Neuberechnung der Zeitleiste für alle Projekte im System</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Automatische Neuberechnung

Standardmäßig werden die Projektzeitpläne täglich, wenn sich der Projektumfang ändert, oder jede Nacht automatisch neu berechnet. Der Workfront-Administrator bestimmt, ob Zeitleisten jede Nacht oder bei jeder Änderung des Umfangs automatisch berechnet werden, indem er die Timelines-Einstellungen im Bereich Projekteinstellungen der Einrichtung verwaltet. Weitere Informationen finden Sie unter [Konfigurieren von Timeline-Neuberechnungen für Projekte](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>Wenn die Zeitleiste eines Projekts länger als 15 Jahre ist, wird die automatische Neuberechnung für dieses Projekt deaktiviert. Sie können einen Aktualisierungstyp nur für ein Projekt auswählen, das länger als 15 Jahre dauert. Wenn Sie die Daten im Projekt auf weniger als 15 Jahre ändern, müssen Sie die Timeline manuell neu berechnen, bevor sie automatisch berechnet wird.

* [Automatische Neuberechnung der Projektzeitpläne](#automatic-recalculation-of-project-timelines)
* [Aktionen, die eine automatische Neuberechnung der Projektzeitpläne Trigger haben](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### Automatische Neuberechnung der Projektzeitpläne {#automatic-recalculation-of-project-timelines}

Adobe Workfront berechnet die Zeitpläne nur für Projekte täglich neu, für die alle der folgenden Bedingungen erfüllt sind:

* Der Status Aktuell
* Der Aktualisierungstyp des Projekts ist auf &quot;Automatisch&quot;oder &quot;Automatisch&quot;und &quot;Bei Änderung&quot;eingestellt

  Informationen zum Typ des Projektaktualisierungstyps finden Sie unter [Übersicht über den Projektaktualisierungstyp](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* Letztes Datum der Aktualisierung innerhalb der letzten drei Monate\
  Der Workfront-Administrator kann diese Standardfunktion ändern, wie unter [Konfigurieren von Zeitleistenneuberechnungen für Projekte](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md) beschrieben.

* Das letzte Berechnungsdatum der Projekt-Timeline liegt nicht innerhalb des aktuellen Kalendertages. Das bedeutet, dass das letzte Berechnungsdatum der Projekt-Timeline vor 00:00 Uhr des aktuellen Tages liegt.

Sie können konfigurieren, wie häufig die Timeline für Ihr Projekt aktualisiert wird. Wenn die Projekt-Timeline aktualisiert wird, wird sie anhand von Änderungen am Projekt neu berechnet.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

Weitere Informationen finden Sie unter [Auswählen des Aktualisierungstyps für das Projekt](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### Aktionen, die eine automatische Neuberechnung der Projektzeitpläne Trigger haben {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

Verschiedene Änderungen des Umfangs während der Laufzeit eines Projekts führen zu einer automatischen Neuberechnung der Projekt-Timeline, einschließlich der folgenden Aktionen:

* Aktualisieren des Aufgabenstatus
* Verschieben einer Aufgabe in ein anderes Projekt.
* Aktualisieren des geplanten Datums oder des geplanten Abschlussdatums der Aufgaben.
* Aktualisieren des Dauer-Typs, der Aufgabenbegrenzung oder der Anzahl der Bevollmächtigten für die Aufgaben.
* Aktualisieren der Vorgängerbeziehungen von Aufgaben.
* Hinzufügen einer Validierung zu einer Aufgabe, die auch dem geplanten Abschlussdatum der Aufgabe Zeit hinzufügt.\
  Weitere Informationen zu den Genehmigungseinstellungen finden Sie unter [Globale Genehmigungseinstellungen konfigurieren](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## Manuelle Neuberechnung {#manual-recalculation}

Als Projekteigentümer können Sie die Zeitpläne für einzelne Projekte manuell neu berechnen. Der Workfront-Administrator kann alle Zeitleisten in Workfront manuell neu berechnen.

* [Zeitleisten für einzelne Projekte oder stapelweise neu berechnen](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [Manuelles Neuberechnen von Zeitleisten in großen Mengen im Feld &quot;Projekte bearbeiten&quot;](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [Zeitpläne für alle Projekte im System neu berechnen (nur Workfront-Administratoren)](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### Neuberechnung der Zeitpläne für einzelne Projekte oder in großen Mengen {#recalculate-timelines-for-individual-projects-or-in-bulk}

Sie können die Timeline eines Projekts in Workfront von der Projektseite oder von einer Projektliste oder einem Bericht aus neu berechnen.

1. Wechseln Sie zu dem Projekt, für das Sie die Timeline neu berechnen möchten, und klicken Sie auf das Symbol **Mehr** ![](assets/qs-more-menu.png) links neben dem Projektnamen.

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oder

   Wechseln Sie zu einer Projektliste oder einem Bericht und wählen Sie ein oder mehrere Projekte aus. Klicken Sie dann oben in der Liste auf das Symbol **Mehr** ![](assets/qs-more-menu.png) .

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >Je nach der Komplexität Ihrer Projekte empfehlen wir, bei der Neuberechnung der Zeitpläne keine große Anzahl von Projekten auszuwählen, um eine optimale Leistung zu gewährleisten. Einige Dinge, die ein Projekt zu komplex machen könnten, sind möglicherweise mehrere Abhängigkeiten oder Zuweisungen oder eine große Anzahl benutzerdefinierter Felder.

1. Klicken Sie auf **Timeline neu berechnen**.

   Nach der Neuberechnung der Zeitleiste wird eine Meldung angezeigt, die angibt, dass die Neuberechnung erfolgreich war.

   >[!TIP]
   >
   >Bevor die Timeline-Neuberechnung abgeschlossen ist, können einige geplante oder geplante Daten abgeblendet angezeigt werden. Das bedeutet, dass die Neuberechnung noch nicht abgeschlossen ist und sich die Daten ändern können.

### Manuelles Neuberechnen von Zeitleisten in großen Mengen im Feld &quot;Projekte bearbeiten&quot; {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

Sie können die Zeitpläne mehrerer Projekte manuell neu berechnen, indem Sie sie stapelweise bearbeiten.

>[!TIP]
>
>Je nach Komplexität Ihrer Projekte empfehlen wir, bei der Massenbearbeitung keine große Anzahl von Projekten auszuwählen, um eine optimale Leistung zu gewährleisten. Einige Dinge, die ein Projekt zu komplex machen könnten, sind möglicherweise mehrere Abhängigkeiten oder Zuweisungen oder eine große Anzahl benutzerdefinierter Felder.

1. Gehen Sie zu einer Projektliste.
1. Wählen Sie mehrere Projekte in der Liste aus und klicken Sie dann auf **Bearbeiten**.
1. Klicken Sie auf **Einstellungen** und wählen Sie dann **Zeitleisten neu berechnen** aus.

1. Klicken Sie auf **Änderungen speichern**.

### Zeitpläne für alle Projekte im System neu berechnen (nur Workfront-Administratoren) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront-Administratoren können die Diagnose Timeline neu berechnen ausführen, um alle Zeitleisten im Workfront-System sofort neu zu berechnen. Dadurch können alle Projektmanager den Einfluss externer Änderungen sofort an geplanten und geplanten Terminen erkennen.

Weitere Informationen zum Neuberechnen von Zeitleisten für die gesamte Workfront-Site finden Sie im Abschnitt &quot;Zeitpläne für die gesamte Workfront-Instanz neu berechnen&quot;in [Konfigurieren von Zeitleistenneuberechnungen für Projekte](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
