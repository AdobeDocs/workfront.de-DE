---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Konfigurieren der Anzeige von Informationen im Diagramm [!UICONTROL Gantt]
description: Sie können konfigurieren, welche Informationen sowohl im Gantt-Diagramm für Aufgabenlisten als auch im Gantt-Diagramm für Projektliste angezeigt werden.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Konfigurieren der Anzeige von Informationen im [!UICONTROL Gantt-Diagramm]

Sie können konfigurieren, welche Informationen sowohl im Aufgabenliste [!UICONTROL Gantt-Diagramm] als auch im Projektliste [!UICONTROL Gantt-Diagramm] angezeigt werden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel zu befolgen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf Projekte und Aufgaben</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf das Projekt</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigeoptionen verstehen

In der folgenden Tabelle sind die Anzeigeoptionen für das [!UICONTROL Gantt-Diagramm] aufgeführt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tatsächliche Datumswerte]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="current_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Tatsächliches Startdatum] und [!UICONTROL Aktuelles Abschlussdatum] werden mit einem Dreieckssymbol angezeigt. Wenn das [!UICONTROL Tatsächliche Abschlussdatum] null ist, wird nur das [!UICONTROL Tatsächliche Startdatum] angezeigt.</p> <p>Weitere Informationen zu Start- und Abschlussdaten finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Überblick über das Projekt [!UICONTROL Tatsächliches Abschlussdatum] </a> und <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Überblick über das Projekt [!UICONTROL Tatsächliches Startdatum] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zuweisung]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assignments_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Zeigt Aufgabenverantwortliche an. Bewegen Sie den Mauszeiger über den Link <strong>[!UICONTROL Details]</strong> neben dem Namen eines Verantwortlichen, um genauere Informationen zu ihm anzuzeigen, einschließlich des Prozentsatzes seiner Zuordnung zur Aufgabe.</p> <p>Zuweisungen werden nicht im [!UICONTROL Gantt-Diagramm] angezeigt, wenn das [!UICONTROL Gantt-Diagramm] nach PDF exportiert wird. Wenn das [!UICONTROL Gantt-Diagramm] nach PDF exportiert wird, werden die Bevollmächtigten nur in der Aufgabenliste angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>Ein Projekt-Schnappschuss, der wichtige Daten zum Projekt darstellt, die im ursprünglichen Projektplan enthalten sind. Grundlinien können während der gesamten Projektlaufzeit eingenommen werden. Wenn Sie die Anzeige von Grundlinien im [!UICONTROL Gantt-Diagramm] aktivieren, wählen Sie die gewünschte Grundlinie aus. Sie können jeweils nur eine Grundlinie im [!UICONTROL Gantt-Diagramm] anzeigen und sie wird in Form einer grauen Leiste angezeigt.</p> <p>Weitere Informationen zu Grundlinien finden Sie unter <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Erstellen von Projekt-Grundlinien</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Veröffentlichungsdatum]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>Das Datum, zu dem ein Bevollmächtigter verpflichtet, wann die Aufgabe abgeschlossen sein wird, wird mit einer Markierung im [!UICONTROL Gantt-Diagramm] angezeigt. </p> <p>Weitere Informationen zu Commit-Datumsangaben finden Sie unter <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Commit Date] Overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % Complete]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  Der Prozentsatz der abgeschlossenen Aufgabe wird in der Aufgabenzeile angezeigt.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kritischer Pfad]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>Die Aufgaben, die sich auf die Zeitleiste des Projekts auswirken könnten, werden als Teil des kritischen Pfads betrachtet und sind deutlich rot markiert. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Diamanten</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>Nach der Aufgabe, die einem Meilenstein zugeordnet ist, wird ein Diamantsymbol angezeigt. Bewegen Sie den Mauszeiger über einen Meilenstein, um Name und Datum des Meilensteins anzuzeigen. Der [!DNL Workfront] -Administrator legt die Farbe jedes Meilensteindiamanten fest.</p> <p>Weitere Informationen zu Meilensteinen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Meilensteinpfad erstellen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Zeilen</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Nach der Aufgabe, die einem Meilenstein zugeordnet ist, wird eine Zeile angezeigt. Bewegen Sie den Mauszeiger über einen Meilenstein, um Name und Datum des Meilensteins anzuzeigen. Der [!DNL Workfront] -Administrator legt die Farbe jeder Meilensteinlinie fest.</p> <p> Weitere Informationen zu Meilensteinen finden Sie unter  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Erstellen eines Meilensteinpfads</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorgänger]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Eine Zeile von einer Aufgabe zu einer anderen, die die Vorgängerbeziehung zwischen den beiden Aufgaben anzeigt. Um eine einzelne Vorläuferlinie hervorzuheben, bewegen Sie den Mauszeiger darüber. Klicken Sie darauf, um die Markierung beizubehalten. Sie können jeweils nur eine Vorgängerzeile hervorheben.</p> <p>Neben jeder Aufgabe, die über eine Vorgängerbeziehung verfügt, die sich über mehrere Seiten im Gantt-Diagramm oder auf Aufgaben mit einem projektübergreifenden Vorgänger erstreckt, wird ein Symbol vom Typ <strong>[!UICONTROL Vorgänger]</strong> angezeigt.</p> <p>Klicken Sie auf das Symbol "<strong>[!UICONTROL Vorgänger]</strong>", um alle Vorgänger- und Nachfolgeaufgaben sowie Details zu den einzelnen Aufgaben, wie z. B. Aufgabenname, Typ der Vorgängerbeziehung und Schlüsseldaten, anzuzeigen.</p> <p>Hinweis: Das [!UICONTROL Gantt-Diagramm] in einer Liste von Projekten zeigt Informationen zu projektübergreifenden Vorgängern an. Weitere Informationen zum Erstellen von Vorgängerbeziehungen zwischen verschiedenen Projekten finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Erstellen von projektübergreifenden Vorgängern</a></p> <p>Weitere Informationen zu Vorgängern finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Vorgänger erzwingen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fortschrittsstatus]</td> 
   <td> <p>[!UICONTROL Einschaltzeit] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time_Okt._2017.png"></p> <p>[!UICONTROL Hinter]    <img src="assets/task-behind--oct.-2017.png" alt="task_Behind_Okt._2017.png"></p> <p>[!UICONTROL Risiko]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>Verspätet        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>Der Status des aktuellen Fortschritts bei einer bestimmten Aufgabe. </p> <p>Weitere Informationen zu den einzelnen [!UICONTROL Fortschrittsstatus]-Typen finden Sie unter <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task [!UICONTROL Progress Status] Overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projektierte Datumswerte</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_forecast_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>Der erwartete Zeitplan, in dem die [!UICONTROL Projektionsbeginn] und die [!UICONTROL Abschlussdaten] auf der Grundlage der derzeit abgeschlossenen Arbeiten und der verbleibenden Arbeiten markiert werden. </p> <p>Weitere Informationen zu den geplanten Abschlussdaten finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Überblick über das [!UICONTROL Projektionsdatum] für Projekte, Aufgaben und Probleme</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anzeigeoptionen konfigurieren

