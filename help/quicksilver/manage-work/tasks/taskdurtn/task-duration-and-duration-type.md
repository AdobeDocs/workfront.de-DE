---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Übersicht über Aufgabendauer und -dauer
description: Die Aufgabendauer ist die Differenz zwischen dem geplanten Abschlussdatum und dem geplanten Startdatum der Aufgabe. Die Dauer gibt den Zeitraum an, der zum Abschluss der Aufgabe verfügbar ist.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: b42436ad660642bd23638a8a44d9561513d748ed
workflow-type: tm+mt
source-wordcount: '1791'
ht-degree: 1%

---

# Übersicht über Aufgabendauer und -dauer

<!-- Audited: 12/2023 -->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

Die Aufgabendauer ist die Differenz zwischen dem geplanten Abschlussdatum und dem geplanten Startdatum der Aufgabe. Die Dauer gibt den Zeitraum an, der zum Abschluss der Aufgabe verfügbar ist.

Der Aufgabentyp gibt die Beziehung zwischen der Anzahl der einer Aufgabe zugewiesenen Ressourcen, dem Gesamtaufwand und der Gesamtdauer der Aufgabe an.

## Übersicht über die Aufgabendauer

Wenn das tatsächliche Start- und das tatsächliche Abschlussdatum der Aufgabe außerhalb des Zeitplans des Projekts, des primären Verantwortlichen oder des Standardzeitplans liegen, beträgt die Aufgabendauer null.

>[!BEGINSHADEBOX]

**BEISPIEL**
Wenn Sie einen Zeitplan haben, der um 9:00 Uhr beginnt und um 23:00 Uhr endet und für eine Aufgabe geplant ist, die um 14:00 Uhr beginnt und um 16:00 Uhr endet, beträgt die Dauer der Aufgabe null.


>[!ENDSHADEBOX]

Im Folgenden finden Sie zwei Szenarien, in denen die Dauer in Adobe Workfront berechnet wird:

* Wenn die Aufgabe einem Benutzer zugewiesen ist, gibt es je nach verwendeter Umgebung die folgenden Szenarien:

   * In der Produktionsumgebung verwendet Workfront einen der folgenden Zeitpläne, in dieser genauen Reihenfolge, um die Dauer zu berechnen:

   1. Workfront berücksichtigt den Benutzerzeitplan.
   1. Wenn der Benutzer keinem Zeitplan zugeordnet ist, berücksichtigt Workfront den Zeitplan des Projekts.
   1. Wenn das Projekt nicht mit einem Zeitplan verknüpft ist, berücksichtigt Workfront den Standardzeitplan Ihres Systems. Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

<div class="preview">

* In der Vorschau-Umgebung:

   1. Workfront berücksichtigt entweder den Zeitplan des Projekts oder den der Aufgabe zugewiesenen Benutzer.

      Ihr Workfront- oder Gruppenadministrator legt fest, welcher Zeitplan von Workfront verwendet wird, wenn eine Aufgabe einem Benutzer zugewiesen wird. Weitere Informationen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Wenn der Benutzer oder das Projekt keinen Zeitplan hat, verwendet Workfront den Standardzeitplan des Systems.

      Die Schritte ähneln dem ersten Szenario, nachdem Sie ermittelt haben, welcher Zeitplan von Workfront zur Berechnung der Dauer verwendet wird.

</div>

* Wenn die Aufgabe mehreren Benutzern zugewiesen ist:

   1. Workfront berücksichtigt entweder den Zeitplan des Projekts oder den des Hauptverantwortlichen.

      Ihr Workfront- oder Gruppenadministrator legt fest, welcher Zeitplan von Workfront verwendet wird, wenn eine Aufgabe mehreren Benutzern zugewiesen wird. Weitere Informationen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Wenn der primäre Verantwortliche oder das Projekt keinen Zeitplan haben, verwendet Workfront den Standardzeitplan des Systems.

  Die Schritte ähneln dem ersten Szenario, nachdem Sie ermittelt haben, welcher Zeitplan von Workfront zur Berechnung der Dauer verwendet wird.

>[!NOTE]
>
>Unter Berücksichtigung der Projektzeit des Primären Verantwortlichen können sich die geplanten Aufgabendaten anpassen, die Aufgabendauer bleibt jedoch gleich. Weitere Informationen zur Berücksichtigung der Zeitdauer des Primären Verantwortlichen bei der Projektplanung finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Zeiteinheiten für Aufgabendauer

