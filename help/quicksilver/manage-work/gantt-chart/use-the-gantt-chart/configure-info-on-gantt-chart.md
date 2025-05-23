---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: Konfigurieren der Anzeige von Informationen im [!UICONTROL Gantt]Diagramm
description: Sie können konfigurieren, welche Informationen sowohl im Gantt-Diagramm für die Aufgabenliste als auch im Gantt-Diagramm für die Projektliste angezeigt werden.
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Konfigurieren der Anzeige von Informationen im [!UICONTROL Gantt-Diagramm]

<!-- Audited: 5/2025 -->

Sie können konfigurieren, welche Informationen sowohl im Gantt-Diagramm für die Aufgabenliste als auch im Gantt-Diagramm für die Projektliste angezeigt werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel zu befolgen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Neu: Leicht<p>
   <p>Oder</p>
   <p>Aktuell: Überprüfung</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben in [!UICONTROL View] oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL View] oder höher Zugriff auf das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Grundlegendes zu Anzeigeoptionen

In der folgenden Tabelle sind die Anzeigeoptionen für das [!UICONTROL Gantt-Diagramm] aufgeführt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Tatsächliche Termine</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gant.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Tatsächliches Startdatum] und [!UICONTROL Tatsächliches Abschlussdatum] werden mit einem Dreieckssymbol angezeigt. Wenn das tatsächliche Abschlussdatum von  null ist, wird nur das tatsächliche Startdatum von  angezeigt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Übersicht über das Projekt [!UICONTROL Tatsächliches Abschlussdatum] </a> und <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Übersicht über das Projekt [!UICONTROL Tatsächliches Startdatum] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL -Zuweisungen]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assignments_in_gant.png" style="width: 312;height: 203;"> </td> 
   <td> <p>Zeigt die Aufgabenzugewiesenen an. Bewegen Sie den Mauszeiger über den Link Details neben dem Namen des Verantwortlichen, um genauere Informationen über ihn anzuzeigen, einschließlich des Prozentsatzes seiner Zuordnung zur Aufgabe.</p> <p>Bevollmächtigte Personen werden nicht im [!UICONTROL Gantt-Diagramm] angezeigt, wenn das [!UICONTROL Gantt-Diagramm] nach PDF exportiert wird. Wenn das [!UICONTROL Gantt-Diagramm] nach PDF exportiert wird, werden die Verantwortlichen nur in der Aufgabenliste angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gant.png"> </td> 
   <td> <p>Ein Projekt-Snapshot, der die wichtigsten Daten über das Projekt darstellt, die im ursprünglichen Projektplan enthalten sind. Baselines können über die gesamte Zeitleiste des Projekts erstellt werden. Wenn Sie die Anzeige von Baselines im [!UICONTROL Gantt-Diagramm] aktivieren, wählen Sie die Baseline aus, die Sie anzeigen möchten. Sie können jeweils nur eine Baseline auf dem [!UICONTROL Gantt-Diagramm] anzeigen. Sie wird in Form eines grauen Balkens angezeigt.</p> <p>Weitere Informationen zu Baselines finden Sie unter <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">Erstellen von </a>).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commit-Datum]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>Das Datum, das ein Verantwortlicher als Zusage für den Zeitpunkt gibt, zu dem die Aufgabe abgeschlossen wird, wird mit einer Markierung im [!UICONTROL Gantt-Diagramm] angezeigt. </p> <p>Weitere Informationen zu Commit-Terminen finden Sie unter <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Commit Date] - Übersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % complete]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gant.png"> </td> 
   <td>  Der Prozentsatz der abgeschlossenen Aufgabe wird in der Aufgabenzeile angezeigt.<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kritischer Pfad]</td> 
   <td> <img src="assets/critical-path-2.png" alt="critical_path_2.png"> </td> 
   <td>Die Aufgaben, die sich auf die Zeitleiste des Projekts auswirken könnten, werden als Teil des kritischen Pfads betrachtet und sind deutlich rot gekennzeichnet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Diamanten</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>Nach der Aufgabe, die mit einem Meilenstein verbunden ist, wird ein Diamantsymbol angezeigt. Bewegen Sie den Mauszeiger über einen Meilenstein, um den Namen und das Datum des Meilensteins anzuzeigen. Der [!DNL Workfront]-Administrator bestimmt die Farbe jedes Meilenstein-Diamanten.</p> <p>Weitere Informationen zu Meilensteinen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Meilensteinpfad erstellen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] Zeilen</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gant.png" style="width: 270;height: 209;"> </td> 
   <td> <p>Nach der Aufgabe, die mit einem Meilenstein verbunden ist, wird eine Zeile angezeigt. Bewegen Sie den Mauszeiger über einen Meilenstein, um den Namen und das Datum des Meilensteins anzuzeigen. Der [!DNL Workfront] bestimmt die Farbe jeder Meilensteinlinie.</p> <p> Weitere Informationen zu Meilensteinen finden Sie unter  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Meilensteinpfad erstellen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorgänger]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="precessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>Eine Linie zwischen zwei Aufgaben, die die Vorgängerbeziehung zwischen den beiden Aufgaben anzeigt. Um eine einzelne Vorgängerlinie hervorzuheben, bewegen Sie den Mauszeiger darüber. Klicken Sie darauf, um sie hervorgehoben zu halten. Sie können jeweils nur eine Vorgängerzeile markieren.</p> <p>Ein [!UICONTROL Vorgänger]-Symbol wird neben einer Aufgabe angezeigt, die eine Vorgängerbeziehung aufweist, die mehrere Seiten im Gantt-Diagramm umfasst, oder bei einer Aufgabe, die einen projektübergreifenden Vorgänger hat.</p> <p>Klicken Sie auf das Symbol [!UICONTROL Vorgänger], um alle Vorgänger- und Nachfolgeaufgaben und ihre Details anzuzeigen, z. B. Aufgabenname, Typ der Vorgängerbeziehung und wichtige Daten.</p> <p>Hinweis: Das [!UICONTROL Gantt-Diagramm] in einer Liste von Projekten zeigt Informationen zu projektübergreifenden Vorgängern an. Weitere Informationen zum Erstellen von Vorgängerbeziehungen zwischen verschiedenen Projekten finden Sie <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Erstellen von projektübergreifenden Vorgängern</a></p> <p>Weitere Informationen zu Vorgängern finden Sie unter <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">Erzwingen von </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verlaufsstatus]</td> 
   <td> <p>[!UICONTROL on time] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__oct._2017.png"></p> <p>[!UICONTROL dahinter]    <img src="assets/task-behind--oct.-2017.png" alt="task_Behind__Oct._2017.png"></p> <p>[!UICONTROL Gefährdet]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>In Verzug        <img src="assets/task-late-oct.2017.png" alt="task_late_oct.2017.png"></p> </td> 
   <td> <p> </p> <p>Der Status des aktuellen Fortschritts bei einer bestimmten Aufgabe. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Übersicht über den -Fortschrittsstatus</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Voraussichtliche Termine</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gant_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>Die erwartete Zeitleiste, die das voraussichtliche Start- und Abschlussdatum auf der Basis der aktuellen abgeschlossenen Arbeit plus der verbleibenden Arbeit markiert. </p> <p>Weitere Informationen zu voraussichtlichen Abschlussdaten finden Sie unter <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurieren von Anzeigeoptionen

1. Navigieren Sie zum **Gantt-Diagramm für Aufgabenliste** oder **Gantt-Diagramm für Projektliste**.\
   Weitere Informationen dazu, wo sich eines der beiden Gantt-Diagramme befindet, finden Sie unter [Erste Schritte mit dem [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. (Optional) Wählen Sie die Einstellung **Zu voraussichtlichem Datum wechseln**, um die Aufgaben nach ihrem voraussichtlichen Datum anzuzeigen. Standardmäßig werden Aufgaben nach ihrem geplanten Datum angezeigt.
1. Klicken Sie auf **Symbol** Optionen“. Das **Optionen** wird geöffnet.\
   ![options.png](assets/options-350x129.png)

1. Wählen Sie die Konfigurationsoptionen aus, die Sie im [!UICONTROL Gantt-Diagramm“ anzeigen &#x200B;].

   >[!NOTE]
   >
   > Nicht alle Konfigurationsoptionen sind in der Projektliste (Gantt[!UICONTROL Diagramm) &#x200B;].

1. Klicken Sie auf eine beliebige Stelle im Gantt-Diagramm, um das Dialogfeld **Optionen** zu schließen.
