---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Work Effort - Übersicht
description: Work Effort - Übersicht
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 1%

---

# Work Effort - Übersicht

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

Als Projekt-Manager können Sie entscheiden, wie Sie den Arbeitsaufwand schätzen möchten, den Aufgaben in einem Projekt erledigen. Schätzen Sie den Arbeitsaufwand für die Durchführung von Aufgaben anhand eines der folgenden Indikatoren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Geplante Stunden</td> 
   <td> <p> Ein manueller numerischer Eintrag oder eine Adobe Workfront-Berechnung, die die Anzahl der Stunden anzeigt, die für die Fertigstellung einer Aufgabe durch die einer Aufgabe zugewiesenen Ressourcen erforderlich wären. </p> <p>Beachten Sie Folgendes zum Thema „Geplante Stunden“: </p> 
    <ul> 
     <li>Dies ist die Standardmethode. </li> 
     <li>Geplante Stunden können nur für Aufgaben mit dem Dauertyp „Berechnete Zuweisung“ oder „Einfach“ manuell aktualisiert werden. </li> 
    </ul> <p>Informationen zu den geplanten Stunden finden Sie unter <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Übersicht über die geplanten Stunden</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Work Effort </td> 
   <td> <p>Eine manuelle Beschriftung, die definiert, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand benötigt, um eine Aufgabe abzuschließen. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>Beachten Sie Folgendes zum Work Effort:</p> 
    <ul> 
     <li>Dieses Feld ist nur für Aufgaben mit dem Typ Einfache Dauer verfügbar. </li> 
     <li>Sie können die Verwendung dieser Kennzeichnung aktivieren und den Prozentsatz der damit verbundenen Arbeitszeit auf Projektebene definieren. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

In diesem Artikel wird beschrieben, was Work Effort ist und wie Sie ihn zur Schätzung des Arbeitsaufwands für Ihre Aufgaben verwenden sollten.

>[!NOTE]
>
>Geplante Stunden und Arbeitsaufwand beeinflussen sich gegenseitig. Durch die Aktualisierung der geplanten Stunden kann der Arbeitsaufwand aktualisiert werden, während durch die Aktualisierung des Arbeitsaufwands die geplanten Stunden der Aufgabe aktualisiert werden können.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für ein Projekt und dessen Aufgaben</p>  </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current: Plan </p>
   Or
   <p>New: Standard </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project and its tasks</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen zur Verwendung von Work Effort