Sie können die Aufgabendauer sowohl in der regulären Zeit als auch in der verstrichenen Zeit zwischen dem geplanten Start- und dem geplanten Abschlussdatum angeben.

Beim Aktualisieren der Dauer von Aufgaben in einer Liste können Sie die folgenden Abkürzungen verwenden, um Zeiteinheiten in Workfront anzugeben:

| Zeiteinheit | Abkürzung |
|---|---|
| Minuten | M |
| Stunden | H |
| Tage. Dies ist die Standardeinstellung. | D |
| Wochen | W  |
| Monate | T, MO |
| Verstrichene Minuten | EM |
| Verstrichene Stunden | EH |
| Verstrichene Tage | ED |
| Verstrichene Wochen | EW |
| Verstrichene Monate | ET |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**BEISPIEL**

Wenn Sie angeben möchten, dass die Dauer einer Aufgabe 3 Tage ist, geben Sie &quot;3 ED&quot;in das Feld Dauer in eine Aufgabenliste ein.  Sie können auch die bevorzugte Option für die Zeiteinheit im verfügbaren Dropdownmenü beim Bearbeiten einer Aufgabe oder im Abschnitt Aufgabendetails auswählen. Weitere Informationen zum Bearbeiten von Aufgaben finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Beachten Sie Folgendes bei der Angabe der Dauer einer Aufgabe:

* Die verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und eine Verspätung umfasst. Mit anderen Worten, vergangene Zeit ist der Durchgang von Kalendertagen.
* Tage stellen die im System definierten Arbeitstage dar und können im Bereich Einrichtung konfiguriert werden. In den meisten Fällen besteht ein Tag aus 8 Stunden.
* Die reguläre Zeit (Tage oder Arbeitstage) berücksichtigt Feiertage, Wochenenden und Auszeiten und schließt sie von der Dauer der Aufgabe aus.
* Wenn Sie die Dauer einer Aufgabe in Wochen angeben, berechnet Workfront die Dauer in Tagen und Stunden anhand der von Ihrem Workfront-Administrator im Bereich &quot;Projekteinstellungen&quot;festgelegten Einstellungen für die typischen Wochentage und die typischen Stunden pro Arbeitstag.
* Workfront verwendet die Standarddauer von 4 Wochen für einen Monat bei der Berechnung der Dauer in Monaten.

## Übersicht über den Aufgabendauer-Typ

Durch die Verwaltung des Aufgabentyps können Sie konsistente Ressourcenzuweisungen entsprechend den Anforderungen der Aufgabe festlegen.

Der Typ der Dauer hilft bei der Beantwortung der folgenden Fragen:

* Wie beschäftigt werden wir sein?
* Wie groß ist die Arbeit?
* Wie lange wird es dauern?

![duration_type_triangle.png](assets/duration_type_triangle.png)

