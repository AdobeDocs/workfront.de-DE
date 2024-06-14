---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über den Arbeitsaufwand
description: Übersicht über den Arbeitsaufwand
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# Übersicht über den Arbeitsaufwand

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

Als Projektmanager können Sie entscheiden, wie Sie den für die Ausführung von Aufgaben in einem Projekt benötigten Arbeitsaufwand schätzen möchten. Schätzen Sie anhand eines der folgenden Indikatoren den für die Durchführung der Aufgaben erforderlichen Arbeitsaufwand:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Geplante Stunden</td> 
   <td> <p> Ein manueller numerischer Eintrag oder eine Adobe Workfront-Berechnung, die anzeigt, wie viele Stunden es dauern würde, bis die einer Aufgabe zugewiesenen Ressourcen abgeschlossen sind. </p> <p>Beachten Sie Folgendes zu geplanten Stunden: </p> 
    <ul> 
     <li>Dies ist die Standardmethode. </li> 
     <li>Sie können geplante Stunden nur für Aufgaben mit dem Typ "Berechnete Zuweisung"oder "Einfach"manuell aktualisieren. </li> 
    </ul> <p>Weitere Informationen zu geplanten Stunden finden Sie unter <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Übersicht über geplante Stunden</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Work Effort </td> 
   <td> <p>Eine manuelle Bezeichnung, die definiert, ob ein Benutzer einen kleinen, mittleren oder großen täglichen Aufwand für die Ausführung einer Aufgabe benötigt. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>Beachten Sie Folgendes zum Arbeitsaufwand:</p> 
    <ul> 
     <li>Dieses Feld ist nur für Aufgaben mit dem Typ Einfache Dauer verfügbar. </li> 
     <li>Sie können die Verwendung dieses Titels aktivieren und den Prozentsatz der damit verbundenen Arbeitszeit auf Projektebene definieren. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

In diesem Artikel wird beschrieben, was Arbeitsaufwand ist und wie Sie es bei der Schätzung des Arbeitsaufwands für Ihre Aufgaben verwenden sollten.

>[!NOTE]
>
>Geplante Stunden und Arbeitsaufwand beeinflussen einander. Durch die Aktualisierung der geplanten Stunden kann der Arbeitsaufwand aktualisiert werden, und durch die Aktualisierung des Arbeitsaufwands können die geplanten Stunden der Aufgabe aktualisiert werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktuell: Plan </p>
   Oder
   <p>Neu: Standard </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt und dessen Aufgaben verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Verwendung von Arbeitsaufwand

