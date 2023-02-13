---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Übersicht über den Task Tracking Mode
description: Sie können die Einstellung des Tracking-Modus einer Aufgabe beim Erstellen oder Bearbeiten einer Aufgabe anpassen, um zu steuern, wie und wann die Fortschrittsstatus-Indikatoren einer Aufgabe angezeigt werden. In Adobe Workfront werden beim Konfigurieren bestimmter Einstellungen zum Verfolgen des Fortschritts bei Aufgaben Statusflags angezeigt.
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 3%

---

# Übersicht über den Task Tracking Mode

Sie können die Einstellung des Tracking-Modus einer Aufgabe beim Erstellen oder Bearbeiten einer Aufgabe anpassen, um zu steuern, wie und wann die Fortschrittsstatus-Indikatoren einer Aufgabe angezeigt werden. In Adobe Workfront werden beim Konfigurieren bestimmter Einstellungen zum Verfolgen des Fortschritts bei Aufgaben Statusflags angezeigt.

Weitere Informationen zum Fortschrittsstatus von Aufgaben finden Sie unter [Übersicht über den Task Progress Status](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## Optionen für den Tracking-Modus {#tracking-mode-options}

Als Aufgabenbesitzer oder Projektmanager können Sie festlegen, wie Workfront den Fortschrittsstatus für jede Aufgabe anzeigt. Informationen zum Festlegen des Tracking-Modus für Ihre Aufgaben finden Sie unter [Tracking-Modus für Aufgaben festlegen](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

Sie können aus den folgenden Optionen auswählen:

* [Benutzer muss aktualisieren](#user-must-update)
* [Annahme: Im Zeitplan](#assume-on-time)
* [Späte Warnungen ignorieren](#ignore-late-warnings)
* [Automatisch abschließen](#auto-complete)
* [Vorgänger](#predecessor)

### Benutzer muss aktualisieren {#user-must-update}

Wenn diese Option aktiviert ist, verwendet Workfront die &quot;Percent Complete&quot;und die &quot;Actual Hours&quot;der Aufgabe, um den Fortschrittsstatus der Aufgabe zu ermitteln. Dies ist die Standardoption.

### Annahme: Im Zeitplan {#assume-on-time}

Workfront geht davon aus, dass eine Aufgabe unabhängig vom aktuellen Fertigstellungsstatus rechtzeitig abgeschlossen wird. Ist dies nicht der Fall, nimmt Workfront automatisch das geplante Abschlussdatum des nächsten Arbeitstags an. Sie müssen weiterhin angeben, wann die Aufgabe abgeschlossen ist. Verwenden Sie diese Option, wenn Benutzer ihre Aufgaben nicht regelmäßig aktualisieren.

### Späte Warnungen ignorieren {#ignore-late-warnings}

Der Fortschrittsstatus einer Aufgabe lautet &quot;Einschaltzeit&quot;, bis er zu spät wird. Wenn Sie beispielsweise eine Aufgabe für 10 Tage planen und an dem Tag, an dem sie abgeschlossen werden soll, die Aufgabe den Prozentwert &quot;Abgeschlossen&quot;von 60 % anzeigt, aktualisiert Workfront das geplante Abschlussdatum, indem vier Tage hinzugefügt werden und der Fortschrittsstatus der Aufgabe zu &quot;spät&quot; wird.

### Automatisch abschließen {#auto-complete}

Workfront geht davon aus, dass Aufgaben plangemäß abgeschlossen werden und kennzeichnet sie als abgeschlossen am Fälligkeitsdatum oder an dem geplanten Abschlussdatum. Bis dahin nutzt Workfront die &quot;Percent Complete&quot;und die &quot;Actual Hours&quot;, um den Fortschrittsstatus zu ermitteln. Unabhängig vom Fortschrittsstatus vor dem geplanten Abschlussdatum markiert Workfront die Aufgabe jedoch weiterhin als abgeschlossen.

Es gibt die folgenden Ausnahmen:

* Wenn die Aufgabe unvollständige Vorgänger aufweist, wird sie erst automatisch abgeschlossen, wenn alle Vorgänger abgeschlossen sind.
* Wenn die Aufgabe die Beschränkung &quot;Festes Datum&quot;hat, wird die Aufgabe immer am geplanten Abschlussdatum abgeschlossen, unabhängig davon, ob ihre Vorgänger abgeschlossen sind.

>[!IMPORTANT]
>
>Wenn Sie auswählen, dass Aufgaben automatisch abgeschlossen werden sollen, wird die Aufgabe Abgeschlossen, wenn die Projektzeit neu berechnet wird. Wenn der Aktualisierungstyp des Projekts auf Automatisch oder Automatisch und Bei Änderung eingestellt ist, wird die Projekt-Timeline täglich berechnet. Informationen zu Zeitleistenneuberechnungen für Projekte finden Sie unter [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>Die Uhrzeit des tatsächlichen Abschlussdatums ist Mitternacht des Tages, an dem die Timeline automatisch berechnet wird. Die für die Generierung dieses Zeitstempels verwendete Zeit ist die Zeitzone Ihres Systems, die vom Workfront-Administrator im Abschnitt &quot;Kundeninformationen&quot;der Einrichtung definiert wurde. Informationen zum Festlegen der Zeitzone Ihres Systems finden Sie unter [Grundlegende Informationen für Ihr System konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Vorgänger {#predecessor}

Workfront schätzt das voraussichtliche Abschlussdatum einer Aufgabe entsprechend ihrer Vorgängerbeziehung. Der Fortschrittsstatus einer Aufgabe wird anhand dieser Schätzung ermittelt. Beispielsweise hat Aufgabe B eine Dauer von 1 Tag und soll zwei Tage nach ihrer Vorgängerin, Aufgabe A, ausgeführt werden, die fünf Tage dauern sollte. Ein Benutzer aktualisiert dann Aufgabe B auf 50 % &quot;Abgeschlossen&quot;, aber die Vorgängerin, Aufgabe A, hat noch nicht gestartet. Workfront plant die Überprüfung der abhängigen Aufgabe B für den Abschluss sechs Tage nach dem Startdatum der Vorgängeraufgabe, wobei 5 Tage für Aufgabe A und 1 Tag für Aufgabe B zulässig sind.