* Wenn die Projektaufgaben 0 geplante Stunden haben und Sie die Einstellung Work Effort verwenden aktivieren, um die geplanten Stunden für die Aufgabe automatisch für das Projekt zu berechnen, ist der standardmäßige Arbeitsaufwand, der ihnen zugeordnet ist, Medium. Die „Geplante Stunden“ werden für Aufgaben vom Typ „Einfache Dauer“ automatisch aktualisiert. Weitere Informationen finden Sie im Abschnitt [Arbeitsaufwand](#levels-of-work-effort) in diesem Artikel.
* Wenn die Projektaufgaben über Stunden verfügen, die größer als 0 sind, und Sie die Einstellung Work Effort verwenden aktivieren, um die geplanten Stunden für die Aufgabe automatisch für das Projekt zu berechnen, wird die Arbeitsaufwand-Ebene entsprechend der Anzahl der geplanten Stunden aktualisiert, ohne dass der Betrag der geplanten Stunden für Aufgaben vom Typ „Einfache Dauer“ geändert wird. Weitere Informationen finden Sie im Abschnitt [Wie Workfront den Arbeitsaufwand anhand der geplanten Stunden berechnet](#how-workfront-calculates-work-effort-based-on-planned-hours) in diesem Artikel.
* Wenn die Projektaufgaben 0 Geplante Stunden aufweisen und Sie die Einstellung Work Effort verwenden aktivieren, um die geplanten Stunden für die Aufgabe automatisch für das Projekt zu berechnen, und dann den Arbeitsaufwand von Medium auf „Klein“ oder „Groß“ ändern, werden auch die geplanten Stunden aktualisiert. Weitere Informationen finden Sie im Abschnitt [Wie Workfront die geplanten Stunden basierend auf dem Arbeitsaufwand berechnet](#how-workfront-calculates-planned-hours-based-on-work-effort) in diesem Artikel.
* Wenn Sie Aufgaben inline bearbeiten und gleichzeitig die Felder „Geplante Stunden“ und „Arbeitsaufwand“ für die Aufgabe ändern, werden die geplanten Stunden mit dem von Ihnen angegebenen Wert aktualisiert, während der Wert für „Arbeitsaufwand“ auf der Grundlage Ihrer aktualisierten geplanten Stunden berechnet wird.
* Wenn Sie den Work Effort-Wert einer Aufgabe aktualisieren, wird die Dauer nicht mehr automatisch auf der Grundlage der geplanten Stunden berechnet. Weitere Informationen zur Berechnung der Dauer für Aufgaben mit einfacher Dauer finden Sie unter [Duration Type overview: Simple](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* Wenn Sie den Dauertyp einer Aufgabe von „Einfach“ in einen anderen Typ ändern, wird das Work Effort-Feld in der Aufgabe ausgeblendet. Die geplanten Stunden bleiben unverändert.
* Sie können die Work Effort-Ebene für eine übergeordnete Aufgabe nicht aktualisieren. Der Work Effort Level für eine übergeordnete Aufgabe wird automatisch auf Basis der geplanten Stunden für die Aufgaben berechnet, wobei es sich um eine Zusammenfassung aller untergeordneten Aufgaben handelt. Informationen zu übergeordneten Aufgaben finden Sie unter [Unteraufgaben erstellen](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## Work Effort anstelle von „Geplante Stunden“ aktivieren

1. Gehen Sie zu einem Projekt und klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-icon.png) und klicken Sie dann auf **Bearbeiten**.
1. Klicken Sie auf **Aufgabeneinstellungen** und wählen Sie dann die Option **Work Effort verwenden , um die geplanten Stunden für die Aufgabe automatisch zu berechnen**. Diese Option ist standardmäßig deaktiviert.

   ![Work Effort on Projects](assets/nwe-work-effort-on-projects-350x182.png)

   Weiterführende Informationen dazu, wie Sie Work Effort für ein Projekt aktivieren, finden Sie im Abschnitt „Aufgabeneinstellungen“ im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicken Sie **linken** auf „Aufgaben“ und dann auf den Namen einer Aufgabe, um darauf zuzugreifen.
1. Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/more-icon.png) und dann auf **Bearbeiten**. Stellen Sie sicher, dass die Aufgabe einen einfachen Dauertyp aufweist.

   >[!TIP]
   >
   >Sie können den Work Effort für eine Aufgabe auch im Abschnitt „Aufgabendetails“ aktualisieren.

1. Klicken Sie im Bereich **Übersicht** auf das Dropdown-Menü Work Effort , um den für die Ausführung der Aufgabe erforderlichen Arbeitsaufwand zu korrigieren.

   ![Work Effort auf der Seite „Aufgabe bearbeiten“](assets/work-effort-on-edit-task-page-350x239.png)

   Weitere Informationen zum Aktualisieren des Work Effort-Felds in einer Aufgabe finden Sie in den folgenden Artikeln:

   * Der Abschnitt „Übersicht“ im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
   * [Verwalten von Aufgabeninformationen im Bereich „Aufgabendetails - Übersicht“](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## Arbeitsaufwand {#levels-of-work-effort}

Als Projekt-Manager können Sie drei Arbeitsebenen für Ihre Projekte identifizieren. Jeder Aufwand entspricht einem Prozentsatz der täglichen Zeit, die Benutzende benötigen, um die Aufgabe abzuschließen.

Beim Einrichten des Arbeitsaufwands müssen Sie sich die Frage stellen: „Wie viel Zeit sollte ein Benutzer, der dieser Aufgabe zugewiesen ist, täglich darauf verwenden, um sie rechtzeitig zu erledigen?“

Die folgende Tabelle zeigt den möglichen Arbeitsaufwand und die entsprechenden Standardprozentsätze. Als Projekt-Manager können Sie die Prozentsätze an die Bedürfnisse Ihrer Organisation anpassen. Dies geschieht beim Bearbeiten eines Projekts. Informationen zum Bearbeiten von Projekten finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Als Workfront-Administrator definieren Sie unter „Setup“ im Bereich „Projektvoreinstellungen“ die Anzahl der typischen Arbeitsstunden pro Arbeitstag. Dies ist die tägliche Arbeitszeit, die als Arbeitszeit gilt. Informationen zum Konfigurieren von Projektvoreinstellungen für Ihre Workfront-Instanz finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>In den folgenden Beispielen gehen wir davon aus, dass der Workfront-Administrator die typischen Stunden pro Arbeitstag auf 8 Stunden festgelegt hat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Arbeitsaufwand</td> 
   <td>Prozentwerte</td> 
  </tr> 
  <tr> 
   <td>Klein </td> 
   <td>Ein geringer Aufwand zum Erledigen einer Aufgabe ist auf 25 % der typischen Stunden pro Arbeitstag festgelegt. Das bedeutet, dass es bei einer Aufgabe mit diesem Arbeitsaufwand bis zu 2 Stunden pro Tag dauern sollte, bis sie an einem Tag erledigt ist. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Mittel</td> 
   <td> <p>Der Aufwand für die Erfüllung einer Aufgabe in Medium beträgt 50 % der typischen Arbeitszeit pro Arbeitstag. Das bedeutet, dass es bei einer Aufgabe mit diesem Arbeitsaufwand mehr als 2 und weniger als 6 Stunden dauern sollte, bis sie an einem Tag erledigt ist. <code>(0.50*80=4)</code> </p> <p>Hinweis: Wenn die Einstellung Work Effort zur automatischen Berechnung der geplanten Stunden für die Aufgabe verwenden für das Projekt aktiviert ist, ist dies die Standardeinstellung für eine Aufgabe, wenn die Aufgabe 0 geplante Stunden hatte, bevor diese Einstellung aktiviert wurde. Dies führt dazu, dass die geplanten Stunden für die Aufgabe auf 4 Stunden aktualisiert werden. </p> </td> 
  </tr> 
  <tr> 
   <td>Groß</td> 
   <td>Ein hoher Aufwand für die Ausführung einer Aufgabe wird auf 75 % der typischen Stunden pro Arbeitstag festgelegt. Das bedeutet, dass es 6 Stunden oder mehr dauern sollte, bis eine Aufgabe mit diesem Arbeitsaufwand an einem Tag erledigt ist. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Wie Workfront die geplanten Stunden basierend auf dem Work Effort berechnet {#how-workfront-calculates-planned-hours-based-on-work-effort}

Wenn Sie die Einstellung Work Effort zum automatischen Berechnen der geplanten Stunden für eine Aufgabe in einem Projekt verwenden, berechnet Workfront die Anzahl der geplanten Stunden für eine Aufgabe mit einem einfachen Dauertyp anhand der folgenden Formel:

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

Eine Aufgabe mit einer Dauer von 3 Tagen und einem Arbeitsaufwand von Medium hat beispielsweise 12 geplante Stunden:

```
Planned Hours = 3*4=12
```

wobei der Wert für „Typische Stunden pro Arbeitstag“ 8 Stunden beträgt.

>[!TIP]
>
>Wenn ein Vorgang mehreren Ressourcen zugewiesen wird, werden die geplanten Stunden für jeden Tag der Aufgabendauer gleichmäßig auf jede Ressource verteilt.

## Wie Workfront den Arbeitsaufwand anhand der geplanten Stunden berechnet {#how-workfront-calculates-work-effort-based-on-planned-hours}

Wenn Sie die Einstellung Work Effort verwenden aktivieren, um die geplanten Stunden für eine Aufgabe automatisch zu berechnen, und bereits geplante Stunden für die Aufgabe vorhanden sind, oder die Anzahl der geplanten Stunden für die Aufgabe bearbeiten, aktualisiert Workfront den Work Effort-Wert.

Workfront verwendet die folgende Formel, um den Arbeitsaufwand entsprechend den geplanten Stunden zu aktualisieren:

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

Wenn Sie beispielsweise eine Aufgabe mit einer Dauer von 2 Tagen haben und die geplanten Stunden von 8 auf 20 Stunden aktualisieren, wird der Arbeitsaufwand für die Aufgabe von Medium auf „Groß“ aktualisiert:

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Arbeitsaufwand für Aufgaben und Projekte suchen

* [Work Effort für Projekte](#work-effort-for-projects)
* [Work Effort für Aufgaben](#work-effort-for-tasks)

### Work Effort für Projekte {#work-effort-for-projects}

Sie können den Abschnitt Work Effort (Arbeitsaufwand) eines Projekts in folgendem Bereich suchen:

* Der Bereich Aufgabeneinstellungen im Feld Projekt bearbeiten

### Work Effort für Aufgaben {#work-effort-for-tasks}

Sie können das Work Effort -Feld für eine Aufgabe in den folgenden Bereichen suchen:

* Der Bereich Überblick im Feld Aufgabe bearbeiten
* Der Bereich „Übersicht“ im Abschnitt „Aufgabendetails“ im Arbeitszeitbereich
* Aufgabenliste oder Bericht