* Wenn die Projektaufgaben 0 geplante Stunden haben und Sie die Einstellung &quot;Arbeitsaufwand verwenden&quot;aktivieren, um die geplante Aufgabe für das Projekt automatisch zu berechnen, ist der ihnen zugeordnete Arbeitsaufwand standardmäßig &quot;Mittel&quot;. Die Aufgaben &quot;Geplante Stunden&quot;werden automatisch für die einfache Dauer aktualisiert. Weitere Informationen finden Sie im Abschnitt .  [Arbeitsumfang](#levels-of-work-effort) in diesem Artikel.
* Wenn für die Projektaufgaben geplante Stunden größer als 0 sind und Sie die Option &quot;Use Work Effort&quot;aktivieren, um die Einstellung für geplante Aufgaben im Projekt automatisch zu berechnen, wird der Arbeitsaufwand entsprechend der Anzahl der geplanten Stunden aktualisiert, ohne dass sich die Anzahl der geplanten Stunden für einfache Dauer ändert. Weitere Informationen finden Sie im Abschnitt . [Berechnung des Arbeitsaufwands durch Workfront auf der Grundlage geplanter Arbeitszeiten](#how-workfront-calculates-work-effort-based-on-planned-hours) in diesem Artikel.
* Wenn die Projektaufgaben 0 geplante Stunden haben und Sie die Option &quot;Use Work Effort&quot;aktivieren, um die für das Projekt geplante Aufgabe automatisch zu berechnen, und dann die Arbeitsleistung von &quot;Medium&quot;zu &quot;Small&quot;oder &quot;Large&quot;aktualisieren, werden auch die geplanten Stunden aktualisiert. Weitere Informationen finden Sie im Abschnitt . [Berechnung der geplanten Arbeitsstunden durch Workfront auf der Grundlage der Arbeitsbelastung](#how-workfront-calculates-planned-hours-based-on-work-effort) in diesem Artikel.
* Wenn Sie Aufgaben inline bearbeiten und gleichzeitig sowohl das Feld &quot;Geplante Stunden&quot;als auch das Feld &quot;Arbeitsaufwand&quot;für die Aufgabe ändern, werden die geplanten Stunden mit dem von Ihnen angegebenen Wert aktualisiert, während der Wert für Arbeitsaufwand auf der Grundlage der aktualisierten geplanten Stunden berechnet wird.
* Wenn Sie den Arbeitsaufwand einer Aufgabe aktualisieren, wird die Dauer nicht mehr automatisch auf der Grundlage der geplanten Stunden berechnet. Weitere Informationen zur Berechnung der Dauer für Aufgaben mit einfacher Dauer finden Sie unter [Übersicht über den Dauer-Typ: Einfach](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* Wenn Sie die Dauer einer Aufgabe von &quot;Einfach&quot;in einen anderen Typ ändern, wird das Feld &quot;Arbeitsaufwand&quot;für die Aufgabe ausgeblendet. Die geplanten Stunden bleiben unverändert.
* Sie können die Arbeitsaufwand-Ebene für eine übergeordnete Aufgabe nicht aktualisieren. Der Arbeitsaufwand für eine übergeordnete Aufgabe wird automatisch anhand der Anzahl der geplanten Stunden für die Aufgaben berechnet, bei denen es sich um eine Datenaggregation aller untergeordneten Aufgaben handelt. Weitere Informationen zu übergeordneten Aufgaben finden Sie unter [Erstellen von Unteraufgaben](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## Aktivieren Sie die Verwendung von Arbeitsaufwand anstelle von geplanten Stunden.

1. Wechseln Sie zu einem Projekt und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-icon.png)Klicken Sie auf **Bearbeiten**.
1. Klicks **Aufgabeneinstellungen** und wählen Sie dann die Option **Verwenden Sie den Arbeitsaufwand, um die geplanten Aufgaben automatisch zu berechnen.**. Diese Option ist standardmäßig deaktiviert.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   Weitere Informationen zum Aktivieren der Verwendung von Work Effort für ein Projekt finden Sie im Abschnitt &quot;Aufgabeneinstellungen&quot;im [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md) Artikel.

1. Klicks **Aufgaben** Klicken Sie im linken Bereich auf den Namen einer Aufgabe, um darauf zuzugreifen.
1. Klicken Sie auf **Mehr** Menü ![](assets/more-icon.png)Klicken Sie auf **Bearbeiten**. Stellen Sie sicher, dass die Aufgabe einen einfachen Dauerhaltungstyp aufweist.

   >[!TIP]
   >
   >Sie können den Arbeitsaufwand für eine Aufgabe auch im Abschnitt Aufgabendetails aktualisieren.

1. Im **Übersicht** klicken Sie auf das Dropdown-Menü &quot;Arbeitsaufwand&quot;, um den Aufwand zu korrigieren, der zum Abschließen der Aufgabe erforderlich ist.

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   Weitere Informationen zum Aktualisieren des Felds &quot;Arbeitsaufwand&quot;für eine Aufgabe finden Sie in den folgenden Artikeln:

   * Der Abschnitt &quot;Übersicht&quot;im [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md) Artikel
   * [Verwalten von Aufgabeninformationen im Bereich &quot;Aufgabendetails - Übersicht&quot;](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## Arbeitsumfang {#levels-of-work-effort}

Als Projektmanager können Sie drei Arbeitsebenen für Ihre Projekte identifizieren. Jede Aufwandsstufe entspricht einem Prozentsatz der täglichen Zeit, die Benutzer zum Abschließen der Aufgabe benötigen.

Beim Einrichten des Arbeitsaufwands müssen Sie sich die Frage stellen: &quot;Wie viel Zeit sollte ein Benutzer dieser Aufgabe täglich zuweisen, um sie rechtzeitig zu erledigen?&quot;

Die folgende Tabelle zeigt die möglichen Stufen des Arbeitsaufwands und die entsprechenden Standardprozentsätze. Als Projektmanager können Sie die Prozentsätze entsprechend den Anforderungen Ihres Unternehmens aktualisieren. Dies erfolgt beim Bearbeiten eines Projekts. Weitere Informationen zum Bearbeiten von Projekten finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Als Workfront-Administrator definieren Sie die typischen Arbeitszeiten pro Arbeitstag im Bereich &quot;Projekteinstellungen&quot;von &quot;Einrichtung&quot;. Dies ist die tägliche Arbeitszeit, die als Arbeitszeit betrachtet wird. Informationen zum Konfigurieren von Projekteinstellungen für Ihre Instanz von Workfront finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>In den folgenden Beispielen gehen wir davon aus, dass der Workfront-Administrator die typischen Arbeitsstunden pro Arbeitstag auf 8 Stunden festgelegt hat.

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
   <td>Ein geringer Aufwand für das Abschließen einer Aufgabe ist auf 25 % der typischen Arbeitsstunden pro Arbeitstag festgelegt. Dies bedeutet, dass eine Aufgabe, der diese Arbeitsbelastung zugewiesen wurde, bis zu zwei Stunden am Tag in einem Tag abgeschlossen sein sollte. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Mittel</td> 
   <td> <p>Der mittlere Aufwand für das Abschließen einer Aufgabe beträgt 50 % der typischen Arbeitsstunden pro Arbeitstag. Dies bedeutet, dass eine Aufgabe, der dieser Arbeitsaufwand zugewiesen wird, mehr als 2 bis weniger als 6 Stunden in Anspruch nehmen sollte, um sie an einem Tag abzuschließen. <code>(0.50*80=4)</code> </p> <p>Hinweis: Wenn die Einstellung "Arbeitsaufwand zur automatischen Berechnung der geplanten Aufgaben verwenden"für das Projekt aktiviert ist, ist dies die Standardeinstellung für eine Aufgabe, wenn für die Aufgabe vor Aktivierung dieser Einstellung 0 geplante Stunden vorgesehen waren. Dadurch wird die Aufgabe Geplante Stunden auf 4 Stunden aktualisiert. </p> </td> 
  </tr> 
  <tr> 
   <td>Groß</td> 
   <td>Ein großer Aufwand für das Abschließen einer Aufgabe ist auf 75 % der typischen Arbeitsstunden pro Arbeitstag festgelegt. Dies bedeutet, dass eine Aufgabe, der diese Arbeitsleistung zugewiesen wurde, innerhalb eines Tages mindestens sechs Stunden dauern sollte, bis sie abgeschlossen ist. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Berechnung der geplanten Arbeitsstunden durch Workfront auf der Grundlage der Arbeitsbelastung {#how-workfront-calculates-planned-hours-based-on-work-effort}

Wenn Sie die Einstellung &quot;Arbeitsaufwand verwenden&quot;aktivieren, um Aufgaben, die für ein Projekt geplant sind, automatisch zu berechnen, berechnet Workfront die Anzahl der geplanten Stunden für eine Aufgabe mit dem Typ Einfache Dauer anhand der folgenden Formel:

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

Beispielsweise hat eine Aufgabe mit einer Dauer von 3 Tagen und einer Arbeitsaufgabe mit mittlerem Arbeitsaufwand 12 geplante Stunden:

```
Planned Hours = 3*4=12
```

wobei der typische Wert für Stunden pro Arbeitstag 8 Stunden beträgt.

>[!TIP]
>
>Wenn eine Aufgabe mehreren Ressourcen zugewiesen wird, werden die geplanten Stunden für jeden Tag der Dauer der Aufgabe gleichmäßig auf jede Ressource verteilt.

## Berechnung des Arbeitsaufwands durch Workfront auf der Grundlage geplanter Arbeitszeiten {#how-workfront-calculates-work-effort-based-on-planned-hours}

Wenn Sie die Einstellung &quot;Arbeitsaufwand verwenden&quot;aktivieren, um Aufgaben, die für ein Projekt geplant sind, automatisch zu berechnen, und Sie bereits über geplante Stunden für die Aufgabe verfügen oder die Anzahl der geplanten Stunden für die Aufgabe bearbeiten, aktualisiert Workfront den Wert für Arbeitsaufwand.

Workfront verwendet die folgende Formel, um den Arbeitsaufwand entsprechend den geplanten Stunden zu aktualisieren:

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

Wenn Sie beispielsweise eine Aufgabe mit einer Dauer von 2 Tagen haben und die geplanten Stunden von 8 auf 20 Stunden aktualisieren, wird der Arbeitsaufwand für die Aufgabe von &quot;Mittel&quot;auf &quot;Groß&quot;aktualisiert:

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Arbeitsaufwand für Aufgaben und Projekte suchen

* [Arbeitsaufwand für Projekte](#work-effort-for-projects)
* [Arbeitsaufwand für Aufgaben](#work-effort-for-tasks)

### Arbeitsaufwand für Projekte {#work-effort-for-projects}

Sie finden den Abschnitt &quot;Arbeitsaufwand&quot;für ein Projekt in folgendem Bereich:

* Bereich &quot;Aufgabeneinstellungen&quot;im Feld &quot;Projekt bearbeiten&quot;

### Arbeitsaufwand für Aufgaben {#work-effort-for-tasks}

Sie können das Feld &quot;Arbeitsaufwand&quot;für eine Aufgabe in den folgenden Bereichen finden:

* Der Übersichtsbereich im Feld &quot;Aufgabe bearbeiten&quot;
* Der Übersichtsbereich des Abschnitts &quot;Aufgabendetails&quot;im Arbeitszeitbereich
* Aufgabenliste oder Bericht