## Definieren von Dauer-Typen

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>Dauertyp</strong></p></th> 
   <th scope="col"> <p><strong>Funktion</strong> </p> </th> 
   <th scope="col"> <p><strong>Wie sich Ressourcen darauf auswirken</strong> </p> </th> 
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
   <th scope="col"> <p><strong>Leistungsgesteuert</strong></p> </th> 
   <td scope="col"> <p>Bestimmt die geplanten Stunden anhand der Anzahl der Ressourcen.</p> <p>Wenn Sie diesen Dauerhaltungstyp auswählen, können Sie für die Aufgabe eine individuelle Dauer eingeben. Workfront berechnet die geplanten Stunden für die Aufgabe, indem es die Anzahl der Tage in der Dauer durch die Anzahl der Arbeitsstunden im Zeitplan multipliziert und durch die Anzahl der Verantwortlichen für die Aufgabe dividiert. </p> <p>Sie können den Zuordnungsprozentwert jedes Verantwortlichen manuell an die Aufgabe anpassen, aber die Anzahl der geplanten Stunden bleibt gleich.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Übersicht über den Durationstyp: Aufwandsorientiert</a>.</p> </td> 
   <td scope="col"> <p>Die geplanten Stunden werden erhöht, wenn die Bevollmächtigten aus der Aufgabe entfernt werden.</p> <p>Die geplanten Stunden werden reduziert, wenn der Aufgabe die Zuweisung hinzugefügt wird. </p> <p>Die Dauer ändert sich nicht, unabhängig von der Anzahl der Bevollmächtigten oder ihrem Zeitplan. </p> <p>Die Dauer entspricht den geplanten Stunden. Die geplante Dauer entspricht der Anzahl der geplanten Stunden dividiert durch die Anzahl der Bevollmächtigten.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Einfach</strong> </p> </th> 
   <td scope="col"> <p>Bestimmt die geplanten Stunden und die Dauer (die für diesen Durationstyp gleich sind) anhand der Anzahl der Stunden, für die jeder Verantwortliche zugewiesen wird. </p> <p>Workfront berechnet die geplanten Stunden, indem es die geplanten zugewiesenen Stunden für jeden Bevollmächtigten addiert. </p> <p>Sie haben die Möglichkeit, die Anzahl der Stunden, die jedem Bevollmächtigten zugewiesen werden, manuell zu ändern und die Anzahl der geplanten Stunden und die Menge der Dauer entsprechend zu ändern. Wenn Sie eine Gesamtzahl der zugewiesenen Stunden für alle Bevollmächtigten wählen, wird diese Zahl gleichmäßig zwischen jedem Bevollmächtigten aufgeteilt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Übersicht über den Durationstyp: Einfach</a>.</p> </td> 
   <td scope="col"> <p>Die Stunden werden gleichmäßig auf die Bevollmächtigten verteilt, wenn Sie eine Gesamtzahl der zugewiesenen Stunden auswählen. Als Projektmanager können Sie jedoch die Stunden für jeden Verantwortlichen manuell anpassen. </p> <p>Sie können entweder die geplante Stunde und Dauer einer Aufgabe mit dem einfachen Typ Dauer inline oder auf Aufgabenebene bearbeiten. </p> <p>Wenn ein agiles Team einer Aufgabe zugewiesen ist, wird der Typ der Dauer automatisch auf Einfach gesetzt und kann nicht geändert werden. Die Aufgabendauer eines agilen Teams muss größer als 0 Minuten sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Der Typ der neuen Aufgaben mit Dauer

Der Dauer-Typ einer neuen Aufgabe entspricht dem in Ihrem System eingerichteten Dauer-Typ. Der Standardtyp für die Dauer ist &quot;Berechnete Zuweisung&quot;. Ihr Workfront-Administrator oder ein Gruppenadministrator kann den Standardtyp für die Dauer des Projekts für Ihr System oder die mit dem Projekt verknüpfte Gruppe aktualisieren. Weitere Informationen finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Die ursprüngliche Dauer einer übergeordneten Aufgabe

Die ursprüngliche Dauer einer Aufgabe ist die Dauer in Minuten, die eine Aufgabe hatte, bevor sie zur übergeordneten Aufgabe wurde.

Wenn eine Aufgabe übergeordnet wird, wird die Dauer zwischen dem geplanten Startdatum des frühesten untergeordneten Elements und dem geplanten Abschlussdatum des letzten untergeordneten Elements in die übergeordnete Aufgabe aggregiert und wird zur Dauer der übergeordneten Aufgabe. Dadurch wird die Dauer der ursprünglichen Aufgabe ersetzt.

Wenn Kinder die Zeiteinheit &quot;Verstrichene Tage&quot;verwenden und ihr übergeordnetes Element die Zeiteinheit &quot;Tage&quot;verwendet, kann es zu Abweichungen bei der Berechnung der Dauer der übergeordneten Aufgabe durch Workfront kommen.

Beachten Sie Folgendes:

* Die Zeiteinheit &quot;Elapsed Days&quot;stellt Kalendertage dar, die immer aus 24 Stunden pro Tag bestehen.
* Die Tage der Zeiteinheit für die Dauer stellen den im System definierten Arbeitstag dar und sind konfigurierbar. In den meisten Fällen besteht er aus 8 Stunden pro Tag.
* Die Formel zur Berechnung der Dauer der übergeordneten Aufgabe lautet wie folgt:

  `Parent task duration = Planned Completion Date of the child task that is planned to end the latest - Planned Start Date of the child task that starts the earliest`

* Bei der Berechnung der Dauer der Hauptaufgabe berechnet das System zunächst die Dauer anhand der obigen Formel und wendet dann den Zeitplan an.


Weitere Informationen finden Sie unter [Übersicht über die ursprüngliche Dauer der Aufgabe und die ursprünglich geplanten Stunden](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md).

## Ändern der Dauer einer Aufgabe

Weitere Informationen zum Ändern des Dauer-Typs einer Aufgabe finden Sie unter [Aktualisieren des Dauer-Typs einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