1. Gehen Sie zur Aufgabenliste [!UICONTROL Gantt-Diagramm] oder zur Projektliste [!UICONTROL Gantt-Diagramm].\
   Weitere Informationen dazu, wo sich das [!UICONTROL Gantt-Diagramm] befindet, finden Sie unter [Erste Schritte mit dem [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md) .

1. (Optional) Wählen Sie die Einstellung **[!UICONTROL Zu den geplanten Daten wechseln]** aus, um die Aufgaben anhand ihrer [!UICONTROL geplanten Daten] anzuzeigen. Standardmäßig werden Aufgaben durch ihre [!UICONTROL geplanten Datumswerte] im [!UICONTROL Gantt-Diagramm] angezeigt.
1. Klicken Sie auf das Optionssymbol, um das Dialogfeld **[!UICONTROL Optionen]** anzuzeigen.\
   ![options.png](assets/options-350x129.png)

1. Wählen Sie die Konfigurationsoptionen aus, die im [!UICONTROL Gantt-Diagramm] angezeigt werden sollen.

   >[!NOTE]
   > Nicht alle Konfigurationsoptionen sind in der Projektliste [!UICONTROL Gantt-Diagramm] verfügbar.

1. Klicken Sie auf eine beliebige Stelle im [!UICONTROL Gantt-Diagramm], um das Dialogfeld **[!UICONTROL Optionen]** zu schließen.
