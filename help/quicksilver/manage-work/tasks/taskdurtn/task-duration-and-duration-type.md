---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Übersicht über Aufgabendauer und -dauer
description: Die Aufgabendauer ist die Differenz zwischen dem geplanten Abschlussdatum und dem geplanten Startdatum der Aufgabe. Die Dauer gibt den Zeitraum an, der zum Abschluss der Aufgabe verfügbar ist.
author: Alina
feature: Work Management
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1383'
ht-degree: 2%

---

# Übersicht über Aufgabendauer und -dauer

Die Aufgabendauer ist die Differenz zwischen dem geplanten Abschlussdatum und dem geplanten Startdatum der Aufgabe. Die Dauer gibt den Zeitraum an, der zum Abschluss der Aufgabe verfügbar ist.

Der Aufgabentyp gibt die Beziehung zwischen der Anzahl der einer Aufgabe zugewiesenen Ressourcen, dem Gesamtaufwand und der Gesamtdauer der Aufgabe an.

## Aufgabendauer - Übersicht

>[!NOTE]
>
>Unter Berücksichtigung der Projektzeit des Primären Verantwortlichen können sich die geplanten Aufgabendaten anpassen, die Aufgabendauer bleibt jedoch gleich. Informationen zur Berücksichtigung der Zeitdauer des Primären Verantwortlichen bei der Projektplanung finden Sie unter  [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Wenn das tatsächliche Start- und das tatsächliche Abschlussdatum der Aufgabe außerhalb des Zeitplans des Projekts, des primären Verantwortlichen oder des Standardzeitplans liegen, beträgt die Aufgabendauer null.

**Beispiel:** Wenn Sie einen Zeitplan haben, der um 9:00 Uhr beginnt und um 23:00 Uhr endet und für eine Aufgabe geplant ist, die um 14:00 Uhr beginnt und um 16:00 Uhr endet, beträgt die Dauer der Aufgabe null.

Im Folgenden finden Sie zwei Szenarien, in denen die Dauer in Adobe Workfront berechnet wird.

* Wenn die Aufgabe einem Benutzer zugewiesen ist, verwendet Workfront einen der folgenden Zeitpläne, in der angegebenen Reihenfolge, um die Dauer zu berechnen:

   1. Workfront berücksichtigt den Benutzerzeitplan.
   1. Wenn der Benutzer keinem Zeitplan zugeordnet ist, berücksichtigt Workfront den Zeitplan des Projekts.
   1. Wenn das Projekt nicht mit einem Zeitplan verknüpft ist, berücksichtigt Workfront den Standardzeitplan Ihres Systems. Weitere Informationen zu Zeitplänen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Wenn die Aufgabe mehreren Benutzern zugewiesen ist:

   Workfront berücksichtigt entweder den Zeitplan des Projekts oder den des Hauptverantwortlichen.

   Ihr Workfront-Administrator legt fest, welcher Zeitplan von Workfront verwendet wird, wenn eine Aufgabe mehreren Benutzern zugewiesen wird. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Die Schritte ähneln dem ersten Szenario, nachdem Sie ermittelt haben, welcher Zeitplan von Workfront zur Berechnung der Dauer verwendet wird.

## Zeiteinheiten für Aufgabendauer

Sie können die Aufgabendauer sowohl in der regulären Zeit als auch in der verstrichenen Zeit zwischen dem geplanten Start- und dem geplanten Abschlussdatum angeben.

Beim Aktualisieren der Dauer von Aufgaben in einer Liste können Sie die folgenden Abkürzungen verwenden, um Zeiteinheiten in Workfront anzugeben:

| Zeiteinheit | Abkürzung |
|---|---|
| Minuten | M |
| Stunden | H |
| Tage. Dies ist die Standardeinstellung. | D |
| Wochen | M |
| Monate | D |
| Verstrichene Minuten | EM |
| Verstrichene Stunden | EH |
| Verstrichene Tage | ED |
| Verstrichene Wochen | EW |
| Verstrichene Monate | ET |

{style=&quot;table-layout:auto&quot;}

**Beispiel:** Wenn Sie angeben möchten, dass die Dauer einer Aufgabe 3 Tage ist, geben Sie &quot;3 ED&quot;in das Feld Dauer in eine Aufgabenliste ein.  Sie können auch die bevorzugte Option für die Zeiteinheit im verfügbaren Dropdownmenü beim Bearbeiten einer Aufgabe oder im Abschnitt Aufgabendetails auswählen. Informationen zum Bearbeiten von Aufgaben finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Beachten Sie Folgendes bei der Angabe der Dauer einer Aufgabe:

* Die verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und eine Verspätung umfasst. Mit anderen Worten, vergangene Zeit ist der Durchgang von Kalendertagen.
* Bei der regulären Zeit werden Feiertage, Wochenenden und eine Zeitüberschreitung berücksichtigt und von der Dauer der Aufgabe ausgeschlossen.

* Wenn Sie die Dauer einer Aufgabe in Wochen angeben, berechnet Workfront die Dauer in Tagen und Stunden anhand der von Ihrem Workfront-Administrator im Bereich &quot;Projekteinstellungen&quot;festgelegten Einstellungen für die typischen Wochentage und die typischen Stunden pro Arbeitstag.
* Workfront verwendet die Standarddauer von 4 Wochen für einen Monat bei der Berechnung der Dauer in Monaten.

## Übersicht über den Aufgabendauer-Typ

Durch die Verwaltung des Aufgabentyps können Sie konsistente Ressourcenzuweisungen entsprechend den Anforderungen der Aufgabe festlegen.

Der Typ der Dauer hilft bei der Beantwortung der folgenden Fragen:

* Wie beschäftigt werden wir sein?
* Wie groß ist die Arbeit?
* Wie lange wird es dauern?

![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)

## Definieren von Dauer-Typen

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row">Dauertyp </th> 
   <th scope="col"> <p><strong>Funktion</strong> </p> </th> 
   <th scope="col"> <p><strong>Auswirkungen von Ressourcen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Berechnete Zuweisung</strong> </p> </th> 
   <td scope="col"> <p>Berechnet den Zuordnungsprozentsatz für jeden Verantwortlichen einer Aufgabe. </p> <p>Wenn Sie diesen Dauerhaltungstyp auswählen, können Sie für die Aufgabe die jeweilige Dauer und die geplanten Stunden eingeben. Workfront teilt die geplanten Stunden durch die Anzahl der Stunden innerhalb der Aufgabendauer und anschließend durch die Anzahl der Ressourcen, die der Aufgabe zur Berechnung der Zuweisung für jeden Verantwortlichen zugewiesen sind.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Übersicht über den Durationstyp: Berechnete Zuweisung</a>.</p> </td> 
   <td scope="col">Die Dauer und die geplanten Stunden ändern sich nicht, wenn der Aufgabe Bevollmächtigte hinzugefügt oder entfernt werden. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Berechnete Arbeit</strong> </p> </th> 
   <td scope="col"> <p>Bestimmt die geplanten Stunden (Aufwandsmenge), die zum Abschluss der Aufgabe erforderlich sind.</p> <p>Wird normalerweise verwendet, wenn die der Aufgabe zugewiesenen Ressourcen für die gesamte Dauer der Aufgabe zugewiesen werden.</p> <p>Wenn Sie diesen Dauerhaltungstyp auswählen, können Sie für die Aufgabe eine individuelle Dauer eingeben. Workfront berechnet die geplanten Stunden für die Aufgabe, indem es die Anzahl der Tage in der Dauer mit der Anzahl der Arbeitsstunden im Zeitplan und der Anzahl der Verantwortlichen für die Aufgabe multipliziert. </p> <p>Sie können den Zuordnungsprozentwert jedes Bevollmächtigten manuell in die Aufgabe ändern, wodurch sich die Anzahl der geplanten Stunden verkürzt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Übersicht über den Durationstyp: Berechnete Arbeit</a>.</p> </td> 
   <td scope="col"> <p>Geplante Stunden erhöhen sich, wenn der Aufgabe die Zuweisung hinzugefügt wird. </p> <p>Die geplanten Stunden werden reduziert, wenn die Zuweisung aus der Aufgabe entfernt wird.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>Leistungsgesteuert</p> </th> 
   <td scope="col"> <p>Bestimmt die geplanten Stunden anhand der Anzahl der Ressourcen.</p> <p>Wenn Sie diesen Dauerhaltungstyp auswählen, können Sie für die Aufgabe eine individuelle Dauer eingeben. Workfront berechnet die geplanten Stunden für die Aufgabe, indem es die Anzahl der Tage in der Dauer durch die Anzahl der Arbeitsstunden im Zeitplan multipliziert und durch die Anzahl der Verantwortlichen für die Aufgabe dividiert. </p> <p>Sie können den Zuordnungsprozentwert jedes Verantwortlichen manuell an die Aufgabe anpassen, aber die Anzahl der geplanten Stunden bleibt gleich.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Übersicht über den Durationstyp: Aufwandsorientiert</a>.</p> </td> 
   <td scope="col"> <p>Die geplanten Stunden werden erhöht, wenn die Bevollmächtigten aus der Aufgabe entfernt werden.</p> <p>Die geplanten Stunden werden reduziert, wenn der Aufgabe die Zuweisung hinzugefügt wird. </p> <p>Die Dauer ändert sich nicht, unabhängig von der Anzahl der Bevollmächtigten oder ihrem Zeitplan. </p> <p>Die Dauer entspricht den geplanten Stunden. Die geplante Dauer entspricht den geplanten Stunden geteilt durch die Anzahl der Bevollmächtigten.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Einfach</strong> </p> </th> 
   <td scope="col"> <p>Bestimmt die geplanten Stunden und die Dauer (die für diesen Durationstyp gleich sind) anhand der Anzahl der Stunden, für die jeder Verantwortliche zugewiesen wird. </p> <p>Workfront berechnet die geplanten Stunden, indem es die geplanten zugewiesenen Stunden für jeden Bevollmächtigten addiert. </p> <p>Sie haben die Möglichkeit, die Anzahl der Stunden, die jedem Bevollmächtigten zugewiesen werden, manuell zu ändern und die Anzahl der geplanten Stunden und die Menge der Dauer entsprechend zu ändern. Wenn Sie eine Gesamtzahl der zugewiesenen Stunden für alle Bevollmächtigten wählen, wird diese Zahl gleichmäßig zwischen jedem Bevollmächtigten aufgeteilt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Übersicht über den Durationstyp: Einfach</a>.</p> </td> 
   <td scope="col"> <p>Die Stunden werden gleichmäßig auf die Bevollmächtigten verteilt, wenn Sie eine Gesamtzahl der zugewiesenen Stunden auswählen. Als Projektmanager können Sie jedoch die Stunden für jeden Verantwortlichen manuell anpassen. </p> <p>Sie können entweder die geplante Stunde und Dauer einer Aufgabe mit dem einfachen Typ Dauer inline oder auf Aufgabenebene bearbeiten. </p> <p>Wenn ein agiles Team einer Aufgabe zugewiesen ist, wird der Typ der Dauer automatisch auf Einfach gesetzt und kann nicht geändert werden. Die Aufgabendauer eines agilen Teams muss größer als 0 Minuten sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Die Dauer neuer Aufgaben

Der Dauer-Typ einer neuen Aufgabe entspricht dem in Ihrem System eingerichteten Dauer-Typ. Der Standardtyp für die Dauer ist &quot;Berechnete Zuweisung&quot;. Ihr Workfront-Administrator oder ein Gruppenadministrator kann den Standardtyp für die Dauer des Projekts für Ihr System oder die mit dem Projekt verknüpfte Gruppe aktualisieren. Weitere Informationen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Ändern der Dauer einer Aufgabe

Informationen zum Ändern der Dauer einer Aufgabe finden Sie unter [Aktualisierung des Zeitdauer-Typs einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
