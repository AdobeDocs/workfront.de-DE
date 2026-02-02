---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Übersicht über die Aufgabendauer und den Dauertyp
description: Die Aufgabendauer ist die Differenz zwischen dem geplanten Abschlussdatum und dem geplanten Startdatum der Aufgabe. Die Dauer gibt den Zeitrahmen an, in dem die Aufgabe abgeschlossen werden kann.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 1%

---

# Übersicht über die Aufgabendauer und den Dauertyp

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Die Aufgabendauer ist die Differenz zwischen dem geplanten Abschlussdatum und dem geplanten Startdatum der Aufgabe. Die Dauer gibt den Zeitrahmen an, in dem die Aufgabe abgeschlossen werden kann.

Der Dauertyp einer Aufgabe gibt die Beziehung zwischen der Anzahl der einer Aufgabe zugewiesenen Ressourcen, dem Gesamtaufwand und der Gesamtdauer der Aufgabe an.

## Aufgabendauer - Übersicht

Wenn das tatsächliche Start- und Abschlussdatum der Aufgabe außerhalb des Zeitplans des Projekts, des primären Verantwortlichen oder des Standardzeitplans liegt, ist die Aufgabendauer null.

>[!BEGINSHADEBOX]

**BEISPIEL**
Wenn Sie einen Zeitplan haben, der um 9 :00 beginnt und um 12 :00 endet und eine Aufgabe, die um 14 :00 beginnen und um 16 :00 enden soll, ist die Aufgabendauer null.


>[!ENDSHADEBOX]

Im Folgenden finden Sie zwei Szenarien für die Berechnung der Dauer in Adobe Workfront:

* Wenn die Aufgabe einem Benutzer zugewiesen ist:

   1. Workfront berücksichtigt entweder den Zeitplan des Projekts oder den des Benutzers, der der Aufgabe zugewiesen wurde.

      Ihr Workfront- oder Gruppenadministrator bestimmt, welchen Zeitplan Workfront verwendet, wenn eine Aufgabe einem Benutzer zugewiesen wird. Weitere Informationen finden [&#x200B; unter „Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Wenn der/die Benutzende oder das Projekt keinen Zeitplan hat, verwendet Workfront den Systemstandardzeitplan.

      Die Schritte ähneln dem ersten Szenario, nachdem verstanden wurde, welcher Zeitplan von Workfront zur Berechnung der Dauer verwendet wird.

* Wenn die Aufgabe mehreren Benutzern zugewiesen ist:

   1. Workfront berücksichtigt entweder den Zeitplan des Projekts oder den des primären Verantwortlichen.

      Ihr Workfront- oder Gruppenadministrator bestimmt, welchen Zeitplan Workfront verwendet, wenn eine Aufgabe mehreren Benutzern zugewiesen wird. Weitere Informationen finden [&#x200B; unter „Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Wenn der primäre Zugewiesene oder das Projekt keinen Zeitplan hat, verwendet Workfront den Systemstandardzeitplan.

  Die Schritte ähneln dem ersten Szenario, nachdem verstanden wurde, welcher Zeitplan von Workfront zur Berechnung der Dauer verwendet wird.

>[!NOTE]
>
>Wenn die Urlaubstage des Primären Verantwortlichen für ein Projekt berücksichtigt werden, können sich die Termine der Aufgabe anpassen, aber die Aufgabendauer bleibt gleich. Informationen zur Berücksichtigung der Ausfallzeit des Primären Verantwortlichen bei der Projektplanung finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Zeiteinheiten für die Aufgabendauer

Sie können die Aufgabendauer sowohl in der regulären Zeit als auch in der Zeit zwischen dem geplanten Start- und dem geplanten Abschlussdatum angeben.

Beim Aktualisieren der Aufgabendauer in einer Liste können Sie die folgenden Abkürzungen zur Angabe von Zeiteinheiten in Workfront verwenden:

| Zeiteinheit | Abkürzung |
|---|---|
| Minutes | M |
| Stunden | H |
| Tage. Dies ist der Standardwert. | D |
| Weeks | W |
| Months | T, MO |
| Verstrichene Minuten | EM |
| Verstrichene Stunden | EH |
| Verstrichene Tage | ED |
| Verstrichene Wochen | EW |
| Verstrichene Monate | ET |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**BEISPIEL**

Wenn Sie angeben möchten, dass die Dauer einer Aufgabe 3 verstrichene Tage beträgt, geben Sie in das Feld Dauer in einer Aufgabenliste „3 ED“ ein.  Sie können auch die bevorzugte Option für die Zeiteinheit der Dauer beim Bearbeiten einer Aufgabe aus dem verfügbaren Dropdown-Menü oder im Abschnitt Aufgabendetails auswählen. Informationen zum Bearbeiten von Aufgaben finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![Dauer verstrichener Tage bei Aufgaben](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Beachten Sie beim Angeben der Dauer einer Aufgabe Folgendes:

* Verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und Ausfallzeiten umfasst. Mit anderen Worten: Verstrichene Zeit ist der Ablauf von Kalendertagen.
* Tage stellen die im System definierten Arbeitstage dar und können im Bereich Setup konfiguriert werden. In den meisten Fällen besteht ein Tag aus 8 Stunden.
* Die reguläre Zeit (Tage oder Arbeitstage) berücksichtigt Feiertage, Wochenenden und Ausfallzeiten und schließt sie von der Aufgabendauer aus.
* Wenn Sie die Aufgabendauer in Wochen angeben, berechnet Workfront die Dauer in Tagen und Stunden anhand der Einstellungen „Typische Arbeitstage pro Woche“ und „Typische Stunden pro Arbeitstag“, die Ihr Workfront-Administrator im Bereich „Projektvoreinstellungen“ von „Setup“ festgelegt hat.
* Bei der Berechnung der Dauer in Monaten verwendet Workfront die Standarddauer von 4 Wochen für einen Monat.

## Übersicht über den Aufgabendauer-Typ

Die Verwaltung des Dauertyps einer Aufgabe ermöglicht es Ihnen, konsistente Ressourcenzuweisungen basierend auf den Anforderungen der Aufgabe festzulegen.

Der Dauertyp hilft bei der Beantwortung der folgenden Fragen:

* Wie beschäftigt werden wir sein?
* Wie groß ist der Job?
* Wie lange wird es dauern?

![duration_type_triangle.png](assets/duration_type_triangle.png)

## Dauertypen definieren

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
   <td scope="col"> <p>Berechnet den Zuordnungsprozentsatz für jeden Zugewiesenen für eine Aufgabe. </p> <p>Wenn Sie diesen Dauertyp auswählen, können Sie die individuelle Dauer und die geplanten Stunden für die Aufgabe eingeben. Workfront teilt die geplanten Stunden durch die Anzahl der Stunden innerhalb der Aufgabendauer und die Anzahl der Ressourcen, die der Aufgabe zugewiesen wurden, um die Zuordnung für jeden Verantwortlichen zu berechnen.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Duration Type Overview: Calculated Assignment</a>.</p> </td> 
   <td scope="col">Die Dauer und die geplanten Stunden ändern sich nicht, wenn Verantwortliche zur Aufgabe hinzugefügt oder entfernt werden. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Berechnete Arbeit</strong> </p> </th> 
   <td scope="col"> <p>Bestimmt die geplanten Stunden (Aufwand), die für die Erfüllung der Aufgabe erforderlich sind.</p> <p>Wird normalerweise verwendet, wenn die der Aufgabe zugewiesenen Ressourcen für die gesamte Dauer der Aufgabe zugewiesen werden.</p> <p>Wenn Sie diesen Dauertyp auswählen, können Sie eine individuelle Dauer für die Aufgabe eingeben. Workfront berechnet die geplanten Stunden für die Aufgabe, indem die Anzahl der Tage in der Dauer mit der Anzahl der Arbeitsstunden im Zeitplan und mit der Anzahl der Beauftragten für die Aufgabe multipliziert wird. </p> <p>Sie haben die Möglichkeit, den Zuordnungsprozentsatz jedes Zugewiesenen für die Aufgabe manuell zu ändern, wodurch der Betrag der geplanten Stunden verkürzt wird.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Übersicht über den Dauertyp: Berechnete Arbeit</a>.</p> </td> 
   <td scope="col"> <p>Die geplanten Stunden erhöhen sich, wenn Verantwortliche zur Aufgabe hinzugefügt werden. </p> <p>Die geplanten Stunden verringern sich, wenn Verantwortliche aus der Aufgabe entfernt werden.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Leistungsgesteuert</strong></p> </th> 
   <td scope="col"> <p>Bestimmt die geplanten Stunden anhand der Anzahl der Ressourcen.</p> <p>Wenn Sie diesen Dauertyp auswählen, können Sie eine individuelle Dauer für die Aufgabe eingeben. Workfront berechnet die geplanten Stunden für die Aufgabe, indem die Anzahl der Tage in der Dauer mit der Anzahl der Arbeitsstunden im Zeitplan multipliziert und durch die Anzahl der Beauftragten für die Aufgabe dividiert wird. </p> <p>Sie haben die Möglichkeit, den Zuordnungsprozentsatz jedes Zugewiesenen für die Aufgabe manuell zu ändern, aber die Anzahl der geplanten Stunden bleibt gleich.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Übersicht über den Dauertyp: Leistungsgesteuert</a>.</p> </td> 
   <td scope="col"> <p>Die geplanten Stunden erhöhen sich, wenn Verantwortliche aus der Aufgabe entfernt werden.</p> <p>Die geplanten Stunden verringern sich, wenn Verantwortliche zur Aufgabe hinzugefügt werden. </p> <p>Die Dauer ändert sich nicht, unabhängig von Änderungen in der Anzahl der Bevollmächtigten oder ihrem Zeitplan. </p> <p>Dauer ist gleich den geplanten Stunden. Die geplante Dauer ist gleich der geplanten Stunden dividiert durch die Anzahl der zugewiesenen Personen.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Einfach</strong> </p> </th> 
   <td scope="col"> <p>Bestimmt die geplanten Stunden und die Dauer (die für diesen Dauertyp gleich sind) basierend auf der Anzahl der Stunden, für die jeder Zugewiesene zugewiesen wird. </p> <p>Workfront berechnet die geplanten Stunden durch Addition der geplanten zugewiesenen Stunden für jeden Verantwortlichen. </p> <p>Sie haben die Möglichkeit, die Anzahl der Stunden, für die jeder Verantwortliche zugewiesen wird, manuell zu ändern. Die Anzahl der geplanten Stunden und der Betrag der Dauer ändern sich entsprechend. Wenn Sie die Gesamtanzahl der zugewiesenen Stunden für alle Verantwortlichen auswählen, wird diese Zahl zu gleichen Teilen auf die einzelnen Verantwortlichen aufgeteilt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Duration Type Overview: Simple</a>.</p> </td> 
   <td scope="col"> <p>Stunden werden gleichmäßig auf die Verantwortlichen verteilt, wenn Sie eine Gesamtzahl zugewiesener Stunden auswählen. Als Projekt-Manager können Sie jedoch die Stunden für jeden einzelnen Zugewiesenen manuell anpassen. </p> <p>Sie können „Geplante Stunden“ und „Dauer“ einer Aufgabe mit einem einfachen Dauertyp inline oder auf Aufgabenebene bearbeiten. </p> <p>Wenn ein Agile-Team einer Aufgabe zugewiesen wird, wird der Dauertyp automatisch auf „Einfach“ gesetzt und kann nicht geändert werden. Die Aufgabendauer für ein Agile-Team muss länger als 0 Minuten sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Der Dauertyp neuer Aufgaben

Der Dauertyp einer neuen Aufgabe entspricht dem in Ihrem System eingerichteten Dauertyp. Der Standarddauertyp ist Berechnete Zuweisung. Ihr Workfront-Administrator oder ein Gruppenadministrator kann den Standarddauertyp für Ihr System oder für die mit dem Projekt verknüpfte Gruppe aktualisieren. Weitere Informationen finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Die ursprüngliche Dauer einer übergeordneten Aufgabe

Die ursprüngliche Dauer einer Aufgabe ist die Dauer in Minuten, die eine Aufgabe ursprünglich hatte, bevor sie zu einer übergeordneten Aufgabe wurde.

Wenn eine Aufgabe ein übergeordnetes Element wird, wird die Dauer zwischen dem geplanten Startdatum des frühesten untergeordneten Elements und dem geplanten Abschlussdatum des letzten untergeordneten Elements auf die übergeordnete Aufgabe angerechnet und wird zur Dauer der übergeordneten Aufgabe. Dadurch wird die Dauer der ursprünglichen Aufgabe ersetzt.

Wenn untergeordnete Elemente die Einheit Dauer verstrichener Tage verwenden und ihre übergeordneten Elemente die Einheit Dauer von Tagen verwenden, kann es zu Diskrepanzen bei der Berechnung der Dauer der übergeordneten Aufgabe durch Workfront kommen.

Beachten Sie Folgendes:

* Die Einheit Verstrichene Tage stellt Kalendertage dar, die immer aus 24 Stunden pro Tag bestehen.
* Die Einheit Tage stellt den im System definierten Arbeitstag dar und ist konfigurierbar. In den meisten Fällen besteht sie aus 8 Stunden pro Tag.
* Die Formel zur Berechnung der Dauer der übergeordneten Aufgabe lautet wie folgt:

  `Parent task duration = Planned Completion Date of the child task that is planned to end the latest - Planned Start Date of the child task that starts the earliest`

* Bei der Berechnung der Dauer der übergeordneten Aufgabe berechnet das System zuerst die Dauer anhand der obigen Formel und wendet dann den Zeitplan an.


Weitere Informationen finden Sie unter [Übersicht über die ursprüngliche Aufgabendauer und die ursprünglich geplanten Stunden](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md).

## Dauertyp einer Aufgabe ändern

Informationen zum Ändern des Dauertyps einer Aufgabe finden Sie unter [Aktualisieren des Dauertyps einer Aufgabe](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
